# Comparing `tmp/ghak-0.2.728-py3.11.egg` & `tmp/ghak-0.2.734-py3.11.egg`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 15201 bytes, number of entries: 19
--rw-r--r--  2.0 unx      400 b- defN 23-Jul-10 16:24 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      411 b- defN 23-Jul-10 16:24 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-10 16:24 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx       39 b- defN 23-Jul-10 16:24 EGG-INFO/entry_points.txt
--rw-r--r--  2.0 unx       69 b- defN 23-Jul-10 16:24 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-10 16:24 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-10 16:24 EGG-INFO/zip-safe
--rw-r--r--  2.0 unx       90 b- defN 23-Jun-30 19:52 ghak/__init__.py
--rw-r--r--  2.0 unx     3694 b- defN 23-Jul-10 15:55 ghak/ghak.py
--rw-r--r--  2.0 unx      312 b- defN 23-Jul-10 16:24 ghak/__pycache__/__init__.cpython-311.pyc
--rw-r--r--  2.0 unx     4626 b- defN 23-Jul-10 16:24 ghak/__pycache__/ghak.cpython-311.pyc
+Zip file size: 15071 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      405 b- defN 23-Jul-10 16:46 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      411 b- defN 23-Jul-10 16:46 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-10 16:46 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       39 b- defN 23-Jul-10 16:46 EGG-INFO/entry_points.txt
+-rw-r--r--  2.0 unx       69 b- defN 23-Jul-10 16:46 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-10 16:46 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-10 16:46 EGG-INFO/zip-safe
+-rw-r--r--  2.0 unx       90 b- defN 23-Jul-10 16:41 ghak/__init__.py
+-rw-r--r--  2.0 unx     3745 b- defN 23-Jul-10 16:46 ghak/ghak.py
+-rw-r--r--  2.0 unx      312 b- defN 23-Jul-10 16:46 ghak/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--  2.0 unx     4462 b- defN 23-Jul-10 16:46 ghak/__pycache__/ghak.cpython-311.pyc
 -rw-r--r--  2.0 unx     3525 b- defN 23-Jul-10 15:45 ghak/factories/TokenFactory.py
 -rw-r--r--  2.0 unx       28 b- defN 23-Jun-30 18:51 ghak/factories/__init__.py
--rw-r--r--  2.0 unx     5498 b- defN 23-Jul-10 16:24 ghak/factories/__pycache__/TokenFactory.cpython-311.pyc
--rw-r--r--  2.0 unx      204 b- defN 23-Jul-10 16:24 ghak/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--  2.0 unx     5498 b- defN 23-Jul-10 16:46 ghak/factories/__pycache__/TokenFactory.cpython-311.pyc
+-rw-r--r--  2.0 unx      204 b- defN 23-Jul-10 16:46 ghak/factories/__pycache__/__init__.cpython-311.pyc
 -rw-r--r--  2.0 unx       28 b- defN 23-Jun-30 14:14 ghak/secretstores/__init__.py
 -rw-r--r--  2.0 unx     3841 b- defN 23-Jul-10 15:53 ghak/secretstores/secretstores.py
--rw-r--r--  2.0 unx      207 b- defN 23-Jul-10 16:24 ghak/secretstores/__pycache__/__init__.cpython-311.pyc
--rw-r--r--  2.0 unx     5756 b- defN 23-Jul-10 16:24 ghak/secretstores/__pycache__/secretstores.cpython-311.pyc
-19 files, 28735 bytes uncompressed, 12549 bytes compressed:  56.3%
+-rw-r--r--  2.0 unx      207 b- defN 23-Jul-10 16:46 ghak/secretstores/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--  2.0 unx     5756 b- defN 23-Jul-10 16:46 ghak/secretstores/__pycache__/secretstores.cpython-311.pyc
+19 files, 28627 bytes uncompressed, 12419 bytes compressed:  56.6%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ghak
-Version: 0.2.728
+Version: 0.2.734
 Author: William Turner
 Author-email: will@near.org
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

## ghak/ghak.py

```diff
@@ -1,41 +1,41 @@
 #!/usr/bin/env python3
 
 import click
-import click_log
 from .secretstores import SecretStore, SecretStoreGCP
 from .factories import TokenFactory
 import sys
 import logging
 
 logger = logging.getLogger(__name__)
-# click_log.basic_config(logger)
-
-logging.basicConfig(
-    stream=sys.stdout,
-    format="%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s",
-    level=logging.DEBUG,
-)
 
 
 # This project uses click to parse CLI arguments and
 # build the command layout.
 #
 # The method below is the main entrypoint for the cli tool
 @click.group()
-@click_log.simple_verbosity_option(logger)
 @click.pass_context
 @click.option("--debug/--no-debug", default=False, is_flag=True)
 def cli(ctx, debug):
     ctx.max_content_width = 200
     ctx.auto_envvar_prefix = "GHAK_"
     if debug:
-        logger.setLevel(logging.DEBUG)
+        logging.basicConfig(
+            stream=sys.stdout,
+            format="%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s",
+            level=logging.DEBUG,
+        )
+
     else:
-        logger.setLevel(logging.ERROR)
+        logging.basicConfig(
+            stream=sys.stdout,
+            format="%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s",
+            level=logging.ERROR,
+        )
 
 
 # The generate command is used to generate a GitHub
 # or GitHub Actions runner token.
 #
 # You need access to a PEM file generated when the app
 # was created in GitHub.
```

