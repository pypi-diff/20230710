# Comparing `tmp/cioseq-0.2.2-py2.py3-none-any.whl.zip` & `tmp/cioseq-0.3.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17266 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1079 b- defN 23-May-25 16:08 cioseq/LICENSE
--rw-r--r--  2.0 unx     4287 b- defN 23-May-25 16:08 cioseq/README.md
--rw-r--r--  2.0 unx        5 b- defN 23-May-25 16:08 cioseq/VERSION
--rw-r--r--  2.0 unx        0 b- defN 23-May-25 16:08 cioseq/__init__.py
--rw-r--r--  2.0 unx    20572 b- defN 23-May-25 16:08 cioseq/sequence.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-25 16:08 tests/__init__.py
--rw-r--r--  2.0 unx    26757 b- defN 23-May-25 16:08 tests/test_sequence.py
--rw-r--r--  2.0 unx     1079 b- defN 23-May-25 16:08 cioseq-0.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     6462 b- defN 23-May-25 16:08 cioseq-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-25 16:08 cioseq-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-May-25 16:08 cioseq-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      893 b- defN 23-May-25 16:08 cioseq-0.2.2.dist-info/RECORD
-12 files, 61257 bytes uncompressed, 15786 bytes compressed:  74.2%
+Zip file size: 17631 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1079 b- defN 23-Jul-10 06:48 cioseq/LICENSE
+-rw-r--r--  2.0 unx     4388 b- defN 23-Jul-10 06:48 cioseq/README.md
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-10 06:48 cioseq/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 06:48 cioseq/__init__.py
+-rw-r--r--  2.0 unx    21251 b- defN 23-Jul-10 06:48 cioseq/sequence.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 06:48 tests/__init__.py
+-rw-r--r--  2.0 unx    26907 b- defN 23-Jul-10 06:48 tests/test_sequence.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-Jul-10 06:48 cioseq-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6726 b- defN 23-Jul-10 06:48 cioseq-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-10 06:48 cioseq-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Jul-10 06:48 cioseq-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      893 b- defN 23-Jul-10 06:48 cioseq-0.3.0.dist-info/RECORD
+12 files, 62451 bytes uncompressed, 16151 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_sequence.py
 Comment: 
 
-Filename: cioseq-0.2.2.dist-info/LICENSE
+Filename: cioseq-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: cioseq-0.2.2.dist-info/METADATA
+Filename: cioseq-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: cioseq-0.2.2.dist-info/WHEEL
+Filename: cioseq-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: cioseq-0.2.2.dist-info/top_level.txt
+Filename: cioseq-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cioseq-0.2.2.dist-info/RECORD
+Filename: cioseq-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cioseq/README.md

```diff
@@ -187,14 +187,22 @@
 1:10;14;20:48%4
 
 >>> print(s.to("to", "by", " "))
 1to10 14 20to48by4
 
 ```
 
+Reformat with no step separator
+```
+>>> s = Sequence.create("1-10x2,22-25")
+>>> print(s.to("-", "", ","))
+1,3,5,7,9,22-25
+```
+
+
 Take a subsample of frames
 ```
 s = Sequence.create("1-10")
 >>> print(s.subsample(1))
 6
 
 >>> print(s.subsample(2))
@@ -238,10 +246,7 @@
 ```
 pip install -r requirements_dev.txt
 ```
 
 pip install --upgrade . 
 
 ```
-
-## License
-[MIT](LICENSE)
```

## cioseq/VERSION

```diff
@@ -1 +1 @@
-0.2.2
+0.3.0
```

## cioseq/sequence.py

```diff
@@ -424,16 +424,35 @@
         return int(math.ceil(len(self._iterable) / float(count)))
 
     def is_progression(self):
         """Is this sequence a progression."""
         return isinstance(self, Progression)
 
     def to(self, range_sep, step_sep, block_sep):
+        """
+        Use different symbols to represent a spec.
+        
+        If the step separator is None, then we break the stepped parts of the
+        sequence, if any, into comma delimited frame numbers.
+        
+        Katana requires this format for stepped sequences.
+        """
+        
+        spec = str(self)
+        if step_sep == "":
+            new_parts = []
+            parts=str(self).split(",")
+            for part in parts:
+                if "x" in part:
+                    part = ",".join([str(int(x)) for x in Sequence.create(part)])
+                new_parts.append(part)
+            spec = ",".join(new_parts)
+                
         return (
-            str(self)
+            spec
             .replace("-", range_sep)
             .replace("x", step_sep)
             .replace(",", block_sep)
         )
 
     @property
     def chunk_size(self):
@@ -444,14 +463,15 @@
     def chunk_size(self, value):
         """Set chunk_size.
 
         Max is the length of frames and min is 1. If a value less than 1
         is given, set it to max, which means the default is to output 1
         chunk.
         """
+        value=int(value)
         num = len(self._iterable)
         self._chunk_size = num if value < 1 else sorted([num, value])[0]
 
     @property
     def chunk_strategy(self):
         """Return the current strategy for emitting chunks."""
         return self._chunk_strategy
```

## tests/test_sequence.py

```diff
@@ -648,14 +648,19 @@
         s = Sequence.create("1-10, 14, 20-48x4")
         self.assertEqual(s.to(":", "%", ";"), "1:10;14;20:48%4")
 
     def test_complex_add_spaces(self):
         s = Sequence.create("1-10, 14, 20-48x4")
         self.assertEqual(s.to(":", "%", "; "), "1:10; 14; 20:48%4")
 
