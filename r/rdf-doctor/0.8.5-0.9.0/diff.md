# Comparing `tmp/rdf_doctor-0.8.5-py3-none-any.whl.zip` & `tmp/rdf_doctor-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18942 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-04 08:21 doctor/__init__.py
--rw-r--r--  2.0 unx      631 b- defN 23-Jun-19 02:18 doctor/consts.py
--rw-r--r--  2.0 unx    32735 b- defN 23-Jul-04 07:45 doctor/doctor.py
--rw-r--r--  2.0 unx    20305 b- defN 23-Jun-19 02:18 doctor/reference/correct-prefixes.tsv
--rw-r--r--  2.0 unx       90 b- defN 23-Jun-19 02:18 doctor/reference/refine-classes.tsv
--rw-r--r--  2.0 unx      679 b- defN 23-Jun-19 02:18 doctor/reference/refine-prefixes.tsv
--rw-r--r--  2.0 unx     1061 b- defN 23-Jul-04 08:25 rdf_doctor-0.8.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     9140 b- defN 23-Jul-04 08:25 rdf_doctor-0.8.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 08:25 rdf_doctor-0.8.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-04 08:25 rdf_doctor-0.8.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-04 08:25 rdf_doctor-0.8.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      994 b- defN 23-Jul-04 08:25 rdf_doctor-0.8.5.dist-info/RECORD
-12 files, 65808 bytes uncompressed, 17258 bytes compressed:  73.8%
+Zip file size: 23562 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-10 00:48 doctor/__init__.py
+-rw-r--r--  2.0 unx      631 b- defN 23-Jul-10 00:40 doctor/consts.py
+-rw-r--r--  2.0 unx    36220 b- defN 23-Jul-10 00:40 doctor/doctor.py
+-rw-r--r--  2.0 unx    43474 b- defN 23-Jul-10 00:40 doctor/reference/prefixes.tsv
+-rw-r--r--  2.0 unx       90 b- defN 23-Jul-10 00:40 doctor/reference/refine-class-uris.tsv
+-rw-r--r--  2.0 unx      679 b- defN 23-Jul-10 00:40 doctor/reference/refine-prefix-uris.tsv
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jul-10 00:54 rdf_doctor-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9892 b- defN 23-Jul-10 00:54 rdf_doctor-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 00:54 rdf_doctor-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-10 00:54 rdf_doctor-0.9.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-10 00:54 rdf_doctor-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      992 b- defN 23-Jul-10 00:54 rdf_doctor-0.9.0.dist-info/RECORD
+12 files, 93212 bytes uncompressed, 21882 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -3,35 +3,35 @@
 
 Filename: doctor/consts.py
 Comment: 
 
 Filename: doctor/doctor.py
 Comment: 
 
-Filename: doctor/reference/correct-prefixes.tsv
+Filename: doctor/reference/prefixes.tsv
 Comment: 
 
-Filename: doctor/reference/refine-classes.tsv
+Filename: doctor/reference/refine-class-uris.tsv
 Comment: 
 
-Filename: doctor/reference/refine-prefixes.tsv
+Filename: doctor/reference/refine-prefix-uris.tsv
 Comment: 
 
-Filename: rdf_doctor-0.8.5.dist-info/LICENSE
+Filename: rdf_doctor-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-0.8.5.dist-info/METADATA
+Filename: rdf_doctor-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-0.8.5.dist-info/WHEEL
+Filename: rdf_doctor-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-0.8.5.dist-info/entry_points.txt
+Filename: rdf_doctor-0.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-0.8.5.dist-info/top_level.txt
+Filename: rdf_doctor-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-0.8.5.dist-info/RECORD
+Filename: rdf_doctor-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.8.5"
+__version__ = "0.9.0"
```

## doctor/consts.py

```diff
@@ -10,15 +10,15 @@
 
 # Input file extensions
 EXTENSION_NT = ".nt"
 EXTENSION_TTL = ".ttl"
 EXTENSION_GZ = ".gz"
 
 # Correct prefix list file path
-CORRECT_PREFIXES_FILE_PATH = "reference/correct-prefixes.tsv"
+PREFIXES_FILE_PATH = "reference/prefixes.tsv"
 
 # Errata
-CLASS_ERRATA_FILE_PATH = "reference/refine-classes.tsv"
-PREFIX_ERRATA_FILE_PATH = "reference/refine-prefixes.tsv"
+REFINE_CLASS_URIS_FILE_PATH = "reference/refine-class-uris.tsv"
+REFINE_PREFIX_URIS_FILE_PATH = "reference/refine-prefix-uris.tsv"
 
 # Help link URL
 HELP_LINK_URL = "https://github.com/dbcls/rdf-doctor#output-description"
```

## doctor/doctor.py

```diff
@@ -7,16 +7,16 @@
 import csv
 import codecs
 import time
 import datetime
 import threading
 import queue
 from doctor.consts import VERSION_FILE, REPORT_FORMAT_SHEX, REPORT_FORMAT_MD, REPORT_FORMAT_MARKDOWN, \
