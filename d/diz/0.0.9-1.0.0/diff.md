# Comparing `tmp/diz-0.0.9.tar.gz` & `tmp/diz-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diz-0.0.9.tar", last modified: Mon Jul 10 07:32:12 2023, max compression
+gzip compressed data, was "diz-1.0.0.tar", last modified: Mon Jul 10 12:10:09 2023, max compression
```

## Comparing `diz-0.0.9.tar` & `diz-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:32:12.650825 diz-0.0.9/
--rw-r--r--   0 mj         (501) staff       (20)     1368 2023-07-10 07:32:12.650706 diz-0.0.9/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)     1218 2023-07-10 07:28:47.000000 diz-0.0.9/README.md
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:32:12.648302 diz-0.0.9/diz/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-10 03:55:54.000000 diz-0.0.9/diz/__init__.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:32:12.649803 diz-0.0.9/diz/commands/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-0.0.9/diz/commands/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)      480 2023-07-10 07:28:31.000000 diz-0.0.9/diz/commands/install.py
--rw-r--r--   0 mj         (501) staff       (20)     2146 2023-07-10 07:31:06.000000 diz-0.0.9/diz/commands/setup.py
--rw-r--r--   0 mj         (501) staff       (20)      870 2023-07-10 07:08:04.000000 diz-0.0.9/diz/commands/shell.py
--rw-r--r--   0 mj         (501) staff       (20)     1572 2023-07-10 07:26:28.000000 diz-0.0.9/diz/main.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:32:12.650530 diz-0.0.9/diz/utils/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-0.0.9/diz/utils/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)      237 2023-07-09 05:10:52.000000 diz-0.0.9/diz/utils/dir.py
--rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-0.0.9/diz/utils/download.py
--rw-r--r--   0 mj         (501) staff       (20)      762 2023-07-10 04:14:00.000000 diz-0.0.9/diz/utils/pip.py
--rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-0.0.9/diz/utils/validators.py
--rw-r--r--   0 mj         (501) staff       (20)      308 2023-07-10 04:14:09.000000 diz-0.0.9/diz/utils/yaml.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:32:12.649191 diz-0.0.9/diz.egg-info/
--rw-r--r--   0 mj         (501) staff       (20)     1368 2023-07-10 07:32:12.000000 diz-0.0.9/diz.egg-info/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)      423 2023-07-10 07:32:12.000000 diz-0.0.9/diz.egg-info/SOURCES.txt
--rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-10 07:32:12.000000 diz-0.0.9/diz.egg-info/dependency_links.txt
--rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 07:32:12.000000 diz-0.0.9/diz.egg-info/entry_points.txt
--rw-r--r--   0 mj         (501) staff       (20)      129 2023-07-10 07:32:12.000000 diz-0.0.9/diz.egg-info/requires.txt
--rw-r--r--   0 mj         (501) staff       (20)        4 2023-07-10 07:32:12.000000 diz-0.0.9/diz.egg-info/top_level.txt
--rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 07:32:12.650864 diz-0.0.9/setup.cfg
--rw-r--r--   0 mj         (501) staff       (20)      703 2023-07-10 07:31:57.000000 diz-0.0.9/setup.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 12:10:09.751318 diz-1.0.0/
+-rw-r--r--   0 mj         (501) staff       (20)     2242 2023-07-10 12:10:09.751213 diz-1.0.0/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)     2092 2023-07-10 12:09:27.000000 diz-1.0.0/README.md
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 12:10:09.747994 diz-1.0.0/diz/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-10 03:55:54.000000 diz-1.0.0/diz/__init__.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 12:10:09.749364 diz-1.0.0/diz/commands/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-1.0.0/diz/commands/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)      480 2023-07-10 07:28:31.000000 diz-1.0.0/diz/commands/install.py
+-rw-r--r--   0 mj         (501) staff       (20)     2146 2023-07-10 07:31:06.000000 diz-1.0.0/diz/commands/setup.py
+-rw-r--r--   0 mj         (501) staff       (20)     1069 2023-07-10 12:08:33.000000 diz-1.0.0/diz/commands/shell.py
+-rw-r--r--   0 mj         (501) staff       (20)     1979 2023-07-10 12:06:10.000000 diz-1.0.0/diz/main.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 12:10:09.750932 diz-1.0.0/diz/utils/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-1.0.0/diz/utils/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)      237 2023-07-09 05:10:52.000000 diz-1.0.0/diz/utils/dir.py
+-rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-1.0.0/diz/utils/download.py
+-rw-r--r--   0 mj         (501) staff       (20)      831 2023-07-10 08:31:21.000000 diz-1.0.0/diz/utils/pip.py
+-rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-1.0.0/diz/utils/validators.py
+-rw-r--r--   0 mj         (501) staff       (20)     1226 2023-07-10 07:57:15.000000 diz-1.0.0/diz/utils/venv.py
+-rw-r--r--   0 mj         (501) staff       (20)      308 2023-07-10 04:14:09.000000 diz-1.0.0/diz/utils/yaml.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 12:10:09.748633 diz-1.0.0/diz.egg-info/
+-rw-r--r--   0 mj         (501) staff       (20)     2242 2023-07-10 12:10:09.000000 diz-1.0.0/diz.egg-info/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)      441 2023-07-10 12:10:09.000000 diz-1.0.0/diz.egg-info/SOURCES.txt
+-rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-10 12:10:09.000000 diz-1.0.0/diz.egg-info/dependency_links.txt
+-rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 12:10:09.000000 diz-1.0.0/diz.egg-info/entry_points.txt
+-rw-r--r--   0 mj         (501) staff       (20)      129 2023-07-10 12:10:09.000000 diz-1.0.0/diz.egg-info/requires.txt
+-rw-r--r--   0 mj         (501) staff       (20)        4 2023-07-10 12:10:09.000000 diz-1.0.0/diz.egg-info/top_level.txt
+-rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 12:10:09.751355 diz-1.0.0/setup.cfg
+-rw-r--r--   0 mj         (501) staff       (20)      703 2023-07-10 12:09:52.000000 diz-1.0.0/setup.py
```

### Comparing `diz-0.0.9/diz/commands/setup.py` & `diz-1.0.0/diz/commands/setup.py`

 * *Files identical despite different names*

### Comparing `diz-0.0.9/diz/main.py` & `diz-1.0.0/diz/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import typer
 import subprocess
 from diz.commands.setup import SetupCommand
 from diz.commands.install import InstallCommand
 from typing_extensions import Annotated
 from diz.commands.shell import Tmux
