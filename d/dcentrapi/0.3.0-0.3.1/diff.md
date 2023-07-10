# Comparing `tmp/dcentrapi-0.3.0.tar.gz` & `tmp/dcentrapi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.3.0.tar", last modified: Mon Jul  3 11:38:24 2023, max compression
+gzip compressed data, was "dcentrapi-0.3.1.tar", last modified: Mon Jul 10 11:45:11 2023, max compression
```

## Comparing `dcentrapi-0.3.0.tar` & `dcentrapi-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-07-03 11:38:24.548344 dcentrapi-0.3.0/
--rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.3.0/LICENSE.rst
--rw-r--r--   0 oded       (502) staff       (20)     6741 2023-07-03 11:38:24.548210 dcentrapi-0.3.0/PKG-INFO
--rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.3.0/README.md
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-07-03 11:38:24.547293 dcentrapi-0.3.0/dcentrapi/
--rw-r--r--   0 oded       (502) staff       (20)      903 2023-07-03 08:28:48.000000 dcentrapi-0.3.0/dcentrapi/Base.py
--rw-r--r--   0 oded       (502) staff       (20)      434 2023-07-03 08:17:20.000000 dcentrapi-0.3.0/dcentrapi/__init__.py
--rw-r--r--   0 oded       (502) staff       (20)     8761 2023-06-28 06:59:47.000000 dcentrapi-0.3.0/dcentrapi/eventPolling.py
--rw-r--r--   0 oded       (502) staff       (20)      673 2023-07-03 08:17:20.000000 dcentrapi-0.3.0/dcentrapi/gasMonitor.py
--rw-r--r--   0 oded       (502) staff       (20)      561 2023-07-03 08:19:01.000000 dcentrapi-0.3.0/dcentrapi/hackMitigation.py
--rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.3.0/dcentrapi/merkleTree.py
--rw-r--r--   0 oded       (502) staff       (20)      226 2023-06-28 06:59:47.000000 dcentrapi-0.3.0/dcentrapi/requests_dappi.py
--rw-r--r--   0 oded       (502) staff       (20)     3107 2023-06-28 06:59:47.000000 dcentrapi-0.3.0/dcentrapi/rpcAggregation.py
--rw-r--r--   0 oded       (502) staff       (20)      909 2022-11-10 13:20:43.000000 dcentrapi-0.3.0/dcentrapi/test.py
--rw-r--r--   0 oded       (502) staff       (20)      837 2023-06-28 06:59:47.000000 dcentrapi-0.3.0/dcentrapi/web3Index.py
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-07-03 11:38:24.548010 dcentrapi-0.3.0/dcentrapi.egg-info/
--rw-r--r--   0 oded       (502) staff       (20)     6741 2023-07-03 11:38:24.000000 dcentrapi-0.3.0/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 oded       (502) staff       (20)      433 2023-07-03 11:38:24.000000 dcentrapi-0.3.0/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 oded       (502) staff       (20)        1 2023-07-03 11:38:24.000000 dcentrapi-0.3.0/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 oded       (502) staff       (20)        9 2023-07-03 11:38:24.000000 dcentrapi-0.3.0/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 oded       (502) staff       (20)       10 2023-07-03 11:38:24.000000 dcentrapi-0.3.0/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 oded       (502) staff       (20)       38 2023-07-03 11:38:24.548384 dcentrapi-0.3.0/setup.cfg
--rw-r--r--   0 oded       (502) staff       (20)     1109 2023-07-03 08:22:17.000000 dcentrapi-0.3.0/setup.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-07-10 11:45:11.952036 dcentrapi-0.3.1/
+-rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.3.1/LICENSE.rst
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-07-10 11:45:11.951898 dcentrapi-0.3.1/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.3.1/README.md
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-07-10 11:45:11.951080 dcentrapi-0.3.1/dcentrapi/
+-rw-r--r--   0 oded       (502) staff       (20)      903 2023-07-10 11:44:06.000000 dcentrapi-0.3.1/dcentrapi/Base.py
+-rw-r--r--   0 oded       (502) staff       (20)      434 2023-07-03 08:17:20.000000 dcentrapi-0.3.1/dcentrapi/__init__.py
+-rw-r--r--   0 oded       (502) staff       (20)     8761 2023-06-28 06:59:47.000000 dcentrapi-0.3.1/dcentrapi/eventPolling.py
+-rw-r--r--   0 oded       (502) staff       (20)      673 2023-07-03 08:17:20.000000 dcentrapi-0.3.1/dcentrapi/gasMonitor.py
+-rw-r--r--   0 oded       (502) staff       (20)      633 2023-07-10 11:41:57.000000 dcentrapi-0.3.1/dcentrapi/hackMitigation.py
+-rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.3.1/dcentrapi/merkleTree.py
+-rw-r--r--   0 oded       (502) staff       (20)      226 2023-06-28 06:59:47.000000 dcentrapi-0.3.1/dcentrapi/requests_dappi.py
+-rw-r--r--   0 oded       (502) staff       (20)     3107 2023-06-28 06:59:47.000000 dcentrapi-0.3.1/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 oded       (502) staff       (20)     1155 2023-07-03 13:16:19.000000 dcentrapi-0.3.1/dcentrapi/test.py
+-rw-r--r--   0 oded       (502) staff       (20)      837 2023-06-28 06:59:47.000000 dcentrapi-0.3.1/dcentrapi/web3Index.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-07-10 11:45:11.951715 dcentrapi-0.3.1/dcentrapi.egg-info/
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-07-10 11:45:11.000000 dcentrapi-0.3.1/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)      433 2023-07-10 11:45:11.000000 dcentrapi-0.3.1/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 oded       (502) staff       (20)        1 2023-07-10 11:45:11.000000 dcentrapi-0.3.1/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 oded       (502) staff       (20)        9 2023-07-10 11:45:11.000000 dcentrapi-0.3.1/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 oded       (502) staff       (20)       10 2023-07-10 11:45:11.000000 dcentrapi-0.3.1/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 oded       (502) staff       (20)       38 2023-07-10 11:45:11.952077 dcentrapi-0.3.1/setup.cfg
+-rw-r--r--   0 oded       (502) staff       (20)     1109 2023-07-10 11:44:06.000000 dcentrapi-0.3.1/setup.py
```

### Comparing `dcentrapi-0.3.0/LICENSE.rst` & `dcentrapi-0.3.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.0/PKG-INFO` & `dcentrapi-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.3.0
+Version: 0.3.1
 Summary: Dcentralab Pypi packages
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `dcentrapi-0.3.0/README.md` & `dcentrapi-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.0/dcentrapi/Base.py` & `dcentrapi-0.3.1/dcentrapi/Base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 class Base:
     def __init__(self, stage, username=None, key=None):
-        self.__version__ = "0.3.0"
+        self.__version__ = "0.3.1"
 
         if stage == "develop":
             self.headers = {"Authorization": username + "," + key}
             self.url = "https://test-api.dcentralab.com/"
             self.web3index_url = "https://test-api.web3index.info/"
         if stage == "staging":
             self.headers = {"Authorization": username + "," + key}
```

