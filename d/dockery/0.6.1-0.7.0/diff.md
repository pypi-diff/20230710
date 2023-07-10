# Comparing `tmp/dockery-0.6.1.tar.gz` & `tmp/dockery-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockery-0.6.1.tar", last modified: Sun Jul  9 04:29:01 2023, max compression
+gzip compressed data, was "dockery-0.7.0.tar", last modified: Mon Jul 10 02:31:40 2023, max compression
```

## Comparing `dockery-0.6.1.tar` & `dockery-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1082 2023-07-09 04:28:52.567377 dockery-0.6.1/LICENSE
--rw-r--r--   0        0        0     1636 2023-07-09 04:28:52.567377 dockery-0.6.1/README.md
--rw-r--r--   0        0        0      777 2023-07-09 04:29:01.383348 dockery-0.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-09 04:28:52.567377 dockery-0.6.1/src/dockery/__init__.py
--rw-r--r--   0        0        0     4792 2023-07-09 04:28:52.567377 dockery-0.6.1/src/dockery/containers.py
--rw-r--r--   0        0        0     1775 2023-07-09 04:28:52.567377 dockery-0.6.1/src/dockery/custom_widgets.py
--rw-r--r--   0        0        0     1612 2023-07-09 04:28:52.567377 dockery-0.6.1/src/dockery/gui.py
--rw-r--r--   0        0        0     1809 2023-07-09 04:28:52.567377 dockery-0.6.1/src/dockery/images.py
--rw-r--r--   0        0        0     2019 2023-07-09 04:28:52.567377 dockery-0.6.1/src/dockery/logs.py
--rw-r--r--   0        0        0     3738 2023-07-09 04:28:52.567377 dockery-0.6.1/src/dockery/main.py
--rw-r--r--   0        0        0     1742 2023-07-09 04:28:52.571377 dockery-0.6.1/src/dockery/networks.py
--rw-r--r--   0        0        0     1070 2023-07-09 04:28:52.571377 dockery-0.6.1/src/dockery/style.css
--rw-r--r--   0        0        0     1353 2023-07-09 04:28:52.571377 dockery-0.6.1/src/dockery/utils.py
--rw-r--r--   0        0        0     1723 2023-07-09 04:28:52.571377 dockery-0.6.1/src/dockery/volumes.py
--rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 dockery-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-10 02:31:29.778195 dockery-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1640 2023-07-10 02:31:29.778195 dockery-0.7.0/README.md
+-rw-r--r--   0        0        0      777 2023-07-10 02:31:40.654351 dockery-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 02:31:29.778195 dockery-0.7.0/src/dockery/__init__.py
+-rw-r--r--   0        0        0     5201 2023-07-10 02:31:29.778195 dockery-0.7.0/src/dockery/containers.py
+-rw-r--r--   0        0        0     1734 2023-07-10 02:31:29.778195 dockery-0.7.0/src/dockery/custom_widgets.py
+-rw-r--r--   0        0        0     1612 2023-07-10 02:31:29.778195 dockery-0.7.0/src/dockery/gui.py
+-rw-r--r--   0        0        0     2082 2023-07-10 02:31:29.778195 dockery-0.7.0/src/dockery/images.py
+-rw-r--r--   0        0        0     2022 2023-07-10 02:31:29.778195 dockery-0.7.0/src/dockery/logs.py
+-rw-r--r--   0        0        0     4386 2023-07-10 02:31:29.782195 dockery-0.7.0/src/dockery/main.py
+-rw-r--r--   0        0        0      126 2023-07-10 02:31:29.782195 dockery-0.7.0/src/dockery/models.py
+-rw-r--r--   0        0        0     1742 2023-07-10 02:31:29.782195 dockery-0.7.0/src/dockery/networks.py
+-rw-r--r--   0        0        0     1215 2023-07-10 02:31:29.782195 dockery-0.7.0/src/dockery/style.css
+-rw-r--r--   0        0        0     1543 2023-07-10 02:31:29.782195 dockery-0.7.0/src/dockery/utils.py
+-rw-r--r--   0        0        0     1675 2023-07-10 02:31:29.782195 dockery-0.7.0/src/dockery/volumes.py
+-rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 dockery-0.7.0/PKG-INFO
```

### Comparing `dockery-0.6.1/LICENSE` & `dockery-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dockery-0.6.1/README.md` & `dockery-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 </table>
 
 ## Installation
 
 ### From source
 
 ```shell
-git clone git@github.com:marianocarrazana/dockery.git
+git clone https://github.com/marianocarrazana/dockery.git
 cd dockery
 pip install -e .
 # update only:
 git pull
 ```
 
 ### From pip
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 github.com/marianocarrazana/dockery/actions/workflows/release.yml/badge.svg)]
 (https://github.com/marianocarrazana/dockery/actions/workflows/release.yml)
 [https://github.com/marianocarrazana/  [https://github.com/marianocarrazana/
 dockery/assets/17238076/bcff22c9-898c- dockery/assets/17238076/0da0c13c-d84d-
 4877-adac-ddf2e58007c4]                4e8a-8b6f-a0d779c2d98d]
 [https://github.com/marianocarrazana/dockery/assets/17238076/c991ff4b-eebf-
 4495-b67c-2c57e933bd7d]
