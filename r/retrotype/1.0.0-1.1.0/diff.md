# Comparing `tmp/retrotype-1.0.0.tar.gz` & `tmp/retrotype-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retrotype-1.0.0.tar", last modified: Sun May  7 20:17:42 2023, max compression
+gzip compressed data, was "retrotype-1.1.0.tar", last modified: Mon Jul 10 02:22:31 2023, max compression
```

## Comparing `retrotype-1.0.0.tar` & `retrotype-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2023-05-07 20:17:42.552525 retrotype-1.0.0/
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     1072 2022-11-11 18:54:20.000000 retrotype-1.0.0/LICENSE
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     6140 2023-05-07 20:17:42.552525 retrotype-1.0.0/PKG-INFO
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     4223 2022-12-09 04:10:35.000000 retrotype-1.0.0/README.md
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     1310 2023-05-07 20:01:25.000000 retrotype-1.0.0/pyproject.toml
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       38 2023-05-07 20:17:42.552525 retrotype-1.0.0/setup.cfg
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       74 2022-12-09 04:10:35.000000 retrotype-1.0.0/setup.py
-drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2023-05-07 20:17:42.548525 retrotype-1.0.0/src/
-drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2023-05-07 20:17:42.548525 retrotype-1.0.0/src/retrotype/
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)        0 2022-12-09 04:10:35.000000 retrotype-1.0.0/src/retrotype/__init__.py
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     7054 2022-12-09 04:10:35.000000 retrotype-1.0.0/src/retrotype/char_maps.py
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     7977 2023-04-29 20:13:09.000000 retrotype-1.0.0/src/retrotype/retrotype_cli.py
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)    17445 2023-04-29 20:13:09.000000 retrotype-1.0.0/src/retrotype/retrotype_lib.py
-drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2023-05-07 20:17:42.552525 retrotype-1.0.0/src/retrotype.egg-info/
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     6140 2023-05-07 20:17:42.000000 retrotype-1.0.0/src/retrotype.egg-info/PKG-INFO
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)      380 2023-05-07 20:17:42.000000 retrotype-1.0.0/src/retrotype.egg-info/SOURCES.txt
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)        1 2023-05-07 20:17:42.000000 retrotype-1.0.0/src/retrotype.egg-info/dependency_links.txt
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       78 2023-05-07 20:17:42.000000 retrotype-1.0.0/src/retrotype.egg-info/entry_points.txt
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       60 2023-05-07 20:17:42.000000 retrotype-1.0.0/src/retrotype.egg-info/requires.txt
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       10 2023-05-07 20:17:42.000000 retrotype-1.0.0/src/retrotype.egg-info/top_level.txt
+drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2023-07-10 02:22:31.088662 retrotype-1.1.0/
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     1072 2022-11-11 18:54:20.000000 retrotype-1.1.0/LICENSE
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     6226 2023-07-10 02:22:31.084662 retrotype-1.1.0/PKG-INFO
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     4309 2023-07-10 02:17:26.000000 retrotype-1.1.0/README.md
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     1310 2023-07-10 02:17:26.000000 retrotype-1.1.0/pyproject.toml
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       38 2023-07-10 02:22:31.088662 retrotype-1.1.0/setup.cfg
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       74 2022-12-09 04:10:35.000000 retrotype-1.1.0/setup.py
+drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2023-07-10 02:22:31.084662 retrotype-1.1.0/src/
+drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2023-07-10 02:22:31.084662 retrotype-1.1.0/src/retrotype/
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)        0 2022-12-09 04:10:35.000000 retrotype-1.1.0/src/retrotype/__init__.py
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     7054 2022-12-09 04:10:35.000000 retrotype-1.1.0/src/retrotype/char_maps.py
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     8163 2023-07-10 02:17:26.000000 retrotype-1.1.0/src/retrotype/retrotype_cli.py
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)    17445 2023-05-07 21:06:46.000000 retrotype-1.1.0/src/retrotype/retrotype_lib.py
+drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2023-07-10 02:22:31.084662 retrotype-1.1.0/src/retrotype.egg-info/
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     6226 2023-07-10 02:22:31.000000 retrotype-1.1.0/src/retrotype.egg-info/PKG-INFO
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)      380 2023-07-10 02:22:31.000000 retrotype-1.1.0/src/retrotype.egg-info/SOURCES.txt
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)        1 2023-07-10 02:22:31.000000 retrotype-1.1.0/src/retrotype.egg-info/dependency_links.txt
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       78 2023-07-10 02:22:31.000000 retrotype-1.1.0/src/retrotype.egg-info/entry_points.txt
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       60 2023-07-10 02:22:31.000000 retrotype-1.1.0/src/retrotype.egg-info/requires.txt
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       10 2023-07-10 02:22:31.000000 retrotype-1.1.0/src/retrotype.egg-info/top_level.txt
```

### Comparing `retrotype-1.0.0/LICENSE` & `retrotype-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `retrotype-1.0.0/PKG-INFO` & `retrotype-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retrotype
-Version: 1.0.0
+Version: 1.1.0
 Summary: Debuging and conversion tool for 1980s magazine type-in programs
 Author-email: Michael Buhidar <mbuhidar@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Michael Buhidar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -63,15 +63,15 @@
 
 After installation, use `retrotype_cli` directly from the command line -
 consult the help for the latest usage:
 
 **Note:** Currently the only implemented options are for Ahoy C64 programs.
 
 ```
-retrotype_cli [-l load_address] [-s source_format] input_file
+retrotype_cli [-l load_address] [-s source_format] [-w] input_file
 ```
 
 ```
 positional arguments:
   input_file            Specify the input file name, including path.
                         Note:  Output files will use input file basename
 