+    def test_no_step(self):
+        s = Sequence.create("1-4, 6-10x2, 20-28x4")
+        self.assertEqual(s.to("-", "", ","), "1-4,6,8,10,20,24,28")
+
+
 
 class SubsampleTest(unittest.TestCase):
     def test_counts_from_1_to_10(self):
         s = Sequence.create("1-10")
         ss = s.subsample(1)
         self.assertEqual(len(ss), 1)
         self.assertEqual(list(ss), [6])
```

## Comparing `cioseq-0.2.2.dist-info/LICENSE` & `cioseq-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cioseq-0.2.2.dist-info/METADATA` & `cioseq-0.3.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: cioseq
-Version: 0.2.2
+Version: 0.3.0
 Summary: Manage sequences of frame numbers.
 Home-page: https://github.com/ConductorTechnologies/cioseq
 Author: conductor
 Author-email: info@conductortech.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Multimedia :: Graphics :: 3D Rendering
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: future (>=0.18.2)
 
 # sequence
 Manage sequences of frame numbers
 
 ## Install
 
@@ -202,14 +201,22 @@
 1:10;14;20:48%4
 
 >>> print(s.to("to", "by", " "))
 1to10 14 20to48by4
 
 ```
 
+Reformat with no step separator
+```
+>>> s = Sequence.create("1-10x2,22-25")
+>>> print(s.to("-", "", ","))
+1,3,5,7,9,22-25
+```
+
+
 Take a subsample of frames
 ```
 s = Sequence.create("1-10")
 >>> print(s.subsample(1))
 6
 
 >>> print(s.subsample(2))
@@ -254,19 +261,20 @@
 pip install -r requirements_dev.txt
 ```
 
 pip install --upgrade . 
 
 ```
 
-## License
-[MIT](LICENSE)
-
 ## Changelog
 
+## Version:0.3.0 -- 10 Jul 2023
+
+* the `to()` function now handles an empty string for step separator, which enables frame spec strings compatible with Katana's command-line.
+
 ### Version:0.2.2 -- 25 May 2023
 
 * Simple edit to remove circle test release. [b92a2c9]
 
 
 ### Version:0.2.0 -- 25 May 2023
 
@@ -311,15 +319,15 @@
 ### Version:0.1.5 -- 21 Sep 2020
 
 * Bad test name and $f4 token support. [f3c1923]
 
 ### Version:0.1.3 -- 20 Sep 2020
 
 * Added several examples to the README and implemented and indexing. [fdec3b4]
-
+ 
 ### Version:0.1.2 -- 19 Sep 2020
 
 * Python 2 and 3 compatibility. [4aba985]
 
 ### Version:0.1.1 -- 19 Sep 2020
 
 * Transfer from core. As such, this is the first changelog entry. [54f9132]
@@ -329,8 +337,7 @@
 * Lib enhancements (#4)
 * adds sequence intersection check
 * allows uppercase characters in angle-bracket template.. [255f61f]
 * Initial commit. [7cf8fd3]
 
 
 --
-
```

## Comparing `cioseq-0.2.2.dist-info/RECORD` & `cioseq-0.3.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cioseq/LICENSE,sha256=eSiIxE5S7RlI78VJUCpgrHNe5ZkosDjX4mPy6IDuo1c,1079
-cioseq/README.md,sha256=TE-mpF-xmkQyQKYLG2Wls34u5mgqKfu7Yn2BW6Xnofc,4287
-cioseq/VERSION,sha256=yQ34TPijI3G2D_9VaJi-yv9jQDbp5YZSBMGHlXhDWEc,5
+cioseq/README.md,sha256=Cewg5w68Cqwc4xx4wFNSWXJQpUp32yZwdh5B42Zk0gU,4388
+cioseq/VERSION,sha256=VQYTU3_EiPOzcq90pAAYefASyEZbgW8bhcbTRGss-0k,5
 cioseq/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cioseq/sequence.py,sha256=7Y0URfOvcTebM38ReBCUeoHSOZPQuMNRmmYXB25Pulc,20572
+cioseq/sequence.py,sha256=aboJo4cjggDSRTWYEQGo7LmjXTTlgV_IpxRnvqh0SRM,21251
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/test_sequence.py,sha256=rIcoVqYO2Yuep8Ythqzf3WBQTGpXDYGCfpMDoSuBkHo,26757
-cioseq-0.2.2.dist-info/LICENSE,sha256=eSiIxE5S7RlI78VJUCpgrHNe5ZkosDjX4mPy6IDuo1c,1079
-cioseq-0.2.2.dist-info/METADATA,sha256=PuZalsOr9ni8Ytwj-5p099-J--3X7H9oVPJeVRQUQpI,6462
-cioseq-0.2.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-cioseq-0.2.2.dist-info/top_level.txt,sha256=oGyuKelxko4m3F-O4HRyV2wKuX2uomz71qKmgKgjCy8,13
-cioseq-0.2.2.dist-info/RECORD,,
+tests/test_sequence.py,sha256=9hKZUzRlYa4FX9HLB0CpMgYNLBfJwxYNWT0yx897of0,26907
+cioseq-0.3.0.dist-info/LICENSE,sha256=eSiIxE5S7RlI78VJUCpgrHNe5ZkosDjX4mPy6IDuo1c,1079
+cioseq-0.3.0.dist-info/METADATA,sha256=2A_eqNpMc-ly2lLLXTPAhkl6iFmsiOzA8-DWQl0aAOE,6726
+cioseq-0.3.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+cioseq-0.3.0.dist-info/top_level.txt,sha256=oGyuKelxko4m3F-O4HRyV2wKuX2uomz71qKmgKgjCy8,13
+cioseq-0.3.0.dist-info/RECORD,,
```