-                            TARGET_CLASS_ALL, EXTENSION_NT, EXTENSION_TTL, EXTENSION_GZ, CORRECT_PREFIXES_FILE_PATH, \
-                            CLASS_ERRATA_FILE_PATH, PREFIX_ERRATA_FILE_PATH, HELP_LINK_URL
+                            TARGET_CLASS_ALL, EXTENSION_NT, EXTENSION_TTL, EXTENSION_GZ, PREFIXES_FILE_PATH, \
+                            REFINE_CLASS_URIS_FILE_PATH, REFINE_PREFIX_URIS_FILE_PATH, HELP_LINK_URL
 from shexer.shaper import Shaper
 from shexer.consts import NT, TURTLE, GZ, MIXED_INSTANCES
 from unidecode import unidecode
 from collections import defaultdict
 from pathlib import Path
 
 
@@ -77,15 +77,15 @@
     except ValueError as e:
         print(e)
 
     except KeyboardInterrupt:
         print ("Keyboard interrupt occurred.")
 
     except:
-        print("An exception error occurred. Input data format may not be correct. Please review the data.")
+        print("An exception error has occurred. There may be a problem with your input data. Please review the data.")
 
     return
 
 
 # Function for displaying dots during processing
 def monitor_thread(result_queue):
     i = 0
@@ -151,24 +151,30 @@
     # Target class(-c、--classes [URL1, URL2,...]、default: all、Multiple can be specified.)
     parser.add_argument("-c","--classes", type=str,
                         default=[TARGET_CLASS_ALL],
                         nargs="+",
                         help="set the target classes to be inspected to one of: all (defalut) or URL1, URL2,...",
                         metavar="URL")
 
-    # Prefix errata file path(-p, --prefix-dict [FILE]、default: reference/refine-prefixes.tsv)
+    # Prefix URI dictionary file path(-p, --prefix-dict [FILE]、default: reference/refine-prefix-uris.tsv)
     parser.add_argument("-p","--prefix-dict", type=str,
-                        default=str(Path(__file__).resolve().parent.joinpath(PREFIX_ERRATA_FILE_PATH)),
-                        help="path to a tab delimited file listing incorrect and correct URI pairs for the prefix (default: predefined file in rdf-doctor)",
+                        default=str(Path(__file__).resolve().parent.joinpath(REFINE_PREFIX_URIS_FILE_PATH)),
+                        help='(only when md(same as "markdown") is specified with -r, --report option) path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the prefix (default: predefined file in rdf-doctor)',
                         metavar="FILE")
 
-    # Class errata file path(-l, --class-dict [FILE]、default: reference/refine-classes.tsv)
+    # Class URI dictionary file path(-l, --class-dict [FILE]、default: reference/refine-class-uris.tsv)
     parser.add_argument("-l","--class-dict", type=str,
-                        default=str(Path(__file__).resolve().parent.joinpath(CLASS_ERRATA_FILE_PATH)),
-                        help="path to a tab delimited file listing incorrect and correct URI pairs for the class (default: predefined file in rdf-doctor)",
+                        default=str(Path(__file__).resolve().parent.joinpath(REFINE_CLASS_URIS_FILE_PATH)),
+                        help='(only when md(same as "markdown") is specified with -r, --report option) path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the class (default: predefined file in rdf-doctor)',
+                        metavar="FILE")
+
+    # Prefix list file path(-x, --prefix-list [FILE]、default: reference/prefixes.tsv)
+    parser.add_argument("-x","--prefix-list", type=str,
+                        default=str(Path(__file__).resolve().parent.joinpath(PREFIXES_FILE_PATH)),
+                        help="list of prefixes (default: predefined file in rdf-doctor)",
                         metavar="FILE")
 
     # input format (-f、--format [INPUT_FORMAT]、default: Standard output)
     parser.add_argument("-f","--force-format", type=str,
                         help='This option should not normally be used. Because the input format is automatically determined by the file extension. Use it only when you want to force specification. If used, "turtle" or "nt" can be specified.',
                         metavar="INPUT-FORMAT")
 
@@ -282,30 +288,49 @@
     # Input Format only allows "turtle" or "nt"
     if args.force_format is not None:
         if args.force_format != TURTLE and \
             args.force_format != NT:
             error_msg = 'Input format error: "' + args.force_format + '" is an unsupported input format. "' + TURTLE + '" and "' + NT + '" are supported.'
             return False, error_msg
 
+    # Prefix URIs dictionary file can be specified only in md/markdown mode
+    if args.prefix_dict != str(Path(__file__).resolve().parent.joinpath(REFINE_PREFIX_URIS_FILE_PATH)) and args.report == REPORT_FORMAT_SHEX:
+        error_msg = 'Prefix URIs dictionary file error: Prefix URIs dictionary file can only be specified if "md"(same as "markdown") is specified in the -r, --report option.'
+        return False, error_msg
+
     if os.path.isfile(args.prefix_dict) == False:
-        error_msg = "Prefix dictionary file error: Prefix dictionary does not exist or you don't have read permission."
+        error_msg = "Prefix URIs dictionary file error: Prefix dictionary does not exist or you don't have read permission."
         return False, error_msg
 
     # Check if the file has read permission
     if os.access(args.prefix_dict, os.R_OK) == False:
