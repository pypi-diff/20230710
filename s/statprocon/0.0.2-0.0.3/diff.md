# Comparing `tmp/statprocon-0.0.2.tar.gz` & `tmp/statprocon-0.0.3.tar.gz`

## Comparing `statprocon-0.0.2.tar` & `statprocon-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 statprocon-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 statprocon-0.0.2/requirements-dev.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/dataSources.local.xml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/xmr.iml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 statprocon-0.0.2/statprocon/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.2/statprocon/charts/__init__.py
--rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 statprocon-0.0.2/statprocon/charts/xmr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 statprocon-0.0.2/tests/test_xmr.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 statprocon-0.0.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.0.2/LICENSE
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 statprocon-0.0.2/README.md
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 statprocon-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 statprocon-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 statprocon-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.3/py.typed
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 statprocon-0.0.3/requirements-dev.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.0.3/.idea/dataSources.local.xml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 statprocon-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 statprocon-0.0.3/.idea/xmr.iml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 statprocon-0.0.3/statprocon/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.3/statprocon/charts/__init__.py
+-rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 statprocon-0.0.3/statprocon/charts/xmr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 statprocon-0.0.3/tests/test_xmr.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 statprocon-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 statprocon-0.0.3/README.md
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 statprocon-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 statprocon-0.0.3/PKG-INFO
```

### Comparing `statprocon-0.0.2/requirements-dev.txt` & `statprocon-0.0.3/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.2/.idea/workspace.xml` & `statprocon-0.0.3/.idea/workspace.xml`

 * *Files 1% similar despite different names*

#### Comparing `statprocon-0.0.2/.idea/workspace.xml` & `statprocon-0.0.3/.idea/workspace.xml`

```diff
@@ -62,15 +62,15 @@
     <task active="true" id="Default" summary="Default task">
       <changelist id="6b007249-c07a-402d-ab76-cd0adebb4623" name="Default Changelist" comment=""/>
       <created>1688827023388</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1688827023388</updated>
       <workItem from="1688827024910" duration="1917000"/>
-      <workItem from="1688848868641" duration="14801000"/>
+      <workItem from="1688848868641" duration="16452000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
```

### Comparing `statprocon-0.0.2/.idea/xmr.iml` & `statprocon-0.0.3/.idea/xmr.iml`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.2/statprocon/charts/xmr.py` & `statprocon-0.0.3/statprocon/charts/xmr.py`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.2/tests/test_xmr.py` & `statprocon-0.0.3/tests/test_xmr.py`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.2/LICENSE` & `statprocon-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.2/README.md` & `statprocon-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.2/pyproject.toml` & `statprocon-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "statprocon"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Matt McCormick", email="mattmccor@gmail.com" },
 ]
 description = "A Python helper library for generating Process Behaviour Charts"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `statprocon-0.0.2/PKG-INFO` & `statprocon-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statprocon
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python helper library for generating Process Behaviour Charts
 Project-URL: Homepage, https://github.com/mattmccormick/statprocon
 Project-URL: Bug Tracker, https://github.com/mattmccormick/statprocon/issues
 Project-URL: Changelog, https://github.com/mattmccormick/statprocon/blob/main/CHANGELOG.md
 Author-email: Matt McCormick <mattmccor@gmail.com>
 License-File: LICENSE
 Keywords: Process Behavior Chart,Process Behaviour Chart,QCC,Quality Control Chart,SPC,Shewhart,Statistical Process Control,Wheeler,XmR
```

