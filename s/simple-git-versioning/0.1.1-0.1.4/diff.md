# Comparing `tmp/simple-git-versioning-0.1.1.tar.gz` & `tmp/simple-git-versioning-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-git-versioning-0.1.1.tar", last modified: Mon Jul 10 20:13:01 2023, max compression
+gzip compressed data, was "simple-git-versioning-0.1.4.tar", last modified: Mon Jul 10 21:32:54 2023, max compression
```

## Comparing `simple-git-versioning-0.1.1.tar` & `simple-git-versioning-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:13:01.875044 simple-git-versioning-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5175 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3840 2023-07-10 20:13:01.875044 simple-git-versioning-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/Pipfile
--rw-rw-rw-   0 root         (0) root         (0)    46710 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/Pipfile.lock
--rw-rw-rw-   0 root         (0) root         (0)     2974 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1717 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 20:13:01.875044 simple-git-versioning-0.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:13:01.871378 simple-git-versioning-0.1.1/simple_git_versioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3840 2023-07-10 20:13:01.000000 simple-git-versioning-0.1.1/simple_git_versioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      681 2023-07-10 20:13:01.000000 simple-git-versioning-0.1.1/simple_git_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 20:13:01.000000 simple-git-versioning-0.1.1/simple_git_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      204 2023-07-10 20:13:01.000000 simple-git-versioning-0.1.1/simple_git_versioning.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-10 20:13:01.000000 simple-git-versioning-0.1.1/simple_git_versioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-10 20:13:01.000000 simple-git-versioning-0.1.1/simple_git_versioning.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:13:01.871378 simple-git-versioning-0.1.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:13:01.872294 simple-git-versioning-0.1.1/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)     7368 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/tests/unit/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    10566 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/tests/unit/test_pep440.py
--rw-rw-rw-   0 root         (0) root         (0)    14420 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/tests/unit/test_project.py
--rw-rw-rw-   0 root         (0) root         (0)     3196 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/tests/unit/test_semver2.py
--rw-rw-rw-   0 root         (0) root         (0)     3248 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/tests/unit/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:13:01.874128 simple-git-versioning-0.1.1/versioning/
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/versioning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14854 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/versioning/pep440.py
--rw-rw-rw-   0 root         (0) root         (0)     7746 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/versioning/project.py
--rw-rw-rw-   0 root         (0) root         (0)     8643 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/versioning/semver2.py
--rw-rw-rw-   0 root         (0) root         (0)     2040 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/versioning/setuptools.py
--rw-rw-rw-   0 root         (0) root         (0)     1146 2023-07-10 20:12:48.000000 simple-git-versioning-0.1.1/versioning/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:32:54.172634 simple-git-versioning-0.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5099 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3862 2023-07-10 21:32:54.172634 simple-git-versioning-0.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/Pipfile
+-rw-rw-rw-   0 root         (0) root         (0)    46416 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/Pipfile.lock
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1878 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 21:32:54.172634 simple-git-versioning-0.1.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:32:54.169634 simple-git-versioning-0.1.4/simple_git_versioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3862 2023-07-10 21:32:54.000000 simple-git-versioning-0.1.4/simple_git_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      681 2023-07-10 21:32:54.000000 simple-git-versioning-0.1.4/simple_git_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 21:32:54.000000 simple-git-versioning-0.1.4/simple_git_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-10 21:32:54.000000 simple-git-versioning-0.1.4/simple_git_versioning.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-10 21:32:54.000000 simple-git-versioning-0.1.4/simple_git_versioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-10 21:32:54.000000 simple-git-versioning-0.1.4/simple_git_versioning.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:32:54.169634 simple-git-versioning-0.1.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:32:54.170634 simple-git-versioning-0.1.4/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)     7368 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/tests/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/tests/unit/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    10566 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/tests/unit/test_pep440.py
+-rw-rw-rw-   0 root         (0) root         (0)    14420 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/tests/unit/test_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     3196 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/tests/unit/test_semver2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3248 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/tests/unit/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:32:54.171634 simple-git-versioning-0.1.4/versioning/
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/versioning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15269 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/versioning/pep440.py
+-rw-rw-rw-   0 root         (0) root         (0)     7848 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/versioning/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     9062 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/versioning/semver2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2060 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/versioning/setuptools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/versioning/version.py
```

### Comparing `simple-git-versioning-0.1.1/.gitlab-ci.yml` & `simple-git-versioning-0.1.4/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,15 @@
 
 pytest:
   stage: test
   rules:
     - if: $CI_PIPELINE_SOURCE == 'merge_request_event'
   script:
     - git fetch origin "$CI_MERGE_REQUEST_TARGET_BRANCH_NAME"
