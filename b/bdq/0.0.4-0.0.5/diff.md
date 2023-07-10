# Comparing `tmp/bdq-0.0.4.tar.gz` & `tmp/bdq-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdq-0.0.4.tar", last modified: Fri Jun 30 12:59:41 2023, max compression
+gzip compressed data, was "bdq-0.0.5.tar", last modified: Mon Jul 10 06:29:06 2023, max compression
```

## Comparing `bdq-0.0.4.tar` & `bdq-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:59:41.288829 bdq-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 12:59:28.000000 bdq-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-06-30 12:59:41.288829 bdq-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-06-30 12:59:28.000000 bdq-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:59:41.288829 bdq-0.0.4/bdq/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-30 12:59:28.000000 bdq-0.0.4/bdq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-30 12:59:28.000000 bdq-0.0.4/bdq/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-06-30 12:59:28.000000 bdq-0.0.4/bdq/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-30 12:59:28.000000 bdq-0.0.4/bdq/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-30 12:59:28.000000 bdq-0.0.4/bdq/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-30 12:59:28.000000 bdq-0.0.4/bdq/spark_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:59:41.288829 bdq-0.0.4/bdq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-06-30 12:59:41.000000 bdq-0.0.4/bdq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-30 12:59:41.000000 bdq-0.0.4/bdq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:59:41.000000 bdq-0.0.4/bdq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-30 12:59:41.000000 bdq-0.0.4/bdq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-30 12:59:28.000000 bdq-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:59:41.288829 bdq-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:29:06.286850 bdq-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 06:28:56.000000 bdq-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22082 2023-07-10 06:29:06.286850 bdq-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21475 2023-07-10 06:28:56.000000 bdq-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:29:06.286850 bdq-0.0.5/bdq/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-10 06:28:56.000000 bdq-0.0.5/bdq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-10 06:28:56.000000 bdq-0.0.5/bdq/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-07-10 06:28:56.000000 bdq-0.0.5/bdq/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-10 06:28:56.000000 bdq-0.0.5/bdq/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-10 06:28:56.000000 bdq-0.0.5/bdq/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-10 06:28:56.000000 bdq-0.0.5/bdq/spark_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-10 06:28:56.000000 bdq-0.0.5/bdq/spark_ui_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:29:06.286850 bdq-0.0.5/bdq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22082 2023-07-10 06:29:06.000000 bdq-0.0.5/bdq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-10 06:29:06.000000 bdq-0.0.5/bdq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:29:06.000000 bdq-0.0.5/bdq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 06:29:06.000000 bdq-0.0.5/bdq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-10 06:28:56.000000 bdq-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 06:29:06.286850 bdq-0.0.5/setup.cfg
```

### Comparing `bdq-0.0.4/LICENSE` & `bdq-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bdq-0.0.4/PKG-INFO` & `bdq-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6264 710a  : 2.1.Name: bdq.
-00000020: 5665 7273 696f 6e3a 2030 2e30 2e34 0a53  Version: 0.0.4.S
+00000020: 5665 7273 696f 6e3a 2030 2e30 2e35 0a53  Version: 0.0.5.S
 00000030: 756d 6d61 7279 3a20 4269 6720 4461 7461  ummary: Big Data
 00000040: 2051 7561 6c69 7479 2c20 6120 7365 7420   Quality, a set 
 00000050: 6f66 2074 6f6f 6c73 2f66 756e 6374 696f  of tools/functio
 00000060: 6e20 7468 6174 2068 656c 7020 796f 7520  n that help you 
 00000070: 6576 6572 7920 6461 7920 6173 7365 7274  every day assert
 00000080: 2071 7561 6c69 7479 206f 6620 6461 7461   quality of data
 00000090: 7365 7473 2079 6f75 2068 6176 6520 7072  sets you have pr