### Comparing `dcentrapi-0.3.0/dcentrapi/eventPolling.py` & `dcentrapi-0.3.1/dcentrapi/eventPolling.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.0/dcentrapi/gasMonitor.py` & `dcentrapi-0.3.1/dcentrapi/gasMonitor.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.0/dcentrapi/merkleTree.py` & `dcentrapi-0.3.1/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.0/dcentrapi/rpcAggregation.py` & `dcentrapi-0.3.1/dcentrapi/rpcAggregation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.0/dcentrapi/test.py` & `dcentrapi-0.3.1/dcentrapi/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-from dcentrapi import MerkleTree
-from dcentrapi.merkleTree import verify_leaf
-
-tree = MerkleTree("develop", "Chainport", 'f3taga-mHNLlv8KDh_HE76oOGyU')
-leaf1 = ("0x9D9fF3A3A147fb5F96d773E244BAc63Ffa1F21C9", 307835000000000028, 1)
-leaf2 = ("0x9D9fF3A3A147fb5F96d773E244BAc63Ffa1F21C9", 99366666666666676687, 2)
-leaf3 = ("0x9D9fF3A3A147fb5F96d773E244BAc63Ffa1F21C9", 38500000000000003, 3)
-leaves = [leaf1, leaf2, leaf3]
-encoding = "(address,uint256,uint256)"
-root, layers = tree.build_tree(leaves, encoding)
-print(root.hashValue.hex())
-
-
-leaf_not_in_tree = ("0x9D9fF3A3A147fb5F96d773E244BAc63Ffa1F21C9", 38500000000000003, 4)
-proof1 = tree.get_proof(leaf=leaf1)
-proof1 = [bytes(p.hashValue) for p in proof1]
-assert verify_leaf(root=root.hashValue.hex(), leaf=leaf1, proof=proof1, encoding=encoding)
-assert verify_leaf(root=root.hashValue.hex(), leaf=leaf_not_in_tree, proof=proof1, encoding=encoding) is False
+# from dcentrapi import MerkleTree
+# from dcentrapi.merkleTree import verify_leaf
+#
+# tree = MerkleTree("develop", "Chainport", 'f3taga-mHNLlv8KDh_HE76oOGyU')
+# leaf1 = ("0x9D9fF3A3A147fb5F96d773E244BAc63Ffa1F21C9", 307835000000000028, 1)
+# leaf2 = ("0x9D9fF3A3A147fb5F96d773E244BAc63Ffa1F21C9", 99366666666666676687, 2)
+# leaf3 = ("0x9D9fF3A3A147fb5F96d773E244BAc63Ffa1F21C9", 38500000000000003, 3)
+# leaves = [leaf1, leaf2, leaf3]
+# encoding = "(address,uint256,uint256)"
+# root, layers = tree.build_tree(leaves, encoding)
+# print(root.hashValue.hex())
+#
+#
+# leaf_not_in_tree = ("0x9D9fF3A3A147fb5F96d773E244BAc63Ffa1F21C9", 38500000000000003, 4)
+# proof1 = tree.get_proof(leaf=leaf1)
+# proof1 = [bytes(p.hashValue) for p in proof1]
+# assert verify_leaf(root=root.hashValue.hex(), leaf=leaf1, proof=proof1, encoding=encoding)
+# assert verify_leaf(root=root.hashValue.hex(), leaf=leaf_not_in_tree, proof=proof1, encoding=encoding) is False
+#
+from dcentrapi import GasMonitor
 
+gm = GasMonitor("develop", "Chainport", 'f3taga-mHNLlv8KDh_HE76oOGyU')
+gm.get_optimal_gas_price(network_name="POLYGON", minutes="11", stats=["avg", "max"], values=["gas_price"])
```

### Comparing `dcentrapi-0.3.0/dcentrapi/web3Index.py` & `dcentrapi-0.3.1/dcentrapi/web3Index.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.0/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.3.1/dcentrapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.3.0
+Version: 0.3.1
 Summary: Dcentralab Pypi packages
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `dcentrapi-0.3.0/setup.py` & `dcentrapi-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     return result.group(1)
 
 
 DESCRIPTION = 'Dcentralab Pypi packages'
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 project_name = 'dcentrapi'
-VERSION = "0.3.0"
+VERSION = "0.3.1"
 
 
 # Setting up
 setup(
     name="dcentrapi",
     version=VERSION,
     author="Dcentralab (Niv Shitrit)",
```

