# Comparing `tmp/simple-git-versioning-0.0.4.tar.gz` & `tmp/simple-git-versioning-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-git-versioning-0.0.4.tar", last modified: Sun Feb  5 23:21:57 2023, max compression
+gzip compressed data, was "simple-git-versioning-0.1.0.tar", last modified: Mon Jul 10 20:02:26 2023, max compression
```

## Comparing `simple-git-versioning-0.0.4.tar` & `simple-git-versioning-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 23:21:57.839543 simple-git-versioning-0.0.4/
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     4677 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      887 2023-02-05 23:21:57.839543 simple-git-versioning-0.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/Pipfile
--rw-rw-rw-   0 root         (0) root         (0)    38283 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/Pipfile.lock
--rw-rw-rw-   0 root         (0) root         (0)     1452 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-05 23:21:57.840460 simple-git-versioning-0.0.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 23:21:57.837710 simple-git-versioning-0.0.4/simple_git_versioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)      887 2023-02-05 23:21:57.000000 simple-git-versioning-0.0.4/simple_git_versioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      455 2023-02-05 23:21:57.000000 simple-git-versioning-0.0.4/simple_git_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-05 23:21:57.000000 simple-git-versioning-0.0.4/simple_git_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-02-05 23:21:57.000000 simple-git-versioning-0.0.4/simple_git_versioning.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-05 23:21:57.000000 simple-git-versioning-0.0.4/simple_git_versioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-02-05 23:21:57.000000 simple-git-versioning-0.0.4/simple_git_versioning.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 23:21:57.838626 simple-git-versioning-0.0.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 23:21:57.838626 simple-git-versioning-0.0.4/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6274 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/tests/unit/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 23:21:57.839543 simple-git-versioning-0.0.4/versioning/
--rw-rw-rw-   0 root         (0) root         (0)     3323 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/versioning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/versioning/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:02:26.741561 simple-git-versioning-0.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5175 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3840 2023-07-10 20:02:26.741561 simple-git-versioning-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/Pipfile
+-rw-rw-rw-   0 root         (0) root         (0)    46710 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/Pipfile.lock
+-rw-rw-rw-   0 root         (0) root         (0)     2974 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 20:02:26.741561 simple-git-versioning-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:02:26.738561 simple-git-versioning-0.1.0/simple_git_versioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3840 2023-07-10 20:02:26.000000 simple-git-versioning-0.1.0/simple_git_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      681 2023-07-10 20:02:26.000000 simple-git-versioning-0.1.0/simple_git_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 20:02:26.000000 simple-git-versioning-0.1.0/simple_git_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-10 20:02:26.000000 simple-git-versioning-0.1.0/simple_git_versioning.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-10 20:02:26.000000 simple-git-versioning-0.1.0/simple_git_versioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-10 20:02:26.000000 simple-git-versioning-0.1.0/simple_git_versioning.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:02:26.738561 simple-git-versioning-0.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:02:26.739561 simple-git-versioning-0.1.0/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)     7368 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/tests/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/tests/unit/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    10566 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/tests/unit/test_pep440.py
+-rw-rw-rw-   0 root         (0) root         (0)    14420 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/tests/unit/test_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     3196 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/tests/unit/test_semver2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3248 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/tests/unit/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:02:26.740561 simple-git-versioning-0.1.0/versioning/
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/versioning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14854 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/versioning/pep440.py
+-rw-rw-rw-   0 root         (0) root         (0)     7746 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/versioning/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     8643 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/versioning/semver2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2040 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/versioning/setuptools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1146 2023-07-10 20:02:11.000000 simple-git-versioning-0.1.0/versioning/version.py
```

### Comparing `simple-git-versioning-0.0.4/.gitlab-ci.yml` & `simple-git-versioning-0.1.0/.gitlab-ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # SPDX-License-Identifier: MIT
 
 stages:
-  - venv
   - static-analysis
   - build
   - test
   - release
 
 ################################################################################
 #                                   DEFAULTS                                   #
@@ -17,57 +16,64 @@
 
 default:
   image: python:3.11
   cache: &cache
     key: $CI_COMMIT_REF_SLUG
     paths:
       - .cache/pip
+      - .venv
     policy: pull
   before_script:
     - python --version
     - pip install --user pipenv
     - export PATH="$PATH:${XDG_DATA_HOME:-$HOME/.local}/bin"
     - export PIPENV_VENV_IN_PROJECT=true
+    - pipenv sync --dev
 
 ################################################################################
 #                                     .PRE                                     #
 ################################################################################
 
 virtualenv:
-  stage: venv
+  stage: .pre
   cache:
     <<: *cache
     policy: pull-push
+  rules:
+    - when: on_success  # https://gitlab.com/gitlab-org/gitlab-runner/-/issues/5970
   script:
     - pipenv sync --dev
-  artifacts:
-    name: virtualenv
-    paths:
-      - .venv
-    expire_in: 1 day
 
 ################################################################################
 #                               STATIC-ANALYSIS                                #
 ################################################################################
 
 black:
   stage: static-analysis
   rules:
     - if: $CI_PIPELINE_SOURCE == 'merge_request_event'
   script:
     - git fetch origin "$CI_MERGE_REQUEST_TARGET_BRANCH_NAME"
