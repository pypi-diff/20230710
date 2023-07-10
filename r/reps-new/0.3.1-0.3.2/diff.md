# Comparing `tmp/reps_new-0.3.1.tar.gz` & `tmp/reps_new-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reps_new-0.3.1.tar", max compression
+gzip compressed data, was "reps_new-0.3.2.tar", max compression
```

## Comparing `reps_new-0.3.1.tar` & `reps_new-0.3.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    16725 2023-06-26 14:32:18.742202 reps_new-0.3.1/LICENSE
--rw-r--r--   0        0        0     1008 2023-07-06 19:30:10.728667 reps_new-0.3.1/README.md
--rw-r--r--   0        0        0      567 2023-07-07 14:47:02.221268 reps_new-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 14:40:53.482059 reps_new-0.3.1/reps/__init__.py
--rw-r--r--   0        0        0     1556 2023-07-06 19:29:55.318671 reps_new-0.3.1/reps/console.py
--rw-r--r--   0        0        0     3254 2023-07-07 14:46:23.131618 reps_new-0.3.1/reps/hooks.py
--rw-r--r--   0        0        0      446 2023-06-27 15:15:55.197097 reps_new-0.3.1/reps/templates/base/cookiecutter.json
--rw-r--r--   0        0        0       88 2023-06-27 14:22:18.958542 reps_new-0.3.1/reps/templates/base/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-06-26 17:22:22.013700 reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/.codespell-ignore-words.txt
--rw-r--r--   0        0        0      105 2023-06-26 18:33:35.852510 reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/.github/CODEOWNERS
--rw-r--r--   0        0        0     2788 2023-06-26 18:38:23.842430 reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      980 2023-06-26 17:25:52.613642 reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      113 2023-07-07 14:36:27.708041 reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/.yamllint.yml
--rw-r--r--   0        0        0      493 2023-06-26 17:18:54.383758 reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0    16725 2023-06-26 17:19:01.503756 reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/LICENSE
--rw-r--r--   0        0        0      723 2023-06-27 15:07:50.494974 reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/Makefile
--rw-r--r--   0        0        0      958 2023-07-06 14:55:10.046283 reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/README.md
--rw-r--r--   0        0        0       18 2023-06-27 15:37:41.811689 reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/docs/concepts/index.rst
--rw-r--r--   0        0        0     1711 2023-07-07 14:35:05.939061 reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/docs/conf.py
--rw-r--r--   0        0        0       28 2023-06-27 15:37:27.161828 reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/docs/howto/index.rst
--rw-r--r--   0        0        0      255 2023-06-27 15:33:11.684251 reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/docs/index.rst
--rw-r--r--   0        0        0       20 2023-06-27 15:37:52.271590 reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/docs/reference/index.rst
--rw-r--r--   0        0        0       20 2023-06-27 15:38:02.821490 reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/docs/tutorials/index.rst
--rw-r--r--   0        0        0     1120 2023-07-06 19:29:54.578671 reps_new-0.3.1/reps/templates/python/cookiecutter.json
--rw-r--r--   0        0        0      129 2023-06-27 20:05:58.083480 reps_new-0.3.1/reps/templates/python/hooks/post_gen_project.py
--rw-r--r--   0        0        0      113 2023-06-27 20:05:58.083480 reps_new-0.3.1/reps/templates/python/hooks/pre_gen_project.py
--rw-r--r--   0        0        0    16186 2023-07-07 14:40:59.364652 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/.taskcluster.yml
--rw-r--r--   0        0        0      918 2023-06-27 20:05:58.083480 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-29 20:18:22.754371 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/src/{{cookiecutter.__package_name}}/__init__.py
--rw-r--r--   0        0        0     1175 2023-07-06 20:25:24.507743 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/codecov/kind.yml
--rw-r--r--   0        0        0      570 2023-07-05 13:50:01.939464 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/config.yml
--rw-r--r--   0        0        0      512 2023-07-06 19:29:54.578671 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/docker-image/kind.yml
--rw-r--r--   0        0        0      743 2023-06-27 20:05:58.083480 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/fetch/kind.yml
--rw-r--r--   0        0        0      993 2023-07-06 20:28:44.257688 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/test/kind.yml
--rw-r--r--   0        0        0      518 2023-07-04 19:06:10.348905 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/fetch/Dockerfile
--rw-r--r--   0        0        0     1306 2023-07-06 20:23:53.167770 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/python/Dockerfile
--rw-r--r--   0        0        0       22 2023-07-04 19:26:34.218564 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/requirements.in
--rw-r--r--   0        0        0      701 2023-07-06 19:29:55.318671 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/codecov-upload.py
--rwxr-xr-x   0        0        0      179 2023-07-06 19:29:56.058671 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/poetry-setup
--rwxr-xr-x   0        0        0      658 2023-07-06 20:36:16.647561 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/pyenv-setup
--rw-r--r--   0        0        0      345 2023-06-27 15:00:30.932961 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/test/conftest.py
--rw-r--r--   0        0        0      165 2023-07-07 14:39:55.465449 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/test/test_{{cookiecutter.__package_name}}.py
--rw-r--r--   0        0        0      957 2023-07-06 19:30:10.738667 reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/tox.ini
--rw-r--r--   0        0        0     1717 1970-01-01 00:00:00.000000 reps_new-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-06-26 14:32:18.742202 reps_new-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1742 2023-07-07 20:02:08.671202 reps_new-0.3.2/README.md
+-rw-r--r--   0        0        0      911 2023-07-10 15:28:21.959183 reps_new-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 14:40:53.482059 reps_new-0.3.2/reps/__init__.py
+-rw-r--r--   0        0        0     1785 2023-07-08 04:06:54.597967 reps_new-0.3.2/reps/console.py
+-rw-r--r--   0        0        0     3240 2023-07-07 18:25:13.809240 reps_new-0.3.2/reps/hooks.py
+-rw-r--r--   0        0        0      446 2023-06-27 15:15:55.197097 reps_new-0.3.2/reps/templates/base/cookiecutter.json
+-rw-r--r--   0        0        0       88 2023-06-27 14:22:18.958542 reps_new-0.3.2/reps/templates/base/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-06-26 17:22:22.013700 reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/.codespell-ignore-words.txt
+-rw-r--r--   0        0        0      105 2023-06-26 18:33:35.852510 reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/.github/CODEOWNERS
+-rw-r--r--   0        0        0     2788 2023-06-26 18:38:23.842430 reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      980 2023-06-26 17:25:52.613642 reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      113 2023-07-07 14:36:27.708041 reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/.yamllint.yml
+-rw-r--r--   0        0        0      493 2023-06-26 17:18:54.383758 reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    16725 2023-06-26 17:19:01.503756 reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/LICENSE
+-rw-r--r--   0        0        0      723 2023-06-27 15:07:50.494974 reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/Makefile
+-rw-r--r--   0        0        0      958 2023-07-06 14:55:10.046283 reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/README.md
+-rw-r--r--   0        0        0       18 2023-06-27 15:37:41.811689 reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/docs/concepts/index.rst
+-rw-r--r--   0        0        0     1711 2023-07-07 14:35:05.939061 reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/docs/conf.py
+-rw-r--r--   0        0        0       28 2023-06-27 15:37:27.161828 reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/docs/howto/index.rst
+-rw-r--r--   0        0        0      255 2023-06-27 15:33:11.684251 reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/docs/index.rst
+-rw-r--r--   0        0        0       20 2023-06-27 15:37:52.271590 reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/docs/reference/index.rst
+-rw-r--r--   0        0        0       20 2023-06-27 15:38:02.821490 reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/docs/tutorials/index.rst
+-rw-r--r--   0        0        0     1120 2023-07-06 19:29:54.578671 reps_new-0.3.2/reps/templates/python/cookiecutter.json
+-rw-r--r--   0        0        0      129 2023-06-27 20:05:58.083480 reps_new-0.3.2/reps/templates/python/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      113 2023-06-27 20:05:58.083480 reps_new-0.3.2/reps/templates/python/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0    16176 2023-07-10 15:19:50.489325 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/.taskcluster.yml
+-rw-r--r--   0        0        0      918 2023-06-27 20:05:58.083480 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-29 20:18:22.754371 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/src/{{cookiecutter.__package_name}}/__init__.py
+-rw-r--r--   0        0        0     1175 2023-07-06 20:25:24.507743 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/codecov/kind.yml
+-rw-r--r--   0        0        0      570 2023-07-05 13:50:01.939464 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/config.yml
+-rw-r--r--   0        0        0      512 2023-07-06 19:29:54.578671 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/docker-image/kind.yml
+-rw-r--r--   0        0        0      743 2023-06-27 20:05:58.083480 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/fetch/kind.yml
+-rw-r--r--   0        0        0      993 2023-07-06 20:28:44.257688 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/test/kind.yml
+-rw-r--r--   0        0        0      518 2023-07-04 19:06:10.348905 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/fetch/Dockerfile
+-rw-r--r--   0        0        0     1306 2023-07-06 20:23:53.167770 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/python/Dockerfile
+-rw-r--r--   0        0        0       22 2023-07-04 19:26:34.218564 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/requirements.in
+-rw-r--r--   0        0        0      695 2023-07-07 18:30:04.719160 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/codecov-upload.py
+-rwxr-xr-x   0        0        0      179 2023-07-06 19:29:56.058671 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/poetry-setup
+-rwxr-xr-x   0        0        0      658 2023-07-06 20:36:16.647561 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/pyenv-setup
+-rw-r--r--   0        0        0      345 2023-06-27 15:00:30.932961 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/test/conftest.py
+-rw-r--r--   0        0        0      165 2023-07-07 14:39:55.465449 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/test/test_{{cookiecutter.__package_name}}.py
+-rw-r--r--   0        0        0      957 2023-07-06 19:30:10.738667 reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/tox.ini
+-rw-r--r--   0        0        0     2550 1970-01-01 00:00:00.000000 reps_new-0.3.2/PKG-INFO
```

### Comparing `reps_new-0.3.1/LICENSE` & `reps_new-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/console.py` & `reps_new-0.3.2/reps/console.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,16 +41,22 @@
     parser.add_argument(
         "-t",
         "--template",
         default="python",
         choices=available_templates(),
         help="Project template to initialize.",
     )