-        error_msg = "Prefix dictionary file error: you don't have permission to read the input file."
+        error_msg = "Prefix URIs dictionary file error: you don't have permission to read the input file."
+        return False, error_msg
+
+    # Class URIs dictionary file can be specified only in md/markdown mode
+    if args.class_dict != str(Path(__file__).resolve().parent.joinpath(REFINE_CLASS_URIS_FILE_PATH)) and args.report == REPORT_FORMAT_SHEX:
+        error_msg = 'Class URIs dictionary file error: Class URIs dictionary file can only be specified if "md"(same as "markdown") is specified in the -r, --report option.'
         return False, error_msg
 
     if os.path.isfile(args.class_dict) == False:
-        error_msg = "Class dictionary file error: Class dictionary does not exist or you don't have read permission."
+        error_msg = "Class URIs dictionary file error: Class dictionary does not exist or you don't have read permission."
         return False, error_msg
 
     # Check if the file has read permission
     if os.access(args.class_dict, os.R_OK) == False:
-        error_msg = "Class dictionary file error: you don't have permission to read the input file."
+        error_msg = "Class URIs dictionary file error: you don't have permission to read the input file."
+        return False, error_msg
+
+    if os.path.isfile(args.prefix_list) == False:
+        error_msg = "Prefix list file error: Prefix list does not exist or you don't have read permission."
+        return False, error_msg
+
+    # Check if the file has read permission
+    if os.access(args.prefix_list, os.R_OK) == False:
+        error_msg = "Prefix list file error: you don't have permission to read the input file."
         return False, error_msg
 
     return True, None
 
 
 # Processing when the report format is "shex"
 def get_shex_result(args, input_format, compression_mode, result_queue):
@@ -326,28 +351,28 @@
     if args.verbose:
         print_overwrite(get_dt_now() + " -- Checking for duplicate prefixes...")
 
     result_duplicated_prefixes = []
     if len(duplicated_prefixes) != 0:
         result_duplicated_prefixes.append("# Duplicate prefixes found.\n")
         result_duplicated_prefixes.append("\n")
-        result_duplicated_prefixes.append("# Input QName\tURI\n")
+        result_duplicated_prefixes.append("# Input-QName\tInput-prefix-URI\n")
         result_duplicated_prefixes.extend(["# " + s for s in duplicated_prefixes])
         result_duplicated_prefixes.append("\n\n")
 
-    # Suggest QName based on URI of validation expression output by sheXer and correct-prefixes.tsv
+    # Suggest QName based on URI of validation expression output by sheXer and prefixes.tsv
     if args.verbose:
         print_overwrite(get_dt_now() + " -- Creating suggestions for QName...")
 
     result_suggested_qname = []
-    correct_prefixes = get_correct_prefixes()
-    suggested_qname = get_suggested_qname(shaper_result, input_prefixes, correct_prefixes)
+    widely_used_prefixes = get_widely_used_prefixes(args.prefix_list)
+    suggested_qname = get_suggested_qname(shaper_result, input_prefixes, widely_used_prefixes)
     if len(suggested_qname) != 0:
-        result_suggested_qname.append("# There may be a better QName.\n\n")
-        result_suggested_qname.append("# Input QName\tSuggested QName\tURI\n")
+        result_suggested_qname.append("# There is a more widely used QName.\n\n")
+        result_suggested_qname.append("# Input-QName\tWidely-used-QName\tURI\n")
         result_suggested_qname.extend(["# " + s for s in suggested_qname])
         result_suggested_qname.append("\n")
 
     # List for storing the final result
     shex_final_result = []
     shex_final_result.extend(shaper_result)
     if len(result_duplicated_prefixes) != 0:
@@ -376,77 +401,77 @@
     # Get list for result output about prefix reuse percentage
     if args.verbose:
         print_overwrite(get_dt_now() + " -- Calculating prefix reuse percentage...")
 
     result_prefix_reuse_percentage = []
     result_prefix_reuse_percentage.append("## Prefix reuse percentage ([?](" + HELP_LINK_URL + "))\n")
     result_prefix_reuse_percentage.append("Percentage of prefixes used in the input file that are included in the predefined prefix list inside rdf-doctor.\n")
-    prefix_reuse_percentage = get_prefix_reuse_percentage(input_prefixes)
+    prefix_reuse_percentage = get_prefix_reuse_percentage(input_prefixes, args.prefix_list)
     if prefix_reuse_percentage == None:
         result_prefix_reuse_percentage.append("```\n")
         result_prefix_reuse_percentage.append("Not calculated because there is no prefix defined.\n")
         result_prefix_reuse_percentage.append("```\n\n")
     else:
         result_prefix_reuse_percentage.append("```\n")
         result_prefix_reuse_percentage.append(str(prefix_reuse_percentage) + "%\n")
         result_prefix_reuse_percentage.append("```\n\n")
 
-    # Refer to the errata of prefixes and obtain a list for result output that combines incorrect prefixes and correct prefixes
+    # Refer to the dictionary of prefix URIs and obtain a list that combines candidate pairs of URI rewrite source and rewrite destination
     if args.verbose:
