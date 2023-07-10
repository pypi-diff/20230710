# Comparing `tmp/oras-0.1.18.tar.gz` & `tmp/oras-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oras-0.1.18.tar", last modified: Wed Jul  5 12:08:07 2023, max compression
+gzip compressed data, was "oras-0.1.19.tar", last modified: Mon Jul 10 16:16:20 2023, max compression
```

## Comparing `oras-0.1.18.tar` & `oras-0.1.19.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 12:08:07.042038 oras-0.1.18/
--rw-r--r--   0 runner    (1001) docker     (122)    11343 2023-07-05 12:07:29.000000 oras-0.1.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-05 12:07:29.000000 oras-0.1.18/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5736 2023-07-05 12:08:07.042038 oras-0.1.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4892 2023-07-05 12:07:29.000000 oras-0.1.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 12:08:07.038038 oras-0.1.18/oras/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-05 12:07:29.000000 oras-0.1.18/oras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-07-05 12:07:29.000000 oras-0.1.18/oras/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     7530 2023-07-05 12:07:29.000000 oras-0.1.18/oras/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3812 2023-07-05 12:07:29.000000 oras-0.1.18/oras/container.py
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-05 12:07:29.000000 oras-0.1.18/oras/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-05 12:07:29.000000 oras-0.1.18/oras/defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)     8737 2023-07-05 12:07:29.000000 oras-0.1.18/oras/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 12:08:07.042038 oras-0.1.18/oras/main/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 12:07:29.000000 oras-0.1.18/oras/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-05 12:07:29.000000 oras-0.1.18/oras/main/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     4470 2023-07-05 12:07:29.000000 oras-0.1.18/oras/oci.py
--rw-r--r--   0 runner    (1001) docker     (122)    35216 2023-07-05 12:07:29.000000 oras-0.1.18/oras/provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-07-05 12:07:29.000000 oras-0.1.18/oras/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 12:08:07.042038 oras-0.1.18/oras/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 12:07:29.000000 oras-0.1.18/oras/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-05 12:07:29.000000 oras-0.1.18/oras/tests/annotations.json
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-05 12:07:29.000000 oras-0.1.18/oras/tests/artifact.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      185 2023-07-05 12:07:29.000000 oras-0.1.18/oras/tests/run_registry.sh
--rw-r--r--   0 runner    (1001) docker     (122)     5066 2023-07-05 12:07:29.000000 oras-0.1.18/oras/tests/test_oras.py
--rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-07-05 12:07:29.000000 oras-0.1.18/oras/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-07-05 12:07:29.000000 oras-0.1.18/oras/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 12:08:07.042038 oras-0.1.18/oras/tests/upload_data/
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-05 12:07:29.000000 oras-0.1.18/oras/tests/upload_data/artifact.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 12:08:07.042038 oras-0.1.18/oras/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-05 12:07:29.000000 oras-0.1.18/oras/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8512 2023-07-05 12:07:29.000000 oras-0.1.18/oras/utils/fileio.py
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-05 12:07:29.000000 oras-0.1.18/oras/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (122)      985 2023-07-05 12:07:29.000000 oras-0.1.18/oras/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 12:08:07.042038 oras-0.1.18/oras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5736 2023-07-05 12:08:06.000000 oras-0.1.18/oras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-05 12:08:06.000000 oras-0.1.18/oras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 12:08:06.000000 oras-0.1.18/oras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 12:08:02.000000 oras-0.1.18/oras.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-05 12:08:06.000000 oras-0.1.18/oras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-05 12:08:06.000000 oras-0.1.18/oras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-05 12:07:29.000000 oras-0.1.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-07-05 12:08:07.042038 oras-0.1.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3370 2023-07-05 12:07:29.000000 oras-0.1.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 16:16:20.064996 oras-0.1.19/
+-rw-r--r--   0 runner    (1001) docker     (122)    11343 2023-07-10 16:15:49.000000 oras-0.1.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-10 16:15:49.000000 oras-0.1.19/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6083 2023-07-10 16:16:20.064996 oras-0.1.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5239 2023-07-10 16:15:49.000000 oras-0.1.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 16:16:20.060995 oras-0.1.19/oras/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-10 16:15:49.000000 oras-0.1.19/oras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-07-10 16:15:49.000000 oras-0.1.19/oras/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7530 2023-07-10 16:15:49.000000 oras-0.1.19/oras/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3812 2023-07-10 16:15:49.000000 oras-0.1.19/oras/container.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-10 16:15:49.000000 oras-0.1.19/oras/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-10 16:15:49.000000 oras-0.1.19/oras/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8737 2023-07-10 16:15:49.000000 oras-0.1.19/oras/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 16:16:20.064996 oras-0.1.19/oras/main/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 16:15:49.000000 oras-0.1.19/oras/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-10 16:15:49.000000 oras-0.1.19/oras/main/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4470 2023-07-10 16:15:49.000000 oras-0.1.19/oras/oci.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35645 2023-07-10 16:15:49.000000 oras-0.1.19/oras/provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-07-10 16:15:49.000000 oras-0.1.19/oras/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 16:16:20.064996 oras-0.1.19/oras/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/annotations.json
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/artifact.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      185 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/run_registry.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     5066 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/test_oras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 16:16:20.064996 oras-0.1.19/oras/tests/upload_data/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/upload_data/artifact.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 16:16:20.064996 oras-0.1.19/oras/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-10 16:15:49.000000 oras-0.1.19/oras/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10673 2023-07-10 16:15:49.000000 oras-0.1.19/oras/utils/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-10 16:15:49.000000 oras-0.1.19/oras/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      985 2023-07-10 16:15:49.000000 oras-0.1.19/oras/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 16:16:20.060995 oras-0.1.19/oras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6083 2023-07-10 16:16:19.000000 oras-0.1.19/oras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-10 16:16:19.000000 oras-0.1.19/oras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 16:16:19.000000 oras-0.1.19/oras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 16:16:16.000000 oras-0.1.19/oras.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-10 16:16:19.000000 oras-0.1.19/oras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-10 16:16:19.000000 oras-0.1.19/oras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-10 16:15:49.000000 oras-0.1.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-07-10 16:16:20.064996 oras-0.1.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3370 2023-07-10 16:15:49.000000 oras-0.1.19/setup.py
```

### Comparing `oras-0.1.18/LICENSE` & `oras-0.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `oras-0.1.18/PKG-INFO` & `oras-0.1.19/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oras
-Version: 0.1.18
+Version: 0.1.19
 Summary: OCI Registry as Storage Python SDK
 Home-page: https://github.com/oras-project/oras-py
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: oci,registry,storage
@@ -22,15 +22,15 @@
 Provides-Extra: tests
 Provides-Extra: docker
 License-File: LICENSE
 
 # ORAS Python
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-10-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-11-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ![ORAS Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/oras.png)
 
 OCI Registry as Storage enables libraries to push OCI Artifacts to [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries. This is a Python SDK for Python developers to empower them to do this in their applications.
 
 See our ⭐️ [Documentation](https://oras-project.github.io/oras-py/) ⭐️ to get started.
@@ -61,14 +61,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/magelisk"><img src="https://avatars.githubusercontent.com/u/18201513?v=4?s=100" width="100px;" alt="Matt Warner"/><br /><sub><b>Matt Warner</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=magelisk" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="wolfv.github.io"><img src="https://avatars.githubusercontent.com/u/885054?v=4?s=100" width="100px;" alt="Wolf Vollprecht"/><br /><sub><b>Wolf Vollprecht</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=wolfv" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/shizhMSFT"><img src="https://avatars.githubusercontent.com/u/32161882?v=4?s=100" width="100px;" alt="Shiwei Zhang"/><br /><sub><b>Shiwei Zhang</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=shizhMSFT" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jhlmco"><img src="https://avatars.githubusercontent.com/u/126677738?v=4?s=100" width="100px;" alt="jhlmco"/><br /><sub><b>jhlmco</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=jhlmco" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ananya2003Gupta"><img src="https://avatars.githubusercontent.com/u/90386813?v=4?s=100" width="100px;" alt="Ananya Gupta"/><br /><sub><b>Ananya Gupta</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=Ananya2003Gupta" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sunnycarter"><img src="https://avatars.githubusercontent.com/u/36891339?v=4?s=100" width="100px;" alt="sunnycarter"/><br /><sub><b>sunnycarter</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=sunnycarter" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
-Metadata-Version: 2.1 Name: oras Version: 0.1.18 Summary: OCI Registry as
+Metadata-Version: 2.1 Name: oras Version: 0.1.19 Summary: OCI Registry as
 Storage Python SDK Home-page: https://github.com/oras-project/oras-py Author:
 Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa
 Sochat License: LICENSE Keywords: oci,registry,storage Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
 Unix Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Description-Content-Type: text/markdown
 Provides-Extra: all Provides-Extra: tests Provides-Extra: docker License-File:
 LICENSE # ORAS Python  [![All Contributors](https://img.shields.io/badge/
-all_contributors-10-orange.svg?style=flat-square)](#contributors-)  ![ORAS
+all_contributors-11-orange.svg?style=flat-square)](#contributors-)  ![ORAS
 Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/
 oras.png) OCI Registry as Storage enables libraries to push OCI Artifacts to
 [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries.
 This is a Python SDK for Python developers to empower them to do this in their
 applications. See our â­ï¸ [Documentation](https://oras-project.github.io/
 oras-py/) â­ï¸ to get started. ## Code of Conduct Please note that this
 project has adopted the [CNCF Code of Conduct](https://github.com/cncf/
 foundation/blob/master/code-of-conduct.md). Please follow it in all your
 interactions with the project members and users. ## ðï¸ Contributors
 ðï¸ We use the [all-contributors](https://github.com/all-contributors/all-
 contributors) tool to generate a contributors graphic below.
-[Vanessasaurus] [Lachlan  [Steve    [Josh   [Bridget     [Matt       [Wolf
- Vanessasaurus  Evenson] Lasker]  Dolitsky] Kromhout]   Warner]   Vollprecht]
-     ð»   Lachlan   Steve     Josh     Bridget  Matt_Warner    Wolf
-                Evenson   Lasker  Dolitsky  Kromhout     ð» Vollprecht
-                  ð�  ð�  ð»  ð»               ð»
-[Shiwei_Zhang]  [jhlmco] [Ananya
- Shiwei_Zhang    jhlmco   Gupta]
-     ð»     ð� Ananya
+[Vanessasaurus] [Lachlan  [Steve      [Josh     [Bridget   [Matt      [Wolf
+ Vanessasaurus  Evenson] Lasker]    Dolitsky]   Kromhout] Warner]  Vollprecht]
+     ð»   Lachlan   Steve   Josh_Dolitsky  Bridget    Matt      Wolf
+                Evenson   Lasker      ð»  Kromhout   Warner  Vollprecht
+                  ð�  ð»               ð»  ð�   ð»
+[Shiwei_Zhang]  [jhlmco] [Ananya  [sunnycarter]
+ Shiwei_Zhang    jhlmco   Gupta]   sunnycarter
+     ð»     ð� Ananya      ð»
                           Gupta
                            ð»
    ## License This code is licensed under the Apache 2.0 [LICENSE](LICENSE).
```