+from diz.utils import venv as venv_utils
+from diz.utils import dir
 from enum import Enum
+import os
+
 
 app = typer.Typer()
 
 
 @app.command()
 def setup(path: Annotated[str, typer.Option(prompt="请输入安装目录")],
           pkg: Annotated[str, typer.Option(prompt="请输入配置文件的 URL 地址")]):
@@ -35,30 +39,42 @@
 class Mode(str, Enum):
     attach = 'i'
     detach = 'o'
     kill = 'k'
 
 
 @app.command()
-def shell(index: int = 0, mode: Mode = Mode.attach):
+def shell(index: int = 0, mode: Mode = Mode.attach, auto_venv: bool = False):
     """
     使用 tmux 来实现后台服务管理，方便在服务端进行调试
 
     index: 需要进入第几个后台，默认为 0
 
     mode: 模式，i 为进入，o 为退出，kill 为删除
     """
-    tmux = Tmux(index)
+    tmux = Tmux(index, auto_venv)
     if mode == Mode.attach:
         tmux.attach()
     elif mode == Mode.detach:
         tmux.detach()
     elif mode == Mode.kill:
         tmux.kill()
 
 
+@app.command()
+def venv():
+    """
+    激活虚拟环境
+    """
+    if not dir.is_empty('./venv'):
+        cmd = venv_utils.get_activate_command('./venv')
+        subprocess.run(cmd, shell=True, executable=os.environ.get("SHELL", ''))
+    else:
+        typer.echo("不存在 venv 目录")
+
+
 def main():
     app()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `diz-0.0.9/diz/utils/pip.py` & `diz-1.0.0/diz/utils/pip.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import subprocess
 import requests
 from diz.utils import validators
+from diz.utils import venv
 import os
 import tempfile
 
 
 def run_command_in_venv(command, venv_path):
-    activate_script = f"{venv_path}/bin/activate"
-    cmd = f"source {activate_script} && {command}"
-    subprocess.run(cmd, shell=True)
+    activate_script = venv.get_activate_command(venv_path)
+    cmd = f"{activate_script} && {command}"
+    subprocess.run(cmd, shell=True, executable=os.environ.get("SHELL", ''))
 
 
 def install(dep, venv_path):
     if validators.is_valid_url(dep):
         install_from_url(dep, venv_path)
     else:
         run_command_in_venv(f"pip install {dep}", venv_path)
```

### Comparing `diz-0.0.9/setup.py` & `diz-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='diz',
-    version='0.0.9',
+    version='1.0.0',
     author='mjason',
     description='用来构建大模型环境的工具',
     long_description=readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'GitPython>=3.1.31',
```

