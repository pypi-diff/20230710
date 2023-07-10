# Comparing `tmp/jcci-0.0.5.tar.gz` & `tmp/jcci-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcci-0.0.5.tar", last modified: Tue Jul  4 10:44:36 2023, max compression
+gzip compressed data, was "jcci-0.0.6.tar", last modified: Mon Jul 10 09:22:15 2023, max compression
```

## Comparing `jcci-0.0.5.tar` & `jcci-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 10:44:36.078792 jcci-0.0.5/
--rw-rw-rw-   0        0        0        0 2022-09-20 03:06:31.000000 jcci-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1468 2023-07-04 10:44:36.077793 jcci-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      955 2023-06-26 05:36:35.000000 jcci-0.0.5/README.md
--rw-rw-rw-   0        0        0      695 2023-07-04 10:44:25.000000 jcci-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 10:44:36.078792 jcci-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 10:44:36.064810 jcci-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 10:44:36.070793 jcci-0.0.5/src/jcci/
--rw-rw-rw-   0        0        0        0 2022-09-20 03:04:57.000000 jcci-0.0.5/src/jcci/__init__.py
--rw-rw-rw-   0        0        0     2083 2023-06-25 09:25:01.000000 jcci-0.0.5/src/jcci/java_analyzer.py
--rw-rw-rw-   0        0        0    42459 2023-07-04 10:38:53.000000 jcci-0.0.5/src/jcci/jcci.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:44:36.076829 jcci-0.0.5/src/jcci.egg-info/
--rw-rw-rw-   0        0        0     1468 2023-07-04 10:44:36.000000 jcci-0.0.5/src/jcci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-07-04 10:44:36.000000 jcci-0.0.5/src/jcci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 10:44:36.000000 jcci-0.0.5/src/jcci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-04 10:44:36.000000 jcci-0.0.5/src/jcci.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-04 10:44:36.000000 jcci-0.0.5/src/jcci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 09:22:15.564310 jcci-0.0.6/
+-rw-rw-rw-   0        0        0     1082 2023-06-30 07:21:11.000000 jcci-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3029 2023-07-10 09:22:15.563312 jcci-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2392 2023-07-04 11:32:51.000000 jcci-0.0.6/README.md
+-rw-rw-rw-   0        0        0     1247 2023-07-10 09:21:41.000000 jcci-0.0.6/README.pypi.md
+-rw-rw-rw-   0        0        0      708 2023-07-10 09:21:57.000000 jcci-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-10 09:22:15.564310 jcci-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 09:22:15.547314 jcci-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 09:22:15.555311 jcci-0.0.6/src/jcci/
+-rw-rw-rw-   0        0        0        0 2023-06-30 07:21:11.000000 jcci-0.0.6/src/jcci/__init__.py
+-rw-rw-rw-   0        0        0     2083 2023-06-30 07:21:11.000000 jcci-0.0.6/src/jcci/java_analyzer.py
+-rw-rw-rw-   0        0        0    42861 2023-07-10 09:09:34.000000 jcci-0.0.6/src/jcci/jcci.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:22:15.562318 jcci-0.0.6/src/jcci.egg-info/
+-rw-rw-rw-   0        0        0     3029 2023-07-10 09:22:15.000000 jcci-0.0.6/src/jcci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-07-10 09:22:15.000000 jcci-0.0.6/src/jcci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 09:22:15.000000 jcci-0.0.6/src/jcci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-10 09:22:15.000000 jcci-0.0.6/src/jcci.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-10 09:22:15.000000 jcci-0.0.6/src/jcci.egg-info/top_level.txt
```

### Comparing `jcci-0.0.5/PKG-INFO` & `jcci-0.0.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,66 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.0.5
-Summary: Java code commit impact in pure Python
+Version: 0.0.6
+Summary: Java code commit impact analyze in pure Python
 Author-email: Quan Li <441640312@qq.com>
+License: MIT License
+        
+        Copyright (c) 2023 pipi
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Project-URL: Homepage, https://github.com/baikaishuipp/jcci
 Project-URL: Bug Tracker, https://github.com/baikaishuipp/jcci/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## Project description
-jcci is a pure python library that analyzes the impact of two git submissions of Java projects on the project and generates tree chart data
-for example:
+#### Description
+Java code commit impact analysis, is a pure python library that analyzes the impact of two git submissions of Java projects on the project and generates tree chart data.
 
