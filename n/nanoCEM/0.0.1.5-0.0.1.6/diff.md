# Comparing `tmp/nanoCEM-0.0.1.5.tar.gz` & `tmp/nanoCEM-0.0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.1.5.tar", last modified: Wed Jul  5 04:51:42 2023, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.1.6.tar", last modified: Mon Jul 10 08:05:28 2023, max compression
```

## Comparing `nanoCEM-0.0.1.5.tar` & `nanoCEM-0.0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-05 04:51:42.351661 nanoCEM-0.0.1.5/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.1.5/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-05 04:51:42.351661 nanoCEM-0.0.1.5/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8388 2023-07-03 09:59:45.000000 nanoCEM-0.0.1.5/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-05 04:51:42.351661 nanoCEM-0.0.1.5/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9423 2023-07-04 09:33:19.000000 nanoCEM-0.0.1.5/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.1.5/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 nanoCEM-0.0.1.5/nanoCEM/cem_utils.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7706 2023-07-05 04:51:31.000000 nanoCEM-0.0.1.5/nanoCEM/current_events_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.1.5/nanoCEM/extract_sub_fast5_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.1.5/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7727 2023-06-26 15:00:04.000000 nanoCEM-0.0.1.5/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10994 2023-07-03 10:50:36.000000 nanoCEM-0.0.1.5/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13843 2023-07-05 03:24:20.000000 nanoCEM-0.0.1.5/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-05 04:51:42.351661 nanoCEM-0.0.1.5/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-05 04:51:42.000000 nanoCEM-0.0.1.5/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      429 2023-07-05 04:51:42.000000 nanoCEM-0.0.1.5/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-05 04:51:42.000000 nanoCEM-0.0.1.5/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-07-05 04:51:42.000000 nanoCEM-0.0.1.5/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-05 04:51:42.000000 nanoCEM-0.0.1.5/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-05 04:51:42.351661 nanoCEM-0.0.1.5/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1152 2023-07-05 04:51:41.000000 nanoCEM-0.0.1.5/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-10 08:05:28.064364 nanoCEM-0.0.1.6/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.1.6/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-10 08:05:28.064364 nanoCEM-0.0.1.6/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8388 2023-07-03 09:59:45.000000 nanoCEM-0.0.1.6/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-10 08:05:28.064364 nanoCEM-0.0.1.6/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9561 2023-07-10 08:02:19.000000 nanoCEM-0.0.1.6/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.1.6/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 nanoCEM-0.0.1.6/nanoCEM/cem_utils.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7836 2023-07-10 08:03:26.000000 nanoCEM-0.0.1.6/nanoCEM/current_events_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.1.6/nanoCEM/extract_sub_fast5_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.1.6/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7818 2023-07-05 10:48:45.000000 nanoCEM-0.0.1.6/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11478 2023-07-10 08:05:02.000000 nanoCEM-0.0.1.6/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-06 04:15:59.000000 nanoCEM-0.0.1.6/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-10 08:05:28.064364 nanoCEM-0.0.1.6/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-10 08:05:28.000000 nanoCEM-0.0.1.6/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      429 2023-07-10 08:05:28.000000 nanoCEM-0.0.1.6/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-10 08:05:28.000000 nanoCEM-0.0.1.6/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-07-10 08:05:28.000000 nanoCEM-0.0.1.6/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-10 08:05:28.000000 nanoCEM-0.0.1.6/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-10 08:05:28.064364 nanoCEM-0.0.1.6/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1152 2023-07-10 08:05:20.000000 nanoCEM-0.0.1.6/setup.py
```

### Comparing `nanoCEM-0.0.1.5/LICENSE` & `nanoCEM-0.0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.5/PKG-INFO` & `nanoCEM-0.0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.1.5
+Version: 0.0.1.6
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nanoCEM-0.0.1.5/README.md` & `nanoCEM-0.0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.5/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.1.6/nanoCEM/CE_magnifier_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 import argparse
 import os
-from cem_utils import read_fasta_to_dic,reverse_fasta
+from nanoCEM.cem_utils import read_fasta_to_dic,reverse_fasta
 import pandas as pd