-    - pipenv run pytest --cov-report=xml --junit-xml=unit-test-report.xml
-    # - git rebase -x 'pipenv run pytest --cov-report=xml --junit-xml=unit-test-report.xml' origin/"$CI_MERGE_REQUEST_TARGET_BRANCH_NAME"
+    - git rebase -x 'pipenv run pytest --cov-report=xml --junit-xml=unit-test-report.xml' origin/"$CI_MERGE_REQUEST_TARGET_BRANCH_NAME"
   coverage: '/(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/'
   artifacts:
     reports:
       coverage_report:
         coverage_format: cobertura
         path: coverage.xml
       junit: unit-test-report.xml
```

### Comparing `simple-git-versioning-0.1.1/.pre-commit-config.yaml` & `simple-git-versioning-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.1/LICENSE` & `simple-git-versioning-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.1/PKG-INFO` & `simple-git-versioning-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: simple-git-versioning
-Version: 0.1.1
+Version: 0.1.4
 Summary: Thinly scoped and opinionated tool that computes a version number from git tags and trailers
 Author-email: Quentin Bouget <ypsah@devyard.org>
 License: MIT
 Project-URL: homepage, https://gitlab.com/ypsah/simple-git-versioning
 Project-URL: repository, https://gitlab.com/ypsah/simple-git-versioning
 Keywords: versioning,git,git-trailers
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Opinionated version numbering CLIs, and library
 
@@ -62,18 +65,15 @@
 
 ## Libraries
 
 Libraries that wish to expose their version number programatically may do so by
 including the following snippet:
 
 ```python
-try:
-    from importlib.metadata import version
-except ImportError:  # python<3.11
-    from importlib_metadata import version  # install_requires: `importlib-metadata`
+from importlib.metadata import version
 
 from versioning.pep440 import Project
 
 try:
     __version__ = version("simple-git-versioning")
 except PackageNotFoundError:
     # package is not installed
```

### Comparing `simple-git-versioning-0.1.1/Pipfile.lock` & `simple-git-versioning-0.1.4/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9493055555555555%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'df09517d490da484f41eaf5ab76d0548c60af98f9a3b1ce8f4d44f6dac05ea12'}}",*

 * * "'default'": "{'typing-extensions': {'hashes': "*

 * *              "['sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36', "*

 * *              "'sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2'], "*

 * *              '\'markers\': "python_version < \'3.11\'", \'version\': \'==4.7.1\'}, delete: '*

 * *              "['packaging']}",*

 * * "'develop'": "{'charset-normal […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "5c6a6529c0656e988373e48ebf38139e2c7283e595ea45eab2a03fffec0b3c01"
+            "sha256": "df09517d490da484f41eaf5ab76d0548c60af98f9a3b1ce8f4d44f6dac05ea12"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
@@ -25,22 +25,14 @@
             "hashes": [
                 "sha256:1a441dad41c9a0615c6ae96464190eddccd2de8153254059ff18ffd7b3b84800",
                 "sha256:b87d2b33eb5d7f2c9a5af4770d6d106560c9688c79a821e5fe1bbd41188f5dcc"
             ],
             "index": "pypi",
             "version": "==2.6.2"
         },
