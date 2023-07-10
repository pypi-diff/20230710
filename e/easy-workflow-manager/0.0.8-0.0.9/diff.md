# Comparing `tmp/easy_workflow_manager-0.0.8-py3-none-any.whl.zip` & `tmp/easy_workflow_manager-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,21 @@
-Zip file size: 14943 bytes, number of entries: 18
--rw-r--r--  2.0 unx    31697 b- defN 18-Dec-21 13:59 easy_workflow_manager/__init__.py
+Zip file size: 15487 bytes, number of entries: 19
+-rw-r--r--  2.0 unx    31697 b- defN 18-Dec-21 14:33 easy_workflow_manager/__init__.py
 -rw-rw-r--  2.0 unx      140 b- defN 18-Dec-19 14:00 easy_workflow_manager/settings.ini
 -rw-r--r--  2.0 unx        0 b- defN 18-Dec-19 14:00 easy_workflow_manager/scripts/__init__.py
 -rw-r--r--  2.0 unx      424 b- defN 18-Dec-19 14:27 easy_workflow_manager/scripts/branch_from.py
 -rw-r--r--  2.0 unx      552 b- defN 18-Dec-19 14:00 easy_workflow_manager/scripts/clear_qa.py
 -rw-r--r--  2.0 unx      561 b- defN 18-Dec-19 14:00 easy_workflow_manager/scripts/deploy_to_qa.py
 -rw-r--r--  2.0 unx      370 b- defN 18-Dec-19 14:00 easy_workflow_manager/scripts/new_branch_from_source.py
 -rw-r--r--  2.0 unx      473 b- defN 18-Dec-19 14:00 easy_workflow_manager/scripts/qa_to_source.py
 -rw-r--r--  2.0 unx      709 b- defN 18-Dec-19 15:27 easy_workflow_manager/scripts/show_branches.py
 -rw-r--r--  2.0 unx      436 b- defN 18-Dec-19 14:00 easy_workflow_manager/scripts/show_qa.py
 -rw-r--r--  2.0 unx      180 b- defN 18-Dec-19 14:00 easy_workflow_manager/scripts/show_repo_info.py
 -rw-r--r--  2.0 unx      323 b- defN 18-Dec-19 14:00 easy_workflow_manager/scripts/tag_release.py
--rwxrwxr-x  2.0 unx      608 b- defN 18-Dec-21 13:59 easy_workflow_manager-0.0.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2644 b- defN 18-Dec-21 13:59 easy_workflow_manager-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 18-Dec-21 13:59 easy_workflow_manager-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx      621 b- defN 18-Dec-21 13:59 easy_workflow_manager-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 18-Dec-21 13:59 easy_workflow_manager-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1756 b- defN 18-Dec-21 13:59 easy_workflow_manager-0.0.8.dist-info/RECORD
-18 files, 41608 bytes uncompressed, 11949 bytes compressed:  71.3%
+-rw-r--r--  2.0 unx      541 b- defN 18-Dec-21 14:12 easy_workflow_manager/scripts/update_branch.py
+-rwxrwxr-x  2.0 unx      608 b- defN 18-Dec-21 14:33 easy_workflow_manager-0.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2644 b- defN 18-Dec-21 14:33 easy_workflow_manager-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 18-Dec-21 14:33 easy_workflow_manager-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx      690 b- defN 18-Dec-21 14:33 easy_workflow_manager-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 18-Dec-21 14:33 easy_workflow_manager-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1858 b- defN 18-Dec-21 14:33 easy_workflow_manager-0.0.9.dist-info/RECORD
+19 files, 42320 bytes uncompressed, 12325 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -30,26 +30,29 @@
 
 Filename: easy_workflow_manager/scripts/show_repo_info.py
 Comment: 
 
 Filename: easy_workflow_manager/scripts/tag_release.py
 Comment: 
 
-Filename: easy_workflow_manager-0.0.8.dist-info/LICENSE.txt
+Filename: easy_workflow_manager/scripts/update_branch.py
 Comment: 
 
-Filename: easy_workflow_manager-0.0.8.dist-info/METADATA
+Filename: easy_workflow_manager-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: easy_workflow_manager-0.0.8.dist-info/WHEEL
+Filename: easy_workflow_manager-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: easy_workflow_manager-0.0.8.dist-info/entry_points.txt
+Filename: easy_workflow_manager-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: easy_workflow_manager-0.0.8.dist-info/top_level.txt
+Filename: easy_workflow_manager-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: easy_workflow_manager-0.0.8.dist-info/RECORD
+Filename: easy_workflow_manager-0.0.9.dist-info/top_level.txt
+Comment: 
+
+Filename: easy_workflow_manager-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `easy_workflow_manager-0.0.8.dist-info/LICENSE.txt` & `easy_workflow_manager-0.0.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `easy_workflow_manager-0.0.8.dist-info/METADATA` & `easy_workflow_manager-0.0.9.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: easy-workflow-manager
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools to support a straightforward branch/qa/merge/release process
 Home-page: https://github.com/kenjyco/easy-workflow-manager
 Author: Ken
 Author-email: kenjyco@gmail.com
 License: MIT