-from plot import signal_plot
+from nanoCEM.plot import signal_plot
 from plotnine.exceptions import PlotnineWarning
 import warnings
 import time
 warnings.filterwarnings("ignore", category=PlotnineWarning)
 import numpy as np
 def init_parser():
     def add_public_argument(parser_input):
         parser_input.add_argument("--chrom", required=True, help="Gene or chromosome name(head of your fasta file)")
         parser_input.add_argument("--pos", required=True, type=int, help="site of your interest")
         parser_input.add_argument("--len", default=10, type=int, help="region around the position")
         parser_input.add_argument("--strand", default="+", help="Strand of your interest")
         parser_input.add_argument("--ref", required=True, help="fasta file")
+        parser_input.add_argument('--norm', action='store_true', help='normalization mode')
         parser_input.add_argument("--overplot-number", default=500, type=int,
                                   help="Number of read will be used to plot")
         parser_input.add_argument('--rna', action='store_true', help='RNA mode')
     # Define the argument parser
     parser = argparse.ArgumentParser(description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level. It supports two re-squiggle pipeline(Tombo and f5c).')
     subparsers = parser.add_subparsers(dest='function')
 
@@ -40,30 +41,31 @@
     # f5c subparser
     parser_f5c = subparsers.add_parser('f5c', help='tackle f5c re-squiggle')
     parser_f5c.add_argument("-i", "--input", required=True,
                         help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
                         help="control_blow5_path")
     parser_f5c.add_argument('-o', "--output", default="f5c_result", help="output_file")
+
     parser_f5c.add_argument('--base_shift',type=int, default=0, help="output_file")
     add_public_argument(parser_f5c)
     # parser.set_defaults(function='tombo', chrom="1", pos=150280972, len=10, strand='+', cpu=1,input_fast5='/data/current_test_data/samp/cem_test_dna/WGS/single/',\
     #                     control_fast5='/data/current_test_data/samp/cem_test_dna/WGA/single/',output='tombo_result_dna',\
     #                     overplot_number=300,ref="/data/current_test_data/samp/cem_test_dna/hg.fa",\
     #                     basecall_group="RawGenomeCorrected_000", basecall_subgroup="BaseCalled_template",rna=False)
-    parser.set_defaults(function='tombo', chrom="NR_103073.1", pos=2030, len=10, strand='+', cpu=8,input_fast5='/data/Ecoli_23s/data/L_rep2/single/',\
-                        control_fast5='/data/Ecoli_23s/data/IVT_negative/single/',output='tombo_result_rna',overplot_number=500,\
-                        ref="/data/Ecoli_23s/23S_rRNA.fasta",\
-                         basecall_group="RawGenomeCorrected_000", basecall_subgroup="BaseCalled_template",rna=True)
-    # parser.set_defaults(function='f5c', chrom="NR_103073.1", pos=875, len=10, strand='-', cpu=4,input='/data/Ecoli_23s/data/L_rep2/file',\
-    #                     control='/data/Ecoli_23s/data/IVT_negative/file',\
-    #                     output='f5c_result_rna_new_re',overplot_number=1000,ref="/data/Ecoli_23s/23S_rRNA_reverse.fasta",rna=True,base_shift=2)
-    # parser.set_defaults(function='f5c', chrom="1", pos=150280972, len=10, strand='+', cpu=4,input='/data/current_test_data/samp/cem_test_dna/WGS/file',\
-    #                     control='/data/current_test_data/samp/cem_test_dna/WGA/file',\
-    #                     output='f5c_result_dna_new',overplot_number=1000,ref="/data/current_test_data/samp/cem_test_dna/hg.fa",rna=False,base_shift=2)
+    # parser.set_defaults(function='tombo', chrom="NR_103073.1", pos=2030, len=10, strand='+', cpu=8,input_fast5='/data/Ecoli_23s/data/L_rep2/single/',\
+    #                     control_fast5='/data/Ecoli_23s/data/IVT_negative/single/',output='tombo_result_rna',overplot_number=500,\
+    #                     ref="/data/Ecoli_23s/23S_rRNA.fasta",\
+    #                      basecall_group="RawGenomeCorrected_000", basecall_subgroup="BaseCalled_template",rna=True)
+    parser.set_defaults(function='f5c', chrom="NR_103073.1", pos=2030, len=10, strand='+', cpu=4,input='/data/Ecoli_23s/data/L_rep2/file',\
+                        control='/data/Ecoli_23s/data/IVT_negative/file',\
+                        output='f5c_result_rna_new_re',overplot_number=1000,ref="/data/Ecoli_23s/23S_rRNA.fasta",rna=True,base_shift=0,norm=True)
+    # parser.set_defaults(function='f5c', chrom="1", pos=148545690, len=10, strand='+', cpu=4,input='/data/current_test_data/r1041_test/file',\
+    #                     control='/data/current_test_data/r1041_wga/file',\
+    #                     output='f5c_result_dna_new_norm',overplot_number=1000,ref="/data/current_test_data/r1041_test/hg38.fa",rna=False,base_shift=2,norm=False)
 
     return parser
 
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
     args = parser.parse_args()
@@ -125,21 +127,21 @@
         from nanoCEM.read_f5c_resquiggle import read_blow5
         if args.base_shift < 0:
             raise RuntimeError("base_shift should not less than 0")
         # if (args.rna and args.strand=='+') or (not args.rna and args.strand=='-'):
         #     args.pos = args.pos + args.base_shift
         # else:
         #     args.pos = args.pos - args.base_shift
-        df_wt, aligned_num_wt,nucleotide_type = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand,subsample_num,args.base_shift)
+        df_wt, aligned_num_wt,nucleotide_type = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand,subsample_num,args.base_shift,args.norm)
         df_wt['type'] = 'Sample'
         if nucleotide_type=='RNA' and not args.rna:
             raise RuntimeError("You need to add --rna to turn on the rna mode")
         try:
             df_ivt, aligned_num_ivt,_ = read_blow5(args.control, args.pos, args.len, args.chrom, args.strand,
-                                                 subsample_num)
+                                                 subsample_num,args.base_shift,args.norm)
             df_ivt['type'] = 'Control'
 
             df = pd.concat([df_wt, df_ivt])
             category = pd.api.types.CategoricalDtype(categories=['Sample', "Control"], ordered=True)
             df['type'] = df['type'].astype(category)
 
             title = title + '   Sample:' + str(aligned_num_wt) + '  Control:' + str(aligned_num_ivt)