-        print_overwrite(get_dt_now() + " -- Comparing with prefix dictionary (errata)...")
+        print_overwrite(get_dt_now() + " -- Comparing with prefix URIs dictionary...")
 
-    result_prefix_errata = []
+    result_refine_prefix_uris = []
     prefix_comparison_result = get_prefix_comparison_result(input_prefixes, args.prefix_dict)
     # When there is data to output
     if len(prefix_comparison_result) != 0:
-        result_prefix_errata.append("Found prefixes that looks incorrect.\n")
-        result_prefix_errata.append("```\n")
-        result_prefix_errata.append("Prefix\tInput URI\tSuggested URI\n")
-        result_prefix_errata.extend(prefix_comparison_result)
-        result_prefix_errata.append("```\n\n")
+        result_refine_prefix_uris.append("Found a more widely used one for the prefix URI inputed.\n")
+        result_refine_prefix_uris.append("```\n")
+        result_refine_prefix_uris.append("Input-QName\tInput-prefix-URI\tSuggested-prefix-URI\n")
+        result_refine_prefix_uris.extend(prefix_comparison_result)
+        result_refine_prefix_uris.append("```\n\n")
 
     result_duplicated_prefixes = []
     if len(duplicated_prefixes) != 0:
         result_duplicated_prefixes.append("Duplicate prefixes found.\n")
         result_duplicated_prefixes.append("```\n")
-        result_duplicated_prefixes.append("Input QName\tURI\n")
+        result_duplicated_prefixes.append("Input-QName\tInput-prefix-URI\n")
         result_duplicated_prefixes.extend([s for s in duplicated_prefixes])
         result_duplicated_prefixes.append("```\n\n")
     # -------------------------------------------------
 
     if args.verbose:
         print_overwrite(get_dt_now() + " -- Getting classes from input file...")
 
     # Processing related to classes -------------------
     input_classes = get_input_classes(args.input, input_format, compression_mode, args.classes)
 
-    # Refers to the errata list of the class, acquires the list for result output that combines the incorrect class and the correct class,
-    # and returns the class corresponding to each key in fingerprint format stored in dictionary format.
+    # Refers to the class URIs dictionary, acquires the list for result output that candidate pairs of URI rewrite source and rewrite destinations,
+    # and generate the class corresponding to each key in fingerprint format stored in dictionary format.
     if args.verbose:
-        print_overwrite(get_dt_now() + " -- Comparing with class dictionary (errata)...")
+        print_overwrite(get_dt_now() + " -- Comparing with class URIs dictionary...")
 
-    result_class_errata = []
+    result_refine_class_uris = []
     class_comparison_result, fingerprint_class_dict = get_class_comparison_result(input_classes, args.class_dict)
     # When there is data to output
     if len(class_comparison_result) != 0:
-        result_class_errata.append("Found class names that looks incorrect.\n")
-        result_class_errata.append("```\n")
-        result_class_errata.append("Input class name\tSuggested class name\n")
-        result_class_errata.extend(class_comparison_result)
-        result_class_errata.append("```\n\n")
+        result_refine_class_uris.append("Found a more widely used one for the class URI inputed.\n")
+        result_refine_class_uris.append("```\n")
+        result_refine_class_uris.append("Input-class-URI\tSuggested-class-URI\n")
+        result_refine_class_uris.extend(class_comparison_result)
+        result_refine_class_uris.append("```\n\n")
 
     # Get a result output list to notify about different class strings with the same key as a result of fingerprinting
     if args.verbose:
         print_overwrite(get_dt_now() + " -- Comparing with fingerprint method results...")
 
     result_class_fingerprint = []
     fingerprint_comparison_result = get_fingerprint_comparison_result(fingerprint_class_dict)
     # When there is data to output
     if len(fingerprint_comparison_result) != 0:
-        result_class_fingerprint.append("Found multiple strings that appear to represent the same class name.\n")
+        result_class_fingerprint.append("Found multiple strings that appear to represent the same class.\n")
         result_class_fingerprint.append("```")
         result_class_fingerprint.extend(fingerprint_comparison_result)
         result_class_fingerprint.append("\n```\n\n")
     # -------------------------------------------------
 
     # List for storing the final result
     md_final_result = []
@@ -457,24 +482,24 @@
         md_final_result.append(os.path.basename(input_file) + "\n")
 
     md_final_result.append("```\n\n")
 
     # Merge result
     md_final_result.extend(result_prefix_reuse_percentage)
 
-    prefix_result_exists = len(result_prefix_errata) != 0
+    prefix_result_exists = len(result_refine_prefix_uris) != 0
     if prefix_result_exists:
-        md_final_result.append("## Refine prefixes ([?](" + HELP_LINK_URL + "))\n")
-        md_final_result.extend(result_prefix_errata)
+        md_final_result.append("## Refine prefix URIs ([?](" + HELP_LINK_URL + "))\n")
+        md_final_result.extend(result_refine_prefix_uris)
         md_final_result.extend(result_duplicated_prefixes)
 
