# Comparing `tmp/besecure_developer_toolkit-0.0.6.tar.gz` & `tmp/besecure_developer_toolkit-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besecure_developer_toolkit-0.0.6.tar", max compression
+gzip compressed data, was "besecure_developer_toolkit-0.0.7.tar", max compression
```

## Comparing `besecure_developer_toolkit-0.0.6.tar` & `besecure_developer_toolkit-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/LICENSE
--rw-r--r--   0        0        0     3233 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/README.md
--rw-r--r--   0        0        0      325 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/__init__.py
--rw-r--r--   0        0        0      172 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/__main__.py
--rw-r--r--   0        0        0     9838 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/cli.py
--rw-r--r--   0        0        0        0 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/config.py
--rw-r--r--   0        0        0     9392 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/create_ossp_master.py
--rw-r--r--   0        0        0     5720 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/create_version_data.py
--rw-r--r--   0        0        0     9349 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/generate_report.py
--rw-r--r--   0        0        0     1587 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_assessment.py
--rw-r--r--   0        0        0     5239 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/License_compliance.py
--rw-r--r--   0        0        0      906 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/New_line_char.py
--rw-r--r--   0        0        0     3185 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Objective.py
--rw-r--r--   0        0        0     4452 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Sbom_report.py
--rw-r--r--   0        0        0     5295 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Scorecard_report.py
--rw-r--r--   0        0        0     7094 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Static_code_analysis.py
--rw-r--r--   0        0        0    10013 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/validate_report_file.py
--rw-r--r--   0        0        0     4629 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/validate_version_file.py
--rw-r--r--   0        0        0      668 2023-07-07 11:53:04.881712 besecure_developer_toolkit-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3929 1970-01-01 00:00:00.000000 besecure_developer_toolkit-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3233 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/README.md
+-rw-r--r--   0        0        0      325 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/__init__.py
+-rw-r--r--   0        0        0      172 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/__main__.py
+-rw-r--r--   0        0        0     9838 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/cli.py
+-rw-r--r--   0        0        0        0 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/config.py
+-rw-r--r--   0        0        0     9392 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/src/create_ossp_master.py
+-rw-r--r--   0        0        0     5720 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/src/create_version_data.py
+-rw-r--r--   0        0        0     9349 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/src/generate_report.py
+-rw-r--r--   0        0        0     1587 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/src/risk_assessment.py
+-rw-r--r--   0        0        0     5239 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/src/risk_summary/License_compliance.py
+-rw-r--r--   0        0        0      906 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/src/risk_summary/New_line_char.py
+-rw-r--r--   0        0        0     3185 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/src/risk_summary/Objective.py
+-rw-r--r--   0        0        0     4452 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/src/risk_summary/Sbom_report.py
+-rw-r--r--   0        0        0     5295 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/src/risk_summary/Scorecard_report.py
+-rw-r--r--   0        0        0     7094 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/src/risk_summary/Static_code_analysis.py
+-rw-r--r--   0        0        0    10013 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/src/validate_report_file.py
+-rw-r--r--   0        0        0     4629 2023-07-10 05:07:11.553221 besecure_developer_toolkit-0.0.7/bes_dev_kit/src/validate_version_file.py
+-rw-r--r--   0        0        0      653 2023-07-10 05:07:11.561221 besecure_developer_toolkit-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3929 1970-01-01 00:00:00.000000 besecure_developer_toolkit-0.0.7/PKG-INFO
```

### Comparing `besecure_developer_toolkit-0.0.6/LICENSE` & `besecure_developer_toolkit-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.6/README.md` & `besecure_developer_toolkit-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.6/bes_dev_kit/cli.py` & `besecure_developer_toolkit-0.0.7/bes_dev_kit/cli.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/create_ossp_master.py` & `besecure_developer_toolkit-0.0.7/bes_dev_kit/src/create_ossp_master.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/create_version_data.py` & `besecure_developer_toolkit-0.0.7/bes_dev_kit/src/create_version_data.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/generate_report.py` & `besecure_developer_toolkit-0.0.7/bes_dev_kit/src/generate_report.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_assessment.py` & `besecure_developer_toolkit-0.0.7/bes_dev_kit/src/risk_assessment.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/License_compliance.py` & `besecure_developer_toolkit-0.0.7/bes_dev_kit/src/risk_summary/License_compliance.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/New_line_char.py` & `besecure_developer_toolkit-0.0.7/bes_dev_kit/src/risk_summary/New_line_char.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Objective.py` & `besecure_developer_toolkit-0.0.7/bes_dev_kit/src/risk_summary/Objective.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Sbom_report.py` & `besecure_developer_toolkit-0.0.7/bes_dev_kit/src/risk_summary/Sbom_report.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Scorecard_report.py` & `besecure_developer_toolkit-0.0.7/bes_dev_kit/src/risk_summary/Scorecard_report.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Static_code_analysis.py` & `besecure_developer_toolkit-0.0.7/bes_dev_kit/src/risk_summary/Static_code_analysis.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/validate_report_file.py` & `besecure_developer_toolkit-0.0.7/bes_dev_kit/src/validate_report_file.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/validate_version_file.py` & `besecure_developer_toolkit-0.0.7/bes_dev_kit/src/validate_version_file.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.6/pyproject.toml` & `besecure_developer_toolkit-0.0.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "besecure-developer-toolkit"
-version = "0.0.6"
+version = "0.0.7"
 description = "cli tool for generating metadata and assessment report for [BeSLighthouse](https://github.com/Be-Secure/BeSLighthouse)."
 authors = ["asa1997 <arunsureshampadath@gmail.com>"]
 readme = "README.md"
 packages = [{include = "bes_dev_kit"}]
 
 [tool.poetry.scripts]
-besecure-developer-toolkit = "bes_dev_kit.__main__:cli.app"
+bes-dev-kit = "bes_dev_kit.__main__:cli.app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.9.0"}
 pytest = "^7.3.0"
 requests = "^2.29.0"
 reportlab = "^3.6.8"
```

### Comparing `besecure_developer_toolkit-0.0.6/PKG-INFO` & `besecure_developer_toolkit-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besecure-developer-toolkit
-Version: 0.0.6
+Version: 0.0.7
 Summary: cli tool for generating metadata and assessment report for [BeSLighthouse](https://github.com/Be-Secure/BeSLighthouse).
 Author: asa1997
 Author-email: arunsureshampadath@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

