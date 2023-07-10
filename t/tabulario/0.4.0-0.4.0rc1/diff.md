# Comparing `tmp/tabulario-0.4.0.tar.gz` & `tmp/tabulario-0.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabulario-0.4.0.tar", max compression
+gzip compressed data, was "tabulario-0.4.0rc1.tar", max compression
```

## Comparing `tabulario-0.4.0.tar` & `tabulario-0.4.0rc1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11358 2023-07-10 15:17:11.473249 tabulario-0.4.0/LICENSE
--rw-r--r--   0        0        0     7126 2023-07-10 15:17:11.473249 tabulario-0.4.0/README.md
--rw-r--r--   0        0        0     2487 2023-07-10 15:17:21.881096 tabulario-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      785 2023-07-10 15:17:11.477249 tabulario-0.4.0/tab/__init__.py
--rw-r--r--   0        0        0     4229 2023-07-10 15:17:11.477249 tabulario-0.4.0/tab/cli.py
--rw-r--r--   0        0        0      871 2023-07-10 15:17:11.477249 tabulario-0.4.0/tab/exceptions.py
--rw-r--r--   0        0        0     5018 2023-07-10 15:17:11.477249 tabulario-0.4.0/tab/oauth.py
--rw-r--r--   0        0        0     1004 2023-07-10 15:17:11.477249 tabulario-0.4.0/tab/util.py
--rw-r--r--   0        0        0      836 2023-07-10 15:17:11.477249 tabulario-0.4.0/tabular/__init__.py
--rw-r--r--   0        0        0     4955 2023-07-10 15:17:11.477249 tabulario-0.4.0/tabular/loader.py
--rw-r--r--   0        0        0     2111 2023-07-10 15:17:11.477249 tabulario-0.4.0/tabular/tabular.py
--rw-r--r--   0        0        0     7937 1970-01-01 00:00:00.000000 tabulario-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-26 14:48:22.117095 tabulario-0.4.0rc1/LICENSE
+-rw-r--r--   0        0        0     7126 2023-06-26 14:48:22.117095 tabulario-0.4.0rc1/README.md
+-rw-r--r--   0        0        0     2493 2023-06-26 14:48:35.917175 tabulario-0.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      785 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tab/__init__.py
+-rw-r--r--   0        0        0     4229 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tab/cli.py
+-rw-r--r--   0        0        0      871 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tab/exceptions.py
+-rw-r--r--   0        0        0     5018 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tab/oauth.py
+-rw-r--r--   0        0        0     1004 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tab/util.py
+-rw-r--r--   0        0        0      836 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tabular/__init__.py
+-rw-r--r--   0        0        0     4955 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tabular/loader.py
+-rw-r--r--   0        0        0     2111 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tabular/tabular.py
+-rw-r--r--   0        0        0     7943 1970-01-01 00:00:00.000000 tabulario-0.4.0rc1/PKG-INFO
```

### Comparing `tabulario-0.4.0/LICENSE` & `tabulario-0.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0/README.md` & `tabulario-0.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0/pyproject.toml` & `tabulario-0.4.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 [tool.poetry]
 name = "tabulario"
-version = "0.4.0"
+version = "0.4.0rc1"
 readme = "README.md"
 homepage = "https://tabular.io/"
 repository = "https://github.com/tabular-io/"
 description = "Utility library for Tabular.io"
 authors = ["Tabular Technologies, Inc. <fokko@tabular.io>"]
 license = "Apache License 2.0"
 
@@ -40,15 +40,15 @@
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.1"
 click = "^8.1.3"
-pyiceberg = "0.4.0"
+pyiceberg = "0.4.0rc1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 pytest-checkdocs = "^2.9.0"
 pre-commit = "^2.0.0"
 coverage = { version = "^6.5.0", extras = ["toml"] }
 requests-mock = "^1.10.0"
```

### Comparing `tabulario-0.4.0/tab/__init__.py` & `tabulario-0.4.0rc1/tab/__init__.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0/tab/cli.py` & `tabulario-0.4.0rc1/tab/cli.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0/tab/exceptions.py` & `tabulario-0.4.0rc1/tab/exceptions.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0/tab/oauth.py` & `tabulario-0.4.0rc1/tab/oauth.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0/tab/util.py` & `tabulario-0.4.0rc1/tab/util.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0/tabular/__init__.py` & `tabulario-0.4.0rc1/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0/tabular/loader.py` & `tabulario-0.4.0rc1/tabular/loader.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0/tabular/tabular.py` & `tabulario-0.4.0rc1/tabular/tabular.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0/PKG-INFO` & `tabulario-0.4.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tabulario
-Version: 0.4.0
+Version: 0.4.0rc1
 Summary: Utility library for Tabular.io
 Home-page: https://tabular.io/
 License: Apache-2.0
 Author: Tabular Technologies, Inc.
 Author-email: fokko@tabular.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: pyiceberg (==0.4.0)
+Requires-Dist: pyiceberg (==0.4.0rc1)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://github.com/tabular-io/
 Description-Content-Type: text/markdown
 
 # Tab
 
 This is a helper library to easily fetch and refresh access token from Tabular.
```