### Comparing `oras-0.1.18/README.md` & `oras-0.1.19/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ORAS Python
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-10-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-11-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ![ORAS Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/oras.png)
 
 OCI Registry as Storage enables libraries to push OCI Artifacts to [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries. This is a Python SDK for Python developers to empower them to do this in their applications.
 
 See our ⭐️ [Documentation](https://oras-project.github.io/oras-py/) ⭐️ to get started.
@@ -36,14 +36,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/magelisk"><img src="https://avatars.githubusercontent.com/u/18201513?v=4?s=100" width="100px;" alt="Matt Warner"/><br /><sub><b>Matt Warner</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=magelisk" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="wolfv.github.io"><img src="https://avatars.githubusercontent.com/u/885054?v=4?s=100" width="100px;" alt="Wolf Vollprecht"/><br /><sub><b>Wolf Vollprecht</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=wolfv" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/shizhMSFT"><img src="https://avatars.githubusercontent.com/u/32161882?v=4?s=100" width="100px;" alt="Shiwei Zhang"/><br /><sub><b>Shiwei Zhang</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=shizhMSFT" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jhlmco"><img src="https://avatars.githubusercontent.com/u/126677738?v=4?s=100" width="100px;" alt="jhlmco"/><br /><sub><b>jhlmco</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=jhlmco" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ananya2003Gupta"><img src="https://avatars.githubusercontent.com/u/90386813?v=4?s=100" width="100px;" alt="Ananya Gupta"/><br /><sub><b>Ananya Gupta</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=Ananya2003Gupta" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sunnycarter"><img src="https://avatars.githubusercontent.com/u/36891339?v=4?s=100" width="100px;" alt="sunnycarter"/><br /><sub><b>sunnycarter</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=sunnycarter" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
 # ORAS Python  [![All Contributors](https://img.shields.io/badge/
-all_contributors-10-orange.svg?style=flat-square)](#contributors-)  ![ORAS
+all_contributors-11-orange.svg?style=flat-square)](#contributors-)  ![ORAS
 Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/
 oras.png) OCI Registry as Storage enables libraries to push OCI Artifacts to
 [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries.
 This is a Python SDK for Python developers to empower them to do this in their
 applications. See our â­ï¸ [Documentation](https://oras-project.github.io/
 oras-py/) â­ï¸ to get started. ## Code of Conduct Please note that this
 project has adopted the [CNCF Code of Conduct](https://github.com/cncf/
 foundation/blob/master/code-of-conduct.md). Please follow it in all your
 interactions with the project members and users. ## ðï¸ Contributors
 ðï¸ We use the [all-contributors](https://github.com/all-contributors/all-
 contributors) tool to generate a contributors graphic below.
-[Vanessasaurus] [Lachlan  [Steve    [Josh   [Bridget     [Matt       [Wolf
- Vanessasaurus  Evenson] Lasker]  Dolitsky] Kromhout]   Warner]   Vollprecht]
-     ð»   Lachlan   Steve     Josh     Bridget  Matt_Warner    Wolf
-                Evenson   Lasker  Dolitsky  Kromhout     ð» Vollprecht
-                  ð�  ð�  ð»  ð»               ð»
-[Shiwei_Zhang]  [jhlmco] [Ananya
- Shiwei_Zhang    jhlmco   Gupta]
-     ð»     ð� Ananya
+[Vanessasaurus] [Lachlan  [Steve      [Josh     [Bridget   [Matt      [Wolf
+ Vanessasaurus  Evenson] Lasker]    Dolitsky]   Kromhout] Warner]  Vollprecht]
+     ð»   Lachlan   Steve   Josh_Dolitsky  Bridget    Matt      Wolf
+                Evenson   Lasker      ð»  Kromhout   Warner  Vollprecht
+                  ð�  ð»               ð»  ð�   ð»
+[Shiwei_Zhang]  [jhlmco] [Ananya  [sunnycarter]
+ Shiwei_Zhang    jhlmco   Gupta]   sunnycarter
+     ð»     ð� Ananya      ð»
                           Gupta
                            ð»
    ## License This code is licensed under the Apache 2.0 [LICENSE](LICENSE).
```

### Comparing `oras-0.1.18/oras/auth.py` & `oras-0.1.19/oras/auth.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.18/oras/client.py` & `oras-0.1.19/oras/client.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.18/oras/container.py` & `oras-0.1.19/oras/container.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.18/oras/decorator.py` & `oras-0.1.19/oras/decorator.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.18/oras/defaults.py` & `oras-0.1.19/oras/defaults.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.18/oras/logger.py` & `oras-0.1.19/oras/logger.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.18/oras/main/login.py` & `oras-0.1.19/oras/main/login.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.18/oras/oci.py` & `oras-0.1.19/oras/oci.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.18/oras/provider.py` & `oras-0.1.19/oras/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import oras.auth
 import oras.container
 import oras.decorator as decorator
 import oras.oci
 import oras.schemas
 import oras.utils
 from oras.logger import logger
+from oras.utils.fileio import PathAndOptionalContent
 
 # container type can be string or container
 container_type = Union[str, oras.container.Container]
 
 
 class Registry:
     """
@@ -160,30 +161,33 @@
         Ensure a blob path is in the present working directory or below.
 
         :param path: the path to validate
         :type path: str
         """
         return os.getcwd() in os.path.abspath(path)
 
-    def _parse_manifest_ref(self, ref: str) -> Union[Tuple[str, str], List[str]]:
+    def _parse_manifest_ref(self, ref: str) -> Tuple[str, str]:
         """
-        Parse an optional manifest config, e.g:
+        Parse an optional manifest config.
 
         Examples
         --------
         <path>:<content-type>
         path/to/config:application/vnd.oci.image.config.v1+json
         /dev/null:application/vnd.oci.image.config.v1+json
 
         :param ref: the manifest reference to parse (examples above)
         :type ref: str
+        :return - A Tuple of the path and the content-type, using the default unknown
+                  config media type if none found in the reference
         """
-        if ":" not in ref:
-            return ref, oras.defaults.unknown_config_media_type
-        return ref.split(":", 1)
+        path_content: PathAndOptionalContent = oras.utils.split_path_and_content(ref)
+        if not path_content.content:
+            path_content.content = oras.defaults.unknown_config_media_type
+        return path_content.path, path_content.content
 
     def upload_blob(
         self,
         blob: str,
         container: container_type,
         layer: dict,
         do_chunked: bool = False,
@@ -633,16 +637,19 @@
         # A lookup of annotations we can add (to blobs or manifest)
         annotset = oras.oci.Annotations(kwargs.get("annotation_file"))
         media_type = None
 
         # Upload files as blobs
         for blob in kwargs.get("files", []):
             # You can provide a blob + content type
-            if ":" in str(blob):
-                blob, media_type = str(blob).split(":", 1)
+            path_content: PathAndOptionalContent = oras.utils.split_path_and_content(
+                str(blob)
+            )
+            blob = path_content.path
+            media_type = path_content.content
 
             # Must exist
             if not os.path.exists(blob):
                 raise FileNotFoundError(f"{blob} does not exist.")
 
             # Path validation means blob must be relative to PWD.
             if validate_path:
```

### Comparing `oras-0.1.18/oras/schemas.py` & `oras-0.1.19/oras/schemas.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.18/oras/tests/test_oras.py` & `oras-0.1.19/oras/tests/test_oras.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.18/oras/tests/test_utils.py` & `oras-0.1.19/oras/tests/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -98,7 +98,35 @@
     assert os.path.exists(result)
 
 
 def test_print_json():
     print("Testing utils.print_json")
     result = utils.print_json({1: 1})
     assert result == '{\n    "1": 1\n}'
+
+
+def test_split_path_and_content():
+    """
+    Test split path and content function.
+
+    Function has additional logic for Windows - this isn't included in these tests as
+    they don't usually run on Windows.
+    """
+    testref = "path/to/config:application/vnd.oci.image.config.v1+json"
+    path_content = utils.split_path_and_content(testref)
+    assert path_content.path == "path/to/config"
+    assert path_content.content == "application/vnd.oci.image.config.v1+json"
+
+    testref = "/dev/null:application/vnd.oci.image.config.v1+json"
+    path_content = utils.split_path_and_content(testref)
+    assert path_content.path == "/dev/null"
+    assert path_content.content == "application/vnd.oci.image.config.v1+json"
+
+    testref = "/dev/null"
+    path_content = utils.split_path_and_content(testref)
+    assert path_content.path == "/dev/null"
+    assert not path_content.content
+
+    testref = "path/to/config.json"
+    path_content = utils.split_path_and_content(testref)
+    assert path_content.path == "path/to/config.json"
+    assert not path_content.content
```

### Comparing `oras-0.1.18/oras/utils/request.py` & `oras-0.1.19/oras/utils/request.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.18/oras/version.py` & `oras-0.1.19/oras/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Vanessa Sochat"
 __copyright__ = "Copyright The ORAS Authors."
 __license__ = "Apache-2.0"
 
-__version__ = "0.1.18"
+__version__ = "0.1.19"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "oras"
 PACKAGE_URL = "https://github.com/oras-project/oras-py"
 KEYWORDS = "oci, registry, storage"
 DESCRIPTION = "OCI Registry as Storage Python SDK"
 LICENSE = "LICENSE"
```

### Comparing `oras-0.1.18/oras.egg-info/PKG-INFO` & `oras-0.1.19/oras.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oras
-Version: 0.1.18
+Version: 0.1.19
 Summary: OCI Registry as Storage Python SDK
 Home-page: https://github.com/oras-project/oras-py
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: oci,registry,storage
@@ -22,15 +22,15 @@
 Provides-Extra: tests
 Provides-Extra: docker
 License-File: LICENSE
 
 # ORAS Python
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-10-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-11-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ![ORAS Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/oras.png)
 
 OCI Registry as Storage enables libraries to push OCI Artifacts to [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries. This is a Python SDK for Python developers to empower them to do this in their applications.
 
 See our ⭐️ [Documentation](https://oras-project.github.io/oras-py/) ⭐️ to get started.
@@ -61,14 +61,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/magelisk"><img src="https://avatars.githubusercontent.com/u/18201513?v=4?s=100" width="100px;" alt="Matt Warner"/><br /><sub><b>Matt Warner</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=magelisk" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="wolfv.github.io"><img src="https://avatars.githubusercontent.com/u/885054?v=4?s=100" width="100px;" alt="Wolf Vollprecht"/><br /><sub><b>Wolf Vollprecht</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=wolfv" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/shizhMSFT"><img src="https://avatars.githubusercontent.com/u/32161882?v=4?s=100" width="100px;" alt="Shiwei Zhang"/><br /><sub><b>Shiwei Zhang</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=shizhMSFT" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jhlmco"><img src="https://avatars.githubusercontent.com/u/126677738?v=4?s=100" width="100px;" alt="jhlmco"/><br /><sub><b>jhlmco</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=jhlmco" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ananya2003Gupta"><img src="https://avatars.githubusercontent.com/u/90386813?v=4?s=100" width="100px;" alt="Ananya Gupta"/><br /><sub><b>Ananya Gupta</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=Ananya2003Gupta" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sunnycarter"><img src="https://avatars.githubusercontent.com/u/36891339?v=4?s=100" width="100px;" alt="sunnycarter"/><br /><sub><b>sunnycarter</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=sunnycarter" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
-Metadata-Version: 2.1 Name: oras Version: 0.1.18 Summary: OCI Registry as
+Metadata-Version: 2.1 Name: oras Version: 0.1.19 Summary: OCI Registry as
 Storage Python SDK Home-page: https://github.com/oras-project/oras-py Author:
 Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa
 Sochat License: LICENSE Keywords: oci,registry,storage Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
 Unix Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Description-Content-Type: text/markdown
 Provides-Extra: all Provides-Extra: tests Provides-Extra: docker License-File:
 LICENSE # ORAS Python  [![All Contributors](https://img.shields.io/badge/
-all_contributors-10-orange.svg?style=flat-square)](#contributors-)  ![ORAS
+all_contributors-11-orange.svg?style=flat-square)](#contributors-)  ![ORAS
 Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/
 oras.png) OCI Registry as Storage enables libraries to push OCI Artifacts to
 [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries.
 This is a Python SDK for Python developers to empower them to do this in their
 applications. See our â­ï¸ [Documentation](https://oras-project.github.io/
 oras-py/) â­ï¸ to get started. ## Code of Conduct Please note that this
 project has adopted the [CNCF Code of Conduct](https://github.com/cncf/
 foundation/blob/master/code-of-conduct.md). Please follow it in all your
 interactions with the project members and users. ## ðï¸ Contributors
 ðï¸ We use the [all-contributors](https://github.com/all-contributors/all-
 contributors) tool to generate a contributors graphic below.
-[Vanessasaurus] [Lachlan  [Steve    [Josh   [Bridget     [Matt       [Wolf
- Vanessasaurus  Evenson] Lasker]  Dolitsky] Kromhout]   Warner]   Vollprecht]
-     ð»   Lachlan   Steve     Josh     Bridget  Matt_Warner    Wolf
-                Evenson   Lasker  Dolitsky  Kromhout     ð» Vollprecht
-                  ð�  ð�  ð»  ð»               ð»
-[Shiwei_Zhang]  [jhlmco] [Ananya
- Shiwei_Zhang    jhlmco   Gupta]
-     ð»     ð� Ananya
+[Vanessasaurus] [Lachlan  [Steve      [Josh     [Bridget   [Matt      [Wolf
+ Vanessasaurus  Evenson] Lasker]    Dolitsky]   Kromhout] Warner]  Vollprecht]
+     ð»   Lachlan   Steve   Josh_Dolitsky  Bridget    Matt      Wolf
+                Evenson   Lasker      ð»  Kromhout   Warner  Vollprecht
+                  ð�  ð»               ð»  ð�   ð»
+[Shiwei_Zhang]  [jhlmco] [Ananya  [sunnycarter]
+ Shiwei_Zhang    jhlmco   Gupta]   sunnycarter
+     ð»     ð� Ananya      ð»
                           Gupta
                            ð»
    ## License This code is licensed under the Apache 2.0 [LICENSE](LICENSE).
```

### Comparing `oras-0.1.18/oras.egg-info/SOURCES.txt` & `oras-0.1.19/oras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oras-0.1.18/setup.py` & `oras-0.1.19/setup.py`

 * *Files identical despite different names*