-    class_result_exists = len(result_class_errata) != 0 or len(result_class_fingerprint) != 0
+    class_result_exists = len(result_refine_class_uris) != 0 or len(result_class_fingerprint) != 0
     if class_result_exists:
-        md_final_result.append("## Refine classes ([?](" + HELP_LINK_URL + "))\n")
-        md_final_result.extend(result_class_errata)
+        md_final_result.append("## Refine class URIs ([?](" + HELP_LINK_URL + "))\n")
+        md_final_result.extend(result_refine_class_uris)
         md_final_result.extend(result_class_fingerprint)
 
     result_queue.put(md_final_result)
 
 
 # Call the shex_graph method of shexer's shaper class and output the result
 def get_shaper_result(args, input_format, compression_mode, input_prefixes):
@@ -507,29 +532,29 @@
                             verbose=args.verbose,
                             acceptance_threshold=0.05)
 
 
 # Calculates the percentage of prefixes in the input file that exist in the prefix list file prepared in advance,
 # and returns it after rounding to the second decimal place.
 # If the prefix is not detected, do not calculate and return None.
-def get_prefix_reuse_percentage(input_prefixes):
-    correct_prefixes = get_correct_prefixes()
+def get_prefix_reuse_percentage(input_prefixes, prefix_list_file):
+    widely_used_prefixes = get_widely_used_prefixes(prefix_list_file)
 
     input_prefixes_count = len(input_prefixes)
     if input_prefixes_count == 0:
         return None
     else:
-        correct_count = 0
+        reuse_count = 0
         for prefix in input_prefixes:
-            for correct_prefix in correct_prefixes:
-                if prefix[1] == correct_prefix[1]:
-                    correct_count+=1
+            for widely_used_prefix in widely_used_prefixes:
+                if prefix[1] == widely_used_prefix[1]:
+                    reuse_count+=1
                     break
 
-        prefix_reuse_percentage = round(correct_count / input_prefixes_count * 100, 2)
+        prefix_reuse_percentage = round(reuse_count / input_prefixes_count * 100, 2)
         return prefix_reuse_percentage
 
 
 # Get the classes contained within the input file(s)
 def get_input_classes(input_files, input_format, compression_mode, target_classes):
 
     input_classes = []
@@ -563,58 +588,58 @@
         for row in qres:
             if f"{row.class_name}" not in input_classes:
                 input_classes.append(f"{row.class_name}")
 
     return input_classes
 
 
-# Return class errata in a two-dimensional array
-def get_class_errata(class_errata_file):
-    with open(class_errata_file, mode="r", newline="\n", encoding="utf-8") as f:
+# Return contents of class URIs dictionary in a two-dimensional array
+def get_refine_class_uris(refine_class_uris_file):
+    with open(refine_class_uris_file, mode="r", newline="\n", encoding="utf-8") as f:
         tsv_reader = csv.reader(f, delimiter="\t")
-        class_errata = [row for row in tsv_reader]
+        refine_class_uris = [row for row in tsv_reader]
 
-    return class_errata
+    return refine_class_uris
 
 
-# Return prefix errata in a two-dimensional array
-def get_prefix_errata(prefix_errata_file):
-    with open(prefix_errata_file, mode="r", newline="\n", encoding="utf-8") as f:
+# Return contents of prefix URIs dictionary file in a two-dimensional array
+def get_refine_prefix_uris(refine_prefix_uris_file):
+    with open(refine_prefix_uris_file, mode="r", newline="\n", encoding="utf-8") as f:
         tsv_reader = csv.reader(f, delimiter="\t")
-        prefix_errata = [row for row in tsv_reader]
+        refine_prefix_uris = [row for row in tsv_reader]
 
-    return prefix_errata
+    return refine_prefix_uris
 
 
-# Get a combined list of incorrect and correct classes obtained by referencing the class errata list.
+# Get a list of candidate pairs of URI rewrite source and rewrite destination by referencing the class URLs dictionary.
 # Create a dictionary with a class corresponding to each key in the stored fingerprint format.
 # Return the two.
-def get_class_comparison_result(input_classes, class_errata_file):
-    class_errata = get_class_errata(class_errata_file)
+def get_class_comparison_result(input_classes, refine_class_uris_file):
+    refine_class_uris = get_refine_class_uris(refine_class_uris_file)
     class_comparison_result = []
     fingerprint_class_dict = defaultdict(list)
     # Perform clustering by fingerprint for the acquired class name
     for input_class in input_classes:
         fingerprint_class_dict[fingerprint(input_class)].append(input_class)
-        for eratta in class_errata:
+        for eratta in refine_class_uris:
             if input_class == eratta[0]:
                 class_comparison_result.append(input_class+"\t"+eratta[1]+"\n")
                 break
 
     return class_comparison_result, fingerprint_class_dict
 
 