## ghak/__pycache__/__init__.cpython-311.pyc

### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xbd789f64 (Sat Jul  1 00:52:13 2023 UTC)
+moddate:  0x027bac64 (Mon Jul 10 21:41:22 2023 UTC)
 files sz: 90
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

## ghak/__pycache__/ghak.cpython-311.pyc

### Python bytecode

```diff
@@ -1,440 +1,421 @@
 magic:    0xa70d0d0a
-moddate:  0x4e70ac64 (Mon Jul 10 20:55:42 2023 UTC)
-files sz: 3694
+moddate:  0x207cac64 (Mon Jul 10 21:46:08 2023 UTC)
+files sz: 3745
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 16
    flags     : 0
    code
-      0x9700640064016c005a00640064016c015a01640264036c026d035a036d
-      045a040100640264046c056d065a060100640064016c075a07640064016c
-      085a08020065086a090000000000000000650aa6010000ab010000000000
-      0000005a0b020065086a0c000000000000000065076a0d00000000000000
-      00640565086a0e0000000000000000ac06a6030000ab0300000000000000
-      000100020065006a0f0000000000000000a6000000ab0000000000000000
-      00020065016a100000000000000000650ba6010000ab0100000000000000
-      0065006a110000000000000000020065006a120000000000000000640764
-      086409ac0aa6030000ab030000000000000000640b8400a6000000ab0000
+      0x9700640064016c005a00640264036c016d025a026d035a030100640264
+      046c046d055a050100640064016c065a06640064016c075a07020065076a
+      0800000000000000006509a6010000ab0100000000000000005a0a020065
+      006a0b0000000000000000a6000000ab00000000000000000065006a0c00
+      00000000000000020065006a0d0000000000000000640564066407ac08a6
+      030000ab03000000000000000064098400a6000000ab0000000000000000
+      00a6000000ab000000000000000000a6000000ab0000000000000000005a
+      0e650ea00f0000000000000000000000000000000000000000a6000000ab
+      000000000000000000020065006a0d0000000000000000640a640b640c64
+      0d6407ac0ea6050000ab050000000000000000020065006a0d0000000000
+      000000640f6410641164126407ac0ea6050000ab05000000000000000002
+      0065006a0d000000000000000064136414641564166407ac0ea6050000ab
+      050000000000000000020065006a0d000000000000000064176418641964
+      1a6407ac0ea6050000ab050000000000000000020065006a0d0000000000
+      000000641b641c641d641e020065006a100000000000000000641f642067
+      02a6010000ab010000000000000000641f6407ac21a6070000ab07000000
+      0000000000020065006a0d00000000000000006422642364246425020065
+      006a100000000000000000642664276702a6010000ab0100000000000000
+      0064076426ac28a6070000ab07000000000000000064298400a6000000ab
+      000000000000000000a6000000ab000000000000000000a6000000ab0000
       00000000000000a6000000ab000000000000000000a6000000ab00000000
-      0000000000a6000000ab0000000000000000005a136513a0140000000000
-      000000000000000000000000000000a6000000ab00000000000000000002
-      0065006a120000000000000000640c640d640e640f6409ac10a6050000ab
-      050000000000000000020065006a12000000000000000064116412641364
-      146409ac10a6050000ab050000000000000000020065006a120000000000
-      00000064156416641764186409ac10a6050000ab05000000000000000002
-      0065006a1200000000000000006419641a641b641c6409ac10a6050000ab
-      050000000000000000020065006a120000000000000000641d641e641f64
-      20020065006a150000000000000000642164226702a6010000ab01000000
-      000000000064216409ac23a6070000ab070000000000000000020065006a
-      1200000000000000006424642564266427020065006a1500000000000000
-      00642864296702a6010000ab01000000000000000064096428ac2aa60700
-      00ab070000000000000000642b8400a6000000ab000000000000000000a6
-      000000ab000000000000000000a6000000ab000000000000000000a60000
-      00ab000000000000000000a6000000ab000000000000000000a6000000ab
-      000000000000000000a6000000ab0000000000000000005a166513a01400
-      00000000000000000000000000000000000000a6000000ab000000000000
-      000000020065006a120000000000000000642c642d642e64186409ac10a6
-      050000ab050000000000000000020065006a120000000000000000641564
-      16642f64186409ac10a6050000ab05000000000000000064308400a60000
-      00ab000000000000000000a6000000ab000000000000000000a6000000ab
-      0000000000000000005a1764015300
+      0000000000a6000000ab000000000000000000a6000000ab000000000000
+      0000005a11650ea00f0000000000000000000000000000000000000000a6
+      000000ab000000000000000000020065006a0d0000000000000000642a64
+      2b642c64166407ac0ea6050000ab050000000000000000020065006a0d00
+      0000000000000064136414642d64166407ac0ea6050000ab050000000000
+      000000642e8400a6000000ab000000000000000000a6000000ab00000000
+      0000000000a6000000ab0000000000000000005a1264015300
      0           0 RESUME                   0
    
      3           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (click)
                  8 STORE_NAME               0 (click)
    
-     4          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               1 (None)
-                14 IMPORT_NAME              1 (click_log)
-                16 STORE_NAME               1 (click_log)
-   
-     5          18 LOAD_CONST               2 (1)
-                20 LOAD_CONST               3 (('SecretStore', 'SecretStoreGCP'))
-                22 IMPORT_NAME              2 (secretstores)
-                24 IMPORT_FROM              3 (SecretStore)
-                26 STORE_NAME               3 (SecretStore)
-                28 IMPORT_FROM              4 (SecretStoreGCP)
-                30 STORE_NAME               4 (SecretStoreGCP)
-                32 POP_TOP
-   
-     6          34 LOAD_CONST               2 (1)
-                36 LOAD_CONST               4 (('TokenFactory',))
-                38 IMPORT_NAME              5 (factories)
-                40 IMPORT_FROM              6 (TokenFactory)
-                42 STORE_NAME               6 (TokenFactory)
-                44 POP_TOP
+     4          10 LOAD_CONST               2 (1)
+                12 LOAD_CONST               3 (('SecretStore', 'SecretStoreGCP'))
+                14 IMPORT_NAME              1 (secretstores)
+                16 IMPORT_FROM              2 (SecretStore)
+                18 STORE_NAME               2 (SecretStore)
+                20 IMPORT_FROM              3 (SecretStoreGCP)
+                22 STORE_NAME               3 (SecretStoreGCP)
+                24 POP_TOP
+   
+     5          26 LOAD_CONST               2 (1)
+                28 LOAD_CONST               4 (('TokenFactory',))
+                30 IMPORT_NAME              4 (factories)
+                32 IMPORT_FROM              5 (TokenFactory)
+                34 STORE_NAME               5 (TokenFactory)
+                36 POP_TOP
+   
+     6          38 LOAD_CONST               0 (0)
+                40 LOAD_CONST               1 (None)
+                42 IMPORT_NAME              6 (sys)
+                44 STORE_NAME               6 (sys)
    
      7          46 LOAD_CONST               0 (0)
                 48 LOAD_CONST               1 (None)
-                50 IMPORT_NAME              7 (sys)
-                52 STORE_NAME               7 (sys)
+                50 IMPORT_NAME              7 (logging)
+                52 STORE_NAME               7 (logging)
    
-     8          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               1 (None)
-                58 IMPORT_NAME              8 (logging)
-                60 STORE_NAME               8 (logging)
-   
-    10          62 PUSH_NULL
-                64 LOAD_NAME                8 (logging)
-                66 LOAD_ATTR                9 (getLogger)
-                76 LOAD_NAME               10 (__name__)
-                78 PRECALL                  1
-                82 CALL                     1
-                92 STORE_NAME              11 (logger)
-   
-    13          94 PUSH_NULL
-                96 LOAD_NAME                8 (logging)
-                98 LOAD_ATTR               12 (basicConfig)
-   
-    14         108 LOAD_NAME                7 (sys)
-               110 LOAD_ATTR               13 (stdout)
-   
-    15         120 LOAD_CONST               5 ('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s')
-   
-    16         122 LOAD_NAME                8 (logging)
-               124 LOAD_ATTR               14 (DEBUG)
-   
-    13         134 KW_NAMES                 6
-               136 PRECALL                  3
-               140 CALL                     3
-               150 POP_TOP
-   
-    24         152 PUSH_NULL
-               154 LOAD_NAME                0 (click)
-               156 LOAD_ATTR               15 (group)
-               166 PRECALL                  0
-               170 CALL                     0
-   
-    25         180 PUSH_NULL
-               182 LOAD_NAME                1 (click_log)
-               184 LOAD_ATTR               16 (simple_verbosity_option)
-               194 LOAD_NAME               11 (logger)
-               196 PRECALL                  1
-               200 CALL                     1
-   
-    26         210 LOAD_NAME                0 (click)
-               212 LOAD_ATTR               17 (pass_context)
-   
-    27         222 PUSH_NULL
-               224 LOAD_NAME                0 (click)
-               226 LOAD_ATTR               18 (option)
-               236 LOAD_CONST               7 ('--debug/--no-debug')
-               238 LOAD_CONST               8 (False)
-               240 LOAD_CONST               9 (True)
-               242 KW_NAMES                10
-               244 PRECALL                  3
-               248 CALL                     3
-   
-    28         258 LOAD_CONST              11 (<code object cli, file "build/bdist.macosx-13-arm64/egg/ghak/ghak.py", line 24>)
-               260 MAKE_FUNCTION            0
+     9          54 PUSH_NULL
+                56 LOAD_NAME                7 (logging)
+                58 LOAD_ATTR                8 (getLogger)
+                68 LOAD_NAME                9 (__name__)
+                70 PRECALL                  1
+                74 CALL                     1
+                84 STORE_NAME              10 (logger)
+   
+    16          86 PUSH_NULL
+                88 LOAD_NAME                0 (click)
+                90 LOAD_ATTR               11 (group)
+               100 PRECALL                  0
+               104 CALL                     0
+   
+    17         114 LOAD_NAME                0 (click)
+               116 LOAD_ATTR               12 (pass_context)
+   
+    18         126 PUSH_NULL
+               128 LOAD_NAME                0 (click)
+               130 LOAD_ATTR               13 (option)
+               140 LOAD_CONST               5 ('--debug/--no-debug')
+               142 LOAD_CONST               6 (False)
+               144 LOAD_CONST               7 (True)
+               146 KW_NAMES                 8
+               148 PRECALL                  3
+               152 CALL                     3
    
-    27         262 PRECALL                  0
-               266 CALL                     0
+    19         162 LOAD_CONST               9 (<code object cli, file "build/bdist.macosx-13-arm64/egg/ghak/ghak.py", line 16>)
+               164 MAKE_FUNCTION            0
    
-    26         276 PRECALL                  0
-               280 CALL                     0
+    18         166 PRECALL                  0
+               170 CALL                     0
    
-    25         290 PRECALL                  0
-               294 CALL                     0
+    17         180 PRECALL                  0
+               184 CALL                     0
    
-    24         304 PRECALL                  0
-               308 CALL                     0
+    16         194 PRECALL                  0
+               198 CALL                     0
    
-    28         318 STORE_NAME              19 (cli)
+    19         208 STORE_NAME              14 (cli)
    
-    45         320 LOAD_NAME               19 (cli)
-               322 LOAD_METHOD             20 (command)
-               344 PRECALL                  0
-               348 CALL                     0
+    45         210 LOAD_NAME               14 (cli)
+               212 LOAD_METHOD             15 (command)
+               234 PRECALL                  0
+               238 CALL                     0
    
-    46         358 PUSH_NULL
-               360 LOAD_NAME                0 (click)
-               362 LOAD_ATTR               18 (option)
+    46         248 PUSH_NULL
+               250 LOAD_NAME                0 (click)
+               252 LOAD_ATTR               13 (option)
    
-    47         372 LOAD_CONST              12 ('-i')
+    47         262 LOAD_CONST              10 ('-i')
    
-    48         374 LOAD_CONST              13 ('--installation-id')
+    48         264 LOAD_CONST              11 ('--installation-id')
    
-    49         376 LOAD_CONST              14 ('INSTALLATION_ID')
+    49         266 LOAD_CONST              12 ('INSTALLATION_ID')
    
-    50         378 LOAD_CONST              15 ('App installation ID (can be found in GitHub)')
+    50         268 LOAD_CONST              13 ('App installation ID (can be found in GitHub)')
    
-    51         380 LOAD_CONST               9 (True)
+    51         270 LOAD_CONST               7 (True)
    
-    46         382 KW_NAMES                16
-               384 PRECALL                  5
-               388 CALL                     5
+    46         272 KW_NAMES                14
+               274 PRECALL                  5
+               278 CALL                     5
    
-    53         398 PUSH_NULL
-               400 LOAD_NAME                0 (click)
-               402 LOAD_ATTR               18 (option)
+    53         288 PUSH_NULL
+               290 LOAD_NAME                0 (click)
+               292 LOAD_ATTR               13 (option)
    
-    54         412 LOAD_CONST              17 ('-a')
+    54         302 LOAD_CONST              15 ('-a')
    
-    55         414 LOAD_CONST              18 ('--app-id')
+    55         304 LOAD_CONST              16 ('--app-id')
    
-    56         416 LOAD_CONST              19 ('APP_ID')
+    56         306 LOAD_CONST              17 ('APP_ID')
    
-    57         418 LOAD_CONST              20 ('GitHub application identifier (can be found in GitHub)')
+    57         308 LOAD_CONST              18 ('GitHub application identifier (can be found in GitHub)')
    
-    58         420 LOAD_CONST               9 (True)
+    58         310 LOAD_CONST               7 (True)
    
-    53         422 KW_NAMES                16
-               424 PRECALL                  5
-               428 CALL                     5
+    53         312 KW_NAMES                14
+               314 PRECALL                  5
+               318 CALL                     5
    
-    60         438 PUSH_NULL
-               440 LOAD_NAME                0 (click)
-               442 LOAD_ATTR               18 (option)
+    60         328 PUSH_NULL
+               330 LOAD_NAME                0 (click)
+               332 LOAD_ATTR               13 (option)
    
-    61         452 LOAD_CONST              21 ('-s')
+    61         342 LOAD_CONST              19 ('-s')
    
-    62         454 LOAD_CONST              22 ('--secret-id')
+    62         344 LOAD_CONST              20 ('--secret-id')
    
-    63         456 LOAD_CONST              23 ('KEY_PATH')
+    63         346 LOAD_CONST              21 ('KEY_PATH')
    
-    64         458 LOAD_CONST              24 ("Path to the app's private key in PEM format")
+    64         348 LOAD_CONST              22 ("Path to the app's private key in PEM format")
    
-    65         460 LOAD_CONST               9 (True)
+    65         350 LOAD_CONST               7 (True)
    
-    60         462 KW_NAMES                16
-               464 PRECALL                  5
-               468 CALL                     5
+    60         352 KW_NAMES                14
+               354 PRECALL                  5
+               358 CALL                     5
    
-    67         478 PUSH_NULL
-               480 LOAD_NAME                0 (click)
-               482 LOAD_ATTR               18 (option)
+    67         368 PUSH_NULL
+               370 LOAD_NAME                0 (click)
+               372 LOAD_ATTR               13 (option)
    
-    68         492 LOAD_CONST              25 ('-o')
+    68         382 LOAD_CONST              23 ('-o')
    
-    69         494 LOAD_CONST              26 ('--owner')
+    69         384 LOAD_CONST              24 ('--owner')
    
-    70         496 LOAD_CONST              27 ('OWNER')
+    70         386 LOAD_CONST              25 ('OWNER')
    
-    71         498 LOAD_CONST              28 ('Organization to attach runners to ')
+    71         388 LOAD_CONST              26 ('Organization to attach runners to ')
    
-    72         500 LOAD_CONST               9 (True)
+    72         390 LOAD_CONST               7 (True)
    
-    67         502 KW_NAMES                16
-               504 PRECALL                  5
-               508 CALL                     5
+    67         392 KW_NAMES                14
+               394 PRECALL                  5
+               398 CALL                     5
    
-    74         518 PUSH_NULL
-               520 LOAD_NAME                0 (click)
-               522 LOAD_ATTR               18 (option)
+    74         408 PUSH_NULL
+               410 LOAD_NAME                0 (click)
+               412 LOAD_ATTR               13 (option)
    
-    75         532 LOAD_CONST              29 ('-y')
+    75         422 LOAD_CONST              27 ('-y')
    
-    76         534 LOAD_CONST              30 ('--owner-type')
+    76         424 LOAD_CONST              28 ('--owner-type')
    
-    77         536 LOAD_CONST              31 ('OWNER_TYPE')
+    77         426 LOAD_CONST              29 ('OWNER_TYPE')
    
-    78         538 LOAD_CONST              32 ('Type of owner')
+    78         428 LOAD_CONST              30 ('Type of owner')
    
-    79         540 PUSH_NULL
-               542 LOAD_NAME                0 (click)
-               544 LOAD_ATTR               21 (Choice)
-               554 LOAD_CONST              33 ('organization')
-               556 LOAD_CONST              34 ('repo')
-               558 BUILD_LIST               2
-               560 PRECALL                  1
-               564 CALL                     1
+    79         430 PUSH_NULL
+               432 LOAD_NAME                0 (click)
+               434 LOAD_ATTR               16 (Choice)
+               444 LOAD_CONST              31 ('organization')
+               446 LOAD_CONST              32 ('repo')
+               448 BUILD_LIST               2
+               450 PRECALL                  1
+               454 CALL                     1
    
-    80         574 LOAD_CONST              33 ('organization')
+    80         464 LOAD_CONST              31 ('organization')
    
-    81         576 LOAD_CONST               9 (True)
+    81         466 LOAD_CONST               7 (True)
    
-    74         578 KW_NAMES                35
-               580 PRECALL                  7
-               584 CALL                     7
+    74         468 KW_NAMES                33
+               470 PRECALL                  7
+               474 CALL                     7
    
-    83         594 PUSH_NULL
-               596 LOAD_NAME                0 (click)
-               598 LOAD_ATTR               18 (option)
+    83         484 PUSH_NULL
+               486 LOAD_NAME                0 (click)
+               488 LOAD_ATTR               13 (option)
    
-    84         608 LOAD_CONST              36 ('-t')
+    84         498 LOAD_CONST              34 ('-t')
    
-    85         610 LOAD_CONST              37 ('--token-type')
+    85         500 LOAD_CONST              35 ('--token-type')
    
-    86         612 LOAD_CONST              38 ('TOKEN_TYPE')
+    86         502 LOAD_CONST              36 ('TOKEN_TYPE')
    
-    87         614 LOAD_CONST              39 ('Which type of token to generate')
+    87         504 LOAD_CONST              37 ('Which type of token to generate')
    
-    88         616 PUSH_NULL
-               618 LOAD_NAME                0 (click)
-               620 LOAD_ATTR               21 (Choice)
-               630 LOAD_CONST              40 ('runner')
-               632 LOAD_CONST              41 ('github')
-               634 BUILD_LIST               2
-               636 PRECALL                  1
-               640 CALL                     1
+    88         506 PUSH_NULL
+               508 LOAD_NAME                0 (click)
+               510 LOAD_ATTR               16 (Choice)
+               520 LOAD_CONST              38 ('runner')
+               522 LOAD_CONST              39 ('github')
+               524 BUILD_LIST               2
+               526 PRECALL                  1
+               530 CALL                     1
    
-    89         650 LOAD_CONST               9 (True)
+    89         540 LOAD_CONST               7 (True)
    
-    90         652 LOAD_CONST              40 ('runner')
+    90         542 LOAD_CONST              38 ('runner')
    
-    83         654 KW_NAMES                42
-               656 PRECALL                  7
-               660 CALL                     7
+    83         544 KW_NAMES                40
+               546 PRECALL                  7
+               550 CALL                     7
    
-    92         670 LOAD_CONST              43 (<code object generate, file "build/bdist.macosx-13-arm64/egg/ghak/ghak.py", line 45>)
-               672 MAKE_FUNCTION            0
+    92         560 LOAD_CONST              41 (<code object generate, file "build/bdist.macosx-13-arm64/egg/ghak/ghak.py", line 45>)
+               562 MAKE_FUNCTION            0
    
-    83         674 PRECALL                  0
-               678 CALL                     0
+    83         564 PRECALL                  0
+               568 CALL                     0
    
-    74         688 PRECALL                  0
-               692 CALL                     0
+    74         578 PRECALL                  0
+               582 CALL                     0
    
-    67         702 PRECALL                  0
-               706 CALL                     0
+    67         592 PRECALL                  0
+               596 CALL                     0
    
-    60         716 PRECALL                  0
-               720 CALL                     0
+    60         606 PRECALL                  0
+               610 CALL                     0
    
-    53         730 PRECALL                  0
-               734 CALL                     0
+    53         620 PRECALL                  0
+               624 CALL                     0
    
-    46         744 PRECALL                  0
-               748 CALL                     0
+    46         634 PRECALL                  0
+               638 CALL                     0
    
-    45         758 PRECALL                  0
-               762 CALL                     0
+    45         648 PRECALL                  0
+               652 CALL                     0
    
-    92         772 STORE_NAME              22 (generate)
+    92         662 STORE_NAME              17 (generate)
    
-   118         774 LOAD_NAME               19 (cli)
-               776 LOAD_METHOD             20 (command)
-               798 PRECALL                  0
-               802 CALL                     0
+   118         664 LOAD_NAME               14 (cli)
+               666 LOAD_METHOD             15 (command)
+               688 PRECALL                  0
+               692 CALL                     0
    
-   119         812 PUSH_NULL
-               814 LOAD_NAME                0 (click)
-               816 LOAD_ATTR               18 (option)
+   119         702 PUSH_NULL
+               704 LOAD_NAME                0 (click)
+               706 LOAD_ATTR               13 (option)
    
-   120         826 LOAD_CONST              44 ('-f')
+   120         716 LOAD_CONST              42 ('-f')
    
-   121         828 LOAD_CONST              45 ('--file')
+   121         718 LOAD_CONST              43 ('--file')
    
-   122         830 LOAD_CONST              46 ('GHA_PEM_FILE')
+   122         720 LOAD_CONST              44 ('GHA_PEM_FILE')
    
-   123         832 LOAD_CONST              24 ("Path to the app's private key in PEM format")
+   123         722 LOAD_CONST              22 ("Path to the app's private key in PEM format")
    
-   124         834 LOAD_CONST               9 (True)
+   124         724 LOAD_CONST               7 (True)
    
-   119         836 KW_NAMES                16
-               838 PRECALL                  5
-               842 CALL                     5
+   119         726 KW_NAMES                14
+               728 PRECALL                  5
+               732 CALL                     5
    
-   126         852 PUSH_NULL
-               854 LOAD_NAME                0 (click)
-               856 LOAD_ATTR               18 (option)
+   126         742 PUSH_NULL
+               744 LOAD_NAME                0 (click)
+               746 LOAD_ATTR               13 (option)
    
-   127         866 LOAD_CONST              21 ('-s')
+   127         756 LOAD_CONST              19 ('-s')
    
-   128         868 LOAD_CONST              22 ('--secret-id')
+   128         758 LOAD_CONST              20 ('--secret-id')
    
-   129         870 LOAD_CONST              47 ('GHA_KEY_PATH')
+   129         760 LOAD_CONST              45 ('GHA_KEY_PATH')
    
-   130         872 LOAD_CONST              24 ("Path to the app's private key in PEM format")
+   130         762 LOAD_CONST              22 ("Path to the app's private key in PEM format")
    
-   131         874 LOAD_CONST               9 (True)
+   131         764 LOAD_CONST               7 (True)
    
-   126         876 KW_NAMES                16
-               878 PRECALL                  5
-               882 CALL                     5
+   126         766 KW_NAMES                14
+               768 PRECALL                  5
+               772 CALL                     5
    
-   133         892 LOAD_CONST              48 (<code object upload_pem, file "build/bdist.macosx-13-arm64/egg/ghak/ghak.py", line 118>)
-               894 MAKE_FUNCTION            0
+   133         782 LOAD_CONST              46 (<code object upload_pem, file "build/bdist.macosx-13-arm64/egg/ghak/ghak.py", line 118>)
+               784 MAKE_FUNCTION            0
    
-   126         896 PRECALL                  0
-               900 CALL                     0
+   126         786 PRECALL                  0
+               790 CALL                     0
    
-   119         910 PRECALL                  0
-               914 CALL                     0
+   119         800 PRECALL                  0
+               804 CALL                     0
    
-   118         924 PRECALL                  0
-               928 CALL                     0
+   118         814 PRECALL                  0
+               818 CALL                     0
    
-   133         938 STORE_NAME              23 (upload_pem)
-               940 LOAD_CONST               1 (None)
-               942 RETURN_VALUE
+   133         828 STORE_NAME              18 (upload_pem)
+               830 LOAD_CONST               1 (None)
+               832 RETURN_VALUE
    consts
       0
       None
       1
       ('SecretStore', 'SecretStoreGCP')
       ('TokenFactory',)
-      '%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s'
-      ('stream', 'format', 'level')
       '--debug/--no-debug'
       False
       True
       ('default', 'is_flag')
       code
          argcount  : 2
          nlocals   : 2
-         stacksize : 3
+         stacksize : 5
          flags     : 3
          code
             0x970064017c005f00000000000000000064027c005f0100000000000000
-            007c017226740400000000000000000000a0030000000000000000000000
-            0000000000000000007408000000000000000000006a0500000000000000
-            00a6010000ab010000000000000000010064005300740400000000000000
-            000000a00300000000000000000000000000000000000000007408000000
-            000000000000006a060000000000000000a6010000ab0100000000000000
-            00010064005300
-          24           0 RESUME                   0
+            007c01722d7405000000000000000000006a030000000000000000740800
+            0000000000000000006a0500000000000000006403740400000000000000
+            0000006a060000000000000000ac04a6030000ab03000000000000000001
+            00640053007405000000000000000000006a030000000000000000740800
+            0000000000000000006a0500000000000000006403740400000000000000
+            0000006a070000000000000000ac04a6030000ab03000000000000000001
+            0064005300
+          16           0 RESUME                   0
          
-          29           2 LOAD_CONST               1 (200)
+          20           2 LOAD_CONST               1 (200)
                        4 LOAD_FAST                0 (ctx)
                        6 STORE_ATTR               0 (max_content_width)
          
-          30          16 LOAD_CONST               2 ('GHAK_')
+          21          16 LOAD_CONST               2 ('GHAK_')
                       18 LOAD_FAST                0 (ctx)
                       20 STORE_ATTR               1 (auto_envvar_prefix)
          
-          31          30 LOAD_FAST                1 (debug)
-                      32 POP_JUMP_FORWARD_IF_FALSE    38 (to 110)
+          22          30 LOAD_FAST                1 (debug)
+                      32 POP_JUMP_FORWARD_IF_FALSE    45 (to 124)
+         
+          23          34 LOAD_GLOBAL              5 (NULL + logging)
+                      46 LOAD_ATTR                3 (basicConfig)
+         
+          24          56 LOAD_GLOBAL              8 (sys)
+                      68 LOAD_ATTR                5 (stdout)
+         
+          25          78 LOAD_CONST               3 ('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s')
+         
+          26          80 LOAD_GLOBAL              4 (logging)
+                      92 LOAD_ATTR                6 (DEBUG)
+         
+          23         102 KW_NAMES                 4
+                     104 PRECALL                  3
+                     108 CALL                     3
+                     118 POP_TOP
+                     120 LOAD_CONST               0 (None)
+                     122 RETURN_VALUE
+         
+          30     >>  124 LOAD_GLOBAL              5 (NULL + logging)
+                     136 LOAD_ATTR                3 (basicConfig)
+         
+          31         146 LOAD_GLOBAL              8 (sys)
+                     158 LOAD_ATTR                5 (stdout)
+         
+          32         168 LOAD_CONST               3 ('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s')
+         
+          33         170 LOAD_GLOBAL              4 (logging)
+                     182 LOAD_ATTR                7 (ERROR)
          
-          32          34 LOAD_GLOBAL              4 (logger)
-                      46 LOAD_METHOD              3 (setLevel)
-                      68 LOAD_GLOBAL              8 (logging)
-                      80 LOAD_ATTR                5 (DEBUG)
-                      90 PRECALL                  1
-                      94 CALL                     1
-                     104 POP_TOP
-                     106 LOAD_CONST               0 (None)
-                     108 RETURN_VALUE
-         
-          34     >>  110 LOAD_GLOBAL              4 (logger)
-                     122 LOAD_METHOD              3 (setLevel)
-                     144 LOAD_GLOBAL              8 (logging)
-                     156 LOAD_ATTR                6 (ERROR)
-                     166 PRECALL                  1
-                     170 CALL                     1
-                     180 POP_TOP
-                     182 LOAD_CONST               0 (None)
-                     184 RETURN_VALUE
+          30         192 KW_NAMES                 4
+                     194 PRECALL                  3
+                     198 CALL                     3
+                     208 POP_TOP
+                     210 LOAD_CONST               0 (None)
+                     212 RETURN_VALUE
          consts
             None
             200
             'GHAK_'
-         names      ('max_content_width', 'auto_envvar_prefix', 'logger', 'setLevel', 'logging', 'DEBUG', 'ERROR')
+            '%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s'
+            ('stream', 'format', 'level')
+         names      ('max_content_width', 'auto_envvar_prefix', 'logging', 'basicConfig', 'sys', 'stdout', 'DEBUG', 'ERROR')
          varnames   ('ctx', 'debug')
          freevars   ()
          cellvars   ()
          filename   'build/bdist.macosx-13-arm64/egg/ghak/ghak.py'
          name       'cli'
-         firstlineno 24
-         lnotab 0x02050e010e0104014c02
+         firstlineno 16
+         lnotab 0x02040e010e01040116011601020116fd160716011601020116fd
       '-i'
       '--installation-id'
       'INSTALLATION_ID'
       'App installation ID (can be found in GitHub)'
       ('envvar', 'help', 'required')
       '-a'
       '--app-id'
@@ -639,22 +620,22 @@
          varnames   ('file', 'secret_id', 'filestore', 'secretmanager', 'pem_file')
          freevars   ()
          cellvars   ()
          filename   'build/bdist.macosx-13-arm64/egg/ghak/ghak.py'
          name       'upload_pem'
          firstlineno 118
          lnotab 0x021134031c011c022a022c01
-   names      ('click', 'click_log', 'secretstores', 'SecretStore', 'SecretStoreGCP', 'factories', 'TokenFactory', 'sys', 'logging', 'getLogger', '__name__', 'logger', 'basicConfig', 'stdout', 'DEBUG', 'group', 'simple_verbosity_option', 'pass_context', 'option', 'cli', 'command', 'Choice', 'generate', 'upload_pem')
+   names      ('click', 'secretstores', 'SecretStore', 'SecretStoreGCP', 'factories', 'TokenFactory', 'sys', 'logging', 'getLogger', '__name__', 'logger', 'group', 'pass_context', 'option', 'cli', 'command', 'Choice', 'generate', 'upload_pem')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'build/bdist.macosx-13-arm64/egg/ghak/ghak.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02030801080110010c010801080220030e010c0102010cfd120b1c
-      011e010c01240104ff0eff0eff0eff0e04021126010e0102010201020102
-      0102fb10070e01020102010201020102fb10070e01020102010201020102
-      fb10070e01020102010201020102fb10070e010201020102010201220102
-      0102f910090e0102010201020102012201020102f9100904f70ef70ef90e
-      f90ef90ef90eff0e2f021a26010e01020102010201020102fb10070e0102
-      0102010201020102fb100704f90ef90eff0e0f
+      0x00ff0203080110010c010801080220071c010c01240104ff0eff0eff0e
+      03021a26010e01020102010201020102fb10070e01020102010201020102
+      fb10070e01020102010201020102fb10070e01020102010201020102fb10
+      070e0102010201020102012201020102f910090e01020102010201020122
+      01020102f9100904f70ef70ef90ef90ef90ef90eff0e2f021a26010e0102
+      0102010201020102fb10070e01020102010201020102fb100704f90ef90e
+      ff0e0f
```

