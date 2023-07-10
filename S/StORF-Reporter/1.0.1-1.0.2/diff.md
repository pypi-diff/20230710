# Comparing `tmp/StORF-Reporter-1.0.1.tar.gz` & `tmp/StORF-Reporter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StORF-Reporter-1.0.1.tar", last modified: Tue Jun  6 02:48:35 2023, max compression
+gzip compressed data, was "StORF-Reporter-1.0.2.tar", last modified: Mon Jul 10 20:51:51 2023, max compression
```

## Comparing `StORF-Reporter-1.0.1.tar` & `StORF-Reporter-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-06 02:48:35.307331 StORF-Reporter-1.0.1/
--rw-r--r--   0 nick      (1000) nick      (1000)    35149 2021-12-28 14:08:10.000000 StORF-Reporter-1.0.1/LICENSE
--rw-rw-r--   0 nick      (1000) nick      (1000)    19923 2023-06-06 02:48:35.307331 StORF-Reporter-1.0.1/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)    19279 2023-06-06 02:48:16.000000 StORF-Reporter-1.0.1/README.md
--rw-r--r--   0 nick      (1000) nick      (1000)      147 2022-12-16 17:48:19.000000 StORF-Reporter-1.0.1/pyproject.toml
--rw-r--r--   0 nick      (1000) nick      (1000)     1128 2023-06-06 02:48:35.307331 StORF-Reporter-1.0.1/setup.cfg
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-06 02:48:35.303331 StORF-Reporter-1.0.1/src/
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-06 02:48:35.303331 StORF-Reporter-1.0.1/src/StORF_Reporter/
--rw-r--r--   0 nick      (1000) nick      (1000)       33 2023-06-06 02:48:16.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/Constants.py
--rw-r--r--   0 nick      (1000) nick      (1000)    16596 2023-06-06 02:45:48.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Extractor.py
--rwxr-xr-x   0 nick      (1000) nick      (1000)    47406 2023-06-06 02:45:48.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Finder.py
--rw-r--r--   0 nick      (1000) nick      (1000)     5220 2023-05-14 21:36:54.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Remover.py
--rw-r--r--   0 nick      (1000) nick      (1000)    51993 2023-06-06 02:42:40.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Reporter.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-06 02:48:35.307331 StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/
--rw-r--r--   0 nick      (1000) nick      (1000)     2075 2023-06-06 02:45:48.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/StORF_Adder.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1270 2022-09-29 20:25:03.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/UR_Lenghts.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9682 2022-09-29 20:25:03.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/Un_StORFed.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-09-29 20:25:03.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/__init__.py
--rwxr-xr-x   0 nick      (1000) nick      (1000)    15208 2023-06-06 02:45:48.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/UR_Extractor.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-01-06 11:38:05.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-06 02:48:35.307331 StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)    19923 2023-06-06 02:48:35.000000 StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      695 2023-06-06 02:48:35.000000 StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-06-06 02:48:35.000000 StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      269 2023-06-06 02:48:35.000000 StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       25 2023-06-06 02:48:35.000000 StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       15 2023-06-06 02:48:35.000000 StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/top_level.txt
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-10 20:51:51.525597 StORF-Reporter-1.0.2/
+-rw-r--r--   0 nick      (1000) nick      (1000)    35149 2022-12-19 15:31:53.000000 StORF-Reporter-1.0.2/LICENSE
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19923 2023-07-10 20:51:51.525597 StORF-Reporter-1.0.2/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)    19279 2023-07-10 20:50:43.000000 StORF-Reporter-1.0.2/README.md
+-rw-r--r--   0 nick      (1000) nick      (1000)      147 2022-12-19 15:34:48.000000 StORF-Reporter-1.0.2/pyproject.toml
+-rw-r--r--   0 nick      (1000) nick      (1000)     1128 2023-07-10 20:51:51.525597 StORF-Reporter-1.0.2/setup.cfg
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-10 20:51:51.521597 StORF-Reporter-1.0.2/src/
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-10 20:51:51.525597 StORF-Reporter-1.0.2/src/StORF_Reporter/
+-rw-r--r--   0 nick      (1000) nick      (1000)       34 2023-07-10 20:50:43.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/Constants.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    16601 2023-07-10 18:01:01.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Extractor.py
+-rwxr-xr-x   0 nick      (1000) nick      (1000)    47406 2023-05-29 18:06:24.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Finder.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     5220 2023-07-10 18:01:01.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Remover.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    52121 2023-07-10 20:39:48.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Reporter.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-10 20:51:51.525597 StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/
+-rw-r--r--   0 nick      (1000) nick      (1000)     2075 2023-05-29 18:06:24.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/StORF_Adder.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1270 2022-12-19 15:31:53.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/UR_Lenghts.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     9682 2022-12-19 15:31:53.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/Un_StORFed.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:53.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/__init__.py
+-rwxr-xr-x   0 nick      (1000) nick      (1000)    15208 2023-05-29 18:06:24.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/UR_Extractor.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-01-06 19:37:38.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-10 20:51:51.525597 StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19923 2023-07-10 20:51:51.000000 StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      695 2023-07-10 20:51:51.000000 StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-07-10 20:51:51.000000 StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      269 2023-07-10 20:51:51.000000 StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       25 2023-07-10 20:51:51.000000 StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       15 2023-07-10 20:51:51.000000 StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/top_level.txt
```

### Comparing `StORF-Reporter-1.0.1/LICENSE` & `StORF-Reporter-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.1/PKG-INFO` & `StORF-Reporter-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StORF-Reporter
-Version: 1.0.1
+Version: 1.0.2
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
 
