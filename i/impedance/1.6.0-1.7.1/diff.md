# Comparing `tmp/impedance-1.6.0.tar.gz` & `tmp/impedance-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impedance-1.6.0.tar", last modified: Sat Jun 24 04:43:45 2023, max compression
+gzip compressed data, was "impedance-1.7.1.tar", last modified: Mon Jul 10 02:24:43 2023, max compression
```

## Comparing `impedance-1.6.0.tar` & `impedance-1.7.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:43:45.707716 impedance-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-24 04:43:42.000000 impedance-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14222 2023-06-24 04:43:45.707716 impedance-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-06-24 04:43:42.000000 impedance-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:43:45.707716 impedance-1.6.0/impedance/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:43:45.707716 impedance-1.6.0/impedance/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:43:45.707716 impedance-1.6.0/impedance/models/circuits/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/models/circuits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15946 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/models/circuits/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/models/circuits/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/models/circuits/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:43:45.707716 impedance-1.6.0/impedance/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/tests/test_circuit_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/tests/test_circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/tests/test_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/tests/test_model_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    29741 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/tests/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-06-24 04:43:42.000000 impedance-1.6.0/impedance/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:43:45.707716 impedance-1.6.0/impedance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14222 2023-06-24 04:43:45.000000 impedance-1.6.0/impedance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-24 04:43:45.000000 impedance-1.6.0/impedance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 04:43:45.000000 impedance-1.6.0/impedance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 04:43:45.000000 impedance-1.6.0/impedance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-24 04:43:45.000000 impedance-1.6.0/impedance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 04:43:45.707716 impedance-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-24 04:43:42.000000 impedance-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:24:43.300726 impedance-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-10 02:24:40.000000 impedance-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-07-10 02:24:43.300726 impedance-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-10 02:24:40.000000 impedance-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:24:43.296726 impedance-1.7.1/impedance/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:24:43.296726 impedance-1.7.1/impedance/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:24:43.296726 impedance-1.7.1/impedance/models/circuits/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/models/circuits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15946 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/models/circuits/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/models/circuits/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/models/circuits/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:24:43.300726 impedance-1.7.1/impedance/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/tests/test_circuit_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/tests/test_circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/tests/test_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/tests/test_model_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29741 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-07-10 02:24:40.000000 impedance-1.7.1/impedance/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:24:43.296726 impedance-1.7.1/impedance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-07-10 02:24:43.000000 impedance-1.7.1/impedance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-10 02:24:43.000000 impedance-1.7.1/impedance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 02:24:43.000000 impedance-1.7.1/impedance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 02:24:43.000000 impedance-1.7.1/impedance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 02:24:43.000000 impedance-1.7.1/impedance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 02:24:43.300726 impedance-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-10 02:24:40.000000 impedance-1.7.1/setup.py
```

### Comparing `impedance-1.6.0/LICENSE` & `impedance-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `impedance-1.6.0/PKG-INFO` & `impedance-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impedance
-Version: 1.6.0
+Version: 1.7.1
 Summary: A package for analyzing electrochemical impedance data
 Home-page: https://impedancepy.readthedocs.io/en/latest/
 Author: impedance.py developers
 Author-email: matt.murbach@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -109,15 +109,16 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/lucasfdvx"><img src="https://avatars.githubusercontent.com/u/85888904?v=4?s=100" width="100px;" alt="lucasfdvx"/><br /><sub><b>lucasfdvx</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/issues?q=author%3Alucasfdvx" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/SaftMacki"><img src="https://avatars.githubusercontent.com/u/90030271?v=4?s=100" width="100px;" alt="Marcus Karlstad"/><br /><sub><b>Marcus Karlstad</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/issues?q=author%3ASaftMacki" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/markbouman"><img src="https://avatars.githubusercontent.com/u/103944120?v=4?s=100" width="100px;" alt="Mark Bouman"/><br /><sub><b>Mark Bouman</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/issues?q=author%3Amarkbouman" title="Bug reports">🐛</a> <a href="https://github.com/ECSHackWeek/impedance.py/commits?author=markbouman" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/oslopanda"><img src="https://avatars.githubusercontent.com/u/33810430?v=4?s=100" width="100px;" alt="oslopanda"/><br /><sub><b>oslopanda</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/issues?q=author%3Aoslopanda" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/pililac"><img src="https://avatars.githubusercontent.com/u/60116646?v=4?s=100" width="100px;" alt="pililac"/><br /><sub><b>pililac</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/issues?q=author%3Apililac" title="Bug reports">🐛</a></td>
     </tr>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kevinsmia1939"><img src="https://avatars.githubusercontent.com/u/11407922?v=4?s=100" width="100px;" alt="Kavin Teenakul"/><br /><sub><b>Kavin Teenakul</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/commits?author=kevinsmia1939" title="Code">💻</a> <a href="https://github.com/ECSHackWeek/impedance.py/commits?author=kevinsmia1939" title="Documentation">📖</a>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kevinsmia1939"><img src="https://avatars.githubusercontent.com/u/11407922?v=4?s=100" width="100px;" alt="Kavin Teenakul"/><br /><sub><b>Kavin Teenakul</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/commits?author=kevinsmia1939" title="Code">💻</a> <a href="https://github.com/ECSHackWeek/impedance.py/commits?author=kevinsmia1939" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/etrevis"><img src="https://avatars.githubusercontent.com/u/16451399?v=4?s=100" width="100px;" alt="Enrico"/><br /><sub><b>Enrico</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/commits?author=etrevis" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `impedance-1.6.0/README.md` & `impedance-1.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,16 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/lucasfdvx"><img src="https://avatars.githubusercontent.com/u/85888904?v=4?s=100" width="100px;" alt="lucasfdvx"/><br /><sub><b>lucasfdvx</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/issues?q=author%3Alucasfdvx" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/SaftMacki"><img src="https://avatars.githubusercontent.com/u/90030271?v=4?s=100" width="100px;" alt="Marcus Karlstad"/><br /><sub><b>Marcus Karlstad</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/issues?q=author%3ASaftMacki" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/markbouman"><img src="https://avatars.githubusercontent.com/u/103944120?v=4?s=100" width="100px;" alt="Mark Bouman"/><br /><sub><b>Mark Bouman</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/issues?q=author%3Amarkbouman" title="Bug reports">🐛</a> <a href="https://github.com/ECSHackWeek/impedance.py/commits?author=markbouman" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/oslopanda"><img src="https://avatars.githubusercontent.com/u/33810430?v=4?s=100" width="100px;" alt="oslopanda"/><br /><sub><b>oslopanda</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/issues?q=author%3Aoslopanda" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/pililac"><img src="https://avatars.githubusercontent.com/u/60116646?v=4?s=100" width="100px;" alt="pililac"/><br /><sub><b>pililac</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/issues?q=author%3Apililac" title="Bug reports">🐛</a></td>
     </tr>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kevinsmia1939"><img src="https://avatars.githubusercontent.com/u/11407922?v=4?s=100" width="100px;" alt="Kavin Teenakul"/><br /><sub><b>Kavin Teenakul</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/commits?author=kevinsmia1939" title="Code">💻</a> <a href="https://github.com/ECSHackWeek/impedance.py/commits?author=kevinsmia1939" title="Documentation">📖</a>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kevinsmia1939"><img src="https://avatars.githubusercontent.com/u/11407922?v=4?s=100" width="100px;" alt="Kavin Teenakul"/><br /><sub><b>Kavin Teenakul</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/commits?author=kevinsmia1939" title="Code">💻</a> <a href="https://github.com/ECSHackWeek/impedance.py/commits?author=kevinsmia1939" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/etrevis"><img src="https://avatars.githubusercontent.com/u/16451399?v=4?s=100" width="100px;" alt="Enrico"/><br /><sub><b>Enrico</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/commits?author=etrevis" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -53,13 +53,13 @@
        ð» â ï¸ ð         ð» â ï¸ ð     ð ð�         ð ð â ï¸     ð ð�      ð¤        ð ð»
            [Michael_Plews]                          [Chebuskin]           [environmat]                   [Abdullah_Sumbal]            [nobkat]          [Nick]         [aokomorowski]
             Michael_Plews                            Chebuskin             environmat                     Abdullah_Sumbal              nobkat            Nick           aokomorowski
                  ð¤                              ð               ð                         ð                 ð»       ð ð      ð»
         [Peter_Attia]                           [sdkang]                   [lucasfdvx]                   [Marcus_Karlstad]         [Mark_Bouman]       [oslopanda]        [pililac]
          Peter_Attia                             sdkang                     lucasfdvx                     Marcus_Karlstad           Mark_Bouman         oslopanda          pililac
        ð» â ï¸ ð              â ï¸ ð»          ð                         ð              ð ð      ð          ð