+    parser.add_argument(
+        "--no-input", default=False, action="store_true", help="Use defaults"
+    )
     parser.set_defaults(func=command_new)
 
     kwargs = vars(parser.parse_args(args))
     func = kwargs.pop("func")
+
+    if not kwargs["name"] and kwargs["no_input"]:
+        parser.error("must specify 'name' when --no-input is used!")
     return func(**kwargs)
 
 
 if __name__ == "main":
     sys.exit(run())
```

### Comparing `reps_new-0.3.1/reps/hooks.py` & `reps_new-0.3.2/reps/hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import subprocess
 from collections import defaultdict
 from pathlib import Path
-import sys
 
 import yaml
 from halo import Halo
 
 from reps.console import command_new
 
 
@@ -35,15 +34,14 @@
         subprocess.run(cmd, **kwargs)
     except subprocess.CalledProcessError as e:
         print("+ command failed: {' '.join(cmd)}")
         print(e.output)
         raise
 
 
-
 @hook("pre-gen-py")
 def base_init(items):
     """Generate the 'base' template first."""
     if "_copy_without_render" in items:
         del items["_copy_without_render"]
 
     command_new(
@@ -137,9 +135,7 @@
 def lock_taskgraph_requirements(items):
     run(["pip-compile", "requirements.in", "--generate-hashes"], cwd="taskcluster")
 
 
 @hook("post-gen-base")
 def taskgraph_init(items):
     run(["taskgraph", "init"])
-
-
```

### Comparing `reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/.github/workflows/codeql-analysis.yml` & `reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/.pre-commit-config.yaml` & `reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/LICENSE` & `reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/Makefile` & `reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/README.md` & `reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/base/{{cookiecutter.__project_slug}}/docs/conf.py` & `reps_new-0.3.2/reps/templates/base/{{cookiecutter.__project_slug}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/python/cookiecutter.json` & `reps_new-0.3.2/reps/templates/python/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/.taskcluster.yml` & `reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/.taskcluster.yml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                   'tasks_for == "github-push"': ${event.ref}
                   'tasks_for == "github-release"': '${event.release.target_commitish}'
                   'tasks_for in ["action", "cron"]': '${push.branch}'
           base_ref:
               $switch:
                   'tasks_for[:19] == "github-pull-request"': ${event.pull_request.base.ref}
                   'tasks_for == "github-push" && event.base_ref': ${event.base_ref}
-                  'tasks_for == "github-push"': ${event.ref}
+                  'tasks_for == "github-push"': ''
                   'tasks_for in ["cron", "action"]': '${push.branch}'
           head_ref:
               $switch:
                   'tasks_for[:19] == "github-pull-request"': ${event.pull_request.head.ref}
                   'tasks_for == "github-push"': ${event.ref}
                   'tasks_for in ["cron", "action"]': '${push.branch}'
           base_sha:
```

### Comparing `reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/pyproject.toml` & `reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/codecov/kind.yml` & `reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/codecov/kind.yml`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/config.yml` & `reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/config.yml`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/docker-image/kind.yml` & `reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/docker-image/kind.yml`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/fetch/kind.yml` & `reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/fetch/kind.yml`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/test/kind.yml` & `reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/test/kind.yml`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/fetch/Dockerfile` & `reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/fetch/Dockerfile`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/python/Dockerfile` & `reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/python/Dockerfile`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/codecov-upload.py` & `reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/codecov-upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,13 @@
     """Retrieves the given taskcluster secret"""
     secret_url = SECRET_BASEURL_TPL.format(secret_name)
     r = requests.get(secret_url)
     r.raise_for_status()
     return r.json()["secret"]
 
 
-token = fetch_secret("{{cookiecutter.__secrets_path}}")[
-    "codecov_api_token"
-]
+token = fetch_secret("{{cookiecutter.__secrets_path}}")["codecov_api_token"]
 uploader = FETCHES_DIR / "codecov"
 uploader.chmod(uploader.stat().st_mode | stat.S_IEXEC)
 subprocess.run(
     [str(uploader), "-t", token, "-f", str(FETCHES_DIR / "coverage.xml")], check=True
 )
```

### Comparing `reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/pyenv-setup` & `reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/pyenv-setup`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/reps/templates/python/{{cookiecutter.__project_slug}}/tox.ini` & `reps_new-0.3.2/reps/templates/python/{{cookiecutter.__project_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `reps_new-0.3.1/PKG-INFO` & `reps_new-0.3.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: reps-new
-Version: 0.3.1
+Version: 0.3.2
 Summary: Mozilla Release Engineering Project Standard
 License: MPL-2.0
 Author: Mozilla Release Engineering
 Author-email: release@mozilla.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: pip-tools (>=6.14.0,<7.0.0)
 Requires-Dist: pre-commit (>=3.3.3,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: taskcluster-taskgraph (>=5.4.0,<6.0.0)
 Description-Content-Type: text/markdown
 
+[![Task Status](https://firefox-ci-tc.services.mozilla.com/api/github/v1/repository/mozilla-releng/reps/main/badge.svg)](https://firefox-ci-tc.services.mozilla.com/api/github/v1/repository/mozilla-releng/reps/main/latest)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/mozilla-releng/reps/main.svg)](https://results.pre-commit.ci/latest/github/mozilla-releng/reps/main)
+[![Code Coverage](https://codecov.io/gh/mozilla-releng/reps/branch/main/graph/badge.svg?token=GJIV52ZQNP)](https://codecov.io/gh/mozilla-releng/reps)
+[![PyPI version](https://badge.fury.io/py/reps-new.svg)](https://badge.fury.io/py/reps-new)
+[![License](https://img.shields.io/badge/license-MPL%202.0-orange.svg)](http://mozilla.org/MPL/2.0)
+
 # Release Engineering Project Standard
 
 This repository:
 
 1. Defines the standard tools and workflows that Mozilla Release Engineering
    endeavours to use across its projects.
 2. Implements a `reps` binary that can be used to bootstrap new projects based
```