-# Refer to the errata of prefixes and obtain a list that combines incorrect prefixes and correct prefixes
-def get_prefix_comparison_result(input_prefixes, prefix_errata_file):
-    prefix_errata = get_prefix_errata(prefix_errata_file)
+# Refer to the dictionary of prefix URIs and obtain a list that combines candidate pairs of URI rewrite source and rewrite destination
+def get_prefix_comparison_result(input_prefixes, refine_prefix_uris_file):
+    refine_prefix_uris = get_refine_prefix_uris(refine_prefix_uris_file)
     prefix_comparison_result = []
 
     # Perform clustering by fingerprint for the acquired class name
     for input_prefix in input_prefixes:
-        for eratta in prefix_errata:
+        for eratta in refine_prefix_uris:
             if input_prefix[1] == eratta[0] and eratta[1] != "":
                 prefix_comparison_result.append(str(input_prefix[0]+"\t"+input_prefix[1]+"\t"+eratta[1]+"\n"))
                 break
 
     return prefix_comparison_result
 
 
@@ -665,27 +690,29 @@
     for key, values in duplicated_prefixes_dict.items():
         for value in values:
             duplicated_prefixes_list.append(key + ":\t" + value + "\n")
 
     return input_prefixes, duplicated_prefixes_list
 
 
-# Get the correct prefix from a prepared prefix list
-def get_correct_prefixes():
-    with open(Path(__file__).resolve().parent.joinpath(CORRECT_PREFIXES_FILE_PATH), mode="r", newline="\n", encoding="utf-8") as f:
+# Get the widely used prefix from a prepared prefix list
+def get_widely_used_prefixes(prefix_list_file):
+    with open(prefix_list_file, mode="r", newline="\n", encoding="utf-8") as f:
         tsv_reader = csv.reader(f, delimiter="\t")
-        correct_prefixes = [row for row in tsv_reader]
+        widely_used_prefixes = [row for row in tsv_reader]
 
-    return correct_prefixes
+    return widely_used_prefixes
 
 
 # Compare the URI of the validation expression in the shexer output with the URI of the prepared prefix list
 # and get the matching QName from the prefix list
-def get_suggested_qname(shaper_result, input_prefixes, correct_prefixes):
+def get_suggested_qname(shaper_result, input_prefixes, widely_used_prefixes):
     suggest_qname = []
+
+    # Comparison of prefix list and minimal URI detected by shaXer
     for line in shaper_result.splitlines():
         if ("[<http" in line and ">~]" in line):
             exists_in_input_prefix = False
             shaper_result_uri = line[line.find("[<http")+2:line.find(">~]")]
 
             # Determine if the same URI is included in the prefix defined in the input file,
             # and if it is included, get the QName
@@ -693,34 +720,54 @@
             for input_prefix in input_prefixes:
                 if shaper_result_uri == input_prefix[1]:
                     exists_in_input_prefix = True
                     input_qname = input_prefix[0]
                     break
 
             tmp_suggest_qname = []
-            is_input_correct_qname = False
-            for correct_prefix in correct_prefixes:
-                append_str = input_qname + "\t" + correct_prefix[0]+"\t"+shaper_result_uri+"\n"
-                if (shaper_result_uri == correct_prefix[1] and append_str not in suggest_qname):
+            is_included_list = False
+            for widely_used_prefix in widely_used_prefixes:
+                append_str = input_qname + "\t" + widely_used_prefix[0]+"\t"+shaper_result_uri+"\n"
+                if shaper_result_uri == widely_used_prefix[1] and append_str not in suggest_qname:
                     if exists_in_input_prefix:
                         # If the prefixes defined in the input file include those with the same URI,
                         # add them to the list only if the QName is different
-                        if correct_prefix[0] != input_qname:
+                        if widely_used_prefix[0] != input_qname:
                             tmp_suggest_qname.append(append_str)
                         else:
                             # If the QName defined in the input file is also included in the prefix list,
                             # do not suggest another QName with the same URI in the prefix list
-                            is_input_correct_qname = True
+                            is_included_list = True
                             break
                     else:
                         suggest_qname.append(append_str)
 
-            if is_input_correct_qname == False:
+            if is_included_list == False:
                 suggest_qname.extend(tmp_suggest_qname)
 
+    # Comparing of prefix list and prefixes in input file
+    for input_prefix in input_prefixes:
+        tmp_suggest_qname = []
+        is_included_list = False
+        for widely_used_prefix in widely_used_prefixes:
+            append_str = input_prefix[0] + "\t" + widely_used_prefix[0]+"\t"+input_prefix[1]+"\n"
+            if input_prefix[1] == widely_used_prefix[1] and append_str not in suggest_qname:
+                # If the prefixes defined in the input file include those with the same URI,
+                # add them to the list only if the QName is different
+                if input_prefix[0] != widely_used_prefix[0]:
+                    tmp_suggest_qname.append(append_str)
+                else:
+                    # If the QName defined in the input file is also included in the prefix list,
+                    # do not suggest another QName with the same URI in the prefix list
+                    is_included_list = True
+                    break
+
+        if is_included_list == False:
+            suggest_qname.extend(tmp_suggest_qname)
+
     return suggest_qname
 
 
 # Generates a key from the received string, excluding case differences, symbols, control characters, etc.
 # Values that contain only the most valuable or meaningful part of the string will have the same key
 # returned by this method, useful for clustering.
 # Detailed explanation：https://openrefine.org/docs/technical-reference/clustering-in-depth#fingerprint