-## Installation ### From source ```shell git clone git@github.com:
+## Installation ### From source ```shell git clone https://github.com/
 marianocarrazana/dockery.git cd dockery pip install -e . # update only: git
 pull ``` ### From pip ```shell pip install -U dockery ``` ## Usage Run on your
 console: ```shell dockery ``` **Warning:** you will probably need to install
 and run dockery as a root user, or you can add permissions to your user to run
 docker following [this instructions](https://docs.docker.com/engine/install/
 linux-postinstall/#manage-docker-as-a-non-root-user). ## Utils ```shell dockery
 df dockery ps dockery volumes dockery images dockery networks dockery stats ```
```

### Comparing `dockery-0.6.1/pyproject.toml` & `dockery-0.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dockery"
-version = "0.6.1"
+version = "0.7.0"
 description = "Graphical interface for Docker in your console"
 authors = [
     { name = "Mariano Carrazana", email = "marianocarrazana@gmail.com" },
 ]
 dependencies = [
     "docker>=6.1.3",
     "textual>=0.28.0",
```

### Comparing `dockery-0.6.1/src/dockery/containers.py` & `dockery-0.7.0/src/dockery/containers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,105 +1,113 @@
-from textual import work
 from textual.app import ComposeResult
 from textual.widgets import Static, Label
 from textual.reactive import reactive
 from docker import DockerClient, errors
 from docker.models.containers import Container
 from textual.containers import (
     Horizontal,
     Vertical,
     Container as Group,
 )
 
-from .utils import get_cpu_usage, get_mem_usage
+from .utils import get_cpu_usage, get_mem_usage, daemon
 from .logs import LogsButton
 from .custom_widgets import CustomButton, ResponsiveGrid, ReactiveString
+from .models import store
 
 
 class ContainersList(ResponsiveGrid):
     container_count = reactive(0)
 
     def __init__(self, docker: DockerClient, **kargs):
-        self.containers = []
+        self.containers: list[Container] = []
         self.docker = docker
         super().__init__(**kargs)
 
     def on_mount(self) -> None:
         self.get_containers()
-        self.set_interval(2, self.count_timer)
-
-    def count_timer(self) -> None:
-        self.get_containers()
+        self.set_interval(2, self.get_containers)
 
     async def watch_container_count(self, count: int) -> None:
         await self.grid.remove_children()
+        images_in_use = []
         for c in self.containers:
-            cw = ContainerWidget(c, self.docker)  # type: ignore
+            cw = ContainerWidget(c, self.docker, classes="li")
             self.grid.mount(cw)
+            images_in_use.append(c.image.id)  # type: ignore
+        store.containers_images = images_in_use
 
-    @work(exclusive=True)
+    @daemon
     def get_containers(self) -> None:
-        self.containers = self.docker.containers.list(all=True)
+        self.containers = self.docker.containers.list(all=True)  # type: ignore
         self.container_count = len(self.containers)
 
 
 class ContainerWidget(Static):
     def __init__(self, container: Container, client: DockerClient, **kargs):
         self.container = container
         self.client = client
         self.container_id = container.id
+        self.running = False
         super().__init__(**kargs)
 
     def compose(self) -> ComposeResult:
         yield Group(
             Label("[b]" + (self.container.name or ""), classes="container-name"),
             Vertical(
-                ReactiveString(id="status"),
-                Horizontal(ReactiveString(id="cpu"), ReactiveString(id="mem")),
+                ReactiveString(classes="status"),
+                Horizontal(
+                    ReactiveString(classes="cpu"), ReactiveString(classes="mem")
+                ),
                 classes="stats-text",
             ),
             classes="container-info",
         )
 
         yield Group(StatusButtons(self.container))
 
     def on_mount(self):
-        self.status_widget = self.query_one("#status", ReactiveString)
-        self.cpu_widget = self.query_one("#cpu", ReactiveString)
-        self.mem_widget = self.query_one("#mem", ReactiveString)
-        self.set_interval(1, self.data_timer)
-        self.running = True
+        self.status_widget = self.query_one(".status", ReactiveString)
+        self.cpu_widget = self.query_one(".cpu", ReactiveString)
+        self.mem_widget = self.query_one(".mem", ReactiveString)
+        self.set_interval(1, self.update_data)
+        self.mounted = True
         self.update_usage()
 
-    def data_timer(self) -> None:
-        self.update_data()
-
-    @work(exclusive=True)
+    @daemon
     def update_data(self) -> None:
         try:
             self.container.reload()
         except errors.NotFound:
             return None
         else:
             status = self.container.status.capitalize()
+            self.running = status == "Running"
             self.status_widget.text = (
-                "[green]" if status == "Running" else "[bright_black]"
+                "[green]" if self.running else "[bright_black]"
             ) + status
+            self.classes = "li running" if self.running else "li"
 
-    @work
+    @daemon
     def update_usage(self) -> None:
         for stat in self.container.stats(stream=True, decode=True):
-            if not self.running:  # finish the thread
+            if not self.mounted:  # finish the thread
                 return None
-            mem_mb, mem_percent = get_mem_usage(stat)
-            self.cpu_widget.text = f"CPU: {get_cpu_usage(stat):.1f}%"
-            self.mem_widget.text = f"MEM: {mem_mb:.1f}MB({mem_percent:.1f}%)"
+            if self.running:
+                mem_mb, mem_percent = get_mem_usage(stat)
+                cpu_text = f"CPU: {get_cpu_usage(stat):.1f}%"
+                mem_text = f"MEM: {mem_mb:.1f}MB({mem_percent:.1f}%)"
+            else:
+                cpu_text = "CPU: -"
+                mem_text = "MEM: -"
+            self.cpu_widget.text = cpu_text
+            self.mem_widget.text = mem_text
 
     def on_unmount(self):
-        self.running = False
+        self.mounted = False
 
 
 class StatusButtons(Static):
     def __init__(self, container: Container, **kargs):
         self.container = container
         super().__init__(**kargs)
```

### Comparing `dockery-0.6.1/src/dockery/custom_widgets.py` & `dockery-0.7.0/src/dockery/custom_widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 
     def compose(self) -> ComposeResult:
         yield self.grid
 
     def on_mount(self) -> None:
         self.resize()
         self.grid.styles.grid_columns = "1fr"
-        self.grid.styles.grid_rows = "4"
         self.grid.styles.width = "100%"
         self.grid.styles.height = "auto"
 
     def on_resize(self, e: Resize):
         self.resize()
 
     def resize(self):
```

### Comparing `dockery-0.6.1/src/dockery/gui.py` & `dockery-0.7.0/src/dockery/gui.py`

 * *Files identical despite different names*

### Comparing `dockery-0.6.1/src/dockery/images.py` & `dockery-0.7.0/src/dockery/images.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-from textual import work
 from textual.app import ComposeResult
 from textual.widgets import Static, Label
 from textual.reactive import reactive
 from textual.containers import Vertical
 from docker import DockerClient
 from docker.models.images import Image
 
 from .custom_widgets import ResponsiveGrid
+from .models import store
+from .utils import daemon
 
 
 class ImagesList(ResponsiveGrid):
     images_count = reactive(0)
 
     def __init__(self, docker: DockerClient, **kargs):
-        self.images = []
+        self.images: list[Image] = []
         self.docker = docker
         super().__init__(**kargs)
 
     def on_mount(self) -> None:
         self.get_images()
-        self.set_interval(2, self.count_timer)
-
-    def count_timer(self) -> None:
-        self.get_images()
+        self.set_interval(2, self.get_images)
 
     async def watch_images_count(self, count: int) -> None:
         await self.grid.remove_children()
         for c in self.images:
-            cw = ImageWidget(c, self.docker)  # type: ignore
+            cw = ImageWidget(c, self.docker, classes="li")
             self.grid.mount(cw)
 
-    @work(exclusive=True)
+    @daemon
     def get_images(self) -> None:
-        self.images = self.docker.images.list(all=False)
+        self.images = self.docker.images.list(all=False)  # type: ignore
         self.images_count = len(self.images)
 
 
 class ImageWidget(Static):
     def __init__(self, image: Image, client: DockerClient, **kargs):
         self.image = image
         self.client = client
@@ -53,7 +51,18 @@
 
     def compose(self) -> ComposeResult:
         yield Vertical(
             Label("[b]" + self.tag),
             Label(self.short_id),
             Label(f"Size: {self.isize:.2f}MB"),
         )
+
+    def on_mount(self):
+        self.set_interval(2, self.update_usage)
+
+    @daemon
+    def update_usage(self):
+        print(self.image.id)
+        print(store.containers_images)
+        self.classes = (
+            "li running" if self.image.id in store.containers_images else "li"
+        )
```

### Comparing `dockery-0.6.1/src/dockery/logs.py` & `dockery-0.7.0/src/dockery/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from textual import work
 import time
 from textual.app import ComposeResult
 from textual.widgets import Static, TextLog, Tabs
 from textual.reactive import reactive
 from textual.containers import VerticalScroll
 from docker.models.containers import Container
 
 from .custom_widgets import CustomButton
+from .utils import daemon
 
 
 class LogsButton(Static):
     def __init__(self, container: Container, **kargs):
         self.container = container
         super().__init__(**kargs)
 
@@ -40,15 +40,15 @@
     def on_mount(self) -> None:
         self.running = True
         self.update_log()
 
     async def watch_last_log(self, new_log: str):
         self.write(new_log)
 
-    @work
+    @daemon
     def update_log(self) -> None:
         # Get the last 40 logs(get all logs can be slow)
         logs: bytes = self.container.logs(tail=40)
         self.last_log = logs.decode("utf-8", errors="ignore")
         # Start streaming logs(since last second)
         for log in self.container.logs(stream=True, since=time.time() - 1):
             if not self.running:
```

### Comparing `dockery-0.6.1/src/dockery/main.py` & `dockery-0.7.0/src/dockery/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import docker
 from docker import errors
 from docker.models.containers import Container
 from docker.models.volumes import Volume
 from docker.models.images import Image
 from docker.models.networks import Network
+from docker.models.configs import Config
+from docker.models.secrets import Secret
 import click
 from rich import print
 
 from .gui import AppGUI
 from .utils import var_dump
 
 default_options = [
@@ -125,17 +127,37 @@
             for log in container.logs(stream=True):
                 print(log.decode("utf-8", errors="ignore"), end="")
         else:
             logs: bytes = container.logs()
             print(logs.decode("utf-8", errors="ignore"))
 
 
+@click.command
+@add_options(default_options)
+def configs(**kargs):
+    client = get_client(**kargs)
+    conf: list[Config] = client.configs.list()  # type: ignore
+    conf_list = list(map(lambda x: x.attrs, conf))
+    var_dump(conf_list, kargs["format"])
+
+
+@click.command
+@add_options(default_options)
+def secrets(**kargs):
+    client = get_client(**kargs)
+    secr: list[Secret] = client.secrets.list()  # type: ignore
+    secr_list = list(map(lambda x: x.attrs, secr))
+    var_dump(secr_list, kargs["format"])
+
+
 main.add_command(df)
 main.add_command(volumes)
 main.add_command(ps)
 main.add_command(stats)
 main.add_command(images)
 main.add_command(networks)
 main.add_command(logs)
+main.add_command(configs)
+main.add_command(secrets)
 
 if __name__ == "__main__":
     main()
```

### Comparing `dockery-0.6.1/src/dockery/networks.py` & `dockery-0.7.0/src/dockery/networks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from textual import work
 from textual.app import ComposeResult
 from textual.widgets import Static, Label
 from textual.reactive import reactive
-from textual.containers import  Vertical, Horizontal
+from textual.containers import Vertical, Horizontal
 from docker import DockerClient
 from docker.models.networks import Network
 
 from .custom_widgets import ResponsiveGrid
+from .utils import daemon
 
 
 class NetworkList(ResponsiveGrid):
     networks_count = reactive(0)
 
     def __init__(self, docker: DockerClient, **kargs):
         self.networks = []
@@ -23,18 +23,18 @@
 
     def count_timer(self) -> None:
         self.get_networks()
 
     async def watch_networks_count(self, count: int) -> None:
         await self.grid.remove_children()
         for c in self.networks:
-            cw = NetworkWidget(c, self.docker)  # type: ignore
+            cw = NetworkWidget(c, self.docker, classes="li")  # type: ignore
             self.grid.mount(cw)
 
-    @work(exclusive=True)
+    @daemon
     def get_networks(self) -> None:
         self.networks = self.docker.networks.list()
         self.networks_count = len(self.networks)
 
 
 class NetworkWidget(Static):
     def __init__(self, network: Network, client: DockerClient, **kargs):
```

### Comparing `dockery-0.6.1/src/dockery/style.css` & `dockery-0.7.0/src/dockery/style.css`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-ContainerWidget,
-ImageWidget,
-NetworkWidget,
-VolumeWidget {
+.li {
     layout: horizontal;
-    background: $boost;
-    height: 3;
-    margin: 1;
+    height: 5;
+    margin: 0 2;
     min-width: 50;
-    padding: 0 2;
+    padding: 0 1;
+    border: round gray;
+}
+
+.li.running {
+    border: round greenyellow;
+}
+
+ResponsiveGrid Grid {
+    grid-rows: 5;
+    grid-gutter: 0;
 }
 
 Footer {
     background: $background-lighten-2;
 }
 
 Footer .footer--description {
@@ -34,15 +40,20 @@
     width: 1fr;
 }
 
 .stats-text {
     width: 1fr;
 }
 
-.stats-text > Horizontal > ReactiveString {
+.stats-text > Horizontal > ReactiveString.cpu {
+    width: 12;
+    height: 1;
+}
+
+.stats-text > Horizontal > ReactiveString.mem {
     width: 20;
     height: 1;
 }
 
 CustomButton {
     height: 3;
     padding: 1 2;
@@ -62,15 +73,15 @@
 }
 
 StartStopButton {
     width: 11;
 }
 
 TabPane {
-    height: 100;
+    height: 100%;
 }
 
 #header {
     dock: top;
     height: 3;
 }
```

### Comparing `dockery-0.6.1/src/dockery/utils.py` & `dockery-0.7.0/src/dockery/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from threading import Thread
 from typing import Any, Literal
 from rich.console import Console
 from rich.syntax import Syntax
 import yaml
 
 console = Console()
 
@@ -32,17 +33,24 @@
     mem_used = (
         mem_stats["usage"]
         - mem_stats["stats"].get("cache", 0)
         + mem_stats["stats"]["active_file"]
     )
     limit = stats["memory_stats"]["limit"]
     percentage = mem_used / limit * 100
-    return (mem_used/1000000, percentage)
+    return (mem_used / 1000000, percentage)
 
 
 def var_dump(obj: Any, syntax: Literal["json", "yaml"] = "yaml"):
     if syntax == "yaml":
         text_obj = yaml.safe_dump(obj, indent=2)
     elif syntax == "json":
         text_obj = json.dumps(obj, default=str, indent=2)
     out = Syntax(text_obj, syntax, theme="ansi_dark")
     console.print(out)
+
+
+def daemon(func):
+    def wrapper_func(*args, **kwargs):
+        Thread(target=func, args=args, kwargs=kwargs, daemon=True).start()
+
+    return wrapper_func
```

### Comparing `dockery-0.6.1/src/dockery/volumes.py` & `dockery-0.7.0/src/dockery/volumes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-from textual import work
 from textual.app import ComposeResult
 from textual.widgets import Static, Label
 from textual.reactive import reactive
 from textual.containers import Vertical, Horizontal
 from docker import DockerClient
 from docker.models.volumes import Volume
 
 from .custom_widgets import ResponsiveGrid
+from .utils import daemon
 
 
 class VolumesList(ResponsiveGrid):
     volumes_count = reactive(0)
 
     def __init__(self, docker: DockerClient, **kargs):
-        self.volumes = []
+        self.volumes: list[Volume] = []
         self.docker = docker
         super().__init__(**kargs)
 
     def on_mount(self) -> None:
         self.get_volumes()
-        self.set_interval(2, self.count_timer)
-
-    def count_timer(self) -> None:
-        self.get_volumes()
+        self.set_interval(2, self.get_volumes)
 
     async def watch_volumes_count(self, count: int) -> None:
         await self.grid.remove_children()
         for c in self.volumes:
-            cw = VolumeWidget(c, self.docker)  # type: ignore
+            cw = VolumeWidget(c, self.docker, classes="li")
             self.grid.mount(cw)
 
-    @work(exclusive=True)
+    @daemon
     def get_volumes(self) -> None:
-        self.volumes = self.docker.volumes.list()
+        self.volumes = self.docker.volumes.list()  # type: ignore
         self.volumes_count = len(self.volumes)
 
 
 class VolumeWidget(Static):
     def __init__(self, volume: Volume, client: DockerClient, **kargs):
         self.volume = volume
         self.client = client
```

### Comparing `dockery-0.6.1/PKG-INFO` & `dockery-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockery
-Version: 0.6.1
+Version: 0.7.0
 Summary: Graphical interface for Docker in your console
 Author-Email: Mariano Carrazana <marianocarrazana@gmail.com>
 License: MIT
 Project-URL: Bug tracker, https://github.com/marianocarrazana/dockery/issues
 Project-URL: Source code, https://github.com/marianocarrazana/dockery
 Requires-Python: >=3.9
 Requires-Dist: docker>=6.1.3
@@ -30,15 +30,15 @@
 </table>
 
 ## Installation
 
 ### From source
 
 ```shell
-git clone git@github.com:marianocarrazana/dockery.git
+git clone https://github.com/marianocarrazana/dockery.git
 cd dockery
 pip install -e .
 # update only:
 git pull
 ```
 
 ### From pip
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: dockery Version: 0.6.1 Summary: Graphical interface
+Metadata-Version: 2.1 Name: dockery Version: 0.7.0 Summary: Graphical interface
 for Docker in your console Author-Email: Mariano Carrazana
 gmail.com> License: MIT Project-URL: Bug tracker, https://github.com/
 marianocarrazana/dockery/issues Project-URL: Source code, https://github.com/
 marianocarrazana/dockery Requires-Python: >=3.9 Requires-Dist: docker>=6.1.3
 Requires-Dist: textual>=0.28.0 Requires-Dist: click>=8.1.3 Requires-Dist:
 pyyaml>=6.0 Description-Content-Type: text/markdown # dockery Graphical
 interface for Docker in your console [![Release](https://github.com/
 marianocarrazana/dockery/actions/workflows/release.yml/badge.svg)](https://
 github.com/marianocarrazana/dockery/actions/workflows/release.yml)
 [https://github.com/marianocarrazana/  [https://github.com/marianocarrazana/
 dockery/assets/17238076/bcff22c9-898c- dockery/assets/17238076/0da0c13c-d84d-
 4877-adac-ddf2e58007c4]                4e8a-8b6f-a0d779c2d98d]
 [https://github.com/marianocarrazana/dockery/assets/17238076/c991ff4b-eebf-
 4495-b67c-2c57e933bd7d]
-## Installation ### From source ```shell git clone git@github.com:
+## Installation ### From source ```shell git clone https://github.com/
 marianocarrazana/dockery.git cd dockery pip install -e . # update only: git
 pull ``` ### From pip ```shell pip install -U dockery ``` ## Usage Run on your
 console: ```shell dockery ``` **Warning:** you will probably need to install
 and run dockery as a root user, or you can add permissions to your user to run
 docker following [this instructions](https://docs.docker.com/engine/install/
 linux-postinstall/#manage-docker-as-a-non-root-user). ## Utils ```shell dockery
 df dockery ps dockery volumes dockery images dockery networks dockery stats ```
```