-Download-URL: https://github.com/kenjyco/easy-workflow-manager/tarball/v0.0.8
+Download-URL: https://github.com/kenjyco/easy-workflow-manager/tarball/v0.0.9
 Keywords: git,workflow,helper,branch,merge,qa,deploy
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
```

## Comparing `easy_workflow_manager-0.0.8.dist-info/entry_points.txt` & `easy_workflow_manager-0.0.9.dist-info/entry_points.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,8 +4,9 @@
 ewm-deploy-to-qa = easy_workflow_manager.scripts.deploy_to_qa:main
 ewm-new-branch-from-source = easy_workflow_manager.scripts.new_branch_from_source:main
 ewm-qa-to-source = easy_workflow_manager.scripts.qa_to_source:main
 ewm-repo-info = easy_workflow_manager.scripts.show_repo_info:main
 ewm-show-branches = easy_workflow_manager.scripts.show_branches:main
 ewm-show-qa = easy_workflow_manager.scripts.show_qa:main
 ewm-tag-release = easy_workflow_manager.scripts.tag_release:main
+ewm-update-branch = easy_workflow_manager.scripts.update_branch:main
```

## Comparing `easy_workflow_manager-0.0.8.dist-info/RECORD` & `easy_workflow_manager-0.0.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -6,13 +6,14 @@
 easy_workflow_manager/scripts/deploy_to_qa.py,sha256=znX-HvlkZmK-Nc_odG7ibbN88xApsmX7QoO8I-kSjcg,561
 easy_workflow_manager/scripts/new_branch_from_source.py,sha256=4Oqb5i4TqX-oEENp1wYlR1akLqxvywGHSTyh52KMcLM,370
 easy_workflow_manager/scripts/qa_to_source.py,sha256=drGa6QVt-xn_IjCWjgxki-NRTawgSnlXadOoIZ9LTC4,473
 easy_workflow_manager/scripts/show_branches.py,sha256=OyEbqtgFr9C6inWe8gSoCcoSFrCAOuCBtarZIupL0co,709
 easy_workflow_manager/scripts/show_qa.py,sha256=wK7PWgzZ89zd7YUbnmDJObcGQsRrxLo27H71YwAGOqQ,436
 easy_workflow_manager/scripts/show_repo_info.py,sha256=A10C7E70f2FJ_8CcVRz2on5wSirtFr5oYUR1VCF2K28,180
 easy_workflow_manager/scripts/tag_release.py,sha256=YrIzEAXU9Y4AQ7FEXgaV8hXKdVZHipLmjjR5cigDQRE,323
-easy_workflow_manager-0.0.8.dist-info/LICENSE.txt,sha256=TEfWL0DMfS6p49n4AeLR5CfiihVzu4DFBXxlJKX6e10,608
-easy_workflow_manager-0.0.8.dist-info/METADATA,sha256=ZO97xIZE7ANmkiMX05bEQR6APP16Xv9UnVm8Q4nWlHU,2644
-easy_workflow_manager-0.0.8.dist-info/WHEEL,sha256=_NOXIqFgOaYmlm9RJLPQZ13BJuEIrp5jx5ptRD5uh3Y,92
-easy_workflow_manager-0.0.8.dist-info/entry_points.txt,sha256=wlhKokR4xFy2ukDVEob5WrUA52Gymq1BwX4gcHaM76g,621
-easy_workflow_manager-0.0.8.dist-info/top_level.txt,sha256=akRtjdT2XQouCTfMNFjmxXeRAeE5gEUFalxPLVZjcGA,22
-easy_workflow_manager-0.0.8.dist-info/RECORD,,
+easy_workflow_manager/scripts/update_branch.py,sha256=eqwZDzYNkSLb9BR3bdA67WlJQoDnjGxbbLJWar1ACj4,541
+easy_workflow_manager-0.0.9.dist-info/LICENSE.txt,sha256=TEfWL0DMfS6p49n4AeLR5CfiihVzu4DFBXxlJKX6e10,608
+easy_workflow_manager-0.0.9.dist-info/METADATA,sha256=OrYXBhrHUomliqhe1IqiJMJLG1kz5gpyXyHPOQ-Z_QE,2644
+easy_workflow_manager-0.0.9.dist-info/WHEEL,sha256=_NOXIqFgOaYmlm9RJLPQZ13BJuEIrp5jx5ptRD5uh3Y,92
+easy_workflow_manager-0.0.9.dist-info/entry_points.txt,sha256=PW7zTSY6F93INMeSR_xcqZG1oK-IIP-uK-etg74kOdc,690
+easy_workflow_manager-0.0.9.dist-info/top_level.txt,sha256=akRtjdT2XQouCTfMNFjmxXeRAeE5gEUFalxPLVZjcGA,22
+easy_workflow_manager-0.0.9.dist-info/RECORD,,
```