```

### Comparing `nanoCEM-0.0.1.5/nanoCEM/cem_utils.py` & `nanoCEM-0.0.1.6/nanoCEM/cem_utils.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.5/nanoCEM/current_events_magnifier.py` & `nanoCEM-0.0.1.6/nanoCEM/current_events_magnifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 def init_parser():
     def add_public_argument(parser_input):
         parser_input.add_argument("--chrom", required=True, help="Gene or chromosome name(head of your fasta file)")
         parser_input.add_argument("--pos", required=True, type=int, help="site of your interest")
         parser_input.add_argument("--len", default=10, type=int, help="region around the position")
         parser_input.add_argument("--strand", default="+", help="Strand of your interest")
         parser_input.add_argument("--ref", required=True, help="fasta file")
-        parser_input.add_argument("--overplot_number", default=500, type=int,
+        parser_input.add_argument('--norm', action='store_true', help='normalization mode')
+        parser_input.add_argument("--overplot-number", default=500, type=int,
                                   help="Number of read will be used to plot")
         parser_input.add_argument('--rna', action='store_true', help='RNA mode')
     # Define the argument parser
     parser = argparse.ArgumentParser(description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level. It supports two re-squiggle pipeline(Tombo and f5c).')
     subparsers = parser.add_subparsers(dest='function')
 
     # tombo subparser
@@ -40,14 +41,15 @@
     # f5c subparser
     parser_f5c = subparsers.add_parser('f5c', help='tackle f5c re-squiggle')
     parser_f5c.add_argument("-i", "--input", required=True,
                         help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
                         help="control_blow5_path")
     parser_f5c.add_argument('-o', "--output", default="f5c_result", help="output_file")
+
     parser_f5c.add_argument('--base_shift',type=int, default=0, help="output_file")
     add_public_argument(parser_f5c)
     return parser
 
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
@@ -84,15 +86,15 @@
         print("Output file existed! It will be overwrite after 5 secs ...")
         time.sleep(5)
         print("Continue ...")
 
 
     if args.function == 'tombo' :
 
-        from nanoCEM.read_tombo_resquiggle import create_read_list_file,extract_group
+        from  nanoCEM.read_tombo_resquiggle import create_read_list_file,extract_group
         wt_file = create_read_list_file(args.input_fast5, results_path)
         df_wt, aligned_num_wt = extract_group(args, wt_file, subsample_num)
         df_wt['type'] = 'Sample'
         try:
             ivt_file = create_read_list_file(args.control_fast5, results_path)
             df_ivt, aligned_num_ivt = extract_group(args, ivt_file, subsample_num)
             df_ivt['type'] = 'Control'
@@ -110,21 +112,21 @@
         from nanoCEM.read_f5c_resquiggle import read_blow5
         if args.base_shift < 0:
             raise RuntimeError("base_shift should not less than 0")
         # if (args.rna and args.strand=='+') or (not args.rna and args.strand=='-'):
         #     args.pos = args.pos + args.base_shift
         # else:
         #     args.pos = args.pos - args.base_shift
-        df_wt, aligned_num_wt,nucleotide_type = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand,subsample_num,args.base_shift)
+        df_wt, aligned_num_wt,nucleotide_type = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand,subsample_num,args.base_shift,args.norm)
         df_wt['type'] = 'Sample'
         if nucleotide_type=='RNA' and not args.rna:
             raise RuntimeError("You need to add --rna to turn on the rna mode")
         try:
             df_ivt, aligned_num_ivt,_ = read_blow5(args.control, args.pos, args.len, args.chrom, args.strand,
-                                                 subsample_num)
+                                                 subsample_num,args.base_shift,args.norm)
             df_ivt['type'] = 'Control'
 
             df = pd.concat([df_wt, df_ivt])
             category = pd.api.types.CategoricalDtype(categories=['Sample', "Control"], ordered=True)
             df['type'] = df['type'].astype(category)
 
             title = title + '   Sample:' + str(aligned_num_wt) + '  Control:' + str(aligned_num_ivt)