@@ -1308,8 +1308,74 @@
 000051b0: 7263 6527 2077 696c 6c20 6265 2075 7064  rce' will be upd
 000051c0: 6174 6564 2077 6865 6e20 7468 6973 2066  ated when this f
 000051d0: 756e 6374 696f 6e20 6669 6e69 7368 6573  unction finishes
 000051e0: 2028 6173 2070 6572 2064 6566 696e 7469   (as per definti
 000051f0: 6f6e 2069 6e20 4070 706e 2e73 7465 7020  on in @ppn.step 
 00005200: 6162 6f76 6529 0a72 6177 5f64 6174 615f  above).raw_data_
 00005210: 7369 6e67 6c65 5f73 6f75 7263 6528 290a  single_source().
-00005220: 6060 600a                                ```.
+00005220: 6060 600a 0a23 2320 5370 6172 6b20 5549  ```..## Spark UI
+00005230: 2053 7461 6765 2064 6573 6372 6970 7469   Stage descripti
+00005240: 6f6e 730a 5768 656e 2072 756e 6e69 6e67  ons.When running
+00005250: 2063 6f64 6520 7573 696e 6720 7079 7370   code using pysp
+00005260: 6172 6b2c 2073 7061 726b 2075 6920 6765  ark, spark ui ge
+00005270: 7473 2076 6572 7920 6372 6f77 6465 642e  ts very crowded.
+00005280: 2060 5370 6172 6b55 494c 6f67 6765 7260   `SparkUILogger`
+00005290: 2063 6f6e 7465 7874 206d 616e 6167 6572   context manager
+000052a0: 2061 6e64 2064 6563 6f72 6174 6f72 2061   and decorator a
+000052b0: 7373 696e 6773 2068 756d 616e 2072 6561  ssings human rea
+000052c0: 6461 626c 6520 6e61 6d65 7320 746f 2073  dable names to s
+000052d0: 7061 726b 2073 7461 6765 732e 0a0a 6060  park stages...``
+000052e0: 6070 7974 686f 6e0a 6672 6f6d 2062 6471  `python.from bdq
+000052f0: 0a0a 2320 7573 6167 6520 6f66 2064 6563  ..# usage of dec
+00005300: 6f72 6174 6f72 730a 2320 7370 6172 6b20  orators.# spark 
+00005310: 7569 2073 7461 6765 7320 7769 6c6c 2068  ui stages will h
+00005320: 6176 6520 6465 7363 7269 7074 696f 6e20  ave description 
+00005330: 6f66 2027 7879 7a27 0a40 5370 6172 6b55  of 'xyz'.@SparkU
+00005340: 494c 6f67 6765 722e 7461 6728 6465 7363  ILogger.tag(desc
+00005350: 3d27 7879 7a27 290a 6465 6620 736f 6d65  ='xyz').def some
+00005360: 5f66 756e 6374 696f 6e32 286e 756d 6265  _function2(numbe
+00005370: 7229 3a0a 0a20 2072 6574 7572 6e20 7370  r):..  return sp
+00005380: 6172 6b2e 7261 6e67 6528 6e75 6d62 6572  ark.range(number
+00005390: 292e 636f 756e 7428 290a 0a23 2073 7061  ).count()..# spa
+000053a0: 726b 2075 6920 7374 6167 6573 2077 696c  rk ui stages wil
+000053b0: 6c20 6861 7665 2064 6573 6372 6970 7469  l have descripti
+000053c0: 6f6e 206f 6620 2761 6c70 6861 5f66 756e  on of 'alpha_fun
+000053d0: 6374 696f 6e32 2720 2861 7574 6f6d 6174  ction2' (automat
+000053e0: 6963 616c 6c79 2064 6572 6976 6564 2066  ically derived f
+000053f0: 726f 6d20 6675 6e63 7469 6f6e 206e 616d  rom function nam
+00005400: 6529 0a40 5370 6172 6b55 494c 6f67 6765  e).@SparkUILogge
+00005410: 722e 7461 670a 6465 6620 616c 7068 615f  r.tag.def alpha_
+00005420: 6675 6e63 7469 6f6e 3228 6e75 6d62 6572  function2(number
+00005430: 293a 0a20 2023 2031 7374 2061 6e64 2032  ):.  # 1st and 2
+00005440: 6e64 2073 6f6d 655f 6675 6e63 7469 6f6e  nd some_function
+00005450: 3228 2920 6361 6c6c 7320 7368 6f75 6c64  2() calls should
+00005460: 2062 6520 7669 7369 626c 6520 696e 2073   be visible in s
+00005470: 7061 726b 2075 6920 6173 2027 7879 7a27  park ui as 'xyz'
+00005480: 0a20 2023 2074 6865 2033 7264 2070 6172  .  # the 3rd par
+00005490: 7420 6f66 2072 6573 756c 7420 7368 6f75  t of result shou
+000054a0: 6c64 2062 6520 7669 7369 626c 6520 6173  ld be visible as
+000054b0: 2027 616c 7068 615f 6675 6e63 7469 6f6e   'alpha_function
+000054c0: 320a 2020 7265 7475 726e 2073 6f6d 655f  2.  return some_
+000054d0: 6675 6e63 7469 6f6e 3228 6e75 6d62 6572  function2(number
+000054e0: 2a32 2920 2b20 736f 6d65 5f66 756e 6374  *2) + some_funct
+000054f0: 696f 6e32 286e 756d 6265 722a 3329 202b  ion2(number*3) +
+00005500: 2073 7061 726b 2e72 616e 6765 286e 756d   spark.range(num
+00005510: 6265 722f 3130 292e 636f 756e 7428 290a  ber/10).count().
+00005520: 0a23 2075 7361 6765 206f 6620 636f 6e74  .# usage of cont
+00005530: 6578 7420 6d61 6e61 6765 7273 0a23 2077  ext managers.# w
+00005540: 696c 6c20 6265 2076 6973 6962 6c65 2069  ill be visible i
+00005550: 6e20 7370 6172 6b20 7569 2061 7320 2766  n spark ui as 'f
+00005560: 6972 7374 2d63 6f75 6e74 270a 7769 7468  irst-count'.with
+00005570: 2053 7061 726b 5549 4c6f 6767 6572 2827   SparkUILogger('
+00005580: 6669 7273 742d 636f 756e 7427 293a 0a20  first-count'):. 
+00005590: 2073 7061 726b 2e72 616e 6765 2831 3029   spark.range(10)
+000055a0: 2e63 6f75 6e74 2829 0a0a 2320 7769 6c6c  .count()..# will
+000055b0: 2062 6520 7669 7369 626c 6520 696e 2073   be visible in s
+000055c0: 7061 726b 2075 6920 6173 2027 326e 642d  park ui as '2nd-
+000055d0: 636f 756e 7427 0a77 6974 6820 5370 6172  count'.with Spar
+000055e0: 6b55 494c 6f67 6765 7228 2732 6e64 2d63  kUILogger('2nd-c
+000055f0: 6f75 6e74 2729 3a0a 2020 7370 6172 6b2e  ount'):.  spark.
+00005600: 7261 6e67 6528 3230 292e 636f 756e 7428  range(20).count(
+00005610: 290a 0a73 6f6d 655f 6675 6e63 7469 6f6e  )..some_function
+00005620: 3228 3130 3030 290a 616c 7068 615f 6675  2(1000).alpha_fu
+00005630: 6e63 7469 6f6e 3228 3230 3030 290a 6060  nction2(2000).``
+00005640: 600a                                     `.
```

### Comparing `bdq-0.0.4/README.md` & `bdq-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1270,8 +1270,74 @@
 00004f50: 7572 6365 2720 7769 6c6c 2062 6520 7570  urce' will be up
 00004f60: 6461 7465 6420 7768 656e 2074 6869 7320  dated when this 
 00004f70: 6675 6e63 7469 6f6e 2066 696e 6973 6865  function finishe
 00004f80: 7320 2861 7320 7065 7220 6465 6669 6e74  s (as per defint
 00004f90: 696f 6e20 696e 2040 7070 6e2e 7374 6570  ion in @ppn.step
 00004fa0: 2061 626f 7665 290a 7261 775f 6461 7461   above).raw_data
 00004fb0: 5f73 696e 676c 655f 736f 7572 6365 2829  _single_source()
