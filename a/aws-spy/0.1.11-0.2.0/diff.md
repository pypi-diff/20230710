# Comparing `tmp/aws_spy-0.1.11.tar.gz` & `tmp/aws_spy-0.2.0.tar.gz`

## Comparing `aws_spy-0.1.11.tar` & `aws_spy-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 aws_spy-0.1.11/.pre-commit-config.yaml
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 aws_spy-0.1.11/Makefile
--rw-r--r--   0        0        0    53436 2020-02-02 00:00:00.000000 aws_spy-0.1.11/pdm.lock
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aws_spy-0.1.11/.vscode/settings.json
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/__init__.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/dependencies.py
--rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/main.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/responses.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/test.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/core/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/core/encoders.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/core/event_utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/core/exceptions.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/core/logging.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/core/params.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/core/params_alias.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/core/responses.py
--rw-r--r--   0        0        0     8610 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/core/schemas.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/core/schemas_utils.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/core/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/helpers/__init__.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/helpers/cli.py
--rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/helpers/documentation.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/helpers/exceptions.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/helpers/utils.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 aws_spy-0.1.11/aws_spy/layer/spy-layer.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.1.11/tests/__init__.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 aws_spy-0.1.11/tests/conftest.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 aws_spy-0.1.11/tests/test_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.1.11/tests/integration/__init__.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 aws_spy-0.1.11/tests/integration/test_params.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 aws_spy-0.1.11/tests/integration/test_request_body.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aws_spy-0.1.11/tests/integration/test_response_class.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.1.11/tests/integration/test_test_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.1.11/tests/unit/__init__.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aws_spy-0.1.11/tests/unit/test_encoders.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 aws_spy-0.1.11/tests/unit/test_event_utils.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 aws_spy-0.1.11/tests/unit/test_responses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.1.11/tests/unit/test_schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.1.11/tests/unit/test_utils.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 aws_spy-0.1.11/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aws_spy-0.1.11/LICENSE
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 aws_spy-0.1.11/README.md
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 aws_spy-0.1.11/pyproject.toml
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aws_spy-0.1.11/PKG-INFO
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 aws_spy-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aws_spy-0.2.0/Makefile
+-rw-r--r--   0        0        0    72078 2020-02-02 00:00:00.000000 aws_spy-0.2.0/pdm.lock
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aws_spy-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/dependencies.py
+-rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/main.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/responses.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/test.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/core/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/core/encoders.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/core/event_utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/core/exceptions.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/core/logging.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/core/params.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/core/params_alias.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/core/responses.py
+-rw-r--r--   0        0        0     8825 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/core/schemas.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/core/schemas_utils.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/core/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/helpers/__init__.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/helpers/cli.py
+-rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/helpers/documentation.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/helpers/exceptions.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/helpers/utils.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 aws_spy-0.2.0/aws_spy/layer/spy-layer.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 aws_spy-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 aws_spy-0.2.0/tests/test_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 aws_spy-0.2.0/tests/integration/test_params.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 aws_spy-0.2.0/tests/integration/test_request_body.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aws_spy-0.2.0/tests/integration/test_response_class.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.0/tests/integration/test_test_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aws_spy-0.2.0/tests/unit/test_encoders.py
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 aws_spy-0.2.0/tests/unit/test_event_utils.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 aws_spy-0.2.0/tests/unit/test_responses.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.0/tests/unit/test_schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.0/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 aws_spy-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aws_spy-0.2.0/LICENSE
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 aws_spy-0.2.0/README.md
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 aws_spy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aws_spy-0.2.0/PKG-INFO
```

### Comparing `aws_spy-0.1.11/.pre-commit-config.yaml` & `aws_spy-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aws_spy-0.1.11/pdm.lock` & `aws_spy-0.2.0/pdm.lock`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # This file is @generated by PDM.
 # It is not intended for manual editing.
 
 [[package]]
+name = "annotated-types"
+version = "0.5.0"
+requires_python = ">=3.7"
+summary = "Reusable constraint types to use with typing.Annotated"
+
+[[package]]
 name = "black"
 version = "23.3.0"
 requires_python = ">=3.7"
 summary = "The uncompromising code formatter."
 dependencies = [
     "click>=8.0.0",
     "mypy-extensions>=0.4.3",
@@ -107,19 +113,30 @@
 name = "pluggy"
 version = "1.2.0"
 requires_python = ">=3.7"
 summary = "plugin and hook calling mechanisms for python"
 
 [[package]]
 name = "pydantic"
-version = "1.10.11"
+version = "2.0.2"
 requires_python = ">=3.7"
-summary = "Data validation and settings management using python type hints"
+summary = "Data validation using Python type hints"
 dependencies = [
-    "typing-extensions>=4.2.0",
+    "annotated-types>=0.4.0",
+    "pydantic-core==2.1.2",
+    "typing-extensions>=4.6.1",
+]
+
+[[package]]
+name = "pydantic-core"
+version = "2.1.2"
+requires_python = ">=3.7"
+summary = ""
+dependencies = [
+    "typing-extensions!=4.7.0,>=4.6.0",
 ]
 
 [[package]]
 name = "pytest"
 version = "7.4.0"
 requires_python = ">=3.7"
 summary = "pytest: simple powerful testing with Python"
@@ -155,17 +172,21 @@
 requires_python = ">=3.7"
 summary = "Backported and Experimental Type Hints for Python 3.7+"
 
 [metadata]
 lock_version = "4.2"
 cross_platform = true
 groups = ["default", "linting", "mypy", "testing"]
-content_hash = "sha256:1ada1277c5f80f1cb84f6e55980898866a5fe9364e4f26fe59b20958879bb4f4"
+content_hash = "sha256:5eae3a0b29043c7c85f91e37b80013d817dc62a97d6fe29257c5c288a58c8653"
 
 [metadata.files]
+"annotated-types 0.5.0" = [
+    {url = "https://files.pythonhosted.org/packages/42/97/41ccb6acac36fdd13592a686a21b311418f786f519e5794b957afbcea938/annotated_types-0.5.0.tar.gz", hash = "sha256:47cdc3490d9ac1506ce92c7aaa76c579dc3509ff11e098fc867e5130ab7be802"},
+    {url = "https://files.pythonhosted.org/packages/d8/f0/a2ee543a96cc624c35a9086f39b1ed2aa403c6d355dfe47a11ee5c64a164/annotated_types-0.5.0-py3-none-any.whl", hash = "sha256:58da39888f92c276ad970249761ebea80ba544b77acddaa1a4d6cf78287d45fd"},
+]
 "black 23.3.0" = [
     {url = "https://files.pythonhosted.org/packages/06/1e/273d610249f0335afb1ddb03664a03223f4826e3d1a95170a0142cb19fb4/black-23.3.0-cp39-cp39-win_amd64.whl", hash = "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb"},
     {url = "https://files.pythonhosted.org/packages/12/4b/99c71d1cf1353edd5aff2700b8960f92e9b805c9dab72639b67dbb449d3a/black-23.3.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961"},
     {url = "https://files.pythonhosted.org/packages/13/0a/ed8b66c299e896780e4528eed4018f5b084da3b9ba4ee48328550567d866/black-23.3.0-cp38-cp38-macosx_10_16_x86_64.whl", hash = "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5"},
     {url = "https://files.pythonhosted.org/packages/13/25/cfa06788d0a936f2445af88f13604b5bcd5c9d050db618c718e6ebe66f74/black-23.3.0-cp39-cp39-macosx_10_16_arm64.whl", hash = "sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30"},
     {url = "https://files.pythonhosted.org/packages/21/14/d5a2bec5fb15f9118baab7123d344646fac0b1c6939d51c2b05259cd2d9c/black-23.3.0-cp38-cp38-macosx_10_16_universal2.whl", hash = "sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331"},
     {url = "https://files.pythonhosted.org/packages/24/eb/2d2d2c27cb64cfd073896f62a952a802cd83cf943a692a2f278525b57ca9/black-23.3.0-cp37-cp37m-macosx_10_16_x86_64.whl", hash = "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b"},
@@ -315,51 +336,120 @@
     {url = "https://files.pythonhosted.org/packages/92/38/3dd18a282991c004851ea1f0953105a186cfc691eee2792778ac2ca060f8/platformdirs-3.8.1.tar.gz", hash = "sha256:f87ca4fcff7d2b0f81c6a748a77973d7af0f4d526f98f308477c3c436c74d528"},
     {url = "https://files.pythonhosted.org/packages/9e/d8/563a9fc17153c588c8c2042d2f0f84a89057cdb1c30270f589c88b42d62c/platformdirs-3.8.1-py3-none-any.whl", hash = "sha256:cec7b889196b9144d088e4c57d9ceef7374f6c39694ad1577a0aab50d27ea28c"},
 ]
 "pluggy 1.2.0" = [
     {url = "https://files.pythonhosted.org/packages/51/32/4a79112b8b87b21450b066e102d6608907f4c885ed7b04c3fdb085d4d6ae/pluggy-1.2.0-py3-none-any.whl", hash = "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849"},
     {url = "https://files.pythonhosted.org/packages/8a/42/8f2833655a29c4e9cb52ee8a2be04ceac61bcff4a680fb338cbd3d1e322d/pluggy-1.2.0.tar.gz", hash = "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"},
 ]
-"pydantic 1.10.11" = [
-    {url = "https://files.pythonhosted.org/packages/04/70/8314870d16db3984417dc74404eb6518a8ae6324960da56505047accf6c3/pydantic-1.10.11-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:e6cbfbd010b14c8a905a7b10f9fe090068d1744d46f9e0c021db28daeb8b6de1"},
-    {url = "https://files.pythonhosted.org/packages/05/2c/09a35e6c16e206c80906ce93c0dd1e86d8b9738ea05eb82fe38c8f0cfab1/pydantic-1.10.11-cp310-cp310-win_amd64.whl", hash = "sha256:c3339a46bbe6013ef7bdd2844679bfe500347ac5742cd4019a88312aa58a9847"},
-    {url = "https://files.pythonhosted.org/packages/11/54/a010e20824e6bfe04902830f92923997e8000d64d14099999edee9076924/pydantic-1.10.11-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:41e0bb6efe86281623abbeeb0be64eab740c865388ee934cd3e6a358784aca6e"},
-    {url = "https://files.pythonhosted.org/packages/22/aa/24ef442d21b1ddafb52fae1e50ebe76cfaf36cb0c58a046fa6eb1d87310d/pydantic-1.10.11-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:469adf96c8e2c2bbfa655fc7735a2a82f4c543d9fee97bd113a7fb509bf5e622"},
-    {url = "https://files.pythonhosted.org/packages/3c/c0/57fb46d928d8f76736d99d1d2a3c00483e0f4029cfac6cd57584a3f7379b/pydantic-1.10.11-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:bc64eab9b19cd794a380179ac0e6752335e9555d214cfcb755820333c0784cb3"},
-    {url = "https://files.pythonhosted.org/packages/45/7f/ba7118bbc361bbf10e51f3b90a2072c26c29a20491ab7a31b30ee499e8ab/pydantic-1.10.11-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:ef55392ec4bb5721f4ded1096241e4b7151ba6d50a50a80a2526c854f42e6a2f"},
-    {url = "https://files.pythonhosted.org/packages/46/44/2390ef51d3fc48b4abb7d8928feaa9d43ff66df2c278476862c7754775d4/pydantic-1.10.11-cp37-cp37m-win_amd64.whl", hash = "sha256:7522a7666157aa22b812ce14c827574ddccc94f361237ca6ea8bb0d5c38f1629"},
-    {url = "https://files.pythonhosted.org/packages/4a/48/9dd66a938b0c5bb439ade89f3aac37a580736a8acf2da2c3e14ecdcd34f0/pydantic-1.10.11-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:e297897eb4bebde985f72a46a7552a7556a3dd11e7f76acda0c1093e3dbcf216"},
-    {url = "https://files.pythonhosted.org/packages/4c/4a/3865d5293f04cff244bfcaeb1b14b651ca3bed8ba7dd61cf74d9127a77e9/pydantic-1.10.11-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:373c0840f5c2b5b1ccadd9286782852b901055998136287828731868027a724f"},
-    {url = "https://files.pythonhosted.org/packages/4e/d7/04c964cda3b5e2c05d40d89fffa4449512c757476c9dd6aee9154a2e2603/pydantic-1.10.11-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fe429898f2c9dd209bd0632a606bddc06f8bce081bbd03d1c775a45886e2c1cb"},
-    {url = "https://files.pythonhosted.org/packages/63/cf/023a359e3c86a909494d6729e9d35304449de8231a2d8b3132bc93fb5b0a/pydantic-1.10.11-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:8dc77064471780262b6a68fe67e013298d130414d5aaf9b562c33987dbd2cf4f"},
-    {url = "https://files.pythonhosted.org/packages/65/d3/8ea06a592f4c218d3079ddb6d267015e6635c11ea4b282c2f5a9b62ca60b/pydantic-1.10.11-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:abade85268cc92dff86d6effcd917893130f0ff516f3d637f50dadc22ae93999"},
-    {url = "https://files.pythonhosted.org/packages/6a/19/af6ac6f22f9a2a3866fc5a726dca0b7d524e1660821388dc99d56764e6df/pydantic-1.10.11-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:331c031ba1554b974c98679bd0780d89670d6fd6f53f5d70b10bdc9addee1713"},
-    {url = "https://files.pythonhosted.org/packages/79/3e/6b4d0fb2174beceac9a991ba8e67158b45c35faca9ea4545ae32d47096cd/pydantic-1.10.11-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:a6c098d4ab5e2d5b3984d3cb2527e2d6099d3de85630c8934efcfdc348a9760e"},
-    {url = "https://files.pythonhosted.org/packages/87/18/76af036e978c00d4b1525eeaa84e67a8ea93429ceb1adaa67491af44e214/pydantic-1.10.11-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:8268a735a14c308923e8958363e3a3404f6834bb98c11f5ab43251a4e410170c"},
-    {url = "https://files.pythonhosted.org/packages/90/6c/ef2c34321f035197621171d5cf243aedc43db69148b07308d95ca27bc036/pydantic-1.10.11-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:ff44c5e89315b15ff1f7fdaf9853770b810936d6b01a7bcecaa227d2f8fe444f"},
-    {url = "https://files.pythonhosted.org/packages/93/4c/c1d4530819924e77285a32768629fab5d40bbbbdba2f78a1b1fc0649525a/pydantic-1.10.11-cp311-cp311-win_amd64.whl", hash = "sha256:4400015f15c9b464c9db2d5d951b6a780102cfa5870f2c036d37c23b56f7fc1b"},
-    {url = "https://files.pythonhosted.org/packages/93/63/c2b91f7482bf8e5b7166dba6558287d906587f269158b8fad1146031fdc3/pydantic-1.10.11-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:a451ccab49971af043ec4e0d207cbc8cbe53dbf148ef9f19599024076fe9c25b"},
-    {url = "https://files.pythonhosted.org/packages/96/84/e6d9843d3d865efa54f7080183cbbe8f337a08c469b44a6adf064e45005c/pydantic-1.10.11-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:e9baf78b31da2dc3d3f346ef18e58ec5f12f5aaa17ac517e2ffd026a92a87588"},
-    {url = "https://files.pythonhosted.org/packages/af/c3/216d527637fb6de1d2c08f870a094f239f8e5a127b9693835cedc29616f7/pydantic-1.10.11-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5b02d24f7b2b365fed586ed73582c20f353a4c50e4be9ba2c57ab96f8091ddae"},
-    {url = "https://files.pythonhosted.org/packages/b6/6a/ef5f54d0acdc34dc05d8e72bdf1673d67e0e05b6b7743ece209c76e1f45c/pydantic-1.10.11-cp38-cp38-win_amd64.whl", hash = "sha256:265a60da42f9f27e0b1014eab8acd3e53bd0bad5c5b4884e98a55f8f596b2c19"},
-    {url = "https://files.pythonhosted.org/packages/b6/8e/7dd215f91528487535e7aa048e4092c20ecd0168df958e58809e2235cece/pydantic-1.10.11-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:16928fdc9cb273c6af00d9d5045434c39afba5f42325fb990add2c241402d151"},
-    {url = "https://files.pythonhosted.org/packages/bf/43/3fcc2d7fd6f1352677a9ea47123004da5f68a903fae48fab40f03ca2e0b1/pydantic-1.10.11-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0588788a9a85f3e5e9ebca14211a496409cb3deca5b6971ff37c556d581854e7"},
-    {url = "https://files.pythonhosted.org/packages/ca/79/8b33ca15336599bad10bd15820182fbf4045e7a2f677b7fbf89794785f60/pydantic-1.10.11-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:d7781f1d13b19700b7949c5a639c764a077cbbdd4322ed505b449d3ca8edcb36"},
-    {url = "https://files.pythonhosted.org/packages/ce/bd/beabbb503f06ebe9140752a4cd80a6d3fd8895764a5e34083d9c97ec5f68/pydantic-1.10.11-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e9738b0f2e6c70f44ee0de53f2089d6002b10c33264abee07bdb5c7f03038303"},
-    {url = "https://files.pythonhosted.org/packages/cf/01/e8a380dc6e92a76113f034c58c9ffdbd115753e9b944ddf5d2dbe862f248/pydantic-1.10.11.tar.gz", hash = "sha256:f66d479cf7eb331372c470614be6511eae96f1f120344c25f3f9bb59fb1b5528"},
-    {url = "https://files.pythonhosted.org/packages/d0/30/b295a270bef59eda75d5862bba8a6a27fed9a2b91000cccd5dfddb91ee1c/pydantic-1.10.11-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:d185819a7a059550ecb85d5134e7d40f2565f3dd94cfd870132c5f91a89cf58c"},
-    {url = "https://files.pythonhosted.org/packages/d0/ab/df82ca386c559accacaaf082dc5d178b9257ace0d4f83b09f4a2066a8a61/pydantic-1.10.11-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:2417de68290434461a266271fc57274a138510dca19982336639484c73a07af6"},
-    {url = "https://files.pythonhosted.org/packages/d3/b4/44df92e63c99834a07e2ae0cb7c9c4464b0e3a0539d25f68fc9811e9b12e/pydantic-1.10.11-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3f34739a89260dfa420aa3cbd069fbcc794b25bbe5c0a214f8fb29e363484b66"},
-    {url = "https://files.pythonhosted.org/packages/da/6f/cbd0b6d75c5c35234fdf6feb0fcb26812d87be9b2eab7b2d1596f30f52c0/pydantic-1.10.11-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:44e51ba599c3ef227e168424e220cd3e544288c57829520dc90ea9cb190c3248"},
-    {url = "https://files.pythonhosted.org/packages/dc/f0/604245a9bcaa982c86caeaa98fdeabddc1ddea097ae77753a6f9d6b08e12/pydantic-1.10.11-py3-none-any.whl", hash = "sha256:008c5e266c8aada206d0627a011504e14268a62091450210eda7c07fabe6963e"},
-    {url = "https://files.pythonhosted.org/packages/e6/c7/99b3678f019a1b90e3242a8b7006b5181f6739d1791caaaebe83f1aab5a9/pydantic-1.10.11-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:192c608ad002a748e4a0bed2ddbcd98f9b56df50a7c24d9a931a8c5dd053bd3d"},
-    {url = "https://files.pythonhosted.org/packages/ed/a9/9f6fa825214510f79ce3fae718db66c9c55cba8d087e2e4400e4a634173a/pydantic-1.10.11-cp39-cp39-win_amd64.whl", hash = "sha256:1954f8778489a04b245a1e7b8b22a9d3ea8ef49337285693cf6959e4b757535e"},
-    {url = "https://files.pythonhosted.org/packages/f1/79/e28edde4bca34e08958d02f14e45805c2b18110aa720cdb900022fc210f7/pydantic-1.10.11-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:174899023337b9fc685ac8adaa7b047050616136ccd30e9070627c1aaab53a13"},
-    {url = "https://files.pythonhosted.org/packages/f9/ba/19c03d48e76940b4970e9b9ac626d104e69f9ee2d67ec778f1142ce2f559/pydantic-1.10.11-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:08a6c32e1c3809fbc49debb96bf833164f3438b3696abf0fbeceb417d123e6eb"},
-    {url = "https://files.pythonhosted.org/packages/fe/1b/266ef0137e71d3405762521db8c0a4a07d5883245b7abac9e800fef4729b/pydantic-1.10.11-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:787cf23e5a0cde753f2eabac1b2e73ae3844eb873fd1f5bdbff3048d8dbb7604"},
+"pydantic 2.0.2" = [
+    {url = "https://files.pythonhosted.org/packages/3c/39/e526f3ca06e062e0ad773555f5349ff5d9ed50bfa62c45df8e74fff9ff14/pydantic-2.0.2.tar.gz", hash = "sha256:b802f5245b8576315fe619e5989fd083448fa1258638ef9dac301ca60878396d"},
+    {url = "https://files.pythonhosted.org/packages/79/bf/ce11dc07156bdbf12009c560ba5fdb308522f77e7484b64f4aff682d93cf/pydantic-2.0.2-py3-none-any.whl", hash = "sha256:f5581e0c79b2ec2fa25a9d30d766629811cdda022107fa73d022ab5578873ae3"},
+]
+"pydantic-core 2.1.2" = [
+    {url = "https://files.pythonhosted.org/packages/01/77/53917e943ab939802f0f88d2e0c03f9bee4c167979af3ce2c49f1847073a/pydantic_core-2.1.2-cp312-cp312-manylinux_2_24_ppc64le.whl", hash = "sha256:dc737506b4a0ba2922a2626fc6d620ce50a46aebd0fe2fbcad1b93bbdd8c7e78"},
+    {url = "https://files.pythonhosted.org/packages/02/f0/f27685a4d0b9596487f4cb552d791e7760e844ecf3f49c861db5534c7678/pydantic_core-2.1.2-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:68a2a767953c707d9575dcf14d8edee7930527ee0141a8bb612c22d1f1059f9a"},
+    {url = "https://files.pythonhosted.org/packages/03/cb/f89e2a31bd2a88eb35611ef42830cdeb87c8daa5e8b19dd76a48ef8d590d/pydantic_core-2.1.2-pp39-pypy39_pp73-macosx_10_7_x86_64.whl", hash = "sha256:aa54902fa51f7d921ba80923cf1c7ff3dce796a7903300bd8824deb90e357744"},
+    {url = "https://files.pythonhosted.org/packages/05/94/14fd8f4f94b8e1a97676746c2fbfb9954d3ca98bb2a0ba1842b90e55daf5/pydantic_core-2.1.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7684b5fb906b37e940c5df3f57118f32e033af5e4770e5ae2ae56fbd2fe1a30a"},
+    {url = "https://files.pythonhosted.org/packages/08/9b/e728677175f911b3af5f171b060a6530b1ca652903f9f236756f93e5d889/pydantic_core-2.1.2-pp38-pypy38_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:0855cf8b760fb40f97f0226cb527c8a94a2ab9d8179628beae20d6939aaeacb0"},
+    {url = "https://files.pythonhosted.org/packages/0b/f2/f18a3d48981957f2aa6ab336135ce73a7db92271b6ddab1b2b10554c96e6/pydantic_core-2.1.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:cb854ec52e6e2e05b83d647695f4d913452fdd45a3dfa8233d7dab5967b3908f"},
+    {url = "https://files.pythonhosted.org/packages/0e/66/bfe9935eb0ec55d44a02fde2e6de3a801d8af023a14ac826b3a04c19a829/pydantic_core-2.1.2-cp38-cp38-manylinux_2_24_armv7l.whl", hash = "sha256:e17056390068afd4583d88dcf4d4495764e4e2c7d756464468e0d21abcb8931e"},
+    {url = "https://files.pythonhosted.org/packages/10/55/307805ec7d0917e9e986807d6e46f9ea510596378c929ee973a8a65b476c/pydantic_core-2.1.2-pp37-pypy37_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:f5de2d4167fd4bc5ad205fb7297e25867b8e335ca08d64ed7a561d2955a2c32d"},
+    {url = "https://files.pythonhosted.org/packages/16/ad/f3e582f18b33be4064a229af21f86e3f97344f6c5bb151820168d1ef9ad6/pydantic_core-2.1.2-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:817681d111cb65f07d46496eafec815f48e1aff37713b73135a0a9eb4d3610ab"},
+    {url = "https://files.pythonhosted.org/packages/18/b7/15900b0ec1cf0d0c52ad42c52dca43b62e0ad8ce7d55aa30b049ee4758c5/pydantic_core-2.1.2-cp312-none-win32.whl", hash = "sha256:cd62f73830d4715bc643ae39de0bd4fb9c81d6d743530074da91e77a2cccfe67"},
+    {url = "https://files.pythonhosted.org/packages/1b/86/55872c1c449357531d3ea71d3f7bc672e62edc89a17ddb3e35f285ae7aac/pydantic_core-2.1.2-cp39-none-win32.whl", hash = "sha256:6bf00f56a4468f5b03dadb672a5f1d24aea303d4ccffe8a0f548c9e36017edd3"},
+    {url = "https://files.pythonhosted.org/packages/1d/e6/d344f65bc117cf40faa6e40f9c2d6607951515ee5c97139a87fa1ab05ecc/pydantic_core-2.1.2-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:94d368af9e6563de6e7170a74710a2cbace7a1e9c8e507d9e3ac34c7065d7ae3"},
+    {url = "https://files.pythonhosted.org/packages/1d/e8/4b036ce2bab9a26293ff14c044c726ee74e889342e1421106d66b2f28252/pydantic_core-2.1.2-cp311-none-win_amd64.whl", hash = "sha256:ebf583f4d9b52abd15cc59e5f6eeca7e3e9741c6ea62d8711c00ac3acb067875"},
+    {url = "https://files.pythonhosted.org/packages/1f/1b/7879dcd099983b8a04d8cfc13cbcf2756384736381ea82651095c831d37d/pydantic_core-2.1.2-cp39-cp39-manylinux_2_24_ppc64le.whl", hash = "sha256:b74906e01c7fc938ac889588ef438de812989817095c3c4904721f647d64a4d1"},
+    {url = "https://files.pythonhosted.org/packages/21/e8/17e028d8f81219f4014ed7a2703ec0d90b2f4c439bd307323484a2f58669/pydantic_core-2.1.2-cp312-cp312-manylinux_2_24_s390x.whl", hash = "sha256:bb471ea8650796060afc99909d9b75da583d317e52f660faf64c45f70b3bf1e2"},
+    {url = "https://files.pythonhosted.org/packages/23/44/b15e08895bdc5e9ee7b1afdd1b543dd0a0bfd1af81523059a98232b98153/pydantic_core-2.1.2-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:804cf8f6a859620f8eb754c02f7770f61c3e9c519f8338c331d555b3d6976e3c"},
+    {url = "https://files.pythonhosted.org/packages/25/e8/20c7161daa0849603220443e47d81f77781090d5d02fff9272754b75f3c3/pydantic_core-2.1.2-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:a4ae46769d9a7138d58cd190441cac14ce954010a0081f28462ed916c8e55a4f"},
+    {url = "https://files.pythonhosted.org/packages/27/19/eb3fb40c32fc484ebc89e510cbd07335fa8b281da5fe5c8178d357483dd7/pydantic_core-2.1.2-cp37-cp37m-manylinux_2_24_s390x.whl", hash = "sha256:4663293a36a851a860b1299c50837914269fca127434911297dd39fea9667a01"},
+    {url = "https://files.pythonhosted.org/packages/27/8a/651cca4755894caadf6c081f0e4781dbc390411f7d787fea3c6b0db4d240/pydantic_core-2.1.2-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0681472245ef182554208a25d16884c84f1c5a69f14e6169b88932e5da739a1c"},
+    {url = "https://files.pythonhosted.org/packages/2b/24/a1fd45909761fdd99159cdde3d4e2e87707726f018a7421f06b11ec9c19b/pydantic_core-2.1.2-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:82e09f27edab289187dd924d4d93f2a35f21aa969699b2504aa643da7fbfeff9"},
+    {url = "https://files.pythonhosted.org/packages/32/ed/a7051647101c80e0978ecc3519c6e90b32cdefcbdbafa21b5325dfc2f304/pydantic_core-2.1.2-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:080a7af828388284a68ad7d3d3eac3bcfff6a580292849aff087e7d556ec42d4"},
+    {url = "https://files.pythonhosted.org/packages/3d/23/5482e5112329d60b9e3b1b2832405d937d4a5ff40d31ca159c2c640e6e0d/pydantic_core-2.1.2-pp37-pypy37_pp73-macosx_10_7_x86_64.whl", hash = "sha256:8eb4e2b71562375609c66a79f89acd4fe95c5cba23473d04952c8b14b6f908f5"},
+    {url = "https://files.pythonhosted.org/packages/3f/a0/ef28c4a6233cabd054ae11795af8a09f0d9a6a99352b20e0d2f5e8006428/pydantic_core-2.1.2-cp312-none-win_amd64.whl", hash = "sha256:51968887d6bd1eaa7fc7759701ea8ccb470c04654beaa8ede6835b0533f206a9"},
+    {url = "https://files.pythonhosted.org/packages/40/98/af05b98e7b81b1750f4445363ecc92c46dd144c208ded86c7ea37bdc13a9/pydantic_core-2.1.2-pp310-pypy310_pp73-macosx_10_7_x86_64.whl", hash = "sha256:047e782b9918f35ef534ced36f1fd2064f5581229b7a15e4d3177387a6b53134"},
+    {url = "https://files.pythonhosted.org/packages/40/fa/9b929c6f6db950ee67d61c106b85052609a4cf05ff11f78f3d4956639b45/pydantic_core-2.1.2-pp37-pypy37_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5056afea59651c4e47ec6dadbb77ccae4742c059a3d12bc1c0e393d189d2970d"},
+    {url = "https://files.pythonhosted.org/packages/41/73/fc0f94144f9a1268828d9147a3cc17ce08410f0f5bb74014fdf2e4cd775c/pydantic_core-2.1.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:1635a37137fafbc6ee0a8c879857e05b30b1aabaa927e653872b71f1501b1502"},
+    {url = "https://files.pythonhosted.org/packages/47/01/4c5cafda95fc9f4d2eec38b9a22b2498de5befdbb83c96a96191243255dd/pydantic_core-2.1.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:818f5cb1b209ab1295087c45717178f4bbbd2bd7eda421f7a119e7b9b736a3cb"},
+    {url = "https://files.pythonhosted.org/packages/47/2f/013a4176a16b34f072a3f4b5c5f87d068cdfb55db92a28ac7bae74a02a6d/pydantic_core-2.1.2-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:b1fad38db1744d27061df516e59c5025b09b0a50a337c04e6eebdbddc18951bc"},
+    {url = "https://files.pythonhosted.org/packages/4c/e1/d3e5c5da056bf2e33aeb9536cc318705dcd21900fec3e5c36e230cf9f1d9/pydantic_core-2.1.2-pp38-pypy38_pp73-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:7345b1741bf66a9d8ed0ec291c3eabd534444e139e1ea6db5742ac9fd3be2530"},
+    {url = "https://files.pythonhosted.org/packages/52/b9/2aed9a4dc4f865be11062cb3bc8213d24451512d3d3b152d3a5152d7edc2/pydantic_core-2.1.2-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:06ae67547251135a1b3f8dd465797b13146295a3866bc12ddd73f7512787bb7c"},
+    {url = "https://files.pythonhosted.org/packages/5b/e0/9a55b27e30151f8088a17c0ac1a43b70d4e81b1b538ed8104482ad68473b/pydantic_core-2.1.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:bad7029fb2251c1ac7d3acdd607e540d40d137a7d43a5e5acdcfdbd38db3fc0a"},
+    {url = "https://files.pythonhosted.org/packages/5d/a1/9e04723ccd479b654b762c902b302292b4958c0ffa392d347d402e43682f/pydantic_core-2.1.2-pp310-pypy310_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:ef71e73a81a4cd7e87c93e8ff0170140fd93ba33b0f61e83da3f55f6e0a84fb4"},
+    {url = "https://files.pythonhosted.org/packages/5e/7c/ec92937185491b9cd92009627d4dc3af51e7bbf4b1ec04e14000e3b92e9d/pydantic_core-2.1.2-pp38-pypy38_pp73-macosx_10_7_x86_64.whl", hash = "sha256:1a5c4475510d1a9cc1458a26cfc21442223e52ce9adb640775c38739315d03c7"},
+    {url = "https://files.pythonhosted.org/packages/5e/8b/fb9c24488d196f1a340b12c058b08a8c24790bb1501d5661b384759552a0/pydantic_core-2.1.2-cp311-cp311-macosx_10_7_x86_64.whl", hash = "sha256:76c9c55462740d728b344e3a087775846516c3fee31ec56e2075faa7cfcafcbf"},
+    {url = "https://files.pythonhosted.org/packages/5e/b5/dfd46e35f937564b3d57cd4282e3ca5462bbc03c3d5006294612f79ed4c2/pydantic_core-2.1.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:fc909f62325a631e1401dd07dfc386986dbcac15f98c9ff2145d930678a9d25a"},
+    {url = "https://files.pythonhosted.org/packages/61/2f/b81db8668fa1f0e069cf086be1983f22bb5faacfef9dc00ce47688390bb5/pydantic_core-2.1.2-cp310-cp310-macosx_10_7_x86_64.whl", hash = "sha256:b4815720c266e832b20e27a7a5f3772bb09fdedb31a9a34bab7b49d98967ef5a"},
+    {url = "https://files.pythonhosted.org/packages/61/8b/914248c1a29cb3cdb4f2bd7aa0b00be76f3636947942d8fd41b63a50ce8e/pydantic_core-2.1.2-cp311-cp311-manylinux_2_24_s390x.whl", hash = "sha256:7c7ad8958aadfbcd664078002246796ecd5566b64b22f6af4fd1bbcec6bf8f60"},
+    {url = "https://files.pythonhosted.org/packages/66/68/9703e44f0bcc29eeaacb1c063675687524646a1bbe3c4527d45475cf120e/pydantic_core-2.1.2.tar.gz", hash = "sha256:d2c790f0d928b672484eac4f5696dd0b78f3d6d148a641ea196eb49c0875e30a"},
+    {url = "https://files.pythonhosted.org/packages/66/c4/c4196fe0a5cc7863ce6cc3670260d5020617b5847a3483092b6cea969d0c/pydantic_core-2.1.2-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:e68a404fad8493989d6f07b7b9e066f1d2524d7cb64db2d4e9a84c920032c67f"},
+    {url = "https://files.pythonhosted.org/packages/6c/1e/5760a9a73c99eb50a96642cdbbc4202f62ce5e9bc8afd865c446b7349bf2/pydantic_core-2.1.2-cp37-cp37m-manylinux_2_24_ppc64le.whl", hash = "sha256:cf92dccca8f66e987f6c4378700447f82b79e86407912ab1ee06b16b82f05120"},
+    {url = "https://files.pythonhosted.org/packages/78/27/5983cde04207c6214ecfab13348b9a284cb5f038cb57afc4d5fdcffac21e/pydantic_core-2.1.2-pp310-pypy310_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:840238c845b0f80777151fef0003088ab91c6f7b3467edaff4932b425c4e3c3f"},
+    {url = "https://files.pythonhosted.org/packages/79/0e/ad517daa1640ce098c68f1de64ce161dfb83a428358dc2cae5cea93315ed/pydantic_core-2.1.2-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e7fd334b40c5e13a97becfcaba314de0dcc6f7fe21ec8f992139bcc64700e9dc"},
+    {url = "https://files.pythonhosted.org/packages/7e/9a/e8aa44326d8ec02b940072e07ab5bb58ff40dc5c47abb47f796c40cd654b/pydantic_core-2.1.2-cp38-none-win_amd64.whl", hash = "sha256:5948af62f323252d56acaec8ebfca5f15933f6b72f8dbe3bf21ee97b2d10e3f0"},
+    {url = "https://files.pythonhosted.org/packages/81/34/46b72d608e02680036a52ef3d97f3173c303e8b04adb6c5e6aff19220927/pydantic_core-2.1.2-pp310-pypy310_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c0f481aaf0119f77b200e5a5e2799b3e14c015a317eaa948f42263908735cc9f"},
+    {url = "https://files.pythonhosted.org/packages/82/3a/c169e10b023ad15bf1e92fd4889c71bfe203778a06a566cc2169fdc7afa9/pydantic_core-2.1.2-pp310-pypy310_pp73-win_amd64.whl", hash = "sha256:7648e48ba263ca0a8a2dc55a60a219c9133fb101ba52c89a14a29fb3d4322ca3"},
+    {url = "https://files.pythonhosted.org/packages/85/9a/fbc2afa8bfac8b525bddc5da24ee3b670c9d59f974c367328178c211f738/pydantic_core-2.1.2-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9b9f8bf1d7008a58fbb6eb334dc6e2f2905400cced8dadb46c4ca28f005a8562"},
+    {url = "https://files.pythonhosted.org/packages/8a/c9/af266da519ecc56b7527df0df744e237462f521fc83e3a81c5b9342fd22a/pydantic_core-2.1.2-cp310-none-win_amd64.whl", hash = "sha256:b4673d1f29487608d613ebcc5caa99ba15eb58450a7449fb6d800f29d90bebc1"},
+    {url = "https://files.pythonhosted.org/packages/8b/85/48bf25e95aa349ccefe383eeaaeda9fcc254fe75d8343fbb8ab625d1b2b1/pydantic_core-2.1.2-cp38-cp38-manylinux_2_24_s390x.whl", hash = "sha256:b59a64c367f350873c40a126ffe9184d903d2126c701380b4b55753484df5948"},
+    {url = "https://files.pythonhosted.org/packages/8b/9b/32057ba1c32555598b70d0de4b80077fda64ea0ec0710c027be966f69883/pydantic_core-2.1.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5a014ee88980013d192a718cbb88e8cea20acd3afad69bc6d15672d05a49cdb6"},
+    {url = "https://files.pythonhosted.org/packages/8d/a6/1a3d9c154aa33364e9e5a59dde7310d7b3ee72f0d6680189df5e32c5b3ad/pydantic_core-2.1.2-cp37-cp37m-macosx_11_0_arm64.whl", hash = "sha256:4e67f9b9dfda2e42b39459cbf99d319ccb90da151e35cead3521975b2afbf673"},
+    {url = "https://files.pythonhosted.org/packages/8e/23/123fabb1b80234356f3d31153532884a45ced41788622a6006d5c4c492bb/pydantic_core-2.1.2-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:0e5761ce986ec709897b1b965fad9743f301500434bea3cbab2b6e662571580f"},
+    {url = "https://files.pythonhosted.org/packages/91/25/4af41902e316d607e1d2df6143b95145cf7d095377fdfce3ca3d15bbb616/pydantic_core-2.1.2-pp37-pypy37_pp73-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:aa39499625239da4ec960cf4fc66b023929b24cc77fb8520289cfdb3c1986428"},
+    {url = "https://files.pythonhosted.org/packages/94/dd/41463c95cc8eb98003af4f92be321e92a7a049421b484042245389a9c3df/pydantic_core-2.1.2-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:0b5d37aedea5963f2097bddbcdb255483191646a52d40d8bb66d61c190fcac91"},
+    {url = "https://files.pythonhosted.org/packages/96/3a/890fd045c074b3f1999380ca139d58383eeaa8435bb3864a983cd233f32e/pydantic_core-2.1.2-cp39-cp39-manylinux_2_24_s390x.whl", hash = "sha256:60b7239206a2f61ad89c7518adfacb3ccd6662eaa07c5e437317aea2615a1f18"},
+    {url = "https://files.pythonhosted.org/packages/97/1f/59a620470bb021779cda8c2a0b9b8237159476446c6a3cdcc973062be66f/pydantic_core-2.1.2-cp37-none-win_amd64.whl", hash = "sha256:6e3bcb4a9bc209a61ea2aceb7433ce2ece32c7e670b0c06848bf870c9b3e7d87"},
+    {url = "https://files.pythonhosted.org/packages/9d/2e/33d7d56a438adbcc987c147201b9385d044eb49b2b13140379e0ac2ac258/pydantic_core-2.1.2-cp311-cp311-manylinux_2_24_ppc64le.whl", hash = "sha256:2ca2d2d5ab65fb40dd05259965006edcc62a9d9b30102737c0a6f45bcbd254e8"},
+    {url = "https://files.pythonhosted.org/packages/9d/da/0c8818e8d832f8d042600c25ef37822a4a0494ce5d81953175ff94466e68/pydantic_core-2.1.2-cp312-cp312-manylinux_2_24_armv7l.whl", hash = "sha256:8125152b03dd91deca5afe5b933a1994b39405adf6be2fe8dce3632319283f85"},
+    {url = "https://files.pythonhosted.org/packages/9e/53/b477aec118bf87a35d271ce520989a4cde7072c8c0b8a6cb483d8a8c27bb/pydantic_core-2.1.2-cp310-cp310-manylinux_2_24_armv7l.whl", hash = "sha256:017700236ea2e7afbef5d3803559c80bd8720306778ebd49268de7ce9972e83e"},
+    {url = "https://files.pythonhosted.org/packages/a2/30/3a4086459ed2c684bff589e7457cd23c96da2f46000e1d7ace5c36e3e365/pydantic_core-2.1.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:fa38a76e832743866aed6b715869757074b06357d1a260163ec26d84974245fe"},
+    {url = "https://files.pythonhosted.org/packages/a2/64/3756d93790eced2a352ef1f66ce280852153ef4d710f7269e995deebe011/pydantic_core-2.1.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4ac140d54da366672f6b91f9a1e8e2d4e7e72720143353501ae886d3fca03272"},
+    {url = "https://files.pythonhosted.org/packages/a2/e4/27d2e2307c4f516bbe53c2b11e35bb0669bf3ec24878e5c383ee5679f396/pydantic_core-2.1.2-cp38-none-win32.whl", hash = "sha256:b4038869ba1d8fa33863b4b1286ab07e6075a641ae269b865f94d7e10b3e800e"},
+    {url = "https://files.pythonhosted.org/packages/a5/ae/1b4d8ca308006a6f894c6aa9a04727fe5f2cdccc949e100206ee60e9dffa/pydantic_core-2.1.2-cp38-cp38-macosx_10_7_x86_64.whl", hash = "sha256:2278ca0b0dfbcfb1e12fa58570916dc260dc72bee5e6e342debf5329d8204688"},
+    {url = "https://files.pythonhosted.org/packages/a5/c5/476b1fff3b5886ef0282344e1f7c3c1d3d9e6e65e7a1074863dddb840608/pydantic_core-2.1.2-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:bd95d223de5162811a7b36c73d48eac4fee03b075132f3a1b73c132ce157a60c"},
+    {url = "https://files.pythonhosted.org/packages/a9/1f/c7e6c593e79343091e2a4862a9a6d92a9dca585fffac0c2680191a698d04/pydantic_core-2.1.2-cp39-cp39-manylinux_2_24_armv7l.whl", hash = "sha256:087ddbb754575618a8832ee4ab52fe7eb332f502e2a56088b53dbeb5c4efdf9f"},
+    {url = "https://files.pythonhosted.org/packages/ab/8d/31a057ef6460752d948342d64130a20de64a17e8a3bf33c34a2f4939aeb9/pydantic_core-2.1.2-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:1c917f7a41d9d09b8b024a5d65cf37e5588ccdb6e610d2df565fb7186b1f3b1c"},
+    {url = "https://files.pythonhosted.org/packages/ab/da/e56cea39c24c4fff1b761e30396b8d0e1062206a067452f09fd71aca7c8e/pydantic_core-2.1.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3747a4178139ebf3f19541285b2eb7c886890ca4eb7eec851578c02a13cc1385"},
+    {url = "https://files.pythonhosted.org/packages/ad/93/3cd7a73ca32b946c99a73b6fbb76e4b1114b949ec425f89c27f8088be9b4/pydantic_core-2.1.2-cp310-cp310-manylinux_2_24_s390x.whl", hash = "sha256:2575664f0a559a7b951a518f6f34c23cab7190f34f8220b8c8218c4f403147ee"},
+    {url = "https://files.pythonhosted.org/packages/ae/28/9c03825b73440e9e31de861a5b59ff18db6ff9a4badaab031d325dd21e8e/pydantic_core-2.1.2-cp312-cp312-macosx_10_7_x86_64.whl", hash = "sha256:90b06bb47e60173d24c7cb79670aa8dd6081797290353b9d3c66d3a23e88eb34"},
+    {url = "https://files.pythonhosted.org/packages/af/1f/9a656eedec17bc100f0362d700b4de2b7bb4427132014228c7ae48f1700f/pydantic_core-2.1.2-pp39-pypy39_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:f2de65752fff248319bcd3b29da24e205fa505607539fcd4acc4037355175b63"},
+    {url = "https://files.pythonhosted.org/packages/b5/f4/1728e5c344758b671832dea83b01c6d34318a0fd68db3b0f6fda5aa875a7/pydantic_core-2.1.2-cp311-none-win32.whl", hash = "sha256:eb4301f009a44bb5db5edfe4e51a8175a4112b566baec07f4af8b1f8cb4649a2"},
+    {url = "https://files.pythonhosted.org/packages/b6/5e/29240f4e534163ec2e7670ae6e790509a38af8bc06ce17500d5910ee6777/pydantic_core-2.1.2-cp37-none-win32.whl", hash = "sha256:682ff9228c838018c47dfa89b3d84cca45f88cacde28807ab8296ec221862af4"},
+    {url = "https://files.pythonhosted.org/packages/b7/46/0854a766c4f39f32b7f32dd6af1a486ebeb578d78a60a249149f7b46e032/pydantic_core-2.1.2-cp37-cp37m-macosx_10_7_x86_64.whl", hash = "sha256:7ff6bfe63f447a509ed4d368a7f4ba6a7abc03bc4744fc3fb30f2ffab73f3821"},
+    {url = "https://files.pythonhosted.org/packages/b8/7a/8d5430bf246a5905e7d9ee7c07384feb2bffceb725f2fad6a72814a713a2/pydantic_core-2.1.2-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:f7bcdf70c8b6e70be11c78d3c00b80a24cccfb408128f23e91ec3019bed1ecc1"},
+    {url = "https://files.pythonhosted.org/packages/ba/7b/3438042a95ab0c9b957abeb86e1ee68a2171c6e24277eeec0e7558351302/pydantic_core-2.1.2-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:4938b32c09dbcecbeb652327cb4a449b1ef1a1bf6c8fc2c8241aa6b8f6d63b54"},
+    {url = "https://files.pythonhosted.org/packages/ba/9c/261309df290f1aaf76f642e44d80af816198272363950891f2a26ca256d6/pydantic_core-2.1.2-cp37-cp37m-manylinux_2_24_armv7l.whl", hash = "sha256:2ee3ae58f271851362f6c9b33e4c9f9e866557ec7d8c03dc091e9b5aa5566cec"},
+    {url = "https://files.pythonhosted.org/packages/ba/fb/3aa41c4ee6e5456355267b6f0b60bb0c9d8e41556bc130e3ee4b50bbba7b/pydantic_core-2.1.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:74a33aa69d476773230396396afb8e11908f8dafdcfd422e746770599a3f889d"},
+    {url = "https://files.pythonhosted.org/packages/bc/3e/671527f32e7847d7ed1f982f3ea4307848f5b0c8a50f150e4529c1954599/pydantic_core-2.1.2-cp39-cp39-macosx_10_7_x86_64.whl", hash = "sha256:8e6ce261ccb9a986953c4dce070327e4954f9dd4cd214746dfc70efbc713b6a1"},
+    {url = "https://files.pythonhosted.org/packages/c2/19/a374868e93361b10637626507bc8cfd319c2e4b30b82f7de53cba24d8906/pydantic_core-2.1.2-pp310-pypy310_pp73-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:15eb4cb543ed36f6a4f16e3bee7aa7ed1c3757be95a3f3bbb2b82b9887131e0f"},
+    {url = "https://files.pythonhosted.org/packages/c3/ab/d536d95b62724f0079666772cf620741bbf8250088ebaf3f07cad082c3ad/pydantic_core-2.1.2-pp39-pypy39_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:a8b9c2cc4c5f8169b943d24be4bd1548fe81c016d704126e3a3124a2fc164885"},
+    {url = "https://files.pythonhosted.org/packages/c3/f5/616bfa321206b45eb5307d5fc0d673d5f4a71f14637d24e3e4f6507b061d/pydantic_core-2.1.2-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b815a769b019dd96be6571096f246b74f63330547e9b30244c51b4a2eb0277fc"},
+    {url = "https://files.pythonhosted.org/packages/c4/e5/597f228da2ce3e24c8ad619b2083723e727c13c27d2bb2fac45d14d6872e/pydantic_core-2.1.2-cp311-cp311-manylinux_2_24_armv7l.whl", hash = "sha256:db4564aea8b3cb6cf1e5f3fd80f1ced73a255d492396d1bd8abd688795b34d63"},
+    {url = "https://files.pythonhosted.org/packages/c5/ff/dea9646f5885fa9efc07af91aff6086ac0282f83e66de0424ae523889566/pydantic_core-2.1.2-pp310-pypy310_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8c0213891898fa5b404cf3edf4797e3ac7819a0708ea5473fc6432a2aa27c189"},
+    {url = "https://files.pythonhosted.org/packages/c6/95/e4c8947b57f1a35eacb175cf5717c372197dd837c91296969c782e7d4bad/pydantic_core-2.1.2-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:46cd323371aa7e4053010ccdb94063a4273aa9e5dbe97f8a1147faa769de8d8d"},
+    {url = "https://files.pythonhosted.org/packages/cc/03/6cf597afecaba9ca3f6227cec94e049c760b7ce3ec1577cdb16ca34bb260/pydantic_core-2.1.2-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:be3419204952bbe9b72b90008977379c52f99ae1c6e640488de4be783c345d71"},
+    {url = "https://files.pythonhosted.org/packages/cc/92/e6bb8c9a9cf0d25f7dad6457a194f0c602d13029fab0fa252ecd6f917980/pydantic_core-2.1.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:af832edd384755826e494ffdcf1fdda86e4babc42a0b18d342943fb18181040e"},
+    {url = "https://files.pythonhosted.org/packages/cd/39/32041d9ff711b6972342d1dee1de802b17d76c08dc29e9b0f1f8f515ea25/pydantic_core-2.1.2-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8b9a5fc4058d64c9c826684dcdb43891c1b474a4a88dcf8dfc3e1fb5889496f8"},
+    {url = "https://files.pythonhosted.org/packages/cf/ec/bb7ab23fa6fc75ffd0dff866c2814e7066554ca11bb08cb5af80b74dc4e4/pydantic_core-2.1.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:88a56f0f6d020b4d17641f4b4d1f9540a536d4146768d059c430e97bdb485fc1"},
+    {url = "https://files.pythonhosted.org/packages/d1/bd/3566d5e3f9aca01a418c22798baed893ecd66321607e020861de44c50a3e/pydantic_core-2.1.2-pp37-pypy37_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:9a5fba9168fc27805553760fa8198db46eef83bf52b4e87ebbe1333b823d0e70"},
+    {url = "https://files.pythonhosted.org/packages/d7/0b/3750ebbd83496a6d3c8b8bafc1d81763749b8f302d7a1ffbee615be798e2/pydantic_core-2.1.2-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:24c3c9180a2d19d640bacc2d00f497a9a1f2abadb2a9ee201b56bb03bc5343bd"},
+    {url = "https://files.pythonhosted.org/packages/dc/74/805d5f1423aa1a1dacaf24239c0b30994795f6f7fd268006aae1d03b3da3/pydantic_core-2.1.2-cp38-cp38-manylinux_2_24_ppc64le.whl", hash = "sha256:c720e55cef609d50418bdfdfb5c44a76efc020ae7455505788d0113c54c7df55"},
+    {url = "https://files.pythonhosted.org/packages/e2/31/4438c763c76798afd1d5ea019c3fe6fff54f5d95d7ddcb734d2ad618ec44/pydantic_core-2.1.2-cp310-cp310-manylinux_2_24_ppc64le.whl", hash = "sha256:c2d00a96fdf26295c6f25eaf9e4a233f353146a73713cd97a5f5dc6090c3aef2"},
+    {url = "https://files.pythonhosted.org/packages/e9/42/5facc2d3aca9a21c90f3f3fa9b7a7975951704b47d0eb040fc70b66900e7/pydantic_core-2.1.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:8884a1dbfc5cb8c54b48446ca916d4577c1f4d901126091e4ab25d00194e065f"},
+    {url = "https://files.pythonhosted.org/packages/f1/69/f210945a81631b83f679c4ce084db7d444e19273db2ab54707c39e4004a0/pydantic_core-2.1.2-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4aff436c23c68449601b3fba7075b4f37ef8fbb893c8c1ed3ef898f090332b1e"},
+    {url = "https://files.pythonhosted.org/packages/f1/b9/1e17aa51d549b74fa37f7641b202b9310b2e242a083e85c4dd738becad5e/pydantic_core-2.1.2-cp39-none-win_amd64.whl", hash = "sha256:ac462a28218ea7d592c7ad51b517558f4ac6565a4e53db7a4811eeaf9c9660b0"},
+    {url = "https://files.pythonhosted.org/packages/f4/d9/e0f6d427aa8056c8d04d3339da40303b782d0dafac64efcdf0774cd8604c/pydantic_core-2.1.2-cp310-none-win32.whl", hash = "sha256:a772c652603855d7180015849d483a1f539351a263bb9b81bfe85193a33ce124"},
+    {url = "https://files.pythonhosted.org/packages/f5/c5/28f8b327c228f0ce8c609e3f474e72764be1cd72096bc65c16a37b87f01e/pydantic_core-2.1.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:cbba32fb14e199d0493c6b9c44870dab0a9c37af9f0f729068459d1849279ffd"},
+    {url = "https://files.pythonhosted.org/packages/f6/4b/43b8fd58dca53286e5e96ead82bb3a4becb90c91e7081eb0ddc0690d1100/pydantic_core-2.1.2-pp38-pypy38_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:d281a10837d98db997c0247f45d138522c91ce30cf3ae7a6afdb5e709707d360"},
+    {url = "https://files.pythonhosted.org/packages/f6/9a/dbbdc5f3b9590cd0273d96b7e0a8ce609038558bd894de1c06d643460203/pydantic_core-2.1.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:d35d634d9d1ed280c87bc2a7a6217b8787eedc86f368fc2fa1c0c8c78f7d3c93"},
+    {url = "https://files.pythonhosted.org/packages/f6/ce/29732ae567ec070ac2a56ff05684fb09a8189d8929ab589f3545e4dcfd41/pydantic_core-2.1.2-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:87cff210af3258ca0c829e3ebc849d7981bfde23a99d6cb7a3c17a163b3dbad2"},
+    {url = "https://files.pythonhosted.org/packages/fc/dd/ad4af88dc902e227bde43878487c0deafbb5d72fa6b8bb6480ee0a3e37ad/pydantic_core-2.1.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0be2e2812a43205728a06c9d0fd090432cd76a9bb5bff2bfcfdf8b0e27d51851"},
+    {url = "https://files.pythonhosted.org/packages/fe/83/45780d6424dbf64800497ce694b9b09d588f6c50de9c9c6c189169adbb61/pydantic_core-2.1.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f0eb54b11cd4fe0c6404611eef77086ade03eb1457e92910bbb4f3479efa3f79"},
 ]
 "pytest 7.4.0" = [
     {url = "https://files.pythonhosted.org/packages/33/b2/741130cbcf2bbfa852ed95a60dc311c9e232c7ed25bac3d9b8880a8df4ae/pytest-7.4.0-py3-none-any.whl", hash = "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32"},
     {url = "https://files.pythonhosted.org/packages/a7/f3/dadfbdbf6b6c8b5bd02adb1e08bc9fbb45ba51c68b0893fa536378cdf485/pytest-7.4.0.tar.gz", hash = "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"},
 ]
 "pytz 2023.3" = [
     {url = "https://files.pythonhosted.org/packages/5e/32/12032aa8c673ee16707a9b6cdda2b09c0089131f35af55d443b6a9c69c1d/pytz-2023.3.tar.gz", hash = "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588"},
```

