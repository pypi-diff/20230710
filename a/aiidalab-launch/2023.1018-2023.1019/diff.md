# Comparing `tmp/aiidalab_launch-2023.1018.tar.gz` & `tmp/aiidalab_launch-2023.1019.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiidalab_launch-2023.1018.tar", last modified: Thu Feb 23 10:08:19 2023, max compression
+gzip compressed data, was "aiidalab_launch-2023.1019.tar", last modified: Mon Jul 10 08:19:13 2023, max compression
```

## Comparing `aiidalab_launch-2023.1018.tar` & `aiidalab_launch-2023.1019.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:08:19.179930 aiidalab_launch-2023.1018/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-02-23 10:08:19.179930 aiidalab_launch-2023.1018/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:08:19.179930 aiidalab_launch-2023.1018/aiidalab_launch/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/aiidalab_launch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23504 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/aiidalab_launch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/aiidalab_launch/application_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/aiidalab_launch/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/aiidalab_launch/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/aiidalab_launch/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/aiidalab_launch/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/aiidalab_launch/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/aiidalab_launch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:08:19.179930 aiidalab_launch-2023.1018/aiidalab_launch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-02-23 10:08:19.000000 aiidalab_launch-2023.1018/aiidalab_launch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-02-23 10:08:19.000000 aiidalab_launch-2023.1018/aiidalab_launch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 10:08:19.000000 aiidalab_launch-2023.1018/aiidalab_launch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-23 10:08:19.000000 aiidalab_launch-2023.1018/aiidalab_launch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-02-23 10:08:19.000000 aiidalab_launch-2023.1018/aiidalab_launch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 10:08:19.000000 aiidalab_launch-2023.1018/aiidalab_launch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:08:19.179930 aiidalab_launch-2023.1018/logos/
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/logos/MARVEL.png
--rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/logos/MaX.png
--rw-r--r--   0 runner    (1001) docker     (123)    27591 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/logos/MarketPlace.png
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-02-23 10:08:19.183930 aiidalab_launch-2023.1018/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-02-23 10:08:02.000000 aiidalab_launch-2023.1018/ssh-forward.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:13.631614 aiidalab_launch-2023.1019/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-10 08:19:13.631614 aiidalab_launch-2023.1019/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:13.627614 aiidalab_launch-2023.1019/aiidalab_launch/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/aiidalab_launch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23961 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/aiidalab_launch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/aiidalab_launch/application_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/aiidalab_launch/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/aiidalab_launch/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/aiidalab_launch/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/aiidalab_launch/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/aiidalab_launch/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/aiidalab_launch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:13.627614 aiidalab_launch-2023.1019/aiidalab_launch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-10 08:19:13.000000 aiidalab_launch-2023.1019/aiidalab_launch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-10 08:19:13.000000 aiidalab_launch-2023.1019/aiidalab_launch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:19:13.000000 aiidalab_launch-2023.1019/aiidalab_launch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 08:19:13.000000 aiidalab_launch-2023.1019/aiidalab_launch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-10 08:19:13.000000 aiidalab_launch-2023.1019/aiidalab_launch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 08:19:13.000000 aiidalab_launch-2023.1019/aiidalab_launch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:13.631614 aiidalab_launch-2023.1019/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/logos/MARVEL.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/logos/MaX.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27591 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/logos/MarketPlace.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-10 08:19:13.631614 aiidalab_launch-2023.1019/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-10 08:19:02.000000 aiidalab_launch-2023.1019/ssh-forward.md
```

### Comparing `aiidalab_launch-2023.1018/CONTRIBUTING.md` & `aiidalab_launch-2023.1019/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiidalab_launch-2023.1018/LICENSE` & `aiidalab_launch-2023.1019/LICENSE`

 * *Files identical despite different names*

### Comparing `aiidalab_launch-2023.1018/PKG-INFO` & `aiidalab_launch-2023.1019/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiidalab_launch
-Version: 2023.1018
+Version: 2023.1019
 Summary: Tool to launch AiiDAlab on a local workstation.
 Home-page: https://github.com/aiidalab/aiidalab-launch
 Author: Carl Simon Adorf and the AiiDAlab team
 Author-email: aiidalab@materialscloud.org
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AiiDA
@@ -58,15 +58,15 @@
 ```console
 aiidalab-launch status
 ```
 
 ### Profile Management
 
 The tool allows to manage multiple profiles, e.g., with different home directories or ports.