```

## Comparing `doctor/reference/refine-prefixes.tsv` & `doctor/reference/refine-prefix-uris.tsv`

 * *Files identical despite different names*

## Comparing `rdf_doctor-0.8.5.dist-info/LICENSE` & `rdf_doctor-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-0.8.5.dist-info/METADATA` & `rdf_doctor-0.9.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 0.8.5
+Version: 0.9.0
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -60,17 +60,21 @@
   -r REPORT-FORMAT, --report REPORT-FORMAT
                         set the output format/serializer of report to one of: shex (defalut) or md or markdown(same as md)
   -o FILE, --output FILE
                         write to file instead of stdout
   -c URL [URL ...], --classes URL [URL ...]
                         set the target classes to be inspected to one of: all (defalut) or URL1, URL2,...
   -p FILE, --prefix-dict FILE
-                        path to a tab delimited file listing incorrect and correct URI pairs for the prefix (default: predefined file in rdf-doctor)
+                        (only when md(same as "markdown") is specified with -r, --report option) path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for
+                        the prefix (default: predefined file in rdf-doctor)
   -l FILE, --class-dict FILE
-                        path to a tab delimited file listing incorrect and correct URI pairs for the class (default: predefined file in rdf-doctor)
+                        (only when md(same as "markdown") is specified with -r, --report option) path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for
+                        the class (default: predefined file in rdf-doctor)
+  -x FILE, --prefix-list FILE
+                        list of prefixes (default: predefined file in rdf-doctor)
   -f INPUT-FORMAT, --force-format INPUT-FORMAT
                         This option should not normally be used. Because the input format is automatically determined by the file extension. Use it only when you want to force specification. If used, "turtle" or "nt" can be specified.
 ```
 
 ## See Also
 - [1] https://github.com/DaniFdezAlvarez/shexer
 - [2] http://shex.io/shex-primer/#combined-constraints
@@ -139,22 +143,22 @@
    chebi:name  xsd:string  ;                                   # 100.0 % (1 instance).
    rdf:type  [chebi:PERSON]                                    # 100.0 % (1 instance).
 }
 
 
 # Duplicate prefixes found.
 
-# Input QName	URI
+# Input-QName	Input-prefix-URI
 # ex:	http://example.org1/
 # ex:	http://example.org2/
 
 
-# There may be a better QName.
+# There is a more widely used QName.
 
-# Input QName	Suggested QName	URI
+# Input-QName	Widely-used-QName	URI
 # pobo:	obo:	http://purl.obolibrary.org/obo/
 # pobo:	uo:	http://purl.obolibrary.org/obo/
 ```
 
 ````
 $ rdf-doctor -i example_2.ttl -r md
 # Report on
@@ -164,58 +168,57 @@
 
 ## Prefix reuse percentage ([?](https://github.com/dbcls/rdf-doctor#output-description))
 Percentage of prefixes used in the input file that are included in the predefined prefix list inside rdf-doctor.
 ```
 57.14%
 ```
 
-## Refine prefixes ([?](https://github.com/dbcls/rdf-doctor#output-description))
-Found prefixes that looks incorrect.
+## Refine prefix URIs ([?](https://github.com/dbcls/rdf-doctor#output-description))
+Found a more widely used one for the prefix URI inputed.
 ```
-Prefix	Input URI	Suggested URI
+Input-QName	Input-prefix-URI	Suggested-prefix-URI
 chebi:	http://www.ebi.ac.uk/chebi/searchId.do?chebiId=CHEBI%3A	http://purl.obolibrary.org/obo/CHEBI_
 ```
 
 Duplicate prefixes found.
 ```
-Input QName	URI
+Input-QName	Input-prefix-URI
 ex:	http://example.org1/
 ex:	http://example.org2/
 ```
 
-## Refine classes ([?](https://github.com/dbcls/rdf-doctor#output-description))
-Found class names that looks incorrect.
+## Refine class URIs ([?](https://github.com/dbcls/rdf-doctor#output-description))
+Found a more widely used one for the class URI inputed.
 ```
-Input class name	Suggested class name
+Input-class-URI	Suggested-class-URI
 http://www.ebi.ac.uk/chebi/searchId.do?chebiId=CHEBI%3APErson	http://www.ebi.ac.uk/chebi/searchId.do?chebiId=CHEBI%3APerson
 ```
 
-Found multiple strings that appear to represent the same class name.
+Found multiple strings that appear to represent the same class.
 ```
 http://www.ebi.ac.uk/chebi/searchId.do?chebiId=CHEBI%3APerson
 http://www.ebi.ac.uk/chebi/searchId.do?chebiId=CHEBI%3APErson
 http://www.ebi.ac.uk/chebi/searchId.do?chebiId=CHEBI%3APERSON
 
 http://www.ebi.ac.uk/chebi/searchId.do?chebiId=CHEBI%3ADocument
 http://www.ebi.ac.uk/chebi/searchId.do?chebiId=CHEBI%3ADOCUMENT
 ```
 ````
 
 
 ## Example of dictionary file
