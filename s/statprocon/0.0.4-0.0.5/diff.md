# Comparing `tmp/statprocon-0.0.4.tar.gz` & `tmp/statprocon-0.0.5.tar.gz`

## Comparing `statprocon-0.0.4.tar` & `statprocon-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 statprocon-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 statprocon-0.0.4/requirements-dev.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.0.4/.idea/.gitignore
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.0.4/.idea/dataSources.local.xml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.0.4/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.0.4/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.0.4/.idea/vcs.xml
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 statprocon-0.0.4/.idea/workspace.xml
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 statprocon-0.0.4/.idea/xmr.iml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.0.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 statprocon-0.0.4/statprocon/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.4/statprocon/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.4/statprocon/charts/__init__.py
--rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 statprocon-0.0.4/statprocon/charts/xmr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 statprocon-0.0.4/tests/test_xmr.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 statprocon-0.0.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.0.4/LICENSE
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 statprocon-0.0.4/README.md
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 statprocon-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 statprocon-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 statprocon-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 statprocon-0.0.5/requirements-dev.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/.gitignore
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/dataSources.local.xml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/workspace.xml
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/xmr.iml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 statprocon-0.0.5/statprocon/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.5/statprocon/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.5/statprocon/charts/__init__.py
+-rw-r--r--   0        0        0     7222 2020-02-02 00:00:00.000000 statprocon-0.0.5/statprocon/charts/xmr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     7859 2020-02-02 00:00:00.000000 statprocon-0.0.5/tests/test_xmr.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 statprocon-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 statprocon-0.0.5/README.md
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 statprocon-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 statprocon-0.0.5/PKG-INFO
```

### Comparing `statprocon-0.0.4/requirements-dev.txt` & `statprocon-0.0.5/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.4/.idea/workspace.xml` & `statprocon-0.0.5/.idea/workspace.xml`

 * *Files 27% similar despite different names*

#### Comparing `statprocon-0.0.4/.idea/workspace.xml` & `statprocon-0.0.5/.idea/workspace.xml`

```diff
@@ -3,14 +3,16 @@
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="6b007249-c07a-402d-ab76-cd0adebb4623" name="Default Changelist" comment="">
       <change beforePath="$PROJECT_DIR$/CHANGELOG.md" beforeDir="false" afterPath="$PROJECT_DIR$/CHANGELOG.md" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/statprocon/charts/xmr.py" beforeDir="false" afterPath="$PROJECT_DIR$/statprocon/charts/xmr.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/test_xmr.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test_xmr.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -54,24 +56,47 @@
   </component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/statprocon/charts"/>
       <recent name="$PROJECT_DIR$"/>
     </key>
   </component>
+  <component name="RunManager">
+    <configuration name="Unittests for test_xmr.XmRTestCase.test_rule_1_points_beyond_both_limits" type="tests" factoryName="Unittests" temporary="true" nameIsGenerated="true">
+      <module name="xmr"/>
+      <option name="INTERPRETER_OPTIONS" value=""/>
+      <option name="PARENT_ENVS" value="true"/>
+      <option name="SDK_HOME" value=""/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
+      <option name="IS_MODULE_SDK" value="true"/>
+      <option name="ADD_CONTENT_ROOTS" value="true"/>
+      <option name="ADD_SOURCE_ROOTS" value="true"/>
+      <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
+      <option name="_new_additionalArguments" value="&quot;&quot;"/>
+      <option name="_new_target" value="&quot;test_xmr.XmRTestCase.test_rule_1_points_beyond_both_limits&quot;"/>
+      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
+      <method v="2"/>
+    </configuration>
+    <recent_temporary>
+      <list>
+        <item itemvalue="Python tests.Unittests for test_xmr.XmRTestCase.test_rule_1_points_beyond_both_limits"/>
+      </list>
+    </recent_temporary>
+  </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="6b007249-c07a-402d-ab76-cd0adebb4623" name="Default Changelist" comment=""/>
       <created>1688827023388</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1688827023388</updated>
       <workItem from="1688827024910" duration="1917000"/>
-      <workItem from="1688848868641" duration="17530000"/>
+      <workItem from="1688848868641" duration="17704000"/>
+      <workItem from="1688944372544" duration="1441000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
@@ -80,9 +105,13 @@
         <entry key="MAIN">
           <value>
             <State/>
           </value>
         </entry>
       </map>
     </option>
