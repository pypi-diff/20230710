# Comparing `tmp/queueing_systems-0.1.0.tar.gz` & `tmp/queueing_systems-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queueing_systems-0.1.0.tar", last modified: Mon Jul 10 07:16:30 2023, max compression
+gzip compressed data, was "queueing_systems-0.1.1.tar", last modified: Mon Jul 10 19:26:37 2023, max compression
```

## Comparing `queueing_systems-0.1.0.tar` & `queueing_systems-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 paulius    (501) staff       (20)        0 2023-07-10 07:16:29.000000 queueing_systems-0.1.0/
--rw-r--r--   0 paulius    (501) staff       (20)     1067 2023-07-10 00:45:03.000000 queueing_systems-0.1.0/LICENSE
--rw-r--r--   0 paulius    (501) staff       (20)     1159 2023-07-10 07:16:30.000000 queueing_systems-0.1.0/PKG-INFO
--rw-r--r--   0 paulius    (501) staff       (20)      537 2023-07-10 01:30:32.000000 queueing_systems-0.1.0/README.md
-drwxr-xr-x   0 paulius    (501) staff       (20)        0 2023-07-10 07:16:29.000000 queueing_systems-0.1.0/queueing_systems/
--rw-r--r--   0 paulius    (501) staff       (20)        0 2023-07-10 00:34:09.000000 queueing_systems-0.1.0/queueing_systems/__init__.py
--rw-r--r--   0 paulius    (501) staff       (20)    11426 2023-07-10 07:15:54.000000 queueing_systems-0.1.0/queueing_systems/functions.py
-drwxr-xr-x   0 paulius    (501) staff       (20)        0 2023-07-10 07:16:29.000000 queueing_systems-0.1.0/queueing_systems.egg-info/
--rw-r--r--   0 paulius    (501) staff       (20)     1159 2023-07-10 07:16:30.000000 queueing_systems-0.1.0/queueing_systems.egg-info/PKG-INFO
--rw-r--r--   0 paulius    (501) staff       (20)      284 2023-07-10 07:16:30.000000 queueing_systems-0.1.0/queueing_systems.egg-info/SOURCES.txt
--rw-r--r--   0 paulius    (501) staff       (20)        1 2023-07-10 07:16:30.000000 queueing_systems-0.1.0/queueing_systems.egg-info/dependency_links.txt
--rw-r--r--   0 paulius    (501) staff       (20)       24 2023-07-10 07:16:30.000000 queueing_systems-0.1.0/queueing_systems.egg-info/requires.txt
--rw-r--r--   0 paulius    (501) staff       (20)       17 2023-07-10 07:16:30.000000 queueing_systems-0.1.0/queueing_systems.egg-info/top_level.txt
--rw-r--r--   0 paulius    (501) staff       (20)       38 2023-07-10 07:16:30.000000 queueing_systems-0.1.0/setup.cfg
--rw-r--r--   0 paulius    (501) staff       (20)      901 2023-07-10 06:56:25.000000 queueing_systems-0.1.0/setup.py
+drwxr-xr-x   0 paulius    (501) staff       (20)        0 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/
+-rw-r--r--   0 paulius    (501) staff       (20)     1067 2023-07-10 00:45:03.000000 queueing_systems-0.1.1/LICENSE
+-rw-r--r--   0 paulius    (501) staff       (20)     1159 2023-07-10 19:26:37.000000 queueing_systems-0.1.1/PKG-INFO
+-rw-r--r--   0 paulius    (501) staff       (20)      537 2023-07-10 01:30:32.000000 queueing_systems-0.1.1/README.md
+drwxr-xr-x   0 paulius    (501) staff       (20)        0 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/queueing_systems/
+-rw-r--r--   0 paulius    (501) staff       (20)        0 2023-07-10 00:34:09.000000 queueing_systems-0.1.1/queueing_systems/__init__.py
+-rw-r--r--   0 paulius    (501) staff       (20)    12465 2023-07-10 15:25:12.000000 queueing_systems-0.1.1/queueing_systems/functions.py
+drwxr-xr-x   0 paulius    (501) staff       (20)        0 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/queueing_systems.egg-info/
+-rw-r--r--   0 paulius    (501) staff       (20)     1159 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/queueing_systems.egg-info/PKG-INFO
+-rw-r--r--   0 paulius    (501) staff       (20)      284 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/queueing_systems.egg-info/SOURCES.txt
+-rw-r--r--   0 paulius    (501) staff       (20)        1 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/queueing_systems.egg-info/dependency_links.txt
+-rw-r--r--   0 paulius    (501) staff       (20)       24 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/queueing_systems.egg-info/requires.txt
+-rw-r--r--   0 paulius    (501) staff       (20)       17 2023-07-10 19:26:36.000000 queueing_systems-0.1.1/queueing_systems.egg-info/top_level.txt
+-rw-r--r--   0 paulius    (501) staff       (20)       38 2023-07-10 19:26:37.000000 queueing_systems-0.1.1/setup.cfg
+-rw-r--r--   0 paulius    (501) staff       (20)      902 2023-07-10 19:26:27.000000 queueing_systems-0.1.1/setup.py
```

### Comparing `queueing_systems-0.1.0/LICENSE` & `queueing_systems-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `queueing_systems-0.1.0/PKG-INFO` & `queueing_systems-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queueing_systems
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package for queueing system parameter estimation using queueing theory
 Home-page: https://github.com/pauterv/queueing_systems
 Author: Paulius Tervydis
 Author-email: Paulius.Tervydis@ktu.lt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `queueing_systems-0.1.0/README.md` & `queueing_systems-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `queueing_systems-0.1.0/queueing_systems/functions.py` & `queueing_systems-0.1.1/queueing_systems/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,24 @@
+#   Main functions of queueing_systems package
+#
+#   Author: Paulius Tervydis
+#   Date: 2023-07-09
+#
+# ==============================================================
+
+# ==============================================================
+# ssqs function 
+# ==============================================================
 def ssqs(**parameters):
     """This function calculates the parameters of various single-server queueing systems.
 
     A queueing system is considered stable when the arrival rate is lower than the service rate. 
     If the parameters are incorrect or missing, exceptions will be raised to alert the user. 
     Additionally, certain input parameters are optional and can be automatically calculated based on the selected system type.
-
+   
     Parameters
     ----------
     **parameters : (keyword arguments)
     qs : str
         Type of queueing system according Kendall's notations:
         "MM1", "MD1", "MG1", "DM1","DG1","DD1","GM1","GD1". Defaults "MM1".
         Examples of accepted formats: "mm1", "MM1", "m/m/1", "M/M/1" 
@@ -25,32 +35,32 @@
     vs : float
         Variance of service time. Must be provided only for "MG1","DG1","GG1" type systems.
 
     Returns
     -------
     result : dictionary with such keys
     'qs' - queueing system notation
-    'w' - the mean total time in system
-    'wq' - the mean waiting time in queue
-    'u' - the utilization of the system
     'ar' - arrival rate
     'sr' - service rate
-    'l' - mean number of entities in the system
-    'lq' - mean number of entities in the queue
     'a' - mean inter-arrival time
-    's' - mean service time
-    'va' - variance of inter-arrival time
-    'vs' - variance of service time
+    'va' - variance of inter-arrival time 
+    's' - mean service time 
+    'vs' - variance of service time 
+    'u' - the utilization of the system 
+    'l' - mean number of entities in the system
+    'lq' - mean number of entities in the queue    
+    'w' - the mean waiting (total time) in system
+    'wq' - the mean waiting time in queue
 
     Example
     -------
-    >>> result = ssqs(qs='gg1',ar=10,va=0,s=0.01,vs=0.04)
+    >>> result = ssqs(qs='md1',ar=10,s=0.05)
     >>> print(result)
-    >>> {'qs': 'gg1', 'w': 0.18822222222222224, 'wq': 0.17822222222222223, 'u': 0.1, 'ar': 10.0, 'sr': 100.0, 
-    'l': 1.8822222222222225, 'lq': 1.7822222222222224, 'a': 0.1, 's': 0.01, 'va': 0, 'vs': 0.04} 
+    >>> {'qs': 'md1', 'ar': 10.0, 'sr': 20.0, 'a': 0.1, 'va': 0.01, 
+        's': 0.05, 'vs': 0, 'u': 0.5, 'l': 0.75, 'lq': 0.25, 'wq': 0.025, 'w': 0.075} 
     """
 
     # -------------------------------------------------------------------
     qs = None
     a = None
     s = None
     va = None
@@ -108,15 +118,15 @@
     if qs_f[1] == "M":
         vs = s ** 2
     if qs_f[0] == "D":
         va = 0
     if qs_f[1] == "D":
         vs = 0
     if qs_f[2] != "1":
-        raise Exception("Uncompatble system notation")    
+        raise Exception("Incompatible system notation")    
     if a is None and ar is not None:
         a = 1 / ar
     if a is None and ar is None:
         raise Exception("Missing parameters. 'ar' or 'a' values are not provided")
     if s is None and sr is not None:
         s = 1 / sr
     if s is None and sr is None:
@@ -139,27 +149,42 @@
     u = ar / sr
     # The mean waiting time in queue:
     if qs_f == "MM1":
         wq = (u * s)/(1 - u)
     elif qs_f == "MD1":
         wq = (u * s)/(2*(1 - u))
     else:
-        # The actual mean waiting time in queue is obtained by Marchal’s approximation
+        # The actual mean waiting time in queue is obtained by Marchall’s approximation
         wq = (u * s) / (2 * (1 - u)) * ((va + vs) /
                                         (s ** 2)) * ((s ** 2 + vs) / (a ** 2 + vs))
     # The mean total time in system
     w = wq + s
     # The mean number of entities in the system
     l = ar * w
     # The mean number of entities in the queue
     lq = ar * wq
-    result = {"qs": qs, "w": w, "wq": wq, "u": u, "ar": ar,
-              "sr": sr, "l": l, "lq": lq, "a": a, "s": s, "va": va, "vs": vs}
+    result = {"qs": qs, 
+              "ar": round(ar,15), 
+              "sr": round(sr,15),
+              "a": round(a,15), 
+              "va": round(va,15), 
+              "s": round(s,15), 
+              "vs": round(vs,15),
+              "u": round(u,15),
+              "l": round(l,15),
+              "lq": round(lq,15),
+              "wq": round(wq,15),
+              "w": round(w,15)}
     return result
+# ==============================================================
+
 
+# ==============================================================
+# msqs function 
+# ==============================================================
 def msqs(ar, sn, qs=None, sr1=None, s1=None, vs=None):
     """This function calculates parameters of multi-server queueing systems. 
 
     A multi-server queueing system is considered, where the arrival rate is evenly 
     distributed among the servers upon arrival to the system. The function returns 
     the parameters specific to a single server within the multi-server system. 
     It assumes that all servers in the system are identical.
@@ -170,37 +195,37 @@
         Arrival rate.
     sn : int
         Number of servers
     sr1 : float, optional
         Single server service rate. Optional if s1 is given.
     qs : str, optional
         Type of queueing system according Kendall's notations. By default "MM1" or None
-        With this function only such systems can be analysed: "MM1", "MD1", "MG1","DM1","DD1","DG1". Defaults "MM1".
+        With this function only such systems can be analyzed: "MM1", "MD1", "MG1","DM1","DD1","DG1". Defaults "MM1".
         Examples of accepted formats: "mm1", "MM1", "m/m/1", "M/M/1" 
     s1 : float, optional    
         Mean service time in single server. Optional if sr1 is given.
     vs : float, optional
         Variance of service time. Must be provided only for "MG1" type system.    
 
     Returns
     -------
     result : list of dictionaries for each server with such keys:
     'qs' - queueing system notation
-    'w' - the mean total time in system
-    'wq' - the mean waiting time in queue
-    'u' - the utilization of the system
     'ar' - arrival rate
     'sr' - service rate
-    'l' - mean number of entities in the system
-    'lq' - mean number of entities in the queue
     'a' - mean inter-arrival time
-    's' - mean service time
-    'va' - variance of inter-arrival time
-    'vs' - variance of service time
-
+    'va' - variance of inter-arrival time 
+    's' - mean service time 
+    'vs' - variance of service time 
+    'u' - the utilization of the system 
+    'l' - mean number of entities in the system
+    'lq' - mean number of entities in the queue    
+    'w' - the mean waiting (total time) in system
+    'wq' - the mean waiting time in queue
+    
     Example
     -------
     >>> result = msqs(ar=10, sn=5, sr1=4)
     >>> print(result)
     >>> {'qs': 'mm1', 'w': 0.5, 'wq': 0.25, 'u': 0.5, 'ar': 2.0, 'sr': 4.0, 'l': 1.0, 'lq': 0.5, 'a': 0.5, 's': 0.25, 'va': 0.25, 'vs': 0.0625}
     """
 
@@ -222,15 +247,20 @@
         raise Exception("Unstable system: ar must be < sn*sr1")
     
     if qs[0] == "G" or qs[2]!="1":
         raise Exception('Wrong system type: only "MM1", "MD1", "MG1","DM1","DD1","DG1" are valid')
 
     result = ssqs(qs=qs, ar=ar/sn, sr=sr1, s=s1, vs=vs)
     return result
+# ==============================================================
+
 
+# ==============================================================
+# mssqsa function 
+# ==============================================================
 def msqsa(ar, pl, sl):
     """This function provides advanced estimation for parameters of multi-server queueing systems. 
     
     The arrival rate is distributed based on a provided list of probabilities. 
     Each server in the system can have distinct characteristics.
     
     Parameters
@@ -267,23 +297,23 @@
     'a' - mean inter-arrival time
     's' - mean service time
     'va' - variance of inter-arrival time
     'vs' - variance of service time
     'p' - probability of arrival rate distribution to the server
     'c' - cost (if provided in 'sl')
     'cu' - cost if it depends on utilization (if 'c' provided in 'sl')
-    'r' - ammount of expendable resources of the server ('if 'r' provided in 'sl')
+    'r' - amount of expendable resources of the server ('if 'r' provided in 'sl')
     'rt' - time interval between refills of expendable resources ('if 'r' provided in 'sl')
     'i' - info (if provided in 'sl')
 
     Example
     -------
     >>> pl = [0.4,0.6]
     >>> sl = [{'qs':'md1','sr':1},{'qs':'mg1','sr':1,'vs':0.1}]
-    >>> result = msqs2(ar=1,pl=pl,sl=sl)
+    >>> result = msqsa(ar=1,pl=pl,sl=sl)
     >>> print(result) 
     >>> [{'qs': 'md1', 'w': 1.5, 'wq': 0.5, 'u': 0.5, 'ar': 0.5, 'sr': 1.0, 'l': 0.75, 
         'lq': 0.25, 'a': 2.0, 's': 1.0, 'va': 4.0, 'vs': 0, 'p': 0.5}, 
         {'qs': 'mg1', 'w': 1.5615, 'wq': 0.5615, 'u': 0.5, 'ar': 0.5, 'sr': 1.0, 
         'l': 0.78075, 'lq': 0.28075, 'a': 2.0, 's': 1.0, 'va': 4.0, 'vs': 0.123, 'p': 0.5}]  
     """
     if len(pl) != len(sl):
@@ -305,7 +335,8 @@
                 res["rt"] = sl[i]["r"]*res["s"]/res["u"]
             if sl[i].get("i") is not None:
                 res["i"] = sl[i]["i"]
             result.append(res)
         else:
             print("System unstable: arrival rate > service rate")
     return result
+# ==============================================================
```

### Comparing `queueing_systems-0.1.0/queueing_systems.egg-info/PKG-INFO` & `queueing_systems-0.1.1/queueing_systems.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queueing-systems
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package for queueing system parameter estimation using queueing theory
 Home-page: https://github.com/pauterv/queueing_systems
 Author: Paulius Tervydis
 Author-email: Paulius.Tervydis@ktu.lt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `queueing_systems-0.1.0/setup.py` & `queueing_systems-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup
 
 setup(
     name='queueing_systems',
-    version='0.1.0',
+    version='0.1.1',
     author='Paulius Tervydis',
     author_email='Paulius.Tervydis@ktu.lt',
     description='Python package for queueing system parameter estimation using queueing theory',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/pauterv/queueing_systems',
     packages=['queueing_systems'],
     install_requires=[
         # List any dependencies your package requires
         'numpy',
         'pandas',
-        'matploblib'
+        'matplotlib',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