```

### Comparing `nanoCEM-0.0.1.5/nanoCEM/extract_sub_fast5_from_bam.py` & `nanoCEM-0.0.1.6/nanoCEM/extract_sub_fast5_from_bam.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.5/nanoCEM/normalization.py` & `nanoCEM-0.0.1.6/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.5/nanoCEM/plot.py` & `nanoCEM-0.0.1.6/nanoCEM/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,17 +141,19 @@
         else:
             plot1 = plot + p9.geom_boxplot(outlier_shape='', position=p9.position_dodge(0.9), size=0.2, width=0.75,alpha = 0.8)
             plot1.save(filename=results_path + "/Merged_boxplot.pdf", dpi=300)
             plot2 = plot + p9.geom_violin(style='left-right', position=p9.position_dodge(0), color='none', width=1.5,alpha = 0.8)
             plot2.save(filename=results_path + "/Merged_violin.pdf", dpi=300)
 
 
-def draw_signal(df, start, base):
+def draw_signal(df, start, base,start_index,end_index):
     df = pd.DataFrame(df)
     df.columns = ['raw']
+    start=start[start_index:end_index]
+    df=df[start[0]:start[-1]]
     df = df.reset_index()
     plot = p9.ggplot(df, p9.aes(x='index', y="raw")) \
            + p9.theme_bw() \
            + p9.geom_line() \
            + p9.theme(
         figure_size=(6, 3),
         panel_grid_minor=p9.element_blank(),
@@ -161,11 +163,11 @@
         strip_text=p9.element_text(size=13),
         legend_position='none',
         strip_background=p9.element_rect(alpha=0)
     )
     # plot.save(filename="/home/zhguo/Dropbox/@labfiles/projects/GUO/ONT_showcase_tool/plot/signal.pdf", dpi=300)
     for item in start:
         plot = plot + p9.geom_vline(xintercept=item, linetype='dashed', color='red')
-    print(base)
+    print(plot)
     # plot.save(filename="/home/zhguo/Dropbox/@labfiles/projects/GUO/ONT_showcase_tool/plot/norm_signal_aligned.pdf", dpi=300)
 
     print(1)
```

### Comparing `nanoCEM-0.0.1.5/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.1.6/nanoCEM/read_f5c_resquiggle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import re
 import numpy as np
 import pandas as pd
 import pyslow5
 import pysam
 from tqdm import tqdm
 from nanoCEM.normalization import normalize_signal,normalize_signal_with_lim