-        [Kavin_Teenakul]
-         Kavin_Teenakul
-           ð» ð
+        [Kavin_Teenakul]                             [Enrico]
+         Kavin_Teenakul                               Enrico
+           ð» ð                           ð»
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `impedance-1.6.0/impedance/models/circuits/circuits.py` & `impedance-1.7.1/impedance/models/circuits/circuits.py`

 * *Files identical despite different names*

### Comparing `impedance-1.6.0/impedance/models/circuits/elements.py` & `impedance-1.7.1/impedance/models/circuits/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,14 +309,33 @@
     """
     omega = 2 * np.pi * np.array(f)
     R, tau_k = p[0], p[1]
     Z = R / (1 + 1j * omega * tau_k)
     return Z
 
 
+@element(num_params=3, units=['Ohm', 'sec', ''])
+def Zarc(p, f):
+    """ An RQ element rewritten with resistance and
+    and time constant as paramenters. Equivalent to a
+    Cole-Cole relaxation in dielectrics.
+
+    Notes
+    -----
+    .. math::
+
+        Z = \\frac{R}{1 + (j \\omega \\tau_k)^\\gamma }
+
+    """
+    omega = 2*np.pi*np.array(f)
+    R, tau_k, gamma = p[0], p[1], p[2]
+    Z = R/(1 + ((1j*omega*tau_k)**gamma))
+    return Z
+
+
 @element(num_params=3, units=["Ohm", "F sec^(gamma - 1)", ""])
 def TLMQ(p, f):
     """Simplified transmission-line model as defined in Eq. 11 of [1]
 
     Notes
     -----
     .. math::