-You can specify arbitrary dictionary files (errata) for prefixes and class URIs. It is a file in which pairs of incorrect URIs and correct URIs are tab-separated, one per line, as shown below.
+You can specify arbitrary dictionary files for prefixes and class URIs. It is a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination, one per line, as shown below. This dictionary file is used only if -r or --report option is specified as md (same as markdown).
 Specify -p , --prefix-dict for prefix, -l, --class-dict for class, followed by file.
 See: https://github.com/dbcls/rdf-doctor#command-line-interface
 ```
-http://incorrect/uri1	http://correct/uri1
-http://incorrect/uri2	http://correct/uri2
-http://incorrect/uri3	http://correct/uri3
+http://candidate/for/rewrite/source/uri1	http://candidate/for/rewriting/destination/uri1
+http://candidate/for/rewrite/source/uri2	http://candidate/for/rewriting/destination/uri2
+http://candidate/for/rewrite/source/uri3	http://candidate/for/rewriting/destination/uri3
 ```
 
 
 ## Output Description
 * **Prefix reuse percentage**: Percentage of prefixes used in the input file that are included in the predefined prefix list inside rdf-doctor.
 
-* **Refine prefixes**: The URI entered as a prefix is checked against a list (errata) defined inside rdf-doctor, and if there is matching information, output as correction suggestions.
-Also, if a prefix with the same QName but a different URI is found, it is output as a correction suggestion.
+* **Refine prefix URIs**: The URI entered as a prefix is checked against a list defined inside rdf-doctor (or specified by -p option), and if there is matching information, output as correction suggestions. Also, if a prefix with the same QName but a different URI is found, it is output as a correction suggestion.
 
-* **Refine classes**: The URI of the input class is checked against the list (errata) defined inside rdf-doctor, and if there is matching information, the correct URI is suggested. Also, if the URI of the input class is converted to a key string using the fingerprinting method and multiple different strings are found even though the key strings match, they may represent the same class. Output as correction suggestions.
+* **Refine class URIs**: The URI of the input class is checked against the list defined inside rdf-doctor (or specified by -l option), and if there is matching information, a candidate rewrite URI is suggested. Also, if the URI of the input class is converted to a key string using the fingerprinting method and multiple different strings are found even though the key strings match, they may represent the same class. Output as correction suggestions.
```

## Comparing `rdf_doctor-0.8.5.dist-info/RECORD` & `rdf_doctor-0.9.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-doctor/__init__.py,sha256=K0kGrhh1kzVisZcoSkeuJdC06rTwxufV05Vy2hOVGoo,22
-doctor/consts.py,sha256=jo_-yPRv-Z7OoTYeIEed4RNsKR6nzrm64wVJPmI8vww,631
-doctor/doctor.py,sha256=0U5p3nK5lper5ukFNFp5_D91ga-d5AbwG8D-zZ9HojQ,32735
-doctor/reference/correct-prefixes.tsv,sha256=2IAy3-9YwmWbG9JgoB8R2fxW7T-U-Qr59PzqMApUbpI,20305
-doctor/reference/refine-classes.tsv,sha256=pd_nOSjR7bia96u9hhcjhBg9J6LUAuDFlyy-JE9tsys,90
-doctor/reference/refine-prefixes.tsv,sha256=B5iok0_4VqdBNLn4_Auwx5gSwAnxgIh6OoQ4cgebERY,679
-rdf_doctor-0.8.5.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
-rdf_doctor-0.8.5.dist-info/METADATA,sha256=R06vJz0Z1dOCzkl6B3n1kAn0HoxdZr7bzaBa8lenOek,9140
-rdf_doctor-0.8.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rdf_doctor-0.8.5.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
-rdf_doctor-0.8.5.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
-rdf_doctor-0.8.5.dist-info/RECORD,,
+doctor/__init__.py,sha256=H9NWRZb7NbeRRPLP_V1fARmLNXranorVM-OOY-8_2ug,22
+doctor/consts.py,sha256=g8qN1vFAkkiFWF_HMGBpkoED0SdtPsxNUc33fcyLeow,631
+doctor/doctor.py,sha256=bEKsaQ2wbgcZYG7z9ACYYi5S0FZF7gkCLf-ziIWYP1s,36220
+doctor/reference/prefixes.tsv,sha256=9zIvWdCO3X65YnULmiBEsIapiZvmplZbB6MywGJp54s,43474
+doctor/reference/refine-class-uris.tsv,sha256=pd_nOSjR7bia96u9hhcjhBg9J6LUAuDFlyy-JE9tsys,90
+doctor/reference/refine-prefix-uris.tsv,sha256=B5iok0_4VqdBNLn4_Auwx5gSwAnxgIh6OoQ4cgebERY,679
+rdf_doctor-0.9.0.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
+rdf_doctor-0.9.0.dist-info/METADATA,sha256=qGj9toPi3Kvu624mWNo0yoPeR_OJe9GoOZZINj-KD5g,9892
+rdf_doctor-0.9.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rdf_doctor-0.9.0.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
+rdf_doctor-0.9.0.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
+rdf_doctor-0.9.0.dist-info/RECORD,,
```