+# from nanoCEM.plot import draw_signal
 import os
 import argparse
 score_dict={}
 nucleotide_type=None
-def extract_feature(line,strand,base_shift=2):
+def extract_feature(line,strand,base_shift=2,norm=True):
     global nucleotide_type
     pbar.update(1)
     read_id = line[0]
     # if read_id !='562eeb47-2b86-4fc7-abfc-5dce62f511ed':
     #     return None
     if read_id not in info_dict:
         return None
@@ -68,29 +69,32 @@
     signal = signal[start_index:end_index]
     if nucleotide_type=='RNA':
         signal = np.flip(signal)
         event_length = np.flip(event_length)
 
     event_starts = event_length.cumsum()
     event_starts = np.insert(event_starts, 0, 0)[:-1]
+    if norm:
+        signal = normalize_signal_with_lim(signal)
 
     # filter too short or long dwell time
     # dwell_filter_pctls = (0.5, 99.5)
     # dwell_min, dwell_max = np.percentile(event_length, dwell_filter_pctls)
     # valid_bases = np.logical_and.reduce(
     #     (
     #         event_length > dwell_min,
     #         event_length < dwell_max,
     #         np.logical_not(np.isnan(event_length)),
     #     )
     # )
     # event_length[~valid_bases] = 0
 
     # normalized signal
-    signal = normalize_signal_with_lim(signal)
+    # draw_signal(signal, event_starts,None, 8850,8855)
+
 
     # index query and reference
     aligned_pair=info_dict[read_id]['pairs']
     qlen = info_dict[read_id]['query_length']
     # correct index about DNA and RNA
     if nucleotide_type == 'RNA':
         if strand == '+':
@@ -137,16 +141,16 @@
 
     result_dict={}
     for read in bam_file.fetch(chromosome,position-length, position+length+1):
         if strand == '+' and read.is_reverse:
             continue
         if strand == '-' and not read.is_reverse:
             continue
-        if read.qname == '5f8b9471-64e7-4dd8-b80c-5f88b77edbbe':
-            print(1)
+        # if read.qname == '7dcec2bc-65f3-41fe-8981-dd3af9fa6e67':
+        #     print(1)
         start_position=read.reference_start
         end_position=read.reference_end
         if position < start_position or position > end_position:
             continue
         # unit
         aligned_pair = np.array(read.aligned_pairs)
         aligned_pair = pd.DataFrame(aligned_pair)
@@ -159,38 +163,44 @@
         temp['pairs']=aligned_pair
         temp['query_length'] = read.query_length
         result_dict[read.qname] = temp
     return result_dict
 
 
 
-def read_blow5(path,position,length,chromo,strand,subsapmle_num=500,base_shift=2):
+def read_blow5(path,position,length,chromo,strand,subsapmle_num=500,base_shift=2,norm=True):
     global info_dict,s5,pbar
-    bam_file=path+".bam"
+    bam_file = path+".bam"
+    if not os.path.exists(path+'.bam'):
+        raise RuntimeError(path+'.bam' +"is not exist in your path!")
+    if not os.path.exists(path+'.paf'):
+        raise RuntimeError(path+'.paf' +"is not exist in your path!")
+    if not os.path.exists(path+'.blow5'):
+        raise RuntimeError(path+'.blow5' +"is not exist in your path!")
     bam_file=pysam.AlignmentFile(bam_file,'rb')
     # if rna_mode:
     #     if strand =='+':
     #         position=position+ (kmer_model-1)
     #     else:
     #         position=position- (kmer_model-1)
     info_dict=extract_pairs_pos(bam_file,position,length,chromo,strand)
     if info_dict == {}:
-        raise Exception("There is no read aligned on this position")
+        raise RuntimeError("There is no read aligned on this position")
     info_df = pd.DataFrame(list(info_dict.keys()))
     slow5 = path+".blow5"
     s5 = pyslow5.Open(slow5, 'r')
 
     df=pd.read_csv(path+".paf",sep='\t',header=None)
     df=pd.merge(df,info_df,how='inner',on=0)
     if df.shape[0] == 0:
         raise RuntimeError("cannot found the record from bam in your paf file. Please check your f5c command ... ")
     if df.shape[0] / info_df.shape[0] < 0.8:
         print('There are '+str(info_df.shape[0]-df.shape[0])+" reads not found in your paf file ...")
     pbar = tqdm(total=df.shape[0], position=0, leave=True)