```

### Comparing `impedance-1.6.0/impedance/models/circuits/fitting.py` & `impedance-1.7.1/impedance/models/circuits/fitting.py`

 * *Files identical despite different names*

### Comparing `impedance-1.6.0/impedance/preprocessing.py` & `impedance-1.7.1/impedance/preprocessing.py`

 * *Files identical despite different names*

### Comparing `impedance-1.6.0/impedance/tests/test_circuit_elements.py` & `impedance-1.7.1/impedance/tests/test_circuit_elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,19 @@
             (0.00141056 - 0.00141039j),
         ],
         "K": [
             (0.099999842086579 - 0.000125663507704j),
             (0.038772663673915 - 0.048723166143232j),
             (6.332569967499333e-08 - 7.957742115295703e-05j),
         ],
+        "Zarc": [
+            (0.08900974-0.00486384j),
+            (0.04818879-0.01198904j),
+            (0.00969182-0.00436265j),
+        ],
     }
     input_vals = [0.1, 0.2, 0.3, 0.4]
     for key, f in circuit_elements.items():
         # don't test the outputs of series and parallel functions
         if key not in ["s", "p"]:
             num_inputs = f.num_params
             val = f(input_vals[:num_inputs], freqs)
```

### Comparing `impedance-1.6.0/impedance/tests/test_circuits.py` & `impedance-1.7.1/impedance/tests/test_circuits.py`

 * *Files identical despite different names*

### Comparing `impedance-1.6.0/impedance/tests/test_fitting.py` & `impedance-1.7.1/impedance/tests/test_fitting.py`

 * *Files identical despite different names*

### Comparing `impedance-1.6.0/impedance/tests/test_model_io.py` & `impedance-1.7.1/impedance/tests/test_model_io.py`

 * *Files identical despite different names*

### Comparing `impedance-1.6.0/impedance/tests/test_preprocessing.py` & `impedance-1.7.1/impedance/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `impedance-1.6.0/impedance/tests/test_validation.py` & `impedance-1.7.1/impedance/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `impedance-1.6.0/impedance/tests/test_visualization.py` & `impedance-1.7.1/impedance/tests/test_visualization.py`

 * *Files identical despite different names*

### Comparing `impedance-1.6.0/impedance/validation.py` & `impedance-1.7.1/impedance/validation.py`

 * *Files identical despite different names*

### Comparing `impedance-1.6.0/impedance/visualization.py` & `impedance-1.7.1/impedance/visualization.py`

 * *Files identical despite different names*

### Comparing `impedance-1.6.0/impedance.egg-info/PKG-INFO` & `impedance-1.7.1/impedance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impedance
-Version: 1.6.0
+Version: 1.7.1
 Summary: A package for analyzing electrochemical impedance data
 Home-page: https://impedancepy.readthedocs.io/en/latest/
 Author: impedance.py developers
 Author-email: matt.murbach@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -109,15 +109,16 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/lucasfdvx"><img src="https://avatars.githubusercontent.com/u/85888904?v=4?s=100" width="100px;" alt="lucasfdvx"/><br /><sub><b>lucasfdvx</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/issues?q=author%3Alucasfdvx" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/SaftMacki"><img src="https://avatars.githubusercontent.com/u/90030271?v=4?s=100" width="100px;" alt="Marcus Karlstad"/><br /><sub><b>Marcus Karlstad</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/issues?q=author%3ASaftMacki" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/markbouman"><img src="https://avatars.githubusercontent.com/u/103944120?v=4?s=100" width="100px;" alt="Mark Bouman"/><br /><sub><b>Mark Bouman</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/issues?q=author%3Amarkbouman" title="Bug reports">🐛</a> <a href="https://github.com/ECSHackWeek/impedance.py/commits?author=markbouman" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/oslopanda"><img src="https://avatars.githubusercontent.com/u/33810430?v=4?s=100" width="100px;" alt="oslopanda"/><br /><sub><b>oslopanda</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/issues?q=author%3Aoslopanda" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/pililac"><img src="https://avatars.githubusercontent.com/u/60116646?v=4?s=100" width="100px;" alt="pililac"/><br /><sub><b>pililac</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/issues?q=author%3Apililac" title="Bug reports">🐛</a></td>
     </tr>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kevinsmia1939"><img src="https://avatars.githubusercontent.com/u/11407922?v=4?s=100" width="100px;" alt="Kavin Teenakul"/><br /><sub><b>Kavin Teenakul</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/commits?author=kevinsmia1939" title="Code">💻</a> <a href="https://github.com/ECSHackWeek/impedance.py/commits?author=kevinsmia1939" title="Documentation">📖</a>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kevinsmia1939"><img src="https://avatars.githubusercontent.com/u/11407922?v=4?s=100" width="100px;" alt="Kavin Teenakul"/><br /><sub><b>Kavin Teenakul</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/commits?author=kevinsmia1939" title="Code">💻</a> <a href="https://github.com/ECSHackWeek/impedance.py/commits?author=kevinsmia1939" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/etrevis"><img src="https://avatars.githubusercontent.com/u/16451399?v=4?s=100" width="100px;" alt="Enrico"/><br /><sub><b>Enrico</b></sub></a><br /><a href="https://github.com/ECSHackWeek/impedance.py/commits?author=etrevis" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `impedance-1.6.0/impedance.egg-info/SOURCES.txt` & `impedance-1.7.1/impedance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `impedance-1.6.0/setup.py` & `impedance-1.7.1/setup.py`

 * *Files identical despite different names*