### Comparing `aws_spy-0.1.11/aws_spy/__init__.py` & `aws_spy-0.2.0/aws_spy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ServerlessPy package ;D"""
 
-__version__ = "0.1.11"
+__version__ = "0.2.0"
 
 from aws_spy import responses
 from aws_spy.core.logging import logger
 from aws_spy.core.params_alias import Header, Path, Query
 from aws_spy.core.schemas import (
     CORS,
     VPC,
```

### Comparing `aws_spy-0.1.11/aws_spy/dependencies.py` & `aws_spy-0.2.0/aws_spy/dependencies.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.1.11/aws_spy/main.py` & `aws_spy-0.2.0/aws_spy/main.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.1.11/aws_spy/responses.py` & `aws_spy-0.2.0/aws_spy/responses.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,26 +32,26 @@
         headers = {
             "Content-Type": ContentType.JSON.value,
         }
         if self.additional_headers is not None:
             headers.update(self.additional_headers)
 
         if self.route is not None and self.route.response_class is not None and isinstance(self.data, dict):
-            self.data = self.route.response_class.parse_obj(self.data)
+            self.data = self.route.response_class.model_validate(self.data)
 
         if (
             self.route is not None
             and self.route.response_class is not None
             and isinstance(self.data, BaseModel)
             and not isinstance(self.data, self.route.response_class)
         ):
-            self.data = self.route.response_class.parse_obj(self.data.dict())
+            self.data = self.route.response_class.model_validate(self.data.model_dump())
 
         if isinstance(self.data, BaseModel):
-            self.data = self.data.dict()
+            self.data = self.data.model_dump()
 
         if self.route is None or self.route.status_code is None:
             status_code = 200
         else:
             status_code = self.route.status_code
 
         return {
```

### Comparing `aws_spy-0.1.11/aws_spy/test.py` & `aws_spy-0.2.0/aws_spy/test.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.1.11/aws_spy/core/event_utils.py` & `aws_spy-0.2.0/aws_spy/core/event_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     body: str, request_body_class: type[RequestBodyType]
 ) -> tuple[RequestBodyType | dict[str, Any] | None, list[str]]:
     try:
         body = json.loads(body)
     except json.JSONDecodeError:
         return None, ["Request body is empty!"]
     try:
-        request_body = request_body_class.parse_obj(body)
+        request_body = request_body_class.model_validate(body)
     except ValidationError as e:
         errors = []
         for error in e.errors():
             if error["type"].startswith("type_error"):
                 errors.append(f'Wrong type received at: {error["loc"][0]}. Expected: {error["type"].split(".")[-1]}')
                 continue
             if error["type"].endswith("missing"):
```

### Comparing `aws_spy-0.1.11/aws_spy/core/schemas.py` & `aws_spy-0.2.0/aws_spy/core/schemas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 import os
 from collections.abc import Callable
 from enum import Enum
 from pathlib import Path
 from typing import Any, Literal, TypeVar
 
-from pydantic import BaseModel, Field, root_validator, validator
+from pydantic import BaseModel, Field, field_validator, model_validator
 from typing_extensions import Self  # type: ignore
 
 from aws_spy.core.exceptions import RouteDefinitionError
 from aws_spy.core.schemas_utils import (
     ParamSchema,
     get_path_param_names,
     resolve_handler_args,
@@ -56,68 +56,68 @@
 
 class SpyRoute(BaseModel):
     name: str
     path: str
     method: Methods
     handler: LH
     status_code: int
-    tags: list[str] | None
+    tags: list[str] | None = Field(None)
     summary: str = Field("API endpoint")
-    description: str | None
-    request_body_arg_name: str | None
-    request_body: type[BaseModel] | None
-    response_class: type[BaseModel] | None
+    description: str | None = Field(None)
+    request_body_arg_name: str | None = Field(None)
+    request_body: type[BaseModel] | None = Field(None)
+    response_class: type[BaseModel] | None = Field(None)
     header_params: list[ParamSchema] = Field(default_factory=list)
     path_params: list[ParamSchema] = Field(default_factory=list)
     query_params: list[ParamSchema] = Field(default_factory=list)
     # dependencies: list[DependencySchema] = Field(default_factory=list)
     use_vpc: bool = Field(True)
     authorizer: str | None = Field(None)
     layers: list[str] = Field(default_factory=list)
     add_event: bool = Field(default=False)
     add_context: bool = Field(default=False)
     skip_validation: bool = Field(default=False)
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     def set_status_code(  # type: ignore
         cls: type[Self],  # noqa: N805
         values: dict[str, Any],
     ) -> dict[str, Any]:
         if values.get("status_code") is None:
             values["status_code"] = DEFAULT_STATUS_CODES[values["method"]]
 
         return values
 
-    @validator("summary", pre=True)
+    @field_validator("summary", mode="before")
     def set_summary(cls: type[Self], summary: str | None) -> str:  # type: ignore  # noqa: N805
         return summary or "API endpoint"
 
-    @root_validator
+    @model_validator(mode="after")
     def validate_handler_params(  # type: ignore
         cls: type[Self],  # noqa: N805
-        values: dict[str, Any],
+        model: Self,
     ) -> dict[str, Any]:
-        method: Methods = values["method"]
-        path: str = values["path"]
-        handler: LH = values["handler"]
+        method: Methods = model.method
+        path: str = model.path
+        handler: LH = model.handler
 
         path_params = get_path_param_names(path)
         handler_args = resolve_handler_args(handler)
         # values["dependencies"] = get_dependencies(handler)
 
         args = inspect.signature(handler).parameters
         args_count = len(args)
         # exclude lambdas event and context from count
         if "event" in args:
-            values["add_event"] = True
+            model.add_event = True
             args_count -= 1
         if "context" in args:
-            values["add_context"] = True
+            model.add_context = True
             args_count -= 1
-        if handler_args.count != args_count and not values["skip_validation"]:
+        if handler_args.count != args_count and not model.skip_validation:
             msg = f'Unrecognized params for {method.upper()} method on "{path}" path!'
             raise RouteDefinitionError(msg)
 
         for path_param in path_params:
             if path_param not in handler_args.path.keys():
                 msg = f"You did not specify {path_param} in your handler arguments!"
                 raise RouteDefinitionError(msg)
@@ -128,21 +128,26 @@
                 raise RouteDefinitionError(msg)
 
         if method in (Methods.GET, Methods.DELETE) and handler_args.request_body:
             msg = f'{method.upper()} method on "{path}" cannot have request body!'
             raise RouteDefinitionError(msg)
 
         if handler_args.request_body:
-            values["request_body"] = handler_args.request_body
-            values["request_body_arg_name"] = handler_args.request_body_arg_name
+            model.request_body = handler_args.request_body
+            model.request_body_arg_name = handler_args.request_body_arg_name
 
         for attr_name in ("path", "query", "header"):
-            values[f"{attr_name}_params"] += [param for _, param in getattr(handler_args, attr_name).items()]
+            setattr(
+                model,
+                f"{attr_name}_params",
+                getattr(model, f"{attr_name}_params")
+                + [param for _, param in getattr(handler_args, attr_name).items()],
+            )
 
-        return values
+        return model
 
 
 class _CloudFormationRef(BaseModel):
     stack_name: str
     export_name: str
 
     def __str__(self: Self) -> str:
@@ -235,27 +240,27 @@
 
 class Provider(BaseModel):
     name: str = "aws"
     runtime: str = "python3.9"
     region: str
     role: str | CloudFormationRef | JSONFileRef
     httpApi: HTTPApi  # noqa: N815
-    vpc: VPC | None
+    vpc: VPC | None = Field(None)
 
 
 class ServerlessConfig(YamlModel):
     service: str
     custom: dict[str, Any] | None = Field(None)
     plugins: list[str]
     configValidationMode: str = "error"  # noqa: N815
     provider: Provider
     package: dict[str, bool] = Field({"individually": True})
     functions: dict[str, Function] | None = Field(None)
 
-    @validator("plugins", pre=True)
+    @field_validator("plugins", mode="before")
     def set_default_plugins(cls: type[Self], value: list[str] | None) -> list[str]:  # type: ignore  # noqa: N805
         value = value if value is not None else []
         value += [
             "serverless-python-requirements",
             "serverless-plugin-common-excludes",
             "serverless-plugin-include-dependencies",
         ]
```

### Comparing `aws_spy-0.1.11/aws_spy/core/schemas_utils.py` & `aws_spy-0.2.0/aws_spy/core/schemas_utils.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.1.11/aws_spy/core/types.py` & `aws_spy-0.2.0/aws_spy/core/types.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.1.11/aws_spy/helpers/cli.py` & `aws_spy-0.2.0/aws_spy/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.1.11/aws_spy/helpers/documentation.py` & `aws_spy-0.2.0/aws_spy/helpers/documentation.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.1.11/aws_spy/helpers/utils.py` & `aws_spy-0.2.0/aws_spy/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.1.11/tests/conftest.py` & `aws_spy-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.1.11/tests/test_app.py` & `aws_spy-0.2.0/tests/test_app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 
 from aws_spy import ServerlessConfig, SpyAPI, SpyRouter, __version__
 from aws_spy.core.schemas import Methods
 
 
 def test_app() -> None:
-    assert __version__ == "0.1.10"
+    assert __version__ == "0.2.0"
 
 
 def test_app_conf(app: SpyAPI, config: ServerlessConfig) -> None:
     assert app.config == config
 
 
 @pytest.mark.parametrize("prefix", ["api", "/api", "/somet_other_prefix"])
```

### Comparing `aws_spy-0.1.11/tests/integration/test_params.py` & `aws_spy-0.2.0/tests/integration/test_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     method: Methods,
     param,
     path: str,
     route_param: str,
     param_annotation: type,
     expected_annotation: type,
     is_required: bool,
-    enum: Union[list[str], None],
+    enum: list[str] | None,
 ) -> None:
     app_method = getattr(app, method.value)
     expected_param = ParamSchema(
         name="user_id",
         arg_name="user_id",
         in_=param,
         annotation=expected_annotation,
```

### Comparing `aws_spy-0.1.11/tests/integration/test_request_body.py` & `aws_spy-0.2.0/tests/integration/test_request_body.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.1.11/tests/integration/test_response_class.py` & `aws_spy-0.2.0/tests/integration/test_response_class.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.1.11/tests/unit/test_encoders.py` & `aws_spy-0.2.0/tests/unit/test_encoders.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.1.11/tests/unit/test_event_utils.py` & `aws_spy-0.2.0/tests/unit/test_event_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,24 +14,24 @@
     example = "example"
 
 
 class ExampleRequestBody(BaseModel):
     a: int
     b: str
     c: bool
-    d: Union[int, None]
-    example: Union[ExampleEnum, None] = Field(None)
+    d: int | None
+    example: ExampleEnum | None = Field(None)
 
 
 def gpm(
     name: str,
     arg_name: str,
     annotation: type,
-    is_required: bool = True,
-    enum: Union[list[str], None] = None,
+    is_required: bool = True,  # noqa: FBT001 FBT002
+    enum: list[str] | None = None,
 ) -> ParamSchema:
     return ParamSchema(
         name=name,
         arg_name=arg_name,
         in_=Header(),
         annotation=annotation,
         is_required=is_required,
@@ -90,47 +90,42 @@
             "path",
             {},
             ["user_id should be ExampleEnum type."],
         ],
     ],
 )
 def test_export_params_from_event_success(
-    in_event_params: Union[dict[str, Any], None],
+    in_event_params: dict[str, Any] | None,
     expected_params: list[ParamSchema],
     type_: Literal["path", "header", "query"],
     expected_params_result: dict[str, Any],
     expected_errors_result: list[str],
 ) -> None:
     params, errors = export_params_from_event(in_event_params, expected_params, type_)
     assert params == expected_params_result
     assert errors == expected_errors_result
 
 
 @pytest.mark.parametrize(
-    ["body", "expected_errors"],
+    ["body", "expecting_errors"],
     [
-        (json.dumps({"a": 1, "b": "string", "c": True, "d": None}), []),
-        ["", ["Request body is empty!"]],
+        (json.dumps({"a": 1, "b": "string", "c": True, "d": None}), False),
+        ["", True],
         (
             json.dumps({"a": "str", "b": "string", "c": "str", "d": None}),
-            [
-                "Wrong type received at: a. Expected: integer",
-                "Wrong type received at: c. Expected: bool",
-            ],
+            True,
         ),
         (
-            json.dumps(
-                {"a": 1, "b": "string", "c": True, "d": "10", "example": "not example"}
-            ),
-            ["Wrong type received at: example. Expected: enum"],
+            json.dumps({"a": 1, "b": "string", "c": True, "d": "10", "example": "not example"}),
+            True,
         ),
         (
             json.dumps({"b": "string", "c": True, "d": "10", "example": "example"}),
-            ["Value not found at: a"],
+            True,
         ),
     ],
 )