-### Installing jcci
+Github: [jcci](https://github.com/baikaishuipp/jcci)
+#### Installation
 ```
-  $pip install jcci
+pip install jcci
 ```
 
-### Quick start
+#### Instructions
+Start a new python project, add a new python file, code example:
+
 ```
->>> from jcci import jcci
->>> jcci.analyze('git@xxxx.git','master','commit_id1','commit_id2', 'username1')
+from jcci import jcci
+
+jcci.analyze('git@xxxx.git','master','commit_id1','commit_id2', 'username1')
 ```
+
 At the same time, the project will be cloned in the directory and then analyzed to generate a file with the suffix format commit_id1...commit_id2.cci, which contains the tree diagram data generated by the analysis results, through https://echarts.apache.org/examples/zh/editor.html?c=tree-basic link, replace the data data can be displayed through the view.
 
-#### CCI result
-![result](https://raw.githubusercontent.com/baikaishuipp/jcci/main/cci-result.png)
+##### CCI result
+![result](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/cci-result.png)
+
+##### CCI result tree view
+![treeView](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/cii-result-tree.png)
 
-#### CCI result tree view
-![treeView](https://raw.githubusercontent.com/baikaishuipp/jcci/main/cii-result-tree.png)
+#### Communication
+Communicate via Wechat:
 
+![communicate via Wechat](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/wechat.jpg)
```

### Comparing `jcci-0.0.5/README.md` & `jcci-0.0.6/README.pypi.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,30 @@
-## Project description
-jcci is a pure python library that analyzes the impact of two git submissions of Java projects on the project and generates tree chart data
-for example:
+#### Description
+Java code commit impact analysis, is a pure python library that analyzes the impact of two git submissions of Java projects on the project and generates tree chart data.
 
-### Installing jcci
+Github: [jcci](https://github.com/baikaishuipp/jcci)
+#### Installation
 ```
-  $pip install jcci
+pip install jcci
 ```
 
-### Quick start
+#### Instructions
+Start a new python project, add a new python file, code example:
+
 ```
->>> from jcci import jcci
->>> jcci.analyze('git@xxxx.git','master','commit_id1','commit_id2', 'username1')
+from jcci import jcci
+
+jcci.analyze('git@xxxx.git','master','commit_id1','commit_id2', 'username1')
 ```
+
 At the same time, the project will be cloned in the directory and then analyzed to generate a file with the suffix format commit_id1...commit_id2.cci, which contains the tree diagram data generated by the analysis results, through https://echarts.apache.org/examples/zh/editor.html?c=tree-basic link, replace the data data can be displayed through the view.
 
-#### CCI result
-![result](https://raw.githubusercontent.com/baikaishuipp/jcci/main/cci-result.png)
+##### CCI result
+![result](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/cci-result.png)
+
+##### CCI result tree view
+![treeView](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/cii-result-tree.png)
 
-#### CCI result tree view
-![treeView](https://raw.githubusercontent.com/baikaishuipp/jcci/main/cii-result-tree.png)
+#### Communication
+Communicate via Wechat:
 
+![communicate via Wechat](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/wechat.jpg)
```

### Comparing `jcci-0.0.5/pyproject.toml` & `jcci-0.0.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jcci"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Quan Li", email="441640312@qq.com" },
 ]
-description = "Java code commit impact in pure Python"
-readme = "README.md"
+description = "Java code commit impact analyze in pure Python"
+readme = "README.pypi.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `jcci-0.0.5/src/jcci/java_analyzer.py` & `jcci-0.0.6/src/jcci/java_analyzer.py`

 * *Files identical despite different names*

### Comparing `jcci-0.0.5/src/jcci/jcci.py` & `jcci-0.0.6/src/jcci/jcci.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,26 +57,27 @@
 #        }
 #       'contains_declarators': ['abc','def']
 # 	}]
 # }
 #
 def _analyze_java_file(filepath, folder_name):
     print(filepath)
-    if 'InsightsFeeController' in filepath:
-        print("debug")
     import_list = []
     with open(filepath, encoding='UTF-8') as fp:
         file_content = fp.read()
     lines = file_content.split('\n')
     try:
         tree = javalang.parse.parse(file_content)
         package_name = tree.package.name
         types = tree.types[0]
         class_name = types.name
-    except:
+    except Exception as e:
+        print(e.args)
+        print(str(e))
+        print(repr(e))
         return None
     # is controller or not
     is_controller = False
     base_request = ''
     annotations = types.annotations
     for annotation in annotations:
         if 'Controller' in annotation.name:
@@ -273,21 +274,23 @@
                                 extends_name_path, is_controller)
     file_analyze.imports = imports
     file_analyze.implements = implements_names_list
     file_analyze.declarators = fields_list
     file_analyze.methods = methods_list
     return file_analyze
 
+
 def _get_api_part_route(part):
     part_class = type(part).__name__
     if part_class == 'MemberReference':
         return part.member
     elif part_class == 'Literal':
         return part.value
 
+
 def _get_method_end_line(method_obj):
     method_end_line = method_obj.position.line
     if method_obj.body is not None and len(method_obj.body) > 0:
         method_end_line = method_obj.body[-1].position.line
         method_body = method_obj.body[-1]
         while True:
             method_obj_dict = method_body.__dict__
@@ -405,14 +408,16 @@
         return False, False
     class_path = java_analyze.package_name + '.' + java_analyze.class_name
     implements = java_analyze.implements
     imports = java_file_analyze.imports.imports
     class_path_analyze = java_file_analyze.package_name + '.' + java_file_analyze.class_name
     if class_path_analyze == class_path:
         return True, True
+    if java_file_analyze.package_name == java_analyze.package_name:
+        return True, True
     for import_obj in imports:
         if not import_obj.wildcard:
             if class_path == import_obj.path or import_obj.path in implements:
                 return True, True
         else:
             class_path_parent = '.'.join(class_path.split('.')[0: -1])
             if class_path_parent == import_obj.path:
@@ -536,15 +541,20 @@
 
 
 def _clean_occupy(occupy_path):
     if os.path.exists(occupy_path):
         os.remove(occupy_path)
 
 
-def _class_in_method(class_name, method_content):
+def _class_in_method(class_name, method):
+    if method.contains_declarators is not None:
+        dcl_in_method = [d for d in method.contains_declarators if d.type == class_name]
+        if len(dcl_in_method) > 0:
+            return True
+    method_content = str(method.content)
     if class_name + ' ' in method_content \
             or '<' + class_name + '>' in method_content \
             or class_name + '.' in method_content:
         return True
     else:
         return False
 
@@ -582,15 +592,16 @@
             which_java_file_methods = which_java_file_analyze.methods
             which_java_file_declarators = [declarator for declarator in which_java_file_analyze.declarators if
                                            declarator.type == which_class_name]
             for which_java_file_method in which_java_file_methods:
                 classname_in_method = False
                 tmp = []
                 if diff_result_item.changed_declarators != {}:
-                    classname_in_method = _class_in_method(which_class_name, str(which_java_file_method.content))
+                    classname_in_method = _class_in_method(which_class_name, which_java_file_method)
+                print('classname_in_method: ', classname_in_method)
                 if which_java_file_method.contains_class is not None:
                     for implement in which_implements:
                         if implement in which_java_file_method.contains_class.keys() and 'methods' in \
                                 which_java_file_method.contains_class[implement].keys():
                             java_file_method_includes_methods = which_java_file_method.contains_class[implement][
                                 'methods']
                             tmp = [j for j in diff_result_item.changed_methods.keys() if
@@ -719,9 +730,7 @@
     t2 = datetime.datetime.now()
     try:
         print(datetime.datetime.now(), ':', 'Analyze done, remove occupy, others can analyze now', flush=True)
         os.remove(folder_name + sep + 'Occupy.ing')
     except:
         pass
     print(datetime.datetime.now(), ':', 'Analyze done, spend: ', t2 - t1, flush=True)
-
-
```

### Comparing `jcci-0.0.5/src/jcci.egg-info/PKG-INFO` & `jcci-0.0.6/src/jcci.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,66 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.0.5
-Summary: Java code commit impact in pure Python
+Version: 0.0.6
+Summary: Java code commit impact analyze in pure Python
 Author-email: Quan Li <441640312@qq.com>
+License: MIT License
+        
+        Copyright (c) 2023 pipi
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Project-URL: Homepage, https://github.com/baikaishuipp/jcci
 Project-URL: Bug Tracker, https://github.com/baikaishuipp/jcci/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## Project description
-jcci is a pure python library that analyzes the impact of two git submissions of Java projects on the project and generates tree chart data
-for example:
+#### Description
+Java code commit impact analysis, is a pure python library that analyzes the impact of two git submissions of Java projects on the project and generates tree chart data.
 
-### Installing jcci
+Github: [jcci](https://github.com/baikaishuipp/jcci)
+#### Installation
 ```
-  $pip install jcci
+pip install jcci
 ```
 
-### Quick start
+#### Instructions
+Start a new python project, add a new python file, code example:
+
 ```
->>> from jcci import jcci
->>> jcci.analyze('git@xxxx.git','master','commit_id1','commit_id2', 'username1')
+from jcci import jcci
+
+jcci.analyze('git@xxxx.git','master','commit_id1','commit_id2', 'username1')
 ```
+
 At the same time, the project will be cloned in the directory and then analyzed to generate a file with the suffix format commit_id1...commit_id2.cci, which contains the tree diagram data generated by the analysis results, through https://echarts.apache.org/examples/zh/editor.html?c=tree-basic link, replace the data data can be displayed through the view.
 
-#### CCI result
-![result](https://raw.githubusercontent.com/baikaishuipp/jcci/main/cci-result.png)
+##### CCI result
+![result](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/cci-result.png)
+
+##### CCI result tree view
+![treeView](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/cii-result-tree.png)
 
-#### CCI result tree view
-![treeView](https://raw.githubusercontent.com/baikaishuipp/jcci/main/cii-result-tree.png)
+#### Communication
+Communicate via Wechat:
 
+![communicate via Wechat](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/wechat.jpg)
```