+    <option name="oldMeFiltersMigrated" value="true"/>
+  </component>
+  <component name="com.intellij.coverage.CoverageDataManagerImpl">
+    <SUITE FILE_PATH="coverage/statprocon$Unittests_for_test_xmr_XmRTestCase_test_rule_1_points_beyond_both_limits.coverage" NAME="Unittests for test_xmr.XmRTestCase.test_rule_1_points_beyond_both_limits Coverage Results" MODIFIED="1688952580683" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
   </component>
 </project>
```

### Comparing `statprocon-0.0.4/.idea/xmr.iml` & `statprocon-0.0.5/.idea/xmr.iml`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.4/statprocon/charts/xmr.py` & `statprocon-0.0.5/statprocon/charts/xmr.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
             lower_limit: Decimal = Decimal('0')
     ) -> list[bool]:
         result = [False] * len(data)
         for i, val in enumerate(data):
             if val is None:
                 continue
 
-            if not lower_limit < val < upper_limit:
+            if not lower_limit <= val <= upper_limit:
                 result[i] = True
 
         return result
 
     @staticmethod
     def mean(nums: TYPE_COUNTS) -> Decimal:
         s = sum(nums)
```

### Comparing `statprocon-0.0.4/tests/test_xmr.py` & `statprocon-0.0.5/tests/test_xmr.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,25 +89,31 @@
         self.assertListEqual(xmr.rule_1_x_indices_beyond_limits(group_a_upper, group_a_lower), expected)
 
     def test_rule_1_points_beyond_both_limits(self):
         """
         This test dataset comes from Table 9.2: Accounts Receivable for Years One and Two in Making Sense of Data
         """
 
-        ar_pct_sales = ['55.6', '54.7', '54.9', '54.8', '56.9', '55.7', '53.8', '54.8', '53.4', '57.0', '59.4', '63.2', '60.9', '60.7', '58.6', '57.3', '56.9', '58.1', '58.3', '50.9', '53.3', '52.5', '50.8', '52.9']
+        ar_pct_sales = [
+            '55.6', '54.7', '54.9', '54.8', '56.9', '55.7', '53.8', '54.8', '53.4', '57.0', '59.4', '63.2',
+            '60.9', '60.7', '58.6', '57.3', '56.9', '58.1', '58.3', '50.9', '53.3', '52.5', '50.8', '52.9'
+        ]
         counts_dec = list(map(lambda x: Decimal(x), ar_pct_sales))
         xmr = XmR(counts_dec)
 
         upper_limit = Decimal('60.7')
-        # Index 13 is exactly equal to upper_limit
-        # In Figure 9.5, this point is identified as meeting the criteria
         expected = [False] * len(ar_pct_sales)
-        for i in [11, 12, 13, 19, 22]:
+        for i in [11, 12, 19, 22]:
             expected[i] = True
-        self.assertListEqual(xmr.rule_1_x_indices_beyond_limits(upper_limit=upper_limit), expected)
+
+        actual = xmr.rule_1_x_indices_beyond_limits(upper_limit=upper_limit)
+        self.assertListEqual(actual, expected)
+
+        # Point 13 is detected in the chart in the book because the actual percentage is slightly lower than the limit
+        self.assertFalse(actual[13], 'Point 13 equals the limit and should not be detected')
 
     def test_rule_1_point_beyond_upper_range_limit(self):
         """
         This test dataset also comes from Table 9.2
         """
         ar_pct_sales = ['55.6', '54.7', '54.9', '54.8', '56.9', '55.7', '53.8', '54.8', '53.4', '57.0', '59.4', '63.2',
                         '60.9', '60.7', '58.6', '57.3', '56.9', '58.1', '58.3', '50.9', '53.3', '52.5', '50.8', '52.9']
```

### Comparing `statprocon-0.0.4/LICENSE` & `statprocon-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.4/README.md` & `statprocon-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.4/pyproject.toml` & `statprocon-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "statprocon"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Matt McCormick", email="mattmccor@gmail.com" },
 ]
 description = "A Python helper library for generating Process Behaviour Charts"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `statprocon-0.0.4/PKG-INFO` & `statprocon-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statprocon
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python helper library for generating Process Behaviour Charts
 Project-URL: Homepage, https://github.com/mattmccormick/statprocon
 Project-URL: Bug Tracker, https://github.com/mattmccormick/statprocon/issues
 Project-URL: Changelog, https://github.com/mattmccormick/statprocon/blob/main/CHANGELOG.md
 Author-email: Matt McCormick <mattmccor@gmail.com>
 License-File: LICENSE
 Keywords: Process Behavior Chart,Process Behaviour Chart,QCC,Quality Control Chart,SPC,Shewhart,Statistical Process Control,Wheeler,XmR
```