-00004fc0: 0a60 6060 0a                             .```.
+00004fc0: 0a60 6060 0a0a 2323 2053 7061 726b 2055  .```..## Spark U
+00004fd0: 4920 5374 6167 6520 6465 7363 7269 7074  I Stage descript
+00004fe0: 696f 6e73 0a57 6865 6e20 7275 6e6e 696e  ions.When runnin
+00004ff0: 6720 636f 6465 2075 7369 6e67 2070 7973  g code using pys
+00005000: 7061 726b 2c20 7370 6172 6b20 7569 2067  park, spark ui g
+00005010: 6574 7320 7665 7279 2063 726f 7764 6564  ets very crowded
+00005020: 2e20 6053 7061 726b 5549 4c6f 6767 6572  . `SparkUILogger
+00005030: 6020 636f 6e74 6578 7420 6d61 6e61 6765  ` context manage
+00005040: 7220 616e 6420 6465 636f 7261 746f 7220  r and decorator 
+00005050: 6173 7369 6e67 7320 6875 6d61 6e20 7265  assings human re
+00005060: 6164 6162 6c65 206e 616d 6573 2074 6f20  adable names to 
+00005070: 7370 6172 6b20 7374 6167 6573 2e0a 0a60  spark stages...`
+00005080: 6060 7079 7468 6f6e 0a66 726f 6d20 6264  ``python.from bd
+00005090: 710a 0a23 2075 7361 6765 206f 6620 6465  q..# usage of de
+000050a0: 636f 7261 746f 7273 0a23 2073 7061 726b  corators.# spark
+000050b0: 2075 6920 7374 6167 6573 2077 696c 6c20   ui stages will 
+000050c0: 6861 7665 2064 6573 6372 6970 7469 6f6e  have description
+000050d0: 206f 6620 2778 797a 270a 4053 7061 726b   of 'xyz'.@Spark
+000050e0: 5549 4c6f 6767 6572 2e74 6167 2864 6573  UILogger.tag(des
+000050f0: 633d 2778 797a 2729 0a64 6566 2073 6f6d  c='xyz').def som
+00005100: 655f 6675 6e63 7469 6f6e 3228 6e75 6d62  e_function2(numb
+00005110: 6572 293a 0a0a 2020 7265 7475 726e 2073  er):..  return s
+00005120: 7061 726b 2e72 616e 6765 286e 756d 6265  park.range(numbe
+00005130: 7229 2e63 6f75 6e74 2829 0a0a 2320 7370  r).count()..# sp
+00005140: 6172 6b20 7569 2073 7461 6765 7320 7769  ark ui stages wi
+00005150: 6c6c 2068 6176 6520 6465 7363 7269 7074  ll have descript
+00005160: 696f 6e20 6f66 2027 616c 7068 615f 6675  ion of 'alpha_fu
+00005170: 6e63 7469 6f6e 3227 2028 6175 746f 6d61  nction2' (automa
+00005180: 7469 6361 6c6c 7920 6465 7269 7665 6420  tically derived 
+00005190: 6672 6f6d 2066 756e 6374 696f 6e20 6e61  from function na
+000051a0: 6d65 290a 4053 7061 726b 5549 4c6f 6767  me).@SparkUILogg
+000051b0: 6572 2e74 6167 0a64 6566 2061 6c70 6861  er.tag.def alpha
+000051c0: 5f66 756e 6374 696f 6e32 286e 756d 6265  _function2(numbe
+000051d0: 7229 3a0a 2020 2320 3173 7420 616e 6420  r):.  # 1st and 
+000051e0: 326e 6420 736f 6d65 5f66 756e 6374 696f  2nd some_functio
+000051f0: 6e32 2829 2063 616c 6c73 2073 686f 756c  n2() calls shoul
+00005200: 6420 6265 2076 6973 6962 6c65 2069 6e20  d be visible in 
+00005210: 7370 6172 6b20 7569 2061 7320 2778 797a  spark ui as 'xyz
+00005220: 270a 2020 2320 7468 6520 3372 6420 7061  '.  # the 3rd pa
+00005230: 7274 206f 6620 7265 7375 6c74 2073 686f  rt of result sho
+00005240: 756c 6420 6265 2076 6973 6962 6c65 2061  uld be visible a
+00005250: 7320 2761 6c70 6861 5f66 756e 6374 696f  s 'alpha_functio
+00005260: 6e32 0a20 2072 6574 7572 6e20 736f 6d65  n2.  return some
+00005270: 5f66 756e 6374 696f 6e32 286e 756d 6265  _function2(numbe
+00005280: 722a 3229 202b 2073 6f6d 655f 6675 6e63  r*2) + some_func
+00005290: 7469 6f6e 3228 6e75 6d62 6572 2a33 2920  tion2(number*3) 
+000052a0: 2b20 7370 6172 6b2e 7261 6e67 6528 6e75  + spark.range(nu
+000052b0: 6d62 6572 2f31 3029 2e63 6f75 6e74 2829  mber/10).count()
+000052c0: 0a0a 2320 7573 6167 6520 6f66 2063 6f6e  ..# usage of con
+000052d0: 7465 7874 206d 616e 6167 6572 730a 2320  text managers.# 
+000052e0: 7769 6c6c 2062 6520 7669 7369 626c 6520  will be visible 
+000052f0: 696e 2073 7061 726b 2075 6920 6173 2027  in spark ui as '
+00005300: 6669 7273 742d 636f 756e 7427 0a77 6974  first-count'.wit
+00005310: 6820 5370 6172 6b55 494c 6f67 6765 7228  h SparkUILogger(
+00005320: 2766 6972 7374 2d63 6f75 6e74 2729 3a0a  'first-count'):.
+00005330: 2020 7370 6172 6b2e 7261 6e67 6528 3130    spark.range(10
+00005340: 292e 636f 756e 7428 290a 0a23 2077 696c  ).count()..# wil
+00005350: 6c20 6265 2076 6973 6962 6c65 2069 6e20  l be visible in 
+00005360: 7370 6172 6b20 7569 2061 7320 2732 6e64  spark ui as '2nd
+00005370: 2d63 6f75 6e74 270a 7769 7468 2053 7061  -count'.with Spa
+00005380: 726b 5549 4c6f 6767 6572 2827 326e 642d  rkUILogger('2nd-
+00005390: 636f 756e 7427 293a 0a20 2073 7061 726b  count'):.  spark
+000053a0: 2e72 616e 6765 2832 3029 2e63 6f75 6e74  .range(20).count
+000053b0: 2829 0a0a 736f 6d65 5f66 756e 6374 696f  ()..some_functio
+000053c0: 6e32 2831 3030 3029 0a61 6c70 6861 5f66  n2(1000).alpha_f
+000053d0: 756e 6374 696f 6e32 2832 3030 3029 0a60  unction2(2000).`
+000053e0: 6060 0a                                  ``.
```

### Comparing `bdq-0.0.4/bdq/dag.py` & `bdq-0.0.5/bdq/dag.py`

 * *Files identical despite different names*

### Comparing `bdq-0.0.4/bdq/dataframe.py` & `bdq-0.0.5/bdq/dataframe.py`

 * *Files identical despite different names*

### Comparing `bdq-0.0.4/bdq/functions.py` & `bdq-0.0.5/bdq/functions.py`

 * *Files identical despite different names*

### Comparing `bdq-0.0.4/bdq/schema.py` & `bdq-0.0.5/bdq/schema.py`

 * *Files identical despite different names*

### Comparing `bdq-0.0.4/bdq/spark_pipeline.py` & `bdq-0.0.5/bdq/spark_pipeline.py`

 * *Files identical despite different names*

### Comparing `bdq-0.0.4/bdq.egg-info/PKG-INFO` & `bdq-0.0.5/bdq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6264 710a  : 2.1.Name: bdq.
-00000020: 5665 7273 696f 6e3a 2030 2e30 2e34 0a53  Version: 0.0.4.S
+00000020: 5665 7273 696f 6e3a 2030 2e30 2e35 0a53  Version: 0.0.5.S
 00000030: 756d 6d61 7279 3a20 4269 6720 4461 7461  ummary: Big Data
 00000040: 2051 7561 6c69 7479 2c20 6120 7365 7420   Quality, a set 
 00000050: 6f66 2074 6f6f 6c73 2f66 756e 6374 696f  of tools/functio
 00000060: 6e20 7468 6174 2068 656c 7020 796f 7520  n that help you 
 00000070: 6576 6572 7920 6461 7920 6173 7365 7274  every day assert
 00000080: 2071 7561 6c69 7479 206f 6620 6461 7461   quality of data
 00000090: 7365 7473 2079 6f75 2068 6176 6520 7072  sets you have pr