-StORF-Reporter v1.0.1: StORF-Reporter Run Parameters.
+StORF-Reporter v1.0.2: StORF-Reporter Run Parameters.
 
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
 
-StORF-Reporter v1.0.1: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.2: UR-Extractor Run Parameters.
 
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
 
-StORF-Reporter v1.0.1: StORF-Finder Run Parameters.
+StORF-Reporter v1.0.2: StORF-Finder Run Parameters.
 
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
 
-StORF-Reporter v1.0.1: StORF-Extractor Run Parameters.
+StORF-Reporter v1.0.2: StORF-Extractor Run Parameters.
 
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
 
-StORF-Reporter v1.0.1: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.2: UR-Extractor Run Parameters.
 
 Required Arguments:
   -gff GFF              GFF annotation file for the FASTA
   -blast BLAST          BLAST format 6 annotation file
 
 Optional Arguments:
   -min_score MINSCORE   Minimum BitScore to keep StORF: Default 30
```

### Comparing `StORF-Reporter-1.0.1/README.md` & `StORF-Reporter-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                          [-ex_len EXLEN] [-spos {True,False}] [-rs {True,False}] [-con_storfs {True,False}]
                          [-con_only {True,False}] [-ps {True,False}] [-wc {True,False}] [-short_storfs {False,Nolap,Olap}]
                          [-short_storfs_only {True,False}] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS]
                          [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-so [{start_pos,strand}]]
                          [-f_type [{StORF,CDS,ORF}]] [-olap OVERLAP_NT] [-ao ALLOWED_OVERLAP] [-overwrite {True,False}]
                          [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.1: StORF-Reporter Run Parameters.
+StORF-Reporter v1.0.2: StORF-Reporter Run Parameters.
 
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
 
-StORF-Reporter v1.0.1: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.2: UR-Extractor Run Parameters.
 
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
 
-StORF-Reporter v1.0.1: StORF-Finder Run Parameters.
+StORF-Reporter v1.0.2: StORF-Finder Run Parameters.
 
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
 
-StORF-Reporter v1.0.1: StORF-Extractor Run Parameters.
+StORF-Reporter v1.0.2: StORF-Extractor Run Parameters.
 
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
 
-StORF-Reporter v1.0.1: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.2: UR-Extractor Run Parameters.
 
 Required Arguments:
   -gff GFF              GFF annotation file for the FASTA
   -blast BLAST          BLAST format 6 annotation file
 
 Optional Arguments:
   -min_score MINSCORE   Minimum BitScore to keep StORF: Default 30
```

### Comparing `StORF-Reporter-1.0.1/setup.cfg` & `StORF-Reporter-1.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = StORF-Reporter
-version = v1.0.1
+version = v1.0.2
 author = Nicholas Dimonaco
 author_email = nicholas@dimonaco.co.uk
 description = StORF-Reporter - A a tool that takes an annotated genome and returns missing CDS genes (Stop-to-Stop) from unannotated regions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/NickJD/StORF-Reporter
 project_urls =
```

### Comparing `StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Extractor.py` & `StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,18 +222,18 @@
                 frame = pos.split('_')[2].split(';')[0]
                 ###### This hack is to get over GFF errors where genome-long annotations
                 if stop-start >= 100000:
                     if options.verbose == True:
                         print("UR " + pos + " is more than 100,000 kbs - Please Check Annotation")
                     continue
                 if frame == '+':
-                    StORF_seq = seq[start:stop]
+                    StORF_seq = seq[start-4:stop]
                 elif frame == '-':
                     rev_corrected_start, rev_corrected_stop = reverseCorrectLoci(seq_length, start, None, stop)
-                    StORF_seq = seq_rev[rev_corrected_start:rev_corrected_stop]
+                    StORF_seq = seq_rev[rev_corrected_start-3:rev_corrected_stop]
 
                 Extracted_StORFs[pos] = StORF_seq
         dna_regions.update({key: (seq, seq_length, posns, Extracted_StORFs)})
 
 
 
     write_fasta(dna_regions, options.fasta_outfile)
@@ -274,15 +274,15 @@
                         help='Default - False: Print out runtime messages')
     misc.add_argument('-v', action='store_true', dest='version',
                         help='Default - False: Print out version number and exit')
 
 
 
     options = parser.parse_args()
-    options.tool_ident = ['Single_Genome']#options.tool_ident.split(',')
+    options.tool_ident = ['StORF-Reporter']#options.tool_ident.split(',')
 
 
     if options.storf_input == None or options.path == None:
         if options.version:
             sys.exit(StORF_Reporter_Version)
         else:
             exit('StORF-Extractor: error: the following arguments are required: -storf_input, -p')