-See `aiidalab-launch profiles --help` for more information.
+See `aiidalab-launch profile --help` for more information.
 
 ### Data Management
 
 By default AiiDAlab will store all of its data in a [Docker volume](https://docs.docker.com/storage/volumes/) defined in the profile configuration option `home_mount`.
 You can also provide an absolute path to the AiiDAlab home directory on the host system (so called [bind mount](https://docs.docker.com/storage/bind-mounts/)).
 If this directory does not exist, AiiDAlab launch will try to create it on startup.
```

### Comparing `aiidalab_launch-2023.1018/README.md` & `aiidalab_launch-2023.1019/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 ```console
 aiidalab-launch status
 ```
 
 ### Profile Management
 
 The tool allows to manage multiple profiles, e.g., with different home directories or ports.
-See `aiidalab-launch profiles --help` for more information.
+See `aiidalab-launch profile --help` for more information.
 
 ### Data Management
 
 By default AiiDAlab will store all of its data in a [Docker volume](https://docs.docker.com/storage/volumes/) defined in the profile configuration option `home_mount`.
 You can also provide an absolute path to the AiiDAlab home directory on the host system (so called [bind mount](https://docs.docker.com/storage/bind-mounts/)).
 If this directory does not exist, AiiDAlab launch will try to create it on startup.
```

### Comparing `aiidalab_launch-2023.1018/aiidalab_launch/__main__.py` & `aiidalab_launch-2023.1019/aiidalab_launch/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import docker
 from packaging.version import parse
 from tabulate import tabulate
 
 from .application_state import ApplicationState
 from .core import LOGGER
 from .instance import AiidaLabInstance
-from .profile import DEFAULT_PORT, Profile
+from .profile import DEFAULT_IMAGE, DEFAULT_PORT, Profile
 from .util import confirm_with_value, get_latest_version, spinner, webbrowser_available
 from .version import __version__
 
 MSG_MOUNT_POINT_CONFLICT = """Warning: There is at least one other running
 instance that has the same home mount point ('{home_mount}') as the instance
 you are currently trying to start. Are you sure you want to continue? This may
 lead to data corruption."""
@@ -83,15 +83,15 @@
         return app_state.config.get_profile(name)
 
     return click.option(
         "-p", "--profile", help="Select profile to use.", callback=callback
     )(cmd)
 
 
-@click.group()
+@click.group(context_settings={"help_option_names": ["-h", "--help"]})
 @click.option(
     "-v",
     "--verbose",
     count=True,
     help=(
         "Increase the output verbosity of the launcher. "
         "Use '-vv' or '-vvv' for even more verbose output"
@@ -133,20 +133,20 @@
 @cli.command()
 def version():
     """Show the version of aiidalab-launch."""
     click.echo(click.style(f"AiiDAlab Launch {__version__}", bold=True))
 
 
 @cli.group()
-def profiles():
+def profile():
     """Manage AiiDAlab profiles."""
     pass
 
 
-@profiles.command("list")
+@profile.command("list")
 @pass_app_state
 def list_profiles(app_state):
     """List all configured AiiDAlab profiles.
 
     The default profile is shown in bold.
     """
     default_profile = app_state.config.default_profile
@@ -159,23 +159,23 @@
                 )
                 for profile in app_state.config.profiles
             ]
         )
     )
 
 
-@profiles.command("show")
+@profile.command("show")
 @click.argument("profile")
 @pass_app_state
 def show_profile(app_state, profile):
     """Show an AiiDAlab profile configuration."""
     click.echo(app_state.config.get_profile(profile).dumps(), nl=False)
 
 
-@profiles.command("add")
+@profile.command("add")
 @click.argument("profile")
 @click.option(
     "--port",
     type=click.IntRange(min=1, max=65535),
     help=(
         "Specify port on which this instance will be exposed. The default port "
         "is chosen such that it does not conflict with any currently configured "
@@ -183,46 +183,53 @@
     ),
 )
 @click.option(
     "--home-mount",
     type=click.Path(file_okay=False),
     help="Specify the path to be mounted as home directory.",
 )
+@click.option(
+    "--image",
+    type=click.STRING,
+    help="Specify the image to be used for the profile.",
+)
 @pass_app_state
 @click.pass_context
-def add_profile(ctx, app_state, port, home_mount, profile):
+def add_profile(ctx, app_state, port, home_mount, image, profile):
     """Add a new AiiDAlab profile to the configuration."""
     try:
         app_state.config.get_profile(profile)
     except ValueError:
         pass
     else:
         raise click.ClickException(f"Profile with name '{profile}' already exists.")
 
     # Determine next available port or use the one provided by the user.
     configured_ports = [prof.port for prof in app_state.config.profiles if prof.port]
     port = port or (max(configured_ports, default=-1) + 1) or DEFAULT_PORT
+    image = image or DEFAULT_IMAGE
 
     try:
         new_profile = Profile(
             name=profile,
             port=port,
+            image=image,
             home_mount=home_mount,
         )
     except ValueError as error:  # invalid profile name
         raise click.ClickException(error)
 
     app_state.config.profiles.append(new_profile)
     app_state.save_config()
     click.echo(f"Added profile '{profile}'.")
     if click.confirm("Do you want to edit it now?", default=True):
         ctx.invoke(edit_profile, profile=profile)
 
 
-@profiles.command("remove")
+@profile.command("remove")
 @click.argument("profile")
 @click.option("--yes", is_flag=True, help="Do not ask for confirmation.")
 @click.option("-f", "--force", is_flag=True, help="Proceed, ignoring any warnings.")
 @pass_app_state
 def remove_profile(app_state, profile, yes, force):
     """Remove an AiiDAlab profile from the configuration."""
     try:
@@ -248,15 +255,15 @@
             f"Are you sure you want to remove profile '{profile.name}'?"
         ):
             app_state.config.profiles.remove(profile)
             app_state.save_config()
             click.echo(f"Removed profile with name '{profile.name}'.")
 
 
-@profiles.command("edit")
+@profile.command("edit")
 @click.argument("profile")
 @pass_app_state
 def edit_profile(app_state, profile):
     """Edit an AiiDAlab profile configuration."""
     current_profile = app_state.config.get_profile(profile)
     profile_edit = click.edit(current_profile.dumps(), extension=".toml")
     if profile_edit:
@@ -265,15 +272,15 @@
             app_state.config.profiles.remove(current_profile)
             app_state.config.profiles.append(new_profile)
             app_state.save_config()
             return
     click.echo("No changes.")
 
 
-@profiles.command("set-default")
+@profile.command("set-default")
 @click.argument("profile")
 @pass_app_state
 def set_default_profile(app_state, profile):
     """Set an AiiDAlab profile as default."""
     try:
         app_state.config.get_profile(profile)
     except ValueError:
@@ -325,37 +332,41 @@
             msg_warn = MSG_MOUNT_POINT_CONFLICT.format(home_mount=profile.home_mount)
             click.confirm(
                 click.style("\n".join(wrap(msg_warn)), fg="yellow"),
                 abort=True,
             )
 
     # Obtain image (either via pull or local).
-    if pull:
-        msg = (
-            f"Downloading image '{instance.profile.image}', this may take a while..."
-            if instance.image is None
-            else f"Downloading latest version of '{instance.profile.image}'..."
-        )
+    if instance.image is None:
+        # always pull if no image is available
+        msg = f"Downloading image '{profile.image}', this may take a while..."
         with spinner(msg):
             instance.pull()
+    elif pull:
+        # pull if explicitly requested and pull latest version of image
+        msg = f"Downloading latest version of '{profile.image}'..."
+        with spinner(msg):
+            instance.pull()
+    else:
+        # use local image
+        msg = f"Using local image '{profile.image}'."
 
     if instance.image is None:
         raise click.ClickException(
             f"Unable to find image '{profile.image}'. "
             "Try to use '--pull' to pull the image prior to start."
         )
 
     # Check if the container configuration has changed.
     if instance.container:
         configuration_changed = any(instance.configuration_changes())
     else:
         configuration_changed = False
 
     try:
-
         InstanceStatus = instance.AiidaLabInstanceStatus  # local alias for brevity
 
         status = await instance.status()
 
         # Container needs to be started.
         if status in (
             InstanceStatus.DOWN,
@@ -401,15 +412,15 @@
             )
 
     except docker.errors.APIError as error:
         LOGGER.debug(f"Error during startup: {error}")
         if instance.profile.port and "port is already allocated" in str(error):
             raise click.ClickException(
                 f"Port {instance.profile.port} is already allocated, choose another port "
-                f"for example, by editing the profile: aiidalab-launch profiles edit {instance.profile.name}"
+                f"for example, by editing the profile: aiidalab-launch profile edit {instance.profile.name}"
             )
         raise click.ClickException("Startup failed due to an unexpected error.")
     except asyncio.TimeoutError:
         raise click.ClickException(
             "AiiDAlab instance did not start up within the excepted wait period."
         )
     except Exception as error:
@@ -496,15 +507,15 @@
     "--wait",
     default=120,
     show_default=True,
     help="Time to wait after startup until all services are up. Set to zero to not wait at all and immediately return.",
 )
 @click.option(
     "--pull/--no-pull",
-    default=True,
+    default=False,
     help=(
         "Specify whether to pull the configured image prior to the first start "
         "of the container."
     ),
     show_default=True,
 )
 @click.option(
```

### Comparing `aiidalab_launch-2023.1018/aiidalab_launch/application_state.py` & `aiidalab_launch-2023.1019/aiidalab_launch/application_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         return Config.load(_application_config_path())
     except FileNotFoundError:
         return Config()
 
 
 @dataclass
 class ApplicationState:
-
     config_path: Path = field(default_factory=_application_config_path)
     config: Config = field(default_factory=_load_config)
     docker_client: docker.DockerClient = field(default_factory=get_docker_client)
 
     def save_config(self):
         self.config.save(self.config_path)
```

### Comparing `aiidalab_launch-2023.1018/aiidalab_launch/config.py` & `aiidalab_launch-2023.1019/aiidalab_launch/config.py`

 * *Files identical despite different names*

### Comparing `aiidalab_launch-2023.1018/aiidalab_launch/instance.py` & `aiidalab_launch-2023.1019/aiidalab_launch/instance.py`

 * *Files identical despite different names*

### Comparing `aiidalab_launch-2023.1018/aiidalab_launch/profile.py` & `aiidalab_launch-2023.1019/aiidalab_launch/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 _REGEX_VALID_PROFILE_NAMES = r"[a-zA-Z0-9][a-zA-Z0-9.-]+"
 
 
 def _default_port() -> int:  # explicit function required to enable test patching
     return DEFAULT_PORT
 
 
-_DEFAULT_IMAGE = "aiidalab/full-stack:latest"
+DEFAULT_IMAGE = "aiidalab/full-stack:latest"
 
 
 def _valid_volume_name(source: str) -> None:
     # We do not allow relative paths so if the path is not absolute,
     # we assume volume mount, whose name is restricted by Docker.
     if not Path(source).is_absolute() and not re.fullmatch(
         _REGEX_VALID_IMAGE_NAMES, source
@@ -63,15 +63,15 @@
 
 @dataclass
 class Profile:
     name: str = MAIN_PROFILE_NAME
     port: int | None = field(default_factory=_default_port)
     default_apps: list[str] = field(default_factory=lambda: [])
     system_user: str = "jovyan"
-    image: str = _DEFAULT_IMAGE
+    image: str = DEFAULT_IMAGE
     home_mount: str | None = None
     extra_mounts: set[str] = field(default_factory=set)
 
     def __post_init__(self):
         if (
             not re.fullmatch(_REGEX_VALID_PROFILE_NAMES, self.name)
             or quote_plus(self.name) != self.name
@@ -155,16 +155,16 @@
             raise RuntimeError(
                 f"Container {container.id} does not appear to be an AiiDAlab container."
             )
 
         system_user = get_docker_env(container, "SYSTEM_USER")
 
         image_tag = (
-            _DEFAULT_IMAGE
-            if _DEFAULT_IMAGE in container.image.tags
+            DEFAULT_IMAGE
+            if DEFAULT_IMAGE in container.image.tags
             else container.image.tags[0]
         )
 
         extra_destinations: list[PurePosixPath] = [
             PurePosixPath(mount["Destination"])
             for mount in container.attrs["Mounts"]
             if mount["Destination"]
```

### Comparing `aiidalab_launch-2023.1018/aiidalab_launch/util.py` & `aiidalab_launch-2023.1019/aiidalab_launch/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 @contextmanager
 def spinner(
     msg: Optional[str] = None, final: Optional[str] = "done.", delay: float = 0
 ) -> Generator[None, None, None]:
     """Display spinner only after an optional initial delay."""
 
     def spin() -> None:
-
         # Don't show spinner if verbose output is enabled
         level = logging.getLogger().getEffectiveLevel()
         show_spinner = (
             True if level == logging.NOTSET or level >= logging.ERROR else False
         )
         if msg:
             newline = not show_spinner
```

### Comparing `aiidalab_launch-2023.1018/aiidalab_launch.egg-info/PKG-INFO` & `aiidalab_launch-2023.1019/aiidalab_launch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiidalab-launch
-Version: 2023.1018
+Version: 2023.1019
 Summary: Tool to launch AiiDAlab on a local workstation.
 Home-page: https://github.com/aiidalab/aiidalab-launch
 Author: Carl Simon Adorf and the AiiDAlab team
 Author-email: aiidalab@materialscloud.org
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AiiDA
@@ -58,15 +58,15 @@
 ```console
 aiidalab-launch status
 ```
 
 ### Profile Management
 
 The tool allows to manage multiple profiles, e.g., with different home directories or ports.
-See `aiidalab-launch profiles --help` for more information.
+See `aiidalab-launch profile --help` for more information.
 
 ### Data Management
 
 By default AiiDAlab will store all of its data in a [Docker volume](https://docs.docker.com/storage/volumes/) defined in the profile configuration option `home_mount`.
 You can also provide an absolute path to the AiiDAlab home directory on the host system (so called [bind mount](https://docs.docker.com/storage/bind-mounts/)).
 If this directory does not exist, AiiDAlab launch will try to create it on startup.
```

### Comparing `aiidalab_launch-2023.1018/aiidalab_launch.egg-info/SOURCES.txt` & `aiidalab_launch-2023.1019/aiidalab_launch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiidalab_launch-2023.1018/logos/MARVEL.png` & `aiidalab_launch-2023.1019/logos/MARVEL.png`

 * *Files identical despite different names*

### Comparing `aiidalab_launch-2023.1018/logos/MaX.png` & `aiidalab_launch-2023.1019/logos/MaX.png`

 * *Files identical despite different names*

### Comparing `aiidalab_launch-2023.1018/logos/MarketPlace.png` & `aiidalab_launch-2023.1019/logos/MarketPlace.png`

 * *Files identical despite different names*

### Comparing `aiidalab_launch-2023.1018/setup.cfg` & `aiidalab_launch-2023.1019/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 description = Tool to launch AiiDAlab on a local workstation.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/aiidalab/aiidalab-launch
 author = Carl Simon Adorf and the AiiDAlab team
 author_email = aiidalab@materialscloud.org
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
 	Framework :: AiiDA
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 
 [options]
 packages = find:
 install_requires = 
-	click==8.0.3
+	click==8.1
 	click-spinner==0.1.10
 	docker==5.0.3
 	packaging==21.3
 	python-dotenv==0.19.1
 	requests==2.26.0
 	requests-cache==0.9.1
 	tabulate==0.8.9
@@ -38,18 +38,18 @@
 [options.extras_require]
 dev = 
 	bumpver==2021.1114
 	dunamai==1.7.0
 pre_commit = 
 	pre-commit==2.15.0
 tests = 
-	pytest==6.2.5
-	pytest-asyncio==0.17.2
-	pytest-cov==3.0.0
-	responses==0.18.0
+	pytest==7.2.1
+	pytest-asyncio==0.20.3
+	pytest-cov==4.0.0
+	responses==0.22.0
 
 [flake8]
 ignore = 
 	E501
 	W503
 	E203
 per-file-ignores = 
@@ -59,15 +59,15 @@
 warn_unused_configs = True
 disallow_untyped_calls = True
 
 [mypy-docker.*]
 ignore_missing_imports = True
 
 [bumpver]
-current_version = "v2023.1018"
+current_version = "v2023.1019"
 version_pattern = "vYYYY.BUILD[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
```

### Comparing `aiidalab_launch-2023.1018/ssh-forward.md` & `aiidalab_launch-2023.1019/ssh-forward.md`

 * *Files identical despite different names*