@@ -88,14 +88,16 @@
                         - 0x1201 - VIC20 +24K
 
   -s source_format, --source source_format
                         Specifies the magazine source for conversion and checksum:
                         ahoy1 - Ahoy magazine (Apr-May 1984)
                         ahoy2 - Ahoy magazine (Jun 1984-Apr 1987) (default)
                         ahoy3 - Ahoy magazine (May 1987-)
+
+  -w, --wip             Work in progress, do not output executable binary file.
 ```
 
 As an example for an Ahoy! magazine file:
 
 ```
 Input:  basename.bas
```

### Comparing `retrotype-1.0.0/README.md` & `retrotype-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 After installation, use `retrotype_cli` directly from the command line -
 consult the help for the latest usage:
 
 **Note:** Currently the only implemented options are for Ahoy C64 programs.
 
 ```
-retrotype_cli [-l load_address] [-s source_format] input_file
+retrotype_cli [-l load_address] [-s source_format] [-w] input_file
 ```
 
 ```
 positional arguments:
   input_file            Specify the input file name, including path.
                         Note:  Output files will use input file basename
 
@@ -49,14 +49,16 @@
                         - 0x1201 - VIC20 +24K
 
   -s source_format, --source source_format
                         Specifies the magazine source for conversion and checksum:
                         ahoy1 - Ahoy magazine (Apr-May 1984)
                         ahoy2 - Ahoy magazine (Jun 1984-Apr 1987) (default)
                         ahoy3 - Ahoy magazine (May 1987-)
+
+  -w, --wip             Work in progress, do not output executable binary file.
 ```
 
 As an example for an Ahoy! magazine file:
 
 ```
 Input:  basename.bas
```

### Comparing `retrotype-1.0.0/pyproject.toml` & `retrotype-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "retrotype"
-version = "1.0.0"
+version = "1.1.0"
 description = "Debuging and conversion tool for 1980s magazine type-in programs"
 readme = "README.md"
 authors = [{ name = "Michael Buhidar", email = "mbuhidar@gmail.com" }]
 maintainers = []
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `retrotype-1.0.0/src/retrotype/char_maps.py` & `retrotype-1.1.0/src/retrotype/char_maps.py`

 * *Files identical despite different names*

### Comparing `retrotype-1.0.0/src/retrotype/retrotype_cli.py` & `retrotype-1.1.0/src/retrotype/retrotype_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,21 @@
         help="Specifies the magazine source for conversion and checksum:\n"
         "ahoy1 - Ahoy magazine (Apr-May 1984)\n"
         "ahoy2 - Ahoy magazine (Jun 1984-Apr 1987) (default)\n"
         "ahoy3 - Ahoy magazine (May 1987-)\n",
     )
 
     parser.add_argument(
+        "-w",
+        "--wip",
+        action="store_true",
+        help="Work in progress, do not output executable binary file.\n",
+    )
+
+    parser.add_argument(
         "file_in",
         type=str,
         metavar="input_file",
         help="Specify the input file name including path.\n"
         "Note:  Output file will use input file basename with\n"
         "extension '.prg' for Commodore file format.",
     )
@@ -215,16 +222,17 @@
 
     bytes_out = [byte for sublist in out_list for byte in sublist]
 
     file_stem = args.file_in.split(".")[0]
 
     ofiles = OutputFiles(bytes_out, ahoy_checksums)
 
-    # Write binary file compatible with Commodore computers or emulators
-    ofiles.write_binary(f"{file_stem}.prg")
+    # Write binary file Commodore computers or emulators if not WIP
+    if not args.wip:
+        ofiles.write_binary(f"{file_stem}.prg")
 
     # Write text file containing line numbers, checksums, and line count
     ofiles.write_checksums(f"{file_stem}.chk")
 
     # Print line checksums to terminal, formatted based on screen width
     print("Line Checksums:\n")
     if not width:
```

### Comparing `retrotype-1.0.0/src/retrotype/retrotype_lib.py` & `retrotype-1.1.0/src/retrotype/retrotype_lib.py`

 * *Files identical despite different names*

### Comparing `retrotype-1.0.0/src/retrotype.egg-info/PKG-INFO` & `retrotype-1.1.0/src/retrotype.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retrotype
-Version: 1.0.0
+Version: 1.1.0
 Summary: Debuging and conversion tool for 1980s magazine type-in programs
 Author-email: Michael Buhidar <mbuhidar@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Michael Buhidar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -63,15 +63,15 @@
 
 After installation, use `retrotype_cli` directly from the command line -
 consult the help for the latest usage:
 
 **Note:** Currently the only implemented options are for Ahoy C64 programs.
 
 ```
-retrotype_cli [-l load_address] [-s source_format] input_file
+retrotype_cli [-l load_address] [-s source_format] [-w] input_file
 ```
 
 ```
 positional arguments:
   input_file            Specify the input file name, including path.
                         Note:  Output files will use input file basename
 
@@ -88,14 +88,16 @@
                         - 0x1201 - VIC20 +24K
 
   -s source_format, --source source_format
                         Specifies the magazine source for conversion and checksum:
                         ahoy1 - Ahoy magazine (Apr-May 1984)
                         ahoy2 - Ahoy magazine (Jun 1984-Apr 1987) (default)
                         ahoy3 - Ahoy magazine (May 1987-)
+
+  -w, --wip             Work in progress, do not output executable binary file.
 ```
 
 As an example for an Ahoy! magazine file:
 
 ```
 Input:  basename.bas
```