```

### Comparing `StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Finder.py` & `StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Finder.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Remover.py` & `StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Remover.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Reporter.py` & `StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Reporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,16 +529,16 @@
                              '\tSingle_GFF = To provide a single Prokka or Bakta GFF file (will not provide new FASTA file); \n'
                              '\tMultiple_GFFs = To provide a directory containing multiple GFF files in Prokka/Bakta format (will not provide a new FASTA file); \n\n'
                              
                              '### Standard GFF Annotation Option 2: \n'
                              '\tEnsembl = Report StORFs for an Ensembl Bacteria annotation (ID=gene); \n'
                              '\tFeature_Types = Used in conjunction with -gene_ident to define features such as CDS,rRNA,tRNA for UR extraction (default CDS); \n'
                              '--- Standard GFF Input Options: \n'
-                             '\tSingle_Genome = To provide a single Genome - accompanying FASTA must share same name as given gff file (can be .fna, fa or .fasta); \n'
-                             '\tMultiple_Genomes = To provide a directory containing multiple accompanying GFF and FASTA files - files must share the same name (fasta can be .fna, fa or .fasta); \n'
+                             '\tSingle_Genome = To provide a single Genome - accompanying FASTA must share same name as given gff file (can be .fna, .fa or .fasta); \n'
+                             '\tMultiple_Genomes = To provide a directory containing multiple accompanying GFF and FASTA files - files must share the same name (fasta can be .fna, .fa or .fasta); \n'
                              '\tSingle_Combined_GFF = To provide a GFF file with embedded FASTA at the bottom; \n'
                              '\tMultiple_Combined_GFFs = To provide a directory containing multiple GFF files with embedded FASTA at the bottom; \n\n'
                              
                              '### Complete Annotation Option 3: \n'
                              '\tPyrodigal = Run Pyrodigal then Report StORFs (provide path to single FASTA or directory of multiple FASTA files ;\n'
                              '--- Complete Annotation Input Options: \n'
                              '\tSingle_FASTA = To provide a single FASTA file; \n'
@@ -808,18 +808,18 @@
                 if Reporter_options.verbose == True:
                     print('StORF-Reporter output ' + gff.split('/')[-1] + ' will be overwritten.')
         gff_list = [x for x in gff_list if x not in gffs_to_filter]
         ####
         file_counter = 0
         for gff in gff_list:
             # Finalising output_file name
-            if Reporter_options.annotation_type[1]  == "Multiple_Combined_GFFs" and Reporter_options.o_name != None:
+            if (Reporter_options.annotation_type[1]  == "Multiple_Combined_GFFs" or Reporter_options.annotation_type[1] == "Multiple_Genomes") and Reporter_options.o_name != None:
                 Reporter_options.output_file = output_file + '_' + str(file_counter)
                 file_counter += 1
-            elif Reporter_options.annotation_type[1]  == "Multiple_Combined_GFFs":
+            elif (Reporter_options.annotation_type[1]  == "Multiple_Combined_GFFs" or Reporter_options.annotation_type[1] == "Multiple_Genomes"):
                 tmp_filename = gff.split('/')[-1].split('.gff')[0]  # could be .fa/.fasta etc
                 Reporter_options.output_file = output_file.replace('_StORF-Reporter',tmp_filename + '_StORF-Reporter')
             else:
                 Reporter_options.output_file = output_file
 
 
             if Reporter_options.verbose == True:
```

### Comparing `StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/StORF_Adder.py` & `StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/StORF_Adder.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/UR_Lenghts.py` & `StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/UR_Lenghts.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/Un_StORFed.py` & `StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/Un_StORFed.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.1/src/StORF_Reporter/UR_Extractor.py` & `StORF-Reporter-1.0.2/src/StORF_Reporter/UR_Extractor.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/PKG-INFO` & `StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StORF-Reporter
-Version: 1.0.1
+Version: 1.0.2
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
 
-StORF-Reporter v1.0.1: StORF-Reporter Run Parameters.
+StORF-Reporter v1.0.2: StORF-Reporter Run Parameters.
 
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
 
-StORF-Reporter v1.0.1: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.2: UR-Extractor Run Parameters.
 
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
 
-StORF-Reporter v1.0.1: StORF-Finder Run Parameters.
+StORF-Reporter v1.0.2: StORF-Finder Run Parameters.
 
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
 
-StORF-Reporter v1.0.1: StORF-Extractor Run Parameters.
+StORF-Reporter v1.0.2: StORF-Extractor Run Parameters.
 
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
 
-StORF-Reporter v1.0.1: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.2: UR-Extractor Run Parameters.
 
 Required Arguments:
   -gff GFF              GFF annotation file for the FASTA
   -blast BLAST          BLAST format 6 annotation file
 
 Optional Arguments:
   -min_score MINSCORE   Minimum BitScore to keep StORF: Default 30
```

### Comparing `StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/SOURCES.txt` & `StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