-    - git rebase -x 'pipenv run black --check .' origin/"$CI_MERGE_REQUEST_TARGET_BRANCH_NAME"
+    - pipenv run pre-commit run black --show-diff-on-failure --from-ref origin/"$CI_MERGE_REQUEST_TARGET_BRANCH_NAME" --to-ref HEAD
 
 isort:
   stage: static-analysis
   rules:
     - if: $CI_PIPELINE_SOURCE == 'merge_request_event'
   script:
     - git fetch origin "$CI_MERGE_REQUEST_TARGET_BRANCH_NAME"
-    - git rebase -x 'pipenv run isort --check .' origin/"$CI_MERGE_REQUEST_TARGET_BRANCH_NAME"
+    - pipenv run pre-commit run isort --show-diff-on-failure --from-ref origin/"$CI_MERGE_REQUEST_TARGET_BRANCH_NAME" --to-ref HEAD
+
+ruff:
+  stage: static-analysis
+  rules:
+    - if: $CI_PIPELINE_SOURCE == 'merge_request_event'
+  script:
+    - git fetch origin "$CI_MERGE_REQUEST_TARGET_BRANCH_NAME"
+    - pipenv run pre-commit run ruff --show-diff-on-failure --from-ref origin/"$CI_MERGE_REQUEST_TARGET_BRANCH_NAME" --to-ref HEAD
 
 pipenv-verify:
   stage: static-analysis
   rules:
     - if: $CI_PIPELINE_SOURCE == 'merge_request_event'
   script:
     - git fetch origin "$CI_MERGE_REQUEST_TARGET_BRANCH_NAME"
@@ -111,15 +117,16 @@
 
 pytest:
   stage: test
   rules:
     - if: $CI_PIPELINE_SOURCE == 'merge_request_event'
   script:
     - git fetch origin "$CI_MERGE_REQUEST_TARGET_BRANCH_NAME"
-    - git rebase -x 'pipenv run pytest --cov-report=xml --junit-xml=unit-test-report.xml' origin/"$CI_MERGE_REQUEST_TARGET_BRANCH_NAME"
+    - pipenv run pytest --cov-report=xml --junit-xml=unit-test-report.xml
+    # - git rebase -x 'pipenv run pytest --cov-report=xml --junit-xml=unit-test-report.xml' origin/"$CI_MERGE_REQUEST_TARGET_BRANCH_NAME"
   coverage: '/(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/'
   artifacts:
     reports:
       coverage_report:
         coverage_format: cobertura
         path: coverage.xml
       junit: unit-test-report.xml
@@ -131,15 +138,15 @@
 tag:
   stage: release
   interruptible: false
   resource_group: tagging
   rules:
     - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH
   script:
-    - version=$(pipenv run python -m versioning)
+    - version=$(pipenv run python -m versioning.pep440)
     - git config user.email "$GITLAB_USER_EMAIL"
     - git config user.name "$GITLAB_USER_NAME"
     - git tag -a "$version" -m "version $version"
     - git push --tag "$CI_SERVER_PROTOCOL://oauth2:$TAG_TOKEN@$CI_SERVER_HOST:$CI_SERVER_PORT/$CI_PROJECT_PATH"
 
 publish:
   stage: release
