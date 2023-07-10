# Comparing `tmp/flitenv-0.3.4.tar.gz` & `tmp/flitenv-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flitenv-0.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "flitenv-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flitenv-0.3.4.tar` & `flitenv-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,25 @@
--rw-r--r--   0        0        0       61 2023-07-10 06:51:52.129915 flitenv-0.3.4/.gitignore
--rw-r--r--   0        0        0     1048 2023-07-10 06:51:52.129915 flitenv-0.3.4/LICENSE
--rw-r--r--   0        0        0     3367 2023-07-10 06:51:52.129915 flitenv-0.3.4/README.md
--rw-r--r--   0        0        0     1100 2023-07-10 08:46:08.451460 flitenv-0.3.4/Taskfile.yml
--rw-r--r--   0        0        0      117 2023-07-10 08:45:07.056098 flitenv-0.3.4/flitenv/__init__.py
--rw-r--r--   0        0        0       44 2023-07-10 06:51:52.129915 flitenv-0.3.4/flitenv/__main__.py
--rw-r--r--   0        0        0     2628 2023-07-10 08:44:57.940192 flitenv-0.3.4/flitenv/_cli.py
--rw-r--r--   0        0        0      129 2023-07-10 08:44:57.940192 flitenv-0.3.4/flitenv/_constants.py
--rw-r--r--   0        0        0     3321 2023-07-10 08:44:57.940192 flitenv-0.3.4/flitenv/_deps_manager.py
--rw-r--r--   0        0        0     1463 2023-07-10 08:44:57.940192 flitenv-0.3.4/flitenv/_venv.py
--rw-r--r--   0        0        0      966 2023-07-10 08:44:57.940192 flitenv-0.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 06:51:52.129915 flitenv-0.3.4/tests/__init__.py
--rw-r--r--   0        0        0      259 2023-07-10 06:51:52.129915 flitenv-0.3.4/tests/conftest.py
--rw-r--r--   0        0        0     1018 2023-07-10 06:51:52.129915 flitenv-0.3.4/tests/test_install.py
--rw-r--r--   0        0        0      737 2023-07-10 06:51:52.129915 flitenv-0.3.4/tests/test_lock.py
--rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 flitenv-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-07-10 06:51:52.129915 flitenv-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1048 2023-07-10 06:51:52.129915 flitenv-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3367 2023-07-10 11:20:23.211650 flitenv-0.4.0/README.md
+-rw-r--r--   0        0        0     2210 2023-07-10 12:05:38.909926 flitenv-0.4.0/Taskfile.yml
+-rw-r--r--   0        0        0      117 2023-07-10 12:12:38.144856 flitenv-0.4.0/flitenv/__init__.py
+-rw-r--r--   0        0        0       44 2023-07-10 06:51:52.129915 flitenv-0.4.0/flitenv/__main__.py
+-rw-r--r--   0        0        0     1139 2023-07-10 11:20:23.211650 flitenv-0.4.0/flitenv/_cli.py
+-rw-r--r--   0        0        0      164 2023-07-10 09:08:33.561100 flitenv-0.4.0/flitenv/_constants.py
+-rw-r--r--   0        0        0     5286 2023-07-10 12:08:32.279819 flitenv-0.4.0/flitenv/_deps_manager.py
+-rw-r--r--   0        0        0     1586 2023-07-10 11:20:23.215650 flitenv-0.4.0/flitenv/_meta.py
+-rw-r--r--   0        0        0     2124 2023-07-10 12:05:38.909926 flitenv-0.4.0/flitenv/_venv.py
+-rw-r--r--   0        0        0      457 2023-07-10 11:20:23.215650 flitenv-0.4.0/flitenv/commands/__init__.py
+-rw-r--r--   0        0        0      522 2023-07-10 11:20:23.215650 flitenv-0.4.0/flitenv/commands/_base.py
+-rw-r--r--   0        0        0      761 2023-07-10 12:05:38.913926 flitenv-0.4.0/flitenv/commands/_deps.py
+-rw-r--r--   0        0        0     1132 2023-07-10 12:05:38.913926 flitenv-0.4.0/flitenv/commands/_install.py
+-rw-r--r--   0        0        0     1015 2023-07-10 11:20:23.215650 flitenv-0.4.0/flitenv/commands/_lock.py
+-rw-r--r--   0        0        0      868 2023-07-10 11:20:23.215650 flitenv-0.4.0/flitenv/commands/_run.py
+-rw-r--r--   0        0        0      372 2023-07-10 10:02:02.423079 flitenv-0.4.0/flitenv/commands/_version.py
+-rw-r--r--   0        0        0     1634 2023-07-10 09:08:33.561100 flitenv-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-07-10 09:08:33.561100 flitenv-0.4.0/setup.cfg
+-rw-r--r--   0        0        0        0 2023-07-10 06:51:52.129915 flitenv-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      297 2023-07-10 09:08:33.561100 flitenv-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     1055 2023-07-10 10:02:02.423079 flitenv-0.4.0/tests/test_install.py
+-rw-r--r--   0        0        0      774 2023-07-10 10:02:02.423079 flitenv-0.4.0/tests/test_lock.py
+-rw-r--r--   0        0        0     4344 1970-01-01 00:00:00.000000 flitenv-0.4.0/PKG-INFO
```

### Comparing `flitenv-0.3.4/LICENSE` & `flitenv-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flitenv-0.3.4/README.md` & `flitenv-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 1. "Lock file" is a file with exact versions of all dependencies of the project in the given environment, including the transitive ones.
 1. Flitenv uses [requirements.txt](https://pip.pypa.io/en/stable/user_guide/#requirements-files) files generated by [pip-tools](https://github.com/jazzband/pip-tools) as lock files.
 1. It is recommend to generate a lock file for (and only for) the `main` environment.
 1. flitenv follows the flit philosophy. It provides only the most helpful and flexible commands, and you can do anything you ever need by combining them with each other and with other tools.
 
 Below are usage examples. Each example uses `lint` as the target environment and `flake8` as a command we want to run in this environment.
 
-+ `flitenv lint install`: install dependencies. If the venv doesn't exist, it will be created. Can also be used to upgrade dependencies when the lock file has been changed.
-+ `flitenv lint run flake8`: run a command. If the venv doesn't exist, it will be created, and the dependencies will be installed.
-+ `flitenv lint lock`: generate lock file (`requirements-lint.txt`) for the env.
++ `flitenv install lint`: install dependencies. If the venv doesn't exist, it will be created. Can also be used to upgrade dependencies when the lock file has been changed.
++ `flitenv run lint flake8`: run a command. If the venv doesn't exist, it will be created, and the dependencies will be installed.
++ `flitenv lock lint`: generate lock file (`requirements-lint.txt`) for the env.
 + `flitenv main lock`: generate lock file (`requirements.txt`) for the `main` env. If there is no env-specific lock file, this one will be used instead.
 + `flitenv main lock -c ../other-project/requirements.txt`: generate lock file using lock file from another project as a reference. It allows to ensure compatibility of lock files accross multiple projects.
 + `rm requirements.txt && flitenv main lock`: upgrade all dependencies in the lock file.
-+ `rm -rf .venvs/lint && flitenv lint install`: re-create the venv. It is usefult to ensure that all old dependencies.
++ `rm -rf .venvs/lint && flitenv install lint`: re-create the venv. It is usefult to ensure that all old dependencies.
 + `flit build`: build a distribution for the project.
 + `flit install --symlink --python $(which python3.9) --deps=none`: symlink the project into the given Python interpreter without installing dependencies. It is helpful if you want to have nice go-to-definition in vscode across multiple projects.
```

### Comparing `flitenv-0.3.4/tests/test_install.py` & `flitenv-0.4.0/tests/test_install.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+from __future__ import annotations
+
 import subprocess
 import sys
 from pathlib import Path
+
 from flitenv._cli import main
 
 
 def test_install_main(project: Path) -> None:
-    cmd = ['--root', str(project), 'main', 'install']
-    main(argv=cmd, stream=sys.stdout)
+    cmd = ['--root', str(project), 'install', 'main']
+    main(argv=cmd, stdout=sys.stdout)
     print(list(project.iterdir()))
     assert (project / '.venvs' / 'main' / 'bin').is_dir()
 
 
 def test_install_test(project: Path) -> None:
-    cmd = ['--root', str(project), 'test', 'install']
-    main(argv=cmd, stream=sys.stdout)
+    cmd = ['--root', str(project), 'install', 'test']
+    main(argv=cmd, stdout=sys.stdout)
     assert project.joinpath('.venvs', 'test', 'bin', 'pytest').exists()
 
 
 def test_install_test_with_lockfile(project: Path) -> None:
     (project / 'requirements.txt').write_text('pytest==6.2.1')
-    cmd = ['--root', str(project), 'test', 'install']
-    main(argv=cmd, stream=sys.stdout)
+    cmd = ['--root', str(project), 'install', 'test']
+    main(argv=cmd, stdout=sys.stdout)
     pytest_path = project.joinpath('.venvs', 'test', 'bin', 'pytest')
     assert pytest_path.exists()
     result = subprocess.run([str(pytest_path), '--version'], capture_output=True)
     assert result.returncode == 0
     assert result.stderr.decode() == 'pytest 6.2.1\n'
```

### Comparing `flitenv-0.3.4/tests/test_lock.py` & `flitenv-0.4.0/tests/test_lock.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+from __future__ import annotations
+
 import sys
 from pathlib import Path
+
 from flitenv._cli import main
 
 
 def test_lock_main(project: Path) -> None:
-    cmd = ['--root', str(project), 'main', 'lock']
-    main(argv=cmd, stream=sys.stdout)
+    cmd = ['--root', str(project), 'lock', 'main']
+    main(argv=cmd, stdout=sys.stdout)
     print(list(project.iterdir()))
     path = project / 'requirements.txt'
     assert path.is_file()
     content = path.read_text()
     assert 'pip-tools' in content
     assert 'pytest' not in content
 
 
 def test_lock_test(project: Path) -> None:
-    cmd = ['--root', str(project), 'test', 'lock']
-    main(argv=cmd, stream=sys.stdout)
+    cmd = ['--root', str(project), 'lock', 'test']
+    main(argv=cmd, stdout=sys.stdout)
     print(list(project.iterdir()))
     path = project / 'requirements-test.txt'
     assert path.is_file()
     content = path.read_text()
     assert 'pip-tools' in content
     assert 'pytest' in content
```

### Comparing `flitenv-0.3.4/PKG-INFO` & `flitenv-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flitenv
-Version: 0.3.4
+Version: 0.4.0
 Summary: Manage venvs for a flit project
 Home-page: https://github.com/orsinium-labs/flitenv
 License: MIT
 Keywords: flit,venv
 Author: Gram
 Author-email: gram@orsinium.dev
 Requires-Python: >=3.6
@@ -19,14 +19,15 @@
 Requires-Dist: flit
 Requires-Dist: pip-tools
 Requires-Dist: toml
 Requires-Dist: flake8 ; extra == "lint"
 Requires-Dist: isort ; extra == "lint"
 Requires-Dist: mypy ; extra == "lint"
 Requires-Dist: types-toml ; extra == "lint"
+Requires-Dist: ruff ; extra == "lint"
 Requires-Dist: pytest ; extra == "test"
 Provides-Extra: lint
 Provides-Extra: test
 
 # flitenv
 
 Manage [venvs](https://docs.python.org/3/library/venv.html) and dependencies for [flit](https://flit.pypa.io/en/latest/) projects.
@@ -57,17 +58,17 @@
 1. "Lock file" is a file with exact versions of all dependencies of the project in the given environment, including the transitive ones.
 1. Flitenv uses [requirements.txt](https://pip.pypa.io/en/stable/user_guide/#requirements-files) files generated by [pip-tools](https://github.com/jazzband/pip-tools) as lock files.
 1. It is recommend to generate a lock file for (and only for) the `main` environment.
 1. flitenv follows the flit philosophy. It provides only the most helpful and flexible commands, and you can do anything you ever need by combining them with each other and with other tools.
 
 Below are usage examples. Each example uses `lint` as the target environment and `flake8` as a command we want to run in this environment.
 
-+ `flitenv lint install`: install dependencies. If the venv doesn't exist, it will be created. Can also be used to upgrade dependencies when the lock file has been changed.
-+ `flitenv lint run flake8`: run a command. If the venv doesn't exist, it will be created, and the dependencies will be installed.
-+ `flitenv lint lock`: generate lock file (`requirements-lint.txt`) for the env.
++ `flitenv install lint`: install dependencies. If the venv doesn't exist, it will be created. Can also be used to upgrade dependencies when the lock file has been changed.
++ `flitenv run lint flake8`: run a command. If the venv doesn't exist, it will be created, and the dependencies will be installed.
++ `flitenv lock lint`: generate lock file (`requirements-lint.txt`) for the env.
 + `flitenv main lock`: generate lock file (`requirements.txt`) for the `main` env. If there is no env-specific lock file, this one will be used instead.
 + `flitenv main lock -c ../other-project/requirements.txt`: generate lock file using lock file from another project as a reference. It allows to ensure compatibility of lock files accross multiple projects.
 + `rm requirements.txt && flitenv main lock`: upgrade all dependencies in the lock file.
-+ `rm -rf .venvs/lint && flitenv lint install`: re-create the venv. It is usefult to ensure that all old dependencies.
++ `rm -rf .venvs/lint && flitenv install lint`: re-create the venv. It is usefult to ensure that all old dependencies.
 + `flit build`: build a distribution for the project.
 + `flit install --symlink --python $(which python3.9) --deps=none`: symlink the project into the given Python interpreter without installing dependencies. It is helpful if you want to have nice go-to-definition in vscode across multiple projects.
```