-def test_export_request_body(body: str, expected_errors: list[str]) -> None:
+def test_export_request_body(body: str, expecting_errors: bool) -> None:  # noqa: FBT001
     request_body, errors = export_request_body(body, ExampleRequestBody)
-    assert errors == expected_errors
+    assert bool(errors) == expecting_errors
     if not errors:
         assert isinstance(request_body, ExampleRequestBody)
```

### Comparing `aws_spy-0.1.11/tests/unit/test_responses.py` & `aws_spy-0.2.0/tests/unit/test_responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,18 @@
             ExampleResponseClass,
             json.dumps({"x": 10, "y": 15}),
             None,
         ),
     ],
 )
 def test_json_response(
-    data: Union[BaseModel, dict[str, Any]],
+    data: BaseModel | dict[str, Any],
     response_class: type[BaseModel],
     expected_response_body: str,
-    additional_headers: Union[dict[str, str], None],
+    additional_headers: dict[str, str] | None,
 ) -> None:
     expected_headers = {
         "Content-Type": "application/json",
     }
     if additional_headers:
         expected_headers.update(additional_headers)
```

### Comparing `aws_spy-0.1.11/.gitignore` & `aws_spy-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aws_spy-0.1.11/LICENSE` & `aws_spy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_spy-0.1.11/pyproject.toml` & `aws_spy-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "pydantic<2.0.0"
+    "pydantic>=2.0.0"
 ]
 
 [tool.pdm.dev-dependencies]
 linting = [
     "black",
     "ruff",
     "mypy~=1.1.1",
```

### Comparing `aws_spy-0.1.11/PKG-INFO` & `aws_spy-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-spy
-Version: 0.1.11
+Version: 0.2.0
 Project-URL: Homepage, https://github.com/PiochU19/aws-spy
 Project-URL: Documentation, https://github.com/PiochU19/aws-spy#readme
 Project-URL: Issues, https://github.com/PiochU19/aws-spy/issues
 Project-URL: Source, https://github.com/PiochU19/aws-spy
 Author-email: Dominik Pioś <792954018@wp.pl>
 License: The MIT License (MIT)
         
@@ -31,11 +31,11 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: <3.11.0,>=3.10.0
-Requires-Dist: pydantic<2.0.0
+Requires-Dist: pydantic>=2.0.0
 Description-Content-Type: text/markdown
 
 Hello ;D
```