```

### Comparing `simple-git-versioning-0.0.4/LICENSE` & `simple-git-versioning-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.0.4/Pipfile.lock` & `simple-git-versioning-0.1.0/Pipfile.lock`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8164595516569201%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'5c6a6529c0656e988373e48ebf38139e2c7283e595ea45eab2a03fffec0b3c01'}}",*

 * * "'default'": "{'packaging': {'hashes': "*

 * *              "['sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61', "*

 * *              "'sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f'], "*

 * *              "'version': '==23.1'}, 'sh': {'hashes': "*

 * *              "['sha256:14265a4cd1622429edcf300292ec98193530fb143fe642b3437024eca9bee8c5', "*

 * *              "' […]*

```diff
@@ -1,78 +1,110 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "eaa1beb0a29573daa054d3ffae3583df8a1ccf6389a02a288f6211476e1f7b7c"
+            "sha256": "5c6a6529c0656e988373e48ebf38139e2c7283e595ea45eab2a03fffec0b3c01"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
+        "asttokens": {
+            "hashes": [
+                "sha256:4622110b2a6f30b77e1473affaa97e711bc2f07d3f10848420ff1898edbe94f3",
+                "sha256:6b0ac9e93fb0335014d382b8fa9b3afa7df546984258005da0b9e7095b3deb1c"
+            ],
+            "version": "==2.2.1"
+        },
+        "icontract": {
+            "hashes": [
+                "sha256:1a441dad41c9a0615c6ae96464190eddccd2de8153254059ff18ffd7b3b84800",
+                "sha256:b87d2b33eb5d7f2c9a5af4770d6d106560c9688c79a821e5fe1bbd41188f5dcc"
+            ],
+            "index": "pypi",
+            "version": "==2.6.2"
+        },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "index": "pypi",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "sh": {
             "hashes": [
-                "sha256:e4045b6c732d9ce75d571c79f5ac2234edd9ae4f5fa9d59b09705082bdca18c7"
+                "sha256:14265a4cd1622429edcf300292ec98193530fb143fe642b3437024eca9bee8c5",
+                "sha256:a18920f0839991bc9dfddb6dcc006c360b1064ba96257359f0ea356e9fa75a60"
             ],
             "index": "pypi",
-            "version": "==1.14.3"
+            "version": "==2.0.4"
+        },
+        "six": {
+            "hashes": [
+                "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
+                "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.16.0"
+        },
+        "typing-extensions": {
+            "hashes": [
+                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
+                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==4.6.3"
         }
     },
     "develop": {
         "attrs": {
             "hashes": [
-                "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
-                "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
+                "sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04",
+                "sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==22.2.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==23.1.0"
         },
         "black": {
             "hashes": [
-                "sha256:0052dba51dec07ed029ed61b18183942043e00008ec65d5028814afaab9a22fd",
-                "sha256:0680d4380db3719ebcfb2613f34e86c8e6d15ffeabcf8ec59355c5e7b85bb555",
-                "sha256:121ca7f10b4a01fd99951234abdbd97728e1240be89fde18480ffac16503d481",
-                "sha256:162e37d49e93bd6eb6f1afc3e17a3d23a823042530c37c3c42eeeaf026f38468",
-                "sha256:2a951cc83ab535d248c89f300eccbd625e80ab880fbcfb5ac8afb5f01a258ac9",
-                "sha256:2bf649fda611c8550ca9d7592b69f0637218c2369b7744694c5e4902873b2f3a",
-                "sha256:382998821f58e5c8238d3166c492139573325287820963d2f7de4d518bd76958",
-                "sha256:49f7b39e30f326a34b5c9a4213213a6b221d7ae9d58ec70df1c4a307cf2a1580",
-                "sha256:57c18c5165c1dbe291d5306e53fb3988122890e57bd9b3dcb75f967f13411a26",
-                "sha256:7a0f701d314cfa0896b9001df70a530eb2472babb76086344e688829efd97d32",
-                "sha256:8178318cb74f98bc571eef19068f6ab5613b3e59d4f47771582f04e175570ed8",
-                "sha256:8b70eb40a78dfac24842458476135f9b99ab952dd3f2dab738c1881a9b38b753",
-                "sha256:9880d7d419bb7e709b37e28deb5e68a49227713b623c72b2b931028ea65f619b",
-                "sha256:9afd3f493666a0cd8f8df9a0200c6359ac53940cbde049dcb1a7eb6ee2dd7074",
-                "sha256:a29650759a6a0944e7cca036674655c2f0f63806ddecc45ed40b7b8aa314b651",
-                "sha256:a436e7881d33acaf2536c46a454bb964a50eff59b21b51c6ccf5a40601fbef24",
-                "sha256:a59db0a2094d2259c554676403fa2fac3473ccf1354c1c63eccf7ae65aac8ab6",
-                "sha256:a8471939da5e824b891b25751955be52ee7f8a30a916d570a5ba8e0f2eb2ecad",
-                "sha256:b0bd97bea8903f5a2ba7219257a44e3f1f9d00073d6cc1add68f0beec69692ac",
-                "sha256:b6a92a41ee34b883b359998f0c8e6eb8e99803aa8bf3123bf2b2e6fec505a221",
-                "sha256:bb460c8561c8c1bec7824ecbc3ce085eb50005883a6203dcfb0122e95797ee06",
-                "sha256:bfffba28dc52a58f04492181392ee380e95262af14ee01d4bc7bb1b1c6ca8d27",
-                "sha256:c1c476bc7b7d021321e7d93dc2cbd78ce103b84d5a4cf97ed535fbc0d6660648",
-                "sha256:c91dfc2c2a4e50df0026f88d2215e166616e0c80e86004d0003ece0488db2739",
-                "sha256:e6663f91b6feca5d06f2ccd49a10f254f9298cc1f7f49c46e498a0771b507104"
+                "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5",
+                "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915",
+                "sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326",
+                "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940",
+                "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b",
+                "sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30",
+                "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c",
+                "sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c",
+                "sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab",
+                "sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27",
+                "sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2",
+                "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961",
+                "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9",
+                "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb",
+                "sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70",
+                "sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331",
+                "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2",
+                "sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266",
+                "sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d",
+                "sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6",
+                "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b",
+                "sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925",
+                "sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8",
+                "sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4",
+                "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"
             ],
             "index": "pypi",
-            "version": "==23.1.0"
+            "version": "==23.3.0"
         },
         "bleach": {
             "hashes": [
                 "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414",
                 "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
@@ -84,19 +116,19 @@
                 "sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269"
             ],
             "index": "pypi",
             "version": "==0.10.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -159,227 +191,259 @@
                 "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6",
                 "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b",
                 "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
                 "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
             ],
             "version": "==1.15.1"
         },
+        "cfgv": {
+            "hashes": [
+                "sha256:c6a0883f3917a037485059700b9e75da2464e6c27051014ad85ba6aaa5884426",
+                "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"
+            ],
+            "markers": "python_full_version >= '3.6.1'",
+            "version": "==3.3.1"
+        },
         "charset-normalizer": {
             "hashes": [
-                "sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b",
-                "sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42",
-                "sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d",
-                "sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b",
-                "sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a",
-                "sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59",
-                "sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154",
-                "sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1",
-                "sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c",
-                "sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a",
-                "sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d",
-                "sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6",
-                "sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b",
-                "sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b",
-                "sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783",
-                "sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5",
-                "sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918",
-                "sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555",
-                "sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639",
-                "sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786",
-                "sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e",
-                "sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed",
-                "sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820",
-                "sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8",
-                "sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3",
-                "sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541",
-                "sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14",
-                "sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be",
-                "sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e",
-                "sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76",
-                "sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b",
-                "sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c",
-                "sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b",
-                "sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3",
-                "sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc",
-                "sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6",
-                "sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59",
-                "sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4",
-                "sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d",
-                "sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d",
-                "sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3",
-                "sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a",
-                "sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea",
-                "sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6",
-                "sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e",
-                "sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603",
-                "sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24",
-                "sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a",
-                "sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58",
-                "sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678",
-                "sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a",
-                "sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c",
-                "sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6",
-                "sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18",
-                "sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174",
-                "sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317",
-                "sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f",
-                "sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc",
-                "sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837",
-                "sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41",
-                "sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c",
-                "sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579",
-                "sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753",
-                "sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8",
-                "sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291",
-                "sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087",
-                "sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866",
-                "sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3",
-                "sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d",
-                "sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1",
-                "sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca",
-                "sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e",
-                "sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db",
-                "sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72",
-                "sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d",
-                "sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc",
-                "sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539",
-                "sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d",
-                "sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af",
-                "sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b",
-                "sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602",
-                "sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f",
-                "sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478",
-                "sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c",
-                "sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e",
-                "sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479",
-                "sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7",
-                "sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "version": "==3.0.1"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.1.0"
         },
         "click": {
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==8.1.3"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:04481245ef966fbd24ae9b9e537ce899ae584d521dfbe78f89cad003c38ca2ab",
-                "sha256:0c45948f613d5d18c9ec5eaa203ce06a653334cf1bd47c783a12d0dd4fd9c851",
-                "sha256:10188fe543560ec4874f974b5305cd1a8bdcfa885ee00ea3a03733464c4ca265",
-                "sha256:218fe982371ac7387304153ecd51205f14e9d731b34fb0568181abaf7b443ba0",
-                "sha256:29571503c37f2ef2138a306d23e7270687c0efb9cab4bd8038d609b5c2393a3a",
-                "sha256:2a60d6513781e87047c3e630b33b4d1e89f39836dac6e069ffee28c4786715f5",
-                "sha256:2bf1d5f2084c3932b56b962a683074a3692bce7cabd3aa023c987a2a8e7612f6",
-                "sha256:3164d31078fa9efe406e198aecd2a02d32a62fecbdef74f76dad6a46c7e48311",
-                "sha256:32df215215f3af2c1617a55dbdfb403b772d463d54d219985ac7cd3bf124cada",
-                "sha256:33d1ae9d4079e05ac4cc1ef9e20c648f5afabf1a92adfaf2ccf509c50b85717f",
-                "sha256:33ff26d0f6cc3ca8de13d14fde1ff8efe1456b53e3f0273e63cc8b3c84a063d8",
-                "sha256:38da2db80cc505a611938d8624801158e409928b136c8916cd2e203970dde4dc",
-                "sha256:3b155caf3760408d1cb903b21e6a97ad4e2bdad43cbc265e3ce0afb8e0057e73",
-                "sha256:3b946bbcd5a8231383450b195cfb58cb01cbe7f8949f5758566b881df4b33baf",
-                "sha256:3baf5f126f30781b5e93dbefcc8271cb2491647f8283f20ac54d12161dff080e",
-                "sha256:4b14d5e09c656de5038a3f9bfe5228f53439282abcab87317c9f7f1acb280352",
-                "sha256:51b236e764840a6df0661b67e50697aaa0e7d4124ca95e5058fa3d7cbc240b7c",
-                "sha256:63ffd21aa133ff48c4dff7adcc46b7ec8b565491bfc371212122dd999812ea1c",
-                "sha256:6a43c7823cd7427b4ed763aa7fb63901ca8288591323b58c9cd6ec31ad910f3c",
-                "sha256:755e89e32376c850f826c425ece2c35a4fc266c081490eb0a841e7c1cb0d3bda",
-                "sha256:7a726d742816cb3a8973c8c9a97539c734b3a309345236cd533c4883dda05b8d",
-                "sha256:7c7c0d0827e853315c9bbd43c1162c006dd808dbbe297db7ae66cd17b07830f0",
-                "sha256:7ed681b0f8e8bcbbffa58ba26fcf5dbc8f79e7997595bf071ed5430d8c08d6f3",
-                "sha256:7ee5c9bb51695f80878faaa5598040dd6c9e172ddcf490382e8aedb8ec3fec8d",
-                "sha256:8361be1c2c073919500b6601220a6f2f98ea0b6d2fec5014c1d9cfa23dd07038",
-                "sha256:8ae125d1134bf236acba8b83e74c603d1b30e207266121e76484562bc816344c",
-                "sha256:9817733f0d3ea91bea80de0f79ef971ae94f81ca52f9b66500c6a2fea8e4b4f8",
-                "sha256:98b85dd86514d889a2e3dd22ab3c18c9d0019e696478391d86708b805f4ea0fa",
-                "sha256:9ccb092c9ede70b2517a57382a601619d20981f56f440eae7e4d7eaafd1d1d09",
-                "sha256:9d58885215094ab4a86a6aef044e42994a2bd76a446dc59b352622655ba6621b",
-                "sha256:b643cb30821e7570c0aaf54feaf0bfb630b79059f85741843e9dc23f33aaca2c",
-                "sha256:bc7c85a150501286f8b56bd8ed3aa4093f4b88fb68c0843d21ff9656f0009d6a",
-                "sha256:beeb129cacea34490ffd4d6153af70509aa3cda20fdda2ea1a2be870dfec8d52",
-                "sha256:c31b75ae466c053a98bf26843563b3b3517b8f37da4d47b1c582fdc703112bc3",
-                "sha256:c4e4881fa9e9667afcc742f0c244d9364d197490fbc91d12ac3b5de0bf2df146",
-                "sha256:c5b15ed7644ae4bee0ecf74fee95808dcc34ba6ace87e8dfbf5cb0dc20eab45a",
-                "sha256:d12d076582507ea460ea2a89a8c85cb558f83406c8a41dd641d7be9a32e1274f",
-                "sha256:d248cd4a92065a4d4543b8331660121b31c4148dd00a691bfb7a5cdc7483cfa4",
-                "sha256:d47dd659a4ee952e90dc56c97d78132573dc5c7b09d61b416a9deef4ebe01a0c",
-                "sha256:d4a5a5879a939cb84959d86869132b00176197ca561c664fc21478c1eee60d75",
-                "sha256:da9b41d4539eefd408c46725fb76ecba3a50a3367cafb7dea5f250d0653c1040",
-                "sha256:db61a79c07331e88b9a9974815c075fbd812bc9dbc4dc44b366b5368a2936063",
-                "sha256:ddb726cb861c3117a553f940372a495fe1078249ff5f8a5478c0576c7be12050",
-                "sha256:ded59300d6330be27bc6cf0b74b89ada58069ced87c48eaf9344e5e84b0072f7",
-                "sha256:e2617759031dae1bf183c16cef8fcfb3de7617f394c813fa5e8e46e9b82d4222",
-                "sha256:e5cdbb5cafcedea04924568d990e20ce7f1945a1dd54b560f879ee2d57226912",
-                "sha256:ec8e767f13be637d056f7e07e61d089e555f719b387a7070154ad80a0ff31801",
-                "sha256:ef382417db92ba23dfb5864a3fc9be27ea4894e86620d342a116b243ade5d35d",
-                "sha256:f2cba5c6db29ce991029b5e4ac51eb36774458f0a3b8d3137241b32d1bb91f06",
-                "sha256:f5b4198d85a3755d27e64c52f8c95d6333119e49fd001ae5798dac872c95e0f8",
-                "sha256:ffeeb38ee4a80a30a6877c5c4c359e5498eec095878f1581453202bfacc8fbc2"
+                "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f",
+                "sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2",
+                "sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a",
+                "sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a",
+                "sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01",
+                "sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6",
+                "sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7",
+                "sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f",
+                "sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02",
+                "sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c",
+                "sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063",
+                "sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a",
+                "sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5",
+                "sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959",
+                "sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97",
+                "sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6",
+                "sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f",
+                "sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9",
+                "sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5",
+                "sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f",
+                "sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562",
+                "sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe",
+                "sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9",
+                "sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f",
+                "sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb",
+                "sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb",
+                "sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1",
+                "sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb",
+                "sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250",
+                "sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e",
+                "sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511",
+                "sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5",
+                "sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59",
+                "sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2",
+                "sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d",
+                "sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3",
+                "sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4",
+                "sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de",
+                "sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9",
+                "sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833",
+                "sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0",
+                "sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9",
+                "sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d",
+                "sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050",
+                "sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d",
+                "sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6",
+                "sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353",
+                "sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb",
+                "sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e",
+                "sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8",
+                "sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495",
+                "sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2",
+                "sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd",
+                "sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27",
+                "sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1",
+                "sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818",
+                "sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4",
+                "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e",
+                "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850",
+                "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.1.0"
+            "version": "==7.2.7"
         },
         "cryptography": {
             "hashes": [
-                "sha256:1a6915075c6d3a5e1215eab5d99bcec0da26036ff2102a1038401d6ef5bef25b",
-                "sha256:1ee1fd0de9851ff32dbbb9362a4d833b579b4a6cc96883e8e6d2ff2a6bc7104f",
-                "sha256:407cec680e811b4fc829de966f88a7c62a596faa250fc1a4b520a0355b9bc190",
-                "sha256:50386acb40fbabbceeb2986332f0287f50f29ccf1497bae31cf5c3e7b4f4b34f",
-                "sha256:6f97109336df5c178ee7c9c711b264c502b905c2d2a29ace99ed761533a3460f",
-                "sha256:754978da4d0457e7ca176f58c57b1f9de6556591c19b25b8bcce3c77d314f5eb",
-                "sha256:76c24dd4fd196a80f9f2f5405a778a8ca132f16b10af113474005635fe7e066c",
-                "sha256:7dacfdeee048814563eaaec7c4743c8aea529fe3dd53127313a792f0dadc1773",
-                "sha256:80ee674c08aaef194bc4627b7f2956e5ba7ef29c3cc3ca488cf15854838a8f72",
-                "sha256:844ad4d7c3850081dffba91cdd91950038ee4ac525c575509a42d3fc806b83c8",
-                "sha256:875aea1039d78557c7c6b4db2fe0e9d2413439f4676310a5f269dd342ca7a717",
-                "sha256:887cbc1ea60786e534b00ba8b04d1095f4272d380ebd5f7a7eb4cc274710fad9",
-                "sha256:ad04f413436b0781f20c52a661660f1e23bcd89a0e9bb1d6d20822d048cf2856",
-                "sha256:bae6c7f4a36a25291b619ad064a30a07110a805d08dc89984f4f441f6c1f3f96",
-                "sha256:c52a1a6f81e738d07f43dab57831c29e57d21c81a942f4602fac7ee21b27f288",
-                "sha256:e0a05aee6a82d944f9b4edd6a001178787d1546ec7c6223ee9a848a7ade92e39",
-                "sha256:e324de6972b151f99dc078defe8fb1b0a82c6498e37bff335f5bc6b1e3ab5a1e",
-                "sha256:e5d71c5d5bd5b5c3eebcf7c5c2bb332d62ec68921a8c593bea8c394911a005ce",
-                "sha256:f3ed2d864a2fa1666e749fe52fb8e23d8e06b8012e8bd8147c73797c506e86f1",
-                "sha256:f671c1bb0d6088e94d61d80c606d65baacc0d374e67bf895148883461cd848de",
-                "sha256:f6c0db08d81ead9576c4d94bbb27aed8d7a430fa27890f39084c2d0e2ec6b0df",
-                "sha256:f964c7dcf7802d133e8dbd1565914fa0194f9d683d82411989889ecd701e8adf",
-                "sha256:fec8b932f51ae245121c4671b4bbc030880f363354b2f0e0bd1366017d891458"
+                "sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db",
+                "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a",
+                "sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039",
+                "sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c",
+                "sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3",
+                "sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485",
+                "sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c",
+                "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca",
+                "sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5",
+                "sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5",
+                "sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3",
+                "sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb",
+                "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43",
+                "sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31",
+                "sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc",
+                "sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b",
+                "sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006",
+                "sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a",
+                "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==39.0.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==41.0.1"
+        },
+        "distlib": {
+            "hashes": [
+                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
+                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
+            ],
+            "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
-                "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
-                "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
+                "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
+                "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.20.1"
+        },
+        "filelock": {
+            "hashes": [
+                "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
+                "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.19"
+            "version": "==3.12.2"
+        },
+        "hypothesis": {
+            "hashes": [
+                "sha256:245bed0fcf7612caa0ca1ecaa5c1e3a7100bbf9fd0fe4a24bdd9e46249b2774f",
+                "sha256:69b55ee1dae2c7edd214e273a977d0dfba542946a211c9ef1f958743b49e430e"
+            ],
+            "index": "pypi",
+            "version": "==6.79.3"
+        },
+        "identify": {
+            "hashes": [
+                "sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4",
+                "sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.5.24"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad",
-                "sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d"
+                "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4",
+                "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==6.0.0"
+            "version": "==6.7.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
@@ -407,237 +471,321 @@
                 "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
             ],
             "markers": "sys_platform == 'linux'",
             "version": "==0.8.0"
         },
         "keyring": {
             "hashes": [
-                "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd",
-                "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"
+                "sha256:4901caaf597bfd3bbd78c9a0c7c4c29fcd8310dab2cffefe749e916b6527acd6",
+                "sha256:ca0746a19ec421219f4d713f848fa297a661a8a8c1504867e55bfb5e09091509"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==23.13.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==24.2.0"
         },
         "markdown-it-py": {
             "hashes": [
-                "sha256:93de681e5c021a432c63147656fe21790bc01231e0cd2da73626f1aa3ac0fe27",
-                "sha256:cf7e59fed14b5ae17c0006eff14a2d9a00ed5f3a846148153899a0224e2c07da"
+                "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
+                "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.1.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.0.0"
         },
         "mdurl": {
             "hashes": [
                 "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.1.2"
         },
         "more-itertools": {
             "hashes": [
-                "sha256:250e83d7e81d0c87ca6bd942e6aeab8cc9daa6096d12c5308f3f92fa5e5c1f41",
-                "sha256:5a6257e40878ef0520b1803990e3e22303a41b5714006c32a3fd8304b26ea1ab"
+                "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d",
+                "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==9.0.0"
+            "version": "==9.1.0"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.0"
         },
+        "nodeenv": {
+            "hashes": [
+                "sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2",
+                "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
+            "version": "==1.8.0"
+        },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "index": "pypi",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "pathspec": {
             "hashes": [
-                "sha256:3a66eb970cbac598f9e5ccb5b2cf58930cd8e3ed86d393d541eaf2d8b1705229",
-                "sha256:64d338d4e0914e91c1792321e6907b5a593f1ab1851de7fc269557a21b30ebbc"
+                "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687",
+                "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.11.0"
+            "version": "==0.11.1"
         },
         "pkginfo": {
             "hashes": [
                 "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:83c8f6d04389165de7c9b6f0c682439697887bca0aa2f1c87ef1826be3584490",
-                "sha256:e1fea1fe471b9ff8332e229df3cb7de4f53eeea4998d3b6bfff542115e998bd2"
+                "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc",
+                "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.6.2"
+            "version": "==3.8.0"
         },
         "pluggy": {
             "hashes": [
-                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
-                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
+                "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
+                "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.0.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.2.0"
+        },
+        "pre-commit": {
+            "hashes": [
+                "sha256:10badb65d6a38caff29703362271d7dca483d01da88f9d7e05d0b97171c136cb",
+                "sha256:a2256f489cd913d575c145132ae196fe335da32d91a8294b7afe6622335dd023"
+            ],
+            "index": "pypi",
+            "version": "==3.3.3"
         },
         "pycparser": {
             "hashes": [
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
             "version": "==2.21"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "pyproject-hooks": {
             "hashes": [
                 "sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8",
                 "sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
         "pytest": {
             "hashes": [
-                "sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5",
-                "sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42"
+                "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
+                "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "index": "pypi",
-            "version": "==7.2.1"
+            "version": "==7.4.0"
         },
         "pytest-cov": {
             "hashes": [
-                "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b",
-                "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"
+                "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6",
+                "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"
             ],
             "index": "pypi",
-            "version": "==4.0.0"
+            "version": "==4.1.0"
+        },
+        "pyyaml": {
+            "hashes": [
+                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
+                "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
+                "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
+                "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
+                "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
+                "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
+                "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
+                "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
+                "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
+                "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
+                "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
+                "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
+                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
+                "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
+                "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
+                "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
+                "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
+                "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
+                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
+                "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
+                "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
+                "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
+                "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
+                "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
+                "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
+                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
+                "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
+                "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
+                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
+                "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
+                "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
+                "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
+                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
+                "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
+                "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
+                "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
+                "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
+                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
+                "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
+                "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==6.0"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273",
-                "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
+                "sha256:9f77b519d96d03d7d7dce44977ba543090a14397c4f60de5b6eb5b8048110aa4",
+                "sha256:e18feb2a1e7706f2865b81ebb460056d93fb29d69daa10b223c00faa7bd9a00a"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==37.3"
+            "markers": "python_version >= '3.8'",
+            "version": "==40.0"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.31.0"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7",
-                "sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.1"
+            "version": "==1.0.0"
         },
         "rfc3986": {
             "hashes": [
                 "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:125d96d20c92b946b983d0d392b84ff945461e5a06d3867e9f9e575f8697b67f",
-                "sha256:8aa57747f3fc3e977684f0176a88e789be314a99f99b43b75d1e9cb5dc6db9e9"
+                "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
+                "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.1"
+            "version": "==13.4.2"
+        },
+        "ruff": {
+            "hashes": [
+                "sha256:0c4e6468da26f77b90cae35319d310999f471a8c352998e9b39937a23750149e",
+                "sha256:0dbdea02942131dbc15dd45f431d152224f15e1dd1859fcd0c0487b658f60f1a",
+                "sha256:1cc599022fe5ffb143a965b8d659eb64161ab8ab4433d208777eab018a1aab67",
+                "sha256:22efd9f41af27ef8fb9779462c46c35c89134d33e326c889971e10b2eaf50c63",
+                "sha256:2c09662112cfa22d7467a19252a546291fd0eae4f423e52b75a7a2000a1894db",
+                "sha256:508b13f7ca37274cceaba4fb3ea5da6ca192356323d92acf39462337c33ad14e",
+                "sha256:5206fc1cd8c1c1deadd2e6360c0dbcd690f1c845da588ca9d32e4a764a402c60",
+                "sha256:5859ee543b01b7eb67835dfd505faa8bb7cc1550f0295c92c1401b45b42be399",
+                "sha256:5e6554a072e7ce81eb6f0bec1cebd3dcb0e358652c0f4900d7d630d61691e914",
+                "sha256:6afb1c4422f24f361e877937e2a44b3f8176774a476f5e33845ebfe887dd5ec2",
+                "sha256:80043726662144876a381efaab88841c88e8df8baa69559f96b22d4fa216bef1",
+                "sha256:8347fc16aa185aae275906c4ac5b770e00c896b6a0acd5ba521f158801911998",
+                "sha256:a19ce3bea71023eee5f0f089dde4a4272d088d5ac0b675867e074983238ccc65",
+                "sha256:a63a0b645da699ae5c758fce19188e901b3033ec54d862d93fcd042addf7f38d",
+                "sha256:c8ace4d40a57b5ea3c16555f25a6b16bc5d8b2779ae1912ce2633543d4e9b1da",
+                "sha256:d9b264d78621bf7b698b6755d4913ab52c19bd28bee1a16001f954d64c1a1220",
+                "sha256:ec43658c64bfda44fd84bbea9da8c7a3b34f65448192d1c4dd63e9f4e7abfdd4"
+            ],
+            "index": "pypi",
+            "version": "==0.0.275"
         },
         "secretstorage": {
             "hashes": [
                 "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
             "version": "==3.3.3"
         },
         "setuptools": {
             "hashes": [
-                "sha256:883131c5b6efa70b9101c7ef30b2b7b780a4283d5fc1616383cdf22c83cbefe6",
-                "sha256:9d790961ba6219e9ff7d9557622d2fe136816a264dd01d5997cfc057d804853d"
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.0.0"
-        },
-        "setuptools-scm": {
-            "hashes": [
-                "sha256:6c508345a771aad7d56ebff0e70628bf2b0ec7573762be9960214730de278f27",
-                "sha256:73988b6d848709e2af142aa48c986ea29592bbcfca5375678064708205253d8e"
-            ],
-            "index": "pypi",
-            "version": "==7.1.0"
+            "version": "==68.0.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
+        "sortedcontainers": {
+            "hashes": [
+                "sha256:25caa5a06cc30b6b83d11423433f65d1f9d76c4c6a0c90e3379eaa43b9bfdb88",
+                "sha256:a163dcaede0f1c021485e957a39245190e74249897e2ae4b2aa38595db237ee0"
+            ],
+            "version": "==2.4.0"
+        },
         "twine": {
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
             "version": "==4.0.2"
         },
-        "typing-extensions": {
+        "urllib3": {
             "hashes": [
-                "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa",
-                "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.4.0"
+            "version": "==2.0.3"
         },
-        "urllib3": {
+        "virtualenv": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:34da10f14fea9be20e0fd7f04aba9732f84e593dac291b757ce42e3368a39419",
+                "sha256:8ff19a38c1021c742148edc4f81cb43d7f8c6816d2ede2ab72af5b84c749ade1"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "markers": "python_version >= '3.7'",
+            "version": "==20.23.1"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:6c4fe274b8f85ec73c37a8e4e3fa00df9fb9335da96fb789e3b96b318e5097b3",
-                "sha256:a3cac813d40993596b39ea9e93a18e8a2076d5c378b8bc88ec32ab264e04ad02"
+                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
+                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.12.1"
+            "version": "==3.15.0"
         }
     }
 }
```

### Comparing `simple-git-versioning-0.0.4/pyproject.toml` & `simple-git-versioning-0.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "simple-git-versioning"
-description = "Thinly scoped and opinionated project that computes a version number from git tags and trailers"
+description = "Thinly scoped and opinionated tool that computes a version number from git tags and trailers"
 license = { text = "MIT" }
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 authors = [
     { name = "Quentin Bouget", email = "ypsah@devyard.org" },
 ]
 keywords = [
     "versioning",
     "git",
     "git-trailers",
@@ -15,38 +15,47 @@
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-dynamic = ["dependencies", "version"]
+readme = "README.md"
+version = "0.1.0"
+dynamic = ["dependencies"]
+
+[project.urls]
+homepage = "https://gitlab.com/ypsah/simple-git-versioning"
+repository = "https://gitlab.com/ypsah/simple-git-versioning"
 
 [project.scripts]
-version = "versioning:__main__"
+pep440 = "versioning.pep440:main"
+semver2 = "versioning.semver2:main"
+
+[project.entry-points."setuptools.finalize_distribution_options"]
+simple-git-versioning = "versioning.setuptools:finalize_distribution_options"
 
 [build-system]
-requires = ["setuptools>=63", "setuptools_scm[toml]>=6.2", "setuptools-pipfile"]
+requires = ["setuptools>=63", "setuptools-scm", "setuptools-pipfile"]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools_scm]
-
 [tool.setuptools-pipfile]
 
 [tool.black]
 line-length = 120
-target-version = ['py37', 'py38', 'py310', 'py311']
+target-version = ['py311']
 # enrole in feature-preview
 preview = true
 
 [tool.isort]
 profile = "black"
-src_paths = ["snippets", "tests"]
+src_paths = ["versioning", "tests"]
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --cov=versioning --cov-branch --cov-fail-under=90"
+
+[tool.ruff]
+ignore = [
+    "E501",  # line-length: black already covers this
+]
```

