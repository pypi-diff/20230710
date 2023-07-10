# Comparing `tmp/mkdesigner-0.0.1.tar.gz` & `tmp/mkdesigner-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdesigner-0.0.1.tar", last modified: Mon Jun 19 10:12:45 2023, max compression
+gzip compressed data, was "mkdesigner-0.1.1.tar", last modified: Mon Jul 10 01:16:16 2023, max compression
```

## Comparing `mkdesigner-0.0.1.tar` & `mkdesigner-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 chigira   (1000) chigira   (1000)        0 2023-06-19 10:12:45.191991 mkdesigner-0.0.1/
--rw-rw-r--   0 chigira   (1000) chigira   (1000)     1065 2023-06-19 04:58:14.000000 mkdesigner-0.0.1/LICENSE
--rw-rw-r--   0 chigira   (1000) chigira   (1000)       56 2023-06-19 06:54:28.000000 mkdesigner-0.0.1/MANIFEST.in
--rw-rw-r--   0 chigira   (1000) chigira   (1000)      280 2023-06-19 10:12:45.191991 mkdesigner-0.0.1/PKG-INFO
--rw-rw-r--   0 chigira   (1000) chigira   (1000)       83 2023-06-19 04:58:14.000000 mkdesigner-0.0.1/README.md
-drwxrwxr-x   0 chigira   (1000) chigira   (1000)        0 2023-06-19 10:12:45.191991 mkdesigner-0.0.1/mkdesigner/
--rwxrwxr-x   0 chigira   (1000) chigira   (1000)      248 2023-06-19 09:57:43.000000 mkdesigner-0.0.1/mkdesigner/__init__.py
--rw-rw-r--   0 chigira   (1000) chigira   (1000)    17356 2023-06-19 04:58:14.000000 mkdesigner-0.0.1/mkdesigner/addprimertovcf.py
--rw-rw-r--   0 chigira   (1000) chigira   (1000)     8159 2023-06-19 04:58:14.000000 mkdesigner-0.0.1/mkdesigner/haplocall.py
--rw-rw-r--   0 chigira   (1000) chigira   (1000)     2268 2023-06-19 04:58:14.000000 mkdesigner-0.0.1/mkdesigner/mergevcf.py
--rw-rw-r--   0 chigira   (1000) chigira   (1000)     2058 2023-06-19 04:58:14.000000 mkdesigner-0.0.1/mkdesigner/mkprimer.py
--rw-rw-r--   0 chigira   (1000) chigira   (1000)     8429 2023-06-19 04:58:14.000000 mkdesigner-0.0.1/mkdesigner/mkselect.py
--rwxrwxr-x   0 chigira   (1000) chigira   (1000)     1941 2023-06-19 04:58:14.000000 mkdesigner-0.0.1/mkdesigner/mkvcf.py
--rw-rw-r--   0 chigira   (1000) chigira   (1000)     1345 2023-06-19 04:58:14.000000 mkdesigner-0.0.1/mkdesigner/mvinputfiles.py
--rwxrwxr-x   0 chigira   (1000) chigira   (1000)    15238 2023-06-19 04:58:14.000000 mkdesigner-0.0.1/mkdesigner/params.py
--rwxrwxr-x   0 chigira   (1000) chigira   (1000)     1429 2023-06-19 04:58:14.000000 mkdesigner-0.0.1/mkdesigner/refindex.py
--rw-rw-r--   0 chigira   (1000) chigira   (1000)     4447 2023-06-19 04:58:14.000000 mkdesigner-0.0.1/mkdesigner/selectsnp.py
--rwxrwxr-x   0 chigira   (1000) chigira   (1000)      915 2023-06-19 04:58:14.000000 mkdesigner-0.0.1/mkdesigner/utils.py
--rw-rw-r--   0 chigira   (1000) chigira   (1000)     1481 2023-06-19 04:58:14.000000 mkdesigner-0.0.1/mkdesigner/visualize_marker.R
-drwxrwxr-x   0 chigira   (1000) chigira   (1000)        0 2023-06-19 10:12:45.191991 mkdesigner-0.0.1/mkdesigner.egg-info/
--rw-rw-r--   0 chigira   (1000) chigira   (1000)      280 2023-06-19 10:12:45.000000 mkdesigner-0.0.1/mkdesigner.egg-info/PKG-INFO
--rw-rw-r--   0 chigira   (1000) chigira   (1000)      554 2023-06-19 10:12:45.000000 mkdesigner-0.0.1/mkdesigner.egg-info/SOURCES.txt
--rw-rw-r--   0 chigira   (1000) chigira   (1000)        1 2023-06-19 10:12:45.000000 mkdesigner-0.0.1/mkdesigner.egg-info/dependency_links.txt
--rw-rw-r--   0 chigira   (1000) chigira   (1000)      120 2023-06-19 10:12:45.000000 mkdesigner-0.0.1/mkdesigner.egg-info/entry_points.txt
--rw-rw-r--   0 chigira   (1000) chigira   (1000)        7 2023-06-19 10:12:45.000000 mkdesigner-0.0.1/mkdesigner.egg-info/requires.txt
--rw-rw-r--   0 chigira   (1000) chigira   (1000)       11 2023-06-19 10:12:45.000000 mkdesigner-0.0.1/mkdesigner.egg-info/top_level.txt
--rw-rw-r--   0 chigira   (1000) chigira   (1000)       38 2023-06-19 10:12:45.191991 mkdesigner-0.0.1/setup.cfg
--rwxrwxr-x   0 chigira   (1000) chigira   (1000)      705 2023-06-19 09:57:24.000000 mkdesigner-0.0.1/setup.py
+drwxrwxr-x   0 chigira   (1000) chigira   (1000)        0 2023-07-10 01:16:16.402396 mkdesigner-0.1.1/
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)     1065 2023-06-19 04:58:14.000000 mkdesigner-0.1.1/LICENSE
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)       56 2023-06-19 06:54:28.000000 mkdesigner-0.1.1/MANIFEST.in
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)      280 2023-07-10 01:16:16.402396 mkdesigner-0.1.1/PKG-INFO
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)     4563 2023-07-10 01:01:21.000000 mkdesigner-0.1.1/README.md
+drwxrwxr-x   0 chigira   (1000) chigira   (1000)        0 2023-07-10 01:16:16.402396 mkdesigner-0.1.1/mkdesigner/
+-rwxrwxr-x   0 chigira   (1000) chigira   (1000)      248 2023-07-10 01:01:21.000000 mkdesigner-0.1.1/mkdesigner/__init__.py
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)    18652 2023-07-09 23:55:29.000000 mkdesigner-0.1.1/mkdesigner/addprimertovcf.py
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)     8159 2023-06-19 04:58:14.000000 mkdesigner-0.1.1/mkdesigner/haplocall.py
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)     2258 2023-07-05 23:07:26.000000 mkdesigner-0.1.1/mkdesigner/mergevcf.py
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)     2120 2023-07-09 23:45:50.000000 mkdesigner-0.1.1/mkdesigner/mkprimer.py
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)     8411 2023-07-10 00:40:25.000000 mkdesigner-0.1.1/mkdesigner/mkselect.py
+-rwxrwxr-x   0 chigira   (1000) chigira   (1000)     1940 2023-07-04 23:02:18.000000 mkdesigner-0.1.1/mkdesigner/mkvcf.py
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)     1345 2023-06-19 04:58:14.000000 mkdesigner-0.1.1/mkdesigner/mvinputfiles.py
+-rwxrwxr-x   0 chigira   (1000) chigira   (1000)    15951 2023-07-09 23:45:07.000000 mkdesigner-0.1.1/mkdesigner/params.py
+-rwxrwxr-x   0 chigira   (1000) chigira   (1000)     1429 2023-06-19 04:58:14.000000 mkdesigner-0.1.1/mkdesigner/refindex.py
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)     6584 2023-07-09 23:49:08.000000 mkdesigner-0.1.1/mkdesigner/selectvariants.py
+-rwxrwxr-x   0 chigira   (1000) chigira   (1000)      915 2023-06-19 04:58:14.000000 mkdesigner-0.1.1/mkdesigner/utils.py
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)     1481 2023-06-19 04:58:14.000000 mkdesigner-0.1.1/mkdesigner/visualize_marker.R
+drwxrwxr-x   0 chigira   (1000) chigira   (1000)        0 2023-07-10 01:16:16.402396 mkdesigner-0.1.1/mkdesigner.egg-info/
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)      280 2023-07-10 01:16:16.000000 mkdesigner-0.1.1/mkdesigner.egg-info/PKG-INFO
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)      559 2023-07-10 01:16:16.000000 mkdesigner-0.1.1/mkdesigner.egg-info/SOURCES.txt
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)        1 2023-07-10 01:16:16.000000 mkdesigner-0.1.1/mkdesigner.egg-info/dependency_links.txt
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)      120 2023-07-10 01:16:16.000000 mkdesigner-0.1.1/mkdesigner.egg-info/entry_points.txt
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)        7 2023-07-10 01:16:16.000000 mkdesigner-0.1.1/mkdesigner.egg-info/requires.txt
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)       11 2023-07-10 01:16:16.000000 mkdesigner-0.1.1/mkdesigner.egg-info/top_level.txt
+-rw-rw-r--   0 chigira   (1000) chigira   (1000)       38 2023-07-10 01:16:16.402396 mkdesigner-0.1.1/setup.cfg
+-rwxrwxr-x   0 chigira   (1000) chigira   (1000)      705 2023-06-19 09:57:24.000000 mkdesigner-0.1.1/setup.py
```

### Comparing `mkdesigner-0.0.1/LICENSE` & `mkdesigner-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdesigner-0.0.1/mkdesigner/addprimertovcf.py` & `mkdesigner-0.1.1/mkdesigner/addprimertovcf.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,16 @@
         no_primer = 0
         non_specific = 0
         success = 0
         #Multi processing
         ##############################################
         with Pool(self.cpu) as p:
             results = p.map(self.parallel, range(nrow))