-    df["feature"] = df.apply(extract_feature,strand=strand,base_shift=base_shift,axis=1)
+    df["feature"] = df.apply(extract_feature,strand=strand,base_shift=base_shift,norm=norm,axis=1)
     pbar.close()
     df.dropna(inplace=True)
     num_aligned = df.shape[0]
     if subsapmle_num < df.shape[0]:
         df=df.sample(n=subsapmle_num)
     final_feature=[]
     for item in df["feature"]:
@@ -200,15 +210,15 @@
     # if rna_mode:
     #     if strand == '+':
     #         final_feature['position']=final_feature['position'] - (kmer_model-1)
     #     else:
     #         final_feature['position']=final_feature['position'] + (kmer_model-1)
 
     final_feature['position'] = final_feature['position'].astype(int).astype(str)
-    print('\nextracted ', num_aligned, ' aligned reads from blow5 files')
+    print('Extracted ', num_aligned, ' aligned reads from blow5 files')
 
     if num_aligned>50:
         dwell_filter_pctls = (0.5, 99.5)
         dwell_min, dwell_max = np.percentile(final_feature['Dwell time'].values, dwell_filter_pctls)
         final_feature = final_feature[(final_feature['Dwell time'] > dwell_min) & (final_feature['Dwell time'] < dwell_max)]
 
     return final_feature,num_aligned,nucleotide_type
```

### Comparing `nanoCEM-0.0.1.5/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.1.6/nanoCEM/read_tombo_resquiggle.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     fast5_data.close()
     # ~ label_data = np.array(
     # ~ list(zip(event_starts, event_lengths, event_bases)),
     # ~ dtype=[('start', '<u4'), ('length', '<u4'), ('base', 'S1')])
     return (raw_dat, event_bases, event_starts, event_lengths,start_position,strand,chrome)
 
 
-def extract_feature(signal, event_start, event_length, base,start_position,end_position,strand):
+def extract_feature(signal, event_start, event_length, base,start_position,end_position,strand,norm=True):
     global BASE_LIST
     position=FLAG.pos
     if strand == '+':
         current_index = position-start_position
     else:
         current_index = end_position - position - 1
     if current_index-FLAG.len < 0:
@@ -100,15 +100,16 @@
     # uniq_arr = np.unique(signal)
     # signal = (signal - np.median(uniq_arr)) / float(robust.mad(uniq_arr))
     # normalization
 
     signal = signal[event_start[0]:event_start[-1] + event_length[-1]]
 
     event_start = event_start-event_start[0]
-    signal = normalize_signal_with_lim(signal)
+    if norm:
+        signal = normalize_signal_with_lim(signal)
 
     # filter too short or long dwell time
     # dwell_filter_pctls = (5, 95)
     # dwell_min, dwell_max = np.percentile(event_length, dwell_filter_pctls)
     # valid_bases = np.logical_and.reduce(
     #     (
     #         event_length > dwell_min,
@@ -156,15 +157,15 @@
 
     # ~ print(input_file,raw_start,raw_length,raw_label)
     total_seq = "".join([x.decode() for x in raw_label])
     base_len=raw_label.shape[0]
     end_position = start_position+base_len
     if mode:
         raw_data = np.flip(raw_data)
-    matrix_feature = extract_feature(raw_data, raw_start, raw_length, total_seq,start_position,end_position,strand)
+    matrix_feature = extract_feature(raw_data, raw_start, raw_length, total_seq,start_position,end_position,strand,FLAG.norm)
     if matrix_feature is None:
         return None
     del raw_data
 
     return matrix_feature
 
 def extract_group(args, total_fl,subsapmle_num=500):
```

### Comparing `nanoCEM-0.0.1.5/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.1.6/nanoCEM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.1.5
+Version: 0.0.1.6
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nanoCEM-0.0.1.5/setup.py` & `nanoCEM-0.0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.1.5",
+    version="0.0.1.6",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
```