-        "packaging": {
-            "hashes": [
-                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
-                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
-            ],
-            "index": "pypi",
-            "version": "==23.1"
-        },
         "sh": {
             "hashes": [
                 "sha256:14265a4cd1622429edcf300292ec98193530fb143fe642b3437024eca9bee8c5",
                 "sha256:a18920f0839991bc9dfddb6dcc006c360b1064ba96257359f0ea356e9fa75a60"
             ],
             "index": "pypi",
             "version": "==2.0.4"
@@ -51,19 +43,19 @@
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
-                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
+                "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36",
+                "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==4.6.3"
+            "markers": "python_version < '3.11'",
+            "version": "==4.7.1"
         }
     },
     "develop": {
         "attrs": {
             "hashes": [
                 "sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04",
                 "sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015"
@@ -201,100 +193,100 @@
                 "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"
             ],
             "markers": "python_full_version >= '3.6.1'",
             "version": "==3.3.1"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
-                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
-                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
-                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
-                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
-                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
-                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
-                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
-                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
-                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
-                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
-                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
-                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
-                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
-                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
-                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
-                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
-                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
-                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
-                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
-                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
-                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
-                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
-                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
-                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
-                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
-                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
-                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
-                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
-                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
-                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
-                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
-                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
-                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
-                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
-                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
-                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
-                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
-                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
-                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
-                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
-                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
-                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
-                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
-                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
-                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
-                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
-                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
-                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
-                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
-                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
-                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
-                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
-                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
-                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
-                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
-                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
-                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
-                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
-                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
-                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
-                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
-                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
-                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
-                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
-                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
-                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
-                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
-                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
-                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
-                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
-                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
-                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
-                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
-                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
+                "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96",
+                "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c",
+                "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710",
+                "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706",
+                "sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020",
+                "sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252",
+                "sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad",
+                "sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329",
+                "sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a",
+                "sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f",
+                "sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6",
+                "sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4",
+                "sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a",
+                "sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46",
+                "sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2",
+                "sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23",
+                "sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace",
+                "sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd",
+                "sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982",
+                "sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10",
+                "sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2",
+                "sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea",
+                "sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09",
+                "sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5",
+                "sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149",
+                "sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489",
+                "sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9",
+                "sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80",
+                "sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592",
+                "sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3",
+                "sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6",
+                "sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed",
+                "sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c",
+                "sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200",
+                "sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a",
+                "sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e",
+                "sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d",
+                "sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6",
+                "sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623",
+                "sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669",
+                "sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3",
+                "sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa",
+                "sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9",
+                "sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2",
+                "sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f",
+                "sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1",
+                "sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4",
+                "sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a",
+                "sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8",
+                "sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3",
+                "sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029",
+                "sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f",
+                "sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959",
+                "sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22",
+                "sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7",
+                "sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952",
+                "sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346",
+                "sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e",
+                "sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d",
+                "sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299",
+                "sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd",
+                "sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a",
+                "sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3",
+                "sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037",
+                "sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94",
+                "sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c",
+                "sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858",
+                "sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a",
+                "sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449",
+                "sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c",
+                "sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918",
+                "sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1",
+                "sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c",
+                "sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac",
+                "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==3.1.0"
+            "version": "==3.2.0"
         },
         "click": {
             "hashes": [
-                "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
-                "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
+                "sha256:2739815aaa5d2c986a88f1e9230c55e17f0caad3d958a5e13ad0797c166db9e3",
+                "sha256:b97d0c74955da062a7d4ef92fadb583806a585b2ea81958a81bd72726cbb8e37"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==8.1.3"
+            "version": "==8.1.4"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
                 "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f",
@@ -407,19 +399,19 @@
                 "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.12.2"
         },
         "hypothesis": {
             "hashes": [
-                "sha256:245bed0fcf7612caa0ca1ecaa5c1e3a7100bbf9fd0fe4a24bdd9e46249b2774f",
-                "sha256:69b55ee1dae2c7edd214e273a977d0dfba542946a211c9ef1f958743b49e430e"
+                "sha256:315cab90c379efa994816e5d073673600e52bf47545b06a46592496ad1b08ed7",
+                "sha256:accda6cd8706c611f038cd83f2dbdd5ba9488ce3cf7fac25d8a6df9fff4247fc"
             ],
             "index": "pypi",
-            "version": "==6.79.3"
+            "version": "==6.81.0"
         },
         "identify": {
             "hashes": [
                 "sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4",
                 "sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d"
             ],
             "markers": "python_version >= '3.7'",
@@ -431,19 +423,19 @@
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4",
-                "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"
+                "sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb",
+                "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==6.7.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==6.8.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
@@ -455,19 +447,19 @@
                 "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
             ],
             "index": "pypi",
             "version": "==5.12.0"
         },
         "jaraco.classes": {
             "hashes": [
-                "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158",
-                "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"
+                "sha256:10afa92b6743f25c0cf5f37c6bb6e18e2c5bb84a16527ccfc0040ea377e7aaeb",
+                "sha256:c063dd08e89217cee02c8d5e5ec560f2c8ce6cdc2fcdc2e68f7b2e5547ed3621"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.2.3"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.3.0"
         },
         "jeepney": {
             "hashes": [
                 "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
                 "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
             ],
             "markers": "sys_platform == 'linux'",
@@ -522,15 +514,15 @@
             "version": "==1.8.0"
         },
         "packaging": {
             "hashes": [
                 "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
-            "index": "pypi",
+            "markers": "python_version >= '3.7'",
             "version": "==23.1"
         },
         "pathspec": {
             "hashes": [
                 "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687",
                 "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
             ],
@@ -543,19 +535,19 @@
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc",
-                "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"
+                "sha256:cec7b889196b9144d088e4c57d9ceef7374f6c39694ad1577a0aab50d27ea28c",
+                "sha256:f87ca4fcff7d2b0f81c6a748a77973d7af0f4d526f98f308477c3c436c74d528"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.8.0"
+            "version": "==3.8.1"
         },
         "pluggy": {
             "hashes": [
                 "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
                 "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
             "markers": "python_version >= '3.7'",
@@ -692,34 +684,34 @@
                 "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==13.4.2"
         },
         "ruff": {
             "hashes": [
-                "sha256:0c4e6468da26f77b90cae35319d310999f471a8c352998e9b39937a23750149e",
-                "sha256:0dbdea02942131dbc15dd45f431d152224f15e1dd1859fcd0c0487b658f60f1a",
-                "sha256:1cc599022fe5ffb143a965b8d659eb64161ab8ab4433d208777eab018a1aab67",
-                "sha256:22efd9f41af27ef8fb9779462c46c35c89134d33e326c889971e10b2eaf50c63",
-                "sha256:2c09662112cfa22d7467a19252a546291fd0eae4f423e52b75a7a2000a1894db",
-                "sha256:508b13f7ca37274cceaba4fb3ea5da6ca192356323d92acf39462337c33ad14e",
-                "sha256:5206fc1cd8c1c1deadd2e6360c0dbcd690f1c845da588ca9d32e4a764a402c60",
-                "sha256:5859ee543b01b7eb67835dfd505faa8bb7cc1550f0295c92c1401b45b42be399",
-                "sha256:5e6554a072e7ce81eb6f0bec1cebd3dcb0e358652c0f4900d7d630d61691e914",
-                "sha256:6afb1c4422f24f361e877937e2a44b3f8176774a476f5e33845ebfe887dd5ec2",
-                "sha256:80043726662144876a381efaab88841c88e8df8baa69559f96b22d4fa216bef1",
-                "sha256:8347fc16aa185aae275906c4ac5b770e00c896b6a0acd5ba521f158801911998",
-                "sha256:a19ce3bea71023eee5f0f089dde4a4272d088d5ac0b675867e074983238ccc65",
-                "sha256:a63a0b645da699ae5c758fce19188e901b3033ec54d862d93fcd042addf7f38d",
-                "sha256:c8ace4d40a57b5ea3c16555f25a6b16bc5d8b2779ae1912ce2633543d4e9b1da",
-                "sha256:d9b264d78621bf7b698b6755d4913ab52c19bd28bee1a16001f954d64c1a1220",
-                "sha256:ec43658c64bfda44fd84bbea9da8c7a3b34f65448192d1c4dd63e9f4e7abfdd4"
+                "sha256:14a7b2f00f149c5a295f188a643ac25226ff8a4d08f7a62b1d4b0a1dc9f9b85c",
+                "sha256:2d4444c60f2e705c14cd802b55cd2b561d25bf4311702c463a002392d3116b22",
+                "sha256:2dab13cdedbf3af6d4427c07f47143746b6b95d9e4a254ac369a0edb9280a0d2",
+                "sha256:323b674c98078be9aaded5b8b51c0d9c424486566fb6ec18439b496ce79e5998",
+                "sha256:3250b24333ef419b7a232080d9724ccc4d2da1dbbe4ce85c4caa2290d83200f8",
+                "sha256:3a43fbe026ca1a2a8c45aa0d600a0116bec4dfa6f8bf0c3b871ecda51ef2b5dd",
+                "sha256:3e60605e07482183ba1c1b7237eca827bd6cbd3535fe8a4ede28cbe2a323cb97",
+                "sha256:468bfb0a7567443cec3d03cf408d6f562b52f30c3c29df19927f1e0e13a40cd7",
+                "sha256:479864a3ccd8a6a20a37a6e7577bdc2406868ee80b1e65605478ad3b8eb2ba0b",
+                "sha256:6fe81732f788894a00f6ade1fe69e996cc9e485b7c35b0f53fb00284397284b2",
+                "sha256:734165ea8feb81b0d53e3bf523adc2413fdb76f1264cde99555161dd5a725522",
+                "sha256:74e4b206cb24f2e98a615f87dbe0bde18105217cbcc8eb785bb05a644855ba50",
+                "sha256:7baa97c3d7186e5ed4d5d4f6834d759a27e56cf7d5874b98c507335f0ad5aadb",
+                "sha256:88d0f2afb2e0c26ac1120e7061ddda2a566196ec4007bd66d558f13b374b9efc",
+                "sha256:a9879f59f763cc5628aa01c31ad256a0f4dc61a29355c7315b83c2a5aac932b5",
+                "sha256:f32ec416c24542ca2f9cc8c8b65b84560530d338aaf247a4a78e74b99cd476b4",
+                "sha256:f612e0a14b3d145d90eb6ead990064e22f6f27281d847237560b4e10bf2251f3"
             ],
             "index": "pypi",
-            "version": "==0.0.275"
+            "version": "==0.0.277"
         },
         "secretstorage": {
             "hashes": [
                 "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
@@ -777,15 +769,15 @@
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
-                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
+                "sha256:1876cb065531855bbe83b6c489dcf69ecc28f1068d8e95959fe8bbc77774c941",
+                "sha256:5dadc3ad0a1f825fe42ce1bce0f2fc5a13af2e6b2d386af5b0ff295bc0a287d3"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.15.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.16.0"
         }
     }
 }
```

### Comparing `simple-git-versioning-0.1.1/README.md` & `simple-git-versioning-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -41,18 +41,15 @@
 
 ## Libraries
 
 Libraries that wish to expose their version number programatically may do so by
 including the following snippet:
 
 ```python
-try:
-    from importlib.metadata import version
-except ImportError:  # python<3.11
-    from importlib_metadata import version  # install_requires: `importlib-metadata`
+from importlib.metadata import version
 
 from versioning.pep440 import Project
 
 try:
     __version__ = version("simple-git-versioning")
 except PackageNotFoundError:
     # package is not installed
```

### Comparing `simple-git-versioning-0.1.1/pyproject.toml` & `simple-git-versioning-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 readme = "README.md"
 dynamic = ["dependencies", "version"]
 
 [project.urls]
 homepage = "https://gitlab.com/ypsah/simple-git-versioning"
@@ -42,15 +45,15 @@
 [tool.setuptools-pipfile]
 
 [tool.simple-git-versioning]
 setuptools = "pep440"
 
 [tool.black]
 line-length = 120
-target-version = ['py311']
+target-version = ['py38', 'py39', 'py310', 'py311']
 # enrole in feature-preview
 preview = true
 
 [tool.isort]
 profile = "black"
 src_paths = ["versioning", "tests"]
```

### Comparing `simple-git-versioning-0.1.1/simple_git_versioning.egg-info/PKG-INFO` & `simple-git-versioning-0.1.4/simple_git_versioning.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: simple-git-versioning
-Version: 0.1.1
+Version: 0.1.4
 Summary: Thinly scoped and opinionated tool that computes a version number from git tags and trailers
 Author-email: Quentin Bouget <ypsah@devyard.org>
 License: MIT
 Project-URL: homepage, https://gitlab.com/ypsah/simple-git-versioning
 Project-URL: repository, https://gitlab.com/ypsah/simple-git-versioning
 Keywords: versioning,git,git-trailers
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Opinionated version numbering CLIs, and library
 
@@ -62,18 +65,15 @@
 
 ## Libraries
 
 Libraries that wish to expose their version number programatically may do so by
 including the following snippet:
 
 ```python
-try:
-    from importlib.metadata import version
-except ImportError:  # python<3.11
-    from importlib_metadata import version  # install_requires: `importlib-metadata`
+from importlib.metadata import version
 
 from versioning.pep440 import Project
 
 try:
     __version__ = version("simple-git-versioning")
 except PackageNotFoundError:
     # package is not installed
```

### Comparing `simple-git-versioning-0.1.1/simple_git_versioning.egg-info/SOURCES.txt` & `simple-git-versioning-0.1.4/simple_git_versioning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.1/tests/unit/__init__.py` & `simple-git-versioning-0.1.4/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.1/tests/unit/test_cli.py` & `simple-git-versioning-0.1.4/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.1/tests/unit/test_pep440.py` & `simple-git-versioning-0.1.4/tests/unit/test_pep440.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.1/tests/unit/test_project.py` & `simple-git-versioning-0.1.4/tests/unit/test_project.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.1/tests/unit/test_semver2.py` & `simple-git-versioning-0.1.4/tests/unit/test_semver2.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.1/tests/unit/test_version.py` & `simple-git-versioning-0.1.4/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.1/versioning/__init__.py` & `simple-git-versioning-0.1.4/versioning/__init__.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.1/versioning/pep440.py` & `simple-git-versioning-0.1.4/versioning/pep440.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,24 @@
 
 import logging
 import re
 from argparse import ArgumentParser
 from contextlib import suppress
 from dataclasses import dataclass, replace
 from enum import Enum
-from functools import total_ordering, wraps
+from functools import partial, total_ordering, wraps
 from os import EX_DATAERR, EX_NOINPUT, EX_SOFTWARE, EX_USAGE
 from pathlib import Path
-from sys import stdout
-from typing import Any, ClassVar, Iterator, Protocol, Self
+from sys import stdout, version_info
+from typing import Any, ClassVar, Iterator, Protocol
+
+try:
+    from typing import Self
+except ImportError:  # python<3.11
+    from typing_extensions import Self
 
 from .project import (
     AmbiguousRoot,
     AmbiguousVersion,
     InvalidReference,
     InvalidVersionBumpTrailer,
     NotAGitWorkTree,
@@ -25,14 +30,17 @@
 from .project import Project as _Project
 from .version import InvalidVersion as _InvalidVersion
 from .version import Version as _Version
 from .version import VersionBump
 
 LOGGER = logging.getLogger(__name__)
 
+if version_info >= (3, 11):
+    dataclass = partial(dataclass, kw_only=True)
+
 
 class IllegalRelease(ValueError):
     """
     Raised when an operation results in making an illegal release
     """
 
 
@@ -54,29 +62,33 @@
     BETA = B
     RC = "rc"
     C = RC
     PRE = RC
     PREVIEW = RC
 
     def __str__(self) -> str:
-        match self:
-            case PreReleaseLabel.A | PreReleaseLabel.ALPHA:
-                return "alpha"
-            case PreReleaseLabel.B | PreReleaseLabel.BETA:
-                return "beta"
-            case PreReleaseLabel.C | PreReleaseLabel.RC | PreReleaseLabel.PRE | PreReleaseLabel.PREVIEW:
-                return "release candidate"
+        if self is PreReleaseLabel.A or self is PreReleaseLabel.ALPHA:
+            return "alpha"
+        if self is PreReleaseLabel.B or self is PreReleaseLabel.BETA:
+            return "beta"
+        if (
+            self is PreReleaseLabel.C
+            or self is PreReleaseLabel.RC
+            or self is PreReleaseLabel.PRE
+            or self is PreReleaseLabel.PREVIEW
+        ):
+            return "release candidate"
 
     def __lt__(self, other: Any) -> bool:
         if not isinstance(other, PreReleaseLabel):
             return NotImplemented
         return self.value.__lt__(other.value)
 
 
-@dataclass(order=True, frozen=True, kw_only=True)
+@dataclass(order=True, frozen=True)
 class PreRelease:
     """
     PEP440 pre-release: label + revision
     """
 
     label: PreReleaseLabel
     revision: int
@@ -129,15 +141,15 @@
         try:
             yield int(segment)
         except ValueError:
             yield segment
 
 
 @total_ordering
-@dataclass(frozen=True, kw_only=True)
+@dataclass(frozen=True)
 class Version(_Version):
     """
     PEP440 version
     """
 
     epoch: int = 0
     release: tuple[int, ...] = (0, 0, 0)
@@ -202,23 +214,22 @@
 
         dev = int(match.group("dev_n") or "0") if match.group("dev") else None
         local = tuple(_segment(match.group("local") or ""))
 
         return cls(epoch=epoch, release=release, pre=pre, post=post, dev=dev, local=local)
 
     def bump(self, bump: VersionBump) -> Self:
-        match bump:
-            case VersionBump.MAJOR:
-                return replace(self, release=(self.major + 1, 0, 0), pre=None, post=None, dev=None, local=())
-            case VersionBump.MINOR:
-                return replace(self, release=(self.major, self.minor + 1, 0), pre=None, post=None, dev=None, local=())
-            case VersionBump.PATCH:
-                return replace(
-                    self, release=(self.major, self.minor, self.patch + 1), pre=None, post=None, dev=None, local=()
-                )
+        if bump is VersionBump.MAJOR:
+            return replace(self, release=(self.major + 1, 0, 0), pre=None, post=None, dev=None, local=())
+        if bump is VersionBump.MINOR:
+            return replace(self, release=(self.major, self.minor + 1, 0), pre=None, post=None, dev=None, local=())
+        if bump is VersionBump.PATCH:
+            return replace(
+                self, release=(self.major, self.minor, self.patch + 1), pre=None, post=None, dev=None, local=()
+            )
 
     def __lt__(self, other: Any) -> bool:
         if not isinstance(other, Version):
             return NotImplemented
 
         if self.epoch < other.epoch:
             return True
@@ -268,14 +279,21 @@
             return isinstance(left, str)
         return len(self.local) < len(other.local)
 
 
 class Project(_Project[Version]):
     flavor = Version
 
+    if version_info < (3, 11):
+
+        def __init__(self, *args, path: Path, **kwargs):
+            super().__init__(*args, **kwargs)
+            self.path = path
+            self._pushed = []
+
     def release(
         self,
         reference: str = "HEAD",
         *,
         alpha: bool = False,
         beta: bool = False,
         rc: bool = False,
```

### Comparing `simple-git-versioning-0.1.1/versioning/project.py` & `simple-git-versioning-0.1.4/versioning/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 import os
 from abc import abstractmethod
 from collections import deque
 from collections.abc import Iterable, Iterator
 from contextlib import suppress
 from functools import cached_property
 from pathlib import Path
-from typing import Protocol, Self, TypeVar
+from typing import Protocol, TypeVar
+
+try:
+    from typing import Self
+except ImportError:  # python<3.11
+    from typing_extensions import Self
 
 from icontract import require
 from sh import Command, ErrorReturnCode_128, ErrorReturnCode_129
 from sh.contrib import git
 
 from .version import InvalidVersion, Version, VersionBump
```

### Comparing `simple-git-versioning-0.1.1/versioning/semver2.py` & `simple-git-versioning-0.1.4/versioning/semver2.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,28 +4,37 @@
 
 import logging
 import re
 from argparse import ArgumentParser
 from collections.abc import Iterator
 from contextlib import suppress
 from dataclasses import dataclass, field, replace
-from functools import total_ordering, wraps
+from functools import partial, total_ordering, wraps
 from os import EX_DATAERR, EX_NOINPUT, EX_SOFTWARE, EX_USAGE
 from pathlib import Path
-from sys import stdout
-from typing import Any, ClassVar, Protocol, Self
+from platform import python_version_tuple
+from sys import stdout, version_info
+from typing import Any, ClassVar, Protocol
+
+try:
+    from typing import Self
+except ImportError:  # python<3.11
+    from typing_extensions import Self
 
 from .project import InvalidVersionBumpTrailer, NotAGitWorkTree, NoVersion
 from .project import Project as _Project
 from .version import InvalidVersion as _InvalidVersion
 from .version import Version as _Version
 from .version import VersionBump
 
 LOGGER = logging.getLogger(__name__)
 
+if tuple(map(int, python_version_tuple())) >= (3, 11):
+    dataclass = partial(dataclass, kw_only=True)
+
 
 class InvalidVersion(_InvalidVersion):
     """
     Raised when an operation results in an invalid PEP440 version
     """
 
 
@@ -57,15 +66,15 @@
         try:
             yield int(identifier)
         except ValueError:
             yield identifier
 
 
 @total_ordering
-@dataclass(frozen=True, kw_only=True)
+@dataclass(frozen=True)
 class Version(_Version):
     """
     SemVer2 version
     """
 
     major: int = 0
     minor: int = 0
@@ -111,21 +120,20 @@
             minor=int(match.group("minor") or "0"),
             patch=int(match.group("patch") or "0"),
             pre=tuple(_identifierize(match.group("prerelease") or "")),
             build=match.group("buildmetadata") or "",
         )
 
     def bump(self, bump: VersionBump) -> Self:
-        match bump:
-            case VersionBump.MAJOR:
-                return replace(self, major=self.major + 1, minor=0, patch=0, pre=(), build="")
-            case VersionBump.MINOR:
-                return replace(self, minor=self.minor + 1, patch=0, pre=(), build="")
-            case VersionBump.PATCH:
-                return replace(self, patch=self.patch + 1, pre=(), build="")
+        if bump is VersionBump.MAJOR:
+            return replace(self, major=self.major + 1, minor=0, patch=0, pre=(), build="")
+        if bump is VersionBump.MINOR:
+            return replace(self, minor=self.minor + 1, patch=0, pre=(), build="")
+        if VersionBump.PATCH:
+            return replace(self, patch=self.patch + 1, pre=(), build="")
 
     def __lt__(self, other: Any) -> bool:
         if not isinstance(other, Version):
             return NotImplemented
 
         if self.major < other.major:
             return True
@@ -154,14 +162,21 @@
             return isinstance(left, int)
         return len(self.pre) < len(other.pre)
 
 
 class Project(_Project[Version]):
     flavor = Version
 
+    if version_info < (3, 11):
+
+        def __init__(self, *args, path: Path, **kwargs):
+            super().__init__(*args, **kwargs)
+            self.path = path
+            self._pushed = []
+
     def release(
         self,
         reference: str = "HEAD",
         *,
         pre: tuple[str | int, ...] = (),
         release: bool = False,
         build: str = "",
```

### Comparing `simple-git-versioning-0.1.1/versioning/setuptools.py` & `simple-git-versioning-0.1.4/versioning/setuptools.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import Distribution
 from versioning import pep440, semver2
 from versioning.project import NotAGitWorkTree, NoVersion
 
 LOGGER = logging.getLogger(__name__)
 
 
-def finalize_distribution_options(distribution: Distribution) -> None:
+def finalize_distribution_options(distribution: Distribution) -> None:  # pragma: no cover
     with open("pyproject.toml", mode="rb") as stream:
         pyproject = tomllib.load(stream)
 
     try:
         flavor = pyproject["tool"]["simple-git-versioning"]["setuptools"]
     except KeyError:
         LOGGER.debug("simple-git-versioning is not enabled")
```

### Comparing `simple-git-versioning-0.1.1/versioning/version.py` & `simple-git-versioning-0.1.4/versioning/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # SPDX-License-Identifier: MIT
 
 from abc import abstractmethod
 from enum import Enum
-from typing import Protocol, Self
+from typing import Protocol
+
+try:
+    from typing import Self
+except ImportError:  # python<3.11
+    from typing_extensions import Self
 
 
 class InvalidVersion(ValueError):
     """
     Raised when an operation results in an invalid version
     """
```