+            #Each process returns list,
+            #[id(range(nrow)), exit status(0~2), Desciption added to INFO]
         #############################################
         for res in results:
             id = res[0]
             status = res[1]
             add_str = res[2]
             if status == 0:
                 no_primer += 1
@@ -154,42 +156,70 @@
             call_log(self.out, 'samtools', cmd)
             sys.exit(1)
         str_tmp = str.split('\n')
         str_list = [str_tmp[0][1:], ''.join(str_tmp[1:])]
         return str_list
     
     def make_primer3_input(self, series, st_out):
+        #Read INFO column of VCF data
         info = series['INFO'].split(';')
         for elem in info:
             elem_split = elem.split('=')
             if elem_split[0] == 'SPAN':
+                #'span' indicates the distance to the mutations
+                # that exist before and after the current variant.
                 span = elem_split[1].split(',')
                 span = list(map(int, span))
                 break
 
+        #Make parameters for primer3
         target_start = self.scope - self.args.margin + 1
         var_len = len(series['REF'])
         target_length = var_len + self.margin * 2
+        #Avoid designing primers at surrounding variants.
         exclude = ''
         if span[0] <= self.scope:
             exclude += '{},{}'.format(1, self.scope - span[0] + 1)
         if span[1] <= self.scope + var_len - 1:
             exclude += ' {},{}'.format(self.scope + span[1], self.scope - span[1] + var_len)