@@ -1308,8 +1308,74 @@
 000051b0: 7263 6527 2077 696c 6c20 6265 2075 7064  rce' will be upd
 000051c0: 6174 6564 2077 6865 6e20 7468 6973 2066  ated when this f
 000051d0: 756e 6374 696f 6e20 6669 6e69 7368 6573  unction finishes
 000051e0: 2028 6173 2070 6572 2064 6566 696e 7469   (as per definti
 000051f0: 6f6e 2069 6e20 4070 706e 2e73 7465 7020  on in @ppn.step 
 00005200: 6162 6f76 6529 0a72 6177 5f64 6174 615f  above).raw_data_
 00005210: 7369 6e67 6c65 5f73 6f75 7263 6528 290a  single_source().
-00005220: 6060 600a                                ```.
+00005220: 6060 600a 0a23 2320 5370 6172 6b20 5549  ```..## Spark UI
+00005230: 2053 7461 6765 2064 6573 6372 6970 7469   Stage descripti
+00005240: 6f6e 730a 5768 656e 2072 756e 6e69 6e67  ons.When running
+00005250: 2063 6f64 6520 7573 696e 6720 7079 7370   code using pysp
+00005260: 6172 6b2c 2073 7061 726b 2075 6920 6765  ark, spark ui ge
+00005270: 7473 2076 6572 7920 6372 6f77 6465 642e  ts very crowded.
+00005280: 2060 5370 6172 6b55 494c 6f67 6765 7260   `SparkUILogger`
+00005290: 2063 6f6e 7465 7874 206d 616e 6167 6572   context manager
+000052a0: 2061 6e64 2064 6563 6f72 6174 6f72 2061   and decorator a
+000052b0: 7373 696e 6773 2068 756d 616e 2072 6561  ssings human rea
+000052c0: 6461 626c 6520 6e61 6d65 7320 746f 2073  dable names to s
+000052d0: 7061 726b 2073 7461 6765 732e 0a0a 6060  park stages...``
+000052e0: 6070 7974 686f 6e0a 6672 6f6d 2062 6471  `python.from bdq
+000052f0: 0a0a 2320 7573 6167 6520 6f66 2064 6563  ..# usage of dec
+00005300: 6f72 6174 6f72 730a 2320 7370 6172 6b20  orators.# spark 
+00005310: 7569 2073 7461 6765 7320 7769 6c6c 2068  ui stages will h
+00005320: 6176 6520 6465 7363 7269 7074 696f 6e20  ave description 
+00005330: 6f66 2027 7879 7a27 0a40 5370 6172 6b55  of 'xyz'.@SparkU
+00005340: 494c 6f67 6765 722e 7461 6728 6465 7363  ILogger.tag(desc
+00005350: 3d27 7879 7a27 290a 6465 6620 736f 6d65  ='xyz').def some
+00005360: 5f66 756e 6374 696f 6e32 286e 756d 6265  _function2(numbe
+00005370: 7229 3a0a 0a20 2072 6574 7572 6e20 7370  r):..  return sp
+00005380: 6172 6b2e 7261 6e67 6528 6e75 6d62 6572  ark.range(number
+00005390: 292e 636f 756e 7428 290a 0a23 2073 7061  ).count()..# spa
+000053a0: 726b 2075 6920 7374 6167 6573 2077 696c  rk ui stages wil
+000053b0: 6c20 6861 7665 2064 6573 6372 6970 7469  l have descripti
+000053c0: 6f6e 206f 6620 2761 6c70 6861 5f66 756e  on of 'alpha_fun
+000053d0: 6374 696f 6e32 2720 2861 7574 6f6d 6174  ction2' (automat
+000053e0: 6963 616c 6c79 2064 6572 6976 6564 2066  ically derived f
+000053f0: 726f 6d20 6675 6e63 7469 6f6e 206e 616d  rom function nam
+00005400: 6529 0a40 5370 6172 6b55 494c 6f67 6765  e).@SparkUILogge
+00005410: 722e 7461 670a 6465 6620 616c 7068 615f  r.tag.def alpha_
+00005420: 6675 6e63 7469 6f6e 3228 6e75 6d62 6572  function2(number
+00005430: 293a 0a20 2023 2031 7374 2061 6e64 2032  ):.  # 1st and 2
+00005440: 6e64 2073 6f6d 655f 6675 6e63 7469 6f6e  nd some_function
+00005450: 3228 2920 6361 6c6c 7320 7368 6f75 6c64  2() calls should
+00005460: 2062 6520 7669 7369 626c 6520 696e 2073   be visible in s
+00005470: 7061 726b 2075 6920 6173 2027 7879 7a27  park ui as 'xyz'
+00005480: 0a20 2023 2074 6865 2033 7264 2070 6172  .  # the 3rd par
+00005490: 7420 6f66 2072 6573 756c 7420 7368 6f75  t of result shou
+000054a0: 6c64 2062 6520 7669 7369 626c 6520 6173  ld be visible as
+000054b0: 2027 616c 7068 615f 6675 6e63 7469 6f6e   'alpha_function
+000054c0: 320a 2020 7265 7475 726e 2073 6f6d 655f  2.  return some_
+000054d0: 6675 6e63 7469 6f6e 3228 6e75 6d62 6572  function2(number
+000054e0: 2a32 2920 2b20 736f 6d65 5f66 756e 6374  *2) + some_funct
+000054f0: 696f 6e32 286e 756d 6265 722a 3329 202b  ion2(number*3) +
+00005500: 2073 7061 726b 2e72 616e 6765 286e 756d   spark.range(num
+00005510: 6265 722f 3130 292e 636f 756e 7428 290a  ber/10).count().
+00005520: 0a23 2075 7361 6765 206f 6620 636f 6e74  .# usage of cont
+00005530: 6578 7420 6d61 6e61 6765 7273 0a23 2077  ext managers.# w
+00005540: 696c 6c20 6265 2076 6973 6962 6c65 2069  ill be visible i
+00005550: 6e20 7370 6172 6b20 7569 2061 7320 2766  n spark ui as 'f
+00005560: 6972 7374 2d63 6f75 6e74 270a 7769 7468  irst-count'.with
+00005570: 2053 7061 726b 5549 4c6f 6767 6572 2827   SparkUILogger('
+00005580: 6669 7273 742d 636f 756e 7427 293a 0a20  first-count'):. 
+00005590: 2073 7061 726b 2e72 616e 6765 2831 3029   spark.range(10)
+000055a0: 2e63 6f75 6e74 2829 0a0a 2320 7769 6c6c  .count()..# will
+000055b0: 2062 6520 7669 7369 626c 6520 696e 2073   be visible in s
+000055c0: 7061 726b 2075 6920 6173 2027 326e 642d  park ui as '2nd-
+000055d0: 636f 756e 7427 0a77 6974 6820 5370 6172  count'.with Spar
+000055e0: 6b55 494c 6f67 6765 7228 2732 6e64 2d63  kUILogger('2nd-c
+000055f0: 6f75 6e74 2729 3a0a 2020 7370 6172 6b2e  ount'):.  spark.
+00005600: 7261 6e67 6528 3230 292e 636f 756e 7428  range(20).count(
+00005610: 290a 0a73 6f6d 655f 6675 6e63 7469 6f6e  )..some_function
+00005620: 3228 3130 3030 290a 616c 7068 615f 6675  2(1000).alpha_fu
+00005630: 6e63 7469 6f6e 3228 3230 3030 290a 6060  nction2(2000).``
+00005640: 600a                                     `.
```

### Comparing `bdq-0.0.4/pyproject.toml` & `bdq-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdq"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Grzegorz Rusin", email="grzegorz.rusin@databricks.com" },
 ]
 description = "Big Data Quality, a set of tools/function that help you every day assert quality of datasets you have processed or ingested"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