+        #For SNP markers, designated product length is used.
+        #For INDEL markers, product length is determined by 
+        # an expression with the size of INDEL as a variable.
+        if self.args.type == 'SNP' :
+            max_prd = self.args.max_prodlen
+            opt_prd = self.args.opt_prodlen
+            min_prd = self.args.min_prodlen
+        elif self.args.type == 'INDEL' :
+            X = abs(len(series['REF']) - len(series['ALT']))
+            if len(series['REF']) > len(series['ALT']) :
+                ref_shorter = 0
+                alt_shorter = X
+            else :
+                ref_shorter = X
+                alt_shorter = 0
+
+            if X < 5 :
+                max_prd = 100 - ref_shorter
+                opt_prd = 75 - ref_shorter
+            else:
+                max_prd = round((300 * X) / (10 + X) - ref_shorter)
+                opt_prd = round((max_prd * 0.75) - ref_shorter)
+            min_prd = 50 + alt_shorter
 
         primer3_data_list = [
             'SEQUENCE_ID={}\n'.format(st_out[0]),
             'SEQUENCE_TEMPLATE={}\n'.format(st_out[1]),
             'SEQUENCE_TARGET={},{}\n'.format(target_start, target_length),
             'SEQUENCE_EXCLUDED_REGION={}\n'.format(exclude),
             'PRIMER_NUM_RETURN={}\n'.format(self.args.primer_num_consider),
             'PRIMER_OPT_SIZE={}\n'.format(self.args.primer_opt_size),
             'PRIMER_MIN_SIZE={}\n'.format(self.args.primer_min_size),
             'PRIMER_MAX_SIZE={}\n'.format(self.args.primer_max_size),
-            'PRIMER_PRODUCT_OPT_SIZE={}\n'.format(self.args.opt_prodlen),
-            'PRIMER_PRODUCT_SIZE_RANGE={}-{}\n'.format(self.args.min_prodlen, self.args.max_prodlen),
+            'PRIMER_PRODUCT_OPT_SIZE={}\n'.format(opt_prd),
+            'PRIMER_PRODUCT_SIZE_RANGE={}-{}\n'.format(min_prd, max_prd),
             'PRIMER_OPT_GC_PERCENT=50.0\n',
             'PRIMER_MIN_GC=30.0\n',
             'PRIMER_MAX_GC=70.0\n',
             'PRIMER_MIN_TM=55.0\n',
             'PRIMER_OPT_TM=61.0\n',
             'PRIMER_MAX_TM=67.0\n',
             'PRIMER_PAIR_MAX_DIFF_TM=5.0\n',
```

### Comparing `mkdesigner-0.0.1/mkdesigner/haplocall.py` & `mkdesigner-0.1.1/mkdesigner/haplocall.py`

 * *Files identical despite different names*

### Comparing `mkdesigner-0.0.1/mkdesigner/mergevcf.py` & `mkdesigner-0.1.1/mkdesigner/mergevcf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sys
-import os
 import subprocess as sbp
 from mkdesigner.utils import time_stamp, prepare_cmd, call_log
 
 
 class MergeVcf(object):
 
     def __init__(self, args, is2nd=False):
```

### Comparing `mkdesigner-0.0.1/mkdesigner/mkprimer.py` & `mkdesigner-0.1.1/mkdesigner/mkprimer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python3
 
 from mkdesigner.addprimertovcf import AddPrimerToVcf
 from mkdesigner.params import Params
 from mkdesigner.refindex import RefIndex
-from mkdesigner.selectsnp import SelectSnp
+from mkdesigner.selectvariants import SelectVariants
 
 pm = Params('mkprimer')
 args = pm.set_options()
 
 import os
 import sys
 import subprocess as sbp
 from mkdesigner.utils import time_stamp, prepare_cmd
 
 class MKPrimer(object):
     def __init__(self, args):
+        pm.mkprimer_check_args(args)
         self.args = args
         self.ref = args.ref
         self.vcf = args.vcf
         self.name1 = args.name1
         self.name2 = args.name2
         self.type = args.type
         self.proj = args.project
@@ -45,30 +46,30 @@
             print('Error occored at moving input files to the working directory.',flush=True)
             sys.exit(1)
 
     def refindex(self):
         ri = RefIndex(self.args)
         ri.run()
 
-    def selectsnp(self):
-        ss = SelectSnp(self.args)
+    def selectvariants(self):
+        ss = SelectVariants(self.args)
         ss.run()
 
     def addprimertovcf(self):
         ad = AddPrimerToVcf(self.args)
         ad.run()
 
 def main():
     print(time_stamp(), 'MKPrimer started.', flush=True)
 
     prog = MKPrimer(args)
     prog.mkdir()
     prog.mvinputfiles()
     prog.refindex()
-    prog.selectsnp()
+    prog.selectvariants()
     prog.addprimertovcf()
     
     print(time_stamp(), 'MKPrimer successfully finished.\n', flush=True)
 
 if __name__ == '__main__':
     main()
```

### Comparing `mkdesigner-0.0.1/mkdesigner/mkselect.py` & `mkdesigner-0.1.1/mkdesigner/mkselect.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,27 +166,25 @@
 
         print(time_stamp(), '{} markers were selected.\n'.format(len(self.data_s)), flush=True)
 
     def draw(self):
         out_vcf_name = str(self.vcf).replace('.vcf', '_{}mk_selected_{}.vcf'.format(self.num_marker, self.target))
         out_png_name = str(self.vcf).replace('.vcf', '_{}mk_selected_{}.png'.format(self.num_marker, self.target))
         path = os.path.dirname(os.path.abspath(__file__))
-        print(out_vcf_name)
-        print(out_png_name)
-        print(path)
         cmd1 = 'Rscript {}/visualize_marker.R {} {} {}'.format(path, out_vcf_name, self.fai, out_png_name)
         cmd1 = prepare_cmd(cmd1)
         try:
             sbp.run(cmd1,
                     stdout=sbp.DEVNULL,
                     stderr=sbp.DEVNULL,
                     shell=True, check=True)
         except sbp.CalledProcessError:
             print(time_stamp(),
-              'Error occured drawing marker position.',
+              'Error occured drawing marker position. '
+              'Maybe File name of fasta index is wrong.',
               flush=True)
             sys.exit(1) 
         
 
 def main():
     print(time_stamp(), 'MKSelect started.', flush=True)
```

### Comparing `mkdesigner-0.0.1/mkdesigner/mkvcf.py` & `mkdesigner-0.1.1/mkdesigner/mkvcf.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 from mkdesigner.refindex import RefIndex
 from mkdesigner.haplocall import HaploCall
 from mkdesigner.mergevcf import MergeVcf
 
 class MKVcf(object):
 
     def __init__(self, args):
-        self.N_bam = pm.check_args(args)
+        pm.mkvcf_check_args(args)
         self.args = args
-        #self.ref = args.ref
         self.bam = args.bam
+        self.N_bam = len(args.bam)
         self.name = args.name
         self.proj = args.project
         self.cpu = args.cpu
 
     def mkdir(self):
         os.mkdir('{}'.format(self.proj))
         os.mkdir('{}/log'.format(self.proj))
```

### Comparing `mkdesigner-0.0.1/mkdesigner/mvinputfiles.py` & `mkdesigner-0.1.1/mkdesigner/mvinputfiles.py`

 * *Files identical despite different names*

### Comparing `mkdesigner-0.0.1/mkdesigner/params.py` & `mkdesigner-0.1.1/mkdesigner/params.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         else:
             args = parser.parse_args()
         return args
     
     def mkvcf_options(self):
         parser = argparse.ArgumentParser(description='MKDesigner version {}'.format(__version__),
                                          formatter_class=argparse.RawTextHelpFormatter)
-        parser.usage = ('mkvcf -r <FASTA> -b <BAM> -n <name> -p <Project name>\n')
+        parser.usage = ('mkvcf -r <FASTA> -b <BAM_1> -b <BAM_2>... -n <name_1> -n <name_2>... -p <Project name>\n')
 
         # set options
         parser.add_argument('-r', '--ref',
                             action='store',
                             required=True,
                             type=str,
                             help='Reference fasta.',
@@ -99,27 +99,29 @@
                             type=str,
                             help=('VCF file without filtering.\n'
                                   'Recommended to use VCF made by "mkvcf" command.\n'
                                   'VCF must contain GT and DP field.'),
                             metavar='')
         
         parser.add_argument('-n1', '--name1',
-                            action='store',
+                            action='append',
                             required=True,
                             type=str,
                             help=('Variety name 1.\n'
-                                  'Must match VCF column names'),
+                                  'Must match VCF column names.\n'
+                                  'This parameter can be specified multiple times to design common markers for multiple varieties.\n'),
                             metavar='')
         
         parser.add_argument('-n2', '--name2',
-                            action='store',
+                            action='append',
                             required=True,
                             type=str,
                             help=('Variety name 2.\n'
-                                  'Must match VCF column names'),
+                                  'Must match VCF column names.\n'
+                                  'This parameter can be specified multiple times to design common markers for multiple varieties.\n'),
                             metavar='')
         
         parser.add_argument('-p', '--project',
                             action='store',
                             required=True,
                             type=str,
                             help=('Name of project (must be unique).\n'
@@ -148,18 +150,18 @@
                             type=int,
                             help=('Variants with less depth than this\n'
                                   'are judged as valid mutations\ndefault: 200'),
                             metavar='')
         
         parser.add_argument('--mismatch_allowed',
                             action='store',
-                            default=3,
+                            default=5,
                             type=int,
                             help=('Primers with more mismatch than this\n'
-                                  'are ignored in specificity check.\ndefault: 3'),
+                                  'are ignored in specificity check.\ndefault: 5'),
                             metavar='')  
         
         parser.add_argument('--mismatch_allowed_3_terminal',
                             action='store',
                             default=1,
                             type=int,
                             help=('Primers with more mismatch than this\n'
@@ -316,31 +318,41 @@
 
         # set version
         parser.add_argument('-v', '--version',
                             action='version',
                             version='%(prog)s {}'.format(__version__))
         return parser
     
-    def check_args(self, args):
+    def mkvcf_check_args(self, args):
+        #Does a project file with the same name exist?
         if os.path.isdir(args.project):
             sys.stderr.write(('  Output directory already exist.\n'
                               '  Please rename the project name.\n'))
             sys.exit(1)
 
+        #Is the extentions of files designeated as BAM really '.bam' ?
         for input_name in args.bam:
-                root, ext = os.path.splitext(input_name) #get extention as 'ext'
-                if ext != '.bam':
-                    sys.stderr.write(('  Please check "{}".\n'
-                                      '  The extension of this file is not "bam".\n'
-                                      '  If you wanted to specify fastq, please '
-                                        'input them as paired-end reads which is separated '
-                                        'by comma. e.g. -p fastq1,fastq2\n\n').format(input_name))
+                ext = os.path.splitext(input_name)
+                if ext[-1] != '.bam':
+                    sys.stderr.write(('  Please check input BAM file "{}".\n'
+                                      '  The extension of this file is not "bam".\n').format(input_name))
                     sys.exit(1)
 
-        N_bam = len(args.bam)
-
-        if N_bam != len(args.name) :
+        #Do the number of BAM and the number of names match?
+        if len(args.bam) != len(args.name) :
             sys.stderr.write(('  Number of input BAM files is not'
                               '  matched the number of names.\n\n'))
             sys.exit(1)
 
-        return N_bam
+        #Names must be unique.
+        name_unique = set(args.name)
+        if len(args.name) != len(name_unique) :
+            sys.stderr.write(('  Variety names must not be duplicated.\n\n'))
+            sys.exit(1)
+
+    def mkprimer_check_args(self, args):
+        #Does a project file with the same name exist?
+        if os.path.isdir(args.project):
+            sys.stderr.write(('  Output directory already exist.\n'
+                              '  Please rename the project name.\n'))
+            sys.exit(1)
+
```

### Comparing `mkdesigner-0.0.1/mkdesigner/refindex.py` & `mkdesigner-0.1.1/mkdesigner/refindex.py`

 * *Files identical despite different names*

### Comparing `mkdesigner-0.0.1/mkdesigner/utils.py` & `mkdesigner-0.1.1/mkdesigner/utils.py`

 * *Files identical despite different names*

### Comparing `mkdesigner-0.0.1/mkdesigner/visualize_marker.R` & `mkdesigner-0.1.1/mkdesigner/visualize_marker.R`

 * *Files identical despite different names*

### Comparing `mkdesigner-0.0.1/mkdesigner.egg-info/SOURCES.txt` & `mkdesigner-0.1.1/mkdesigner.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 mkdesigner/mergevcf.py
 mkdesigner/mkprimer.py
 mkdesigner/mkselect.py
 mkdesigner/mkvcf.py
 mkdesigner/mvinputfiles.py
 mkdesigner/params.py
 mkdesigner/refindex.py
-mkdesigner/selectsnp.py
+mkdesigner/selectvariants.py
 mkdesigner/utils.py
 mkdesigner/visualize_marker.R
 mkdesigner.egg-info/PKG-INFO
 mkdesigner.egg-info/SOURCES.txt
 mkdesigner.egg-info/dependency_links.txt
 mkdesigner.egg-info/entry_points.txt
 mkdesigner.egg-info/requires.txt
```

### Comparing `mkdesigner-0.0.1/setup.py` & `mkdesigner-0.1.1/setup.py`

 * *Files identical despite different names*

