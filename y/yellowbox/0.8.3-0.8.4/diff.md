# Comparing `tmp/yellowbox-0.8.3.tar.gz` & `tmp/yellowbox-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowbox-0.8.3.tar", max compression
+gzip compressed data, was "yellowbox-0.8.4.tar", max compression
```

## Comparing `yellowbox-0.8.3.tar` & `yellowbox-0.8.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1081 2023-05-28 09:57:20.995778 yellowbox-0.8.3/LICENSE
--rw-r--r--   0        0        0     1265 2023-05-28 09:57:20.995778 yellowbox-0.8.3/README.md
--rw-r--r--   0        0        0     2586 2023-05-28 09:57:20.999778 yellowbox-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      691 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/__init__.py
--rw-r--r--   0        0        0      236 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/_pytest.py
--rw-r--r--   0        0        0       22 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/_version.py
--rw-r--r--   0        0        0      550 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/clients.py
--rw-r--r--   0        0        0    10220 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/containers.py
--rw-r--r--   0        0        0        0 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/__init__.py
--rw-r--r--   0        0        0     2247 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/aerospike.py
--rw-r--r--   0        0        0     4643 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/azure_storage.py
--rw-r--r--   0        0        0     5998 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/fake_gcs.py
--rw-r--r--   0        0        0    10058 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/http_server.py
--rw-r--r--   0        0        0     4792 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/kafka.py
--rw-r--r--   0        0        0    10361 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/logstash.py
--rw-r--r--   0        0        0     2262 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/mssql.py
--rw-r--r--   0        0        0     3598 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/postgresql.py
--rw-r--r--   0        0        0     4426 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/rabbit_mq.py
--rw-r--r--   0        0        0     3255 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/redis.py
--rw-r--r--   0        0        0     7631 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/sql_base.py
--rw-r--r--   0        0        0     5535 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/vault.py
--rw-r--r--   0        0        0      784 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/webserver/__init__.py
--rw-r--r--   0        0        0     4010 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/webserver/class_endpoint.py
--rw-r--r--   0        0        0    13779 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/webserver/endpoints.py
--rw-r--r--   0        0        0    15962 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/webserver/http_request_capture.py
--rw-r--r--   0        0        0     7876 2023-05-28 09:57:20.999778 yellowbox-0.8.3/yellowbox/extras/webserver/request_capture.py
--rw-r--r--   0        0        0     3857 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/extras/webserver/util.py
--rw-r--r--   0        0        0    12332 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/extras/webserver/webserver.py
--rw-r--r--   0        0        0    20155 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/extras/webserver/ws_request_capture.py
--rw-r--r--   0        0        0    14333 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/extras/websocket.py
--rw-r--r--   0        0        0     3408 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/image_build.py
--rw-r--r--   0        0        0     3104 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/networks.py
--rw-r--r--   0        0        0        0 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/py.typed
--rw-r--r--   0        0        0     3564 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/retry.py
--rw-r--r--   0        0        0      578 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/service.py
--rw-r--r--   0        0        0     7164 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/subclasses.py
--rw-r--r--   0        0        0     1986 2023-05-28 09:57:21.003778 yellowbox-0.8.3/yellowbox/utils.py
--rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 yellowbox-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-10 14:48:16.923393 yellowbox-0.8.4/LICENSE
+-rw-r--r--   0        0        0     1265 2023-07-10 14:48:16.923393 yellowbox-0.8.4/README.md
+-rw-r--r--   0        0        0     4879 2023-07-10 14:48:16.923393 yellowbox-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0      728 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/__init__.py
+-rw-r--r--   0        0        0      236 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/_pytest.py
+-rw-r--r--   0        0        0       22 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/_version.py
+-rw-r--r--   0        0        0      546 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/clients.py
+-rw-r--r--   0        0        0    10257 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/containers.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/__init__.py
+-rw-r--r--   0        0        0     2348 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/aerospike.py
+-rw-r--r--   0        0        0     4642 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/azure_storage.py
+-rw-r--r--   0        0        0     6025 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/fake_gcs.py
+-rw-r--r--   0        0        0    10016 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/http_server.py
+-rw-r--r--   0        0        0     5116 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/kafka.py
+-rw-r--r--   0        0        0    10090 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/logstash.py
+-rw-r--r--   0        0        0     2404 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/mssql.py
+-rw-r--r--   0        0        0     3726 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/postgresql.py
+-rw-r--r--   0        0        0     4619 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/rabbit_mq.py
+-rw-r--r--   0        0        0     3234 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/redis.py
+-rw-r--r--   0        0        0     7692 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/sql_base.py
+-rw-r--r--   0        0        0     5597 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/vault.py
+-rw-r--r--   0        0        0      813 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/__init__.py
+-rw-r--r--   0        0        0     4005 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/class_endpoint.py
+-rw-r--r--   0        0        0    13917 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/endpoints.py
+-rw-r--r--   0        0        0    15196 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/http_request_capture.py
+-rw-r--r--   0        0        0     7772 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/request_capture.py
+-rw-r--r--   0        0        0     3812 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/util.py
+-rw-r--r--   0        0        0    12586 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/webserver.py
+-rw-r--r--   0        0        0    19729 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/webserver/ws_request_capture.py
+-rw-r--r--   0        0        0    14228 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/extras/websocket.py
+-rw-r--r--   0        0        0     3456 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/image_build.py
+-rw-r--r--   0        0        0     3104 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/networks.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/py.typed
+-rw-r--r--   0        0        0     3543 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/retry.py
+-rw-r--r--   0        0        0      578 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/service.py
+-rw-r--r--   0        0        0     7596 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/subclasses.py
+-rw-r--r--   0        0        0     2003 2023-07-10 14:48:16.927393 yellowbox-0.8.4/yellowbox/utils.py
+-rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 yellowbox-0.8.4/PKG-INFO
```

### Comparing `yellowbox-0.8.3/LICENSE` & `yellowbox-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.3/README.md` & `yellowbox-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.3/yellowbox/containers.py` & `yellowbox-0.8.4/yellowbox/containers.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,26 @@
 import docker
 from docker import DockerClient
 from docker.errors import ImageNotFound
 from docker.models.containers import Container
 from docker.models.networks import Network
 from requests import HTTPError
 
-__all__ = ['get_ports', 'get_aliases', 'is_alive', 'is_removed', 'killing', 'create_and_pull',
-           'download_file', 'upload_file', 'SafeContainerCreator', 'removing']
+__all__ = [
+    "get_ports",
+    "get_aliases",
+    "is_alive",
+    "is_removed",
+    "killing",
+    "create_and_pull",
+    "download_file",
+    "upload_file",
+    "SafeContainerCreator",
+    "removing",
+]
 
 _DEFAULT_TIMEOUT = 10
 
 _T = TypeVar("_T")
 _CT = TypeVar("_CT", bound=Container)
 
 
@@ -56,16 +66,16 @@
         if external_address is None:
             continue
 
         assert len(external_address) > 0
 
         external_port = int(external_address[0]["HostPort"])
 
-        port, *_ = port.partition("/")  # Strip out type (tcp, udp, ...)
-        ports[int(port)] = int(external_port)
+        port_num, *_ = port.partition("/")  # Strip out type (tcp, udp, ...)
+        ports[int(port_num)] = int(external_port)
 
     return ports
 
 
 def get_aliases(container: Container, network: Union[str, Network]) -> Sequence[str]:
     if not isinstance(network, str):
         network = network.name
@@ -86,20 +96,21 @@
     """
     return container.id[:12]
 
 
 def is_alive(container: Container) -> bool:
     if is_removed(container):
         return False
-    return container.status.lower() not in ('exited', 'stopped')
+    return container.status.lower() not in ("exited", "stopped")
 
 
 @contextmanager
-def killing(container: _CT, *, timeout: float = _DEFAULT_TIMEOUT,
-            signal: str = 'SIGKILL') -> Generator[_CT, None, None]:
+def killing(
+    container: _CT, *, timeout: float = _DEFAULT_TIMEOUT, signal: str = "SIGKILL"
+) -> Generator[_CT, None, None]:
     """A context manager that kills a docker container upon completion.
 
     Example:
         container = DockerContainer(...)
         with killing(container):
             ...
         # Container is now killed with SIGKILL
@@ -118,16 +129,17 @@
     finally:
         if is_alive(container):
             container.kill(signal)
             container.wait(timeout=timeout)
 
 
 @contextmanager
-def removing(container: _CT, *, expected_exit_code: Optional[Union[int, AbstractContainer[int]]] = 0, force=False) \
-        -> Generator[_CT, None, None]:
+def removing(
+    container: _CT, *, expected_exit_code: Optional[Union[int, AbstractContainer[int]]] = 0, force=False
+) -> Generator[_CT, None, None]:
     """A context manager that removes a docker container upon completion.
 
     Example:
         container = DockerContainer(...)
         with removing(container):
             ...
         # Container is now removed
@@ -140,29 +152,28 @@
 
     Returns:
         A context manager to be used in a 'with' statement.
     """
     try:
         yield container
     finally:
-        if is_removed(container):
-            return
-        # checking if the container is removed reloads the container
-        if is_alive(container):
-            if not force:
-                raise RuntimeError(f"Container {container.id} is still alive (status: {container.status})")
-            container.kill('SIGKILL')
-        result = container.wait(timeout=10)
-        if expected_exit_code is not None:
-            if isinstance(expected_exit_code, int):
-                expected_exit_code = (expected_exit_code,)
-
-            if result['StatusCode'] not in expected_exit_code:
-                raise RuntimeError(f"Container {container.id} exited with code {result['StatusCode']}")
-        container.remove(force=force, v=True)
+        if not is_removed(container):
+            # checking if the container is removed reloads the container
+            if is_alive(container):
+                if not force:
+                    raise RuntimeError(f"Container {container.id} is still alive (status: {container.status})")
+                container.kill("SIGKILL")
+            result = container.wait(timeout=10)
+            if expected_exit_code is not None:
+                if isinstance(expected_exit_code, int):
+                    expected_exit_code = (expected_exit_code,)
+
+                if result["StatusCode"] not in expected_exit_code:
+                    raise RuntimeError(f"Container {container.id} exited with code {result['StatusCode']}")
+            container.remove(force=force, v=True)
 
 
 def create_and_pull(docker_client: DockerClient, image: str, *args, **kwargs) -> Container:
     """
     Create a docker container, pulling the image if necessary.
     Args:
         docker_client: the docker client to use.
@@ -175,15 +186,15 @@
 
     Note:
         Due to inconsistent behaviour of docker's "pull" command across
         platforms, this function will raise an error if no tag is specified
     """
     name, _, tag = image.partition(":")
     if not tag:
-        raise ValueError('the image name must contain a tag')
+        raise ValueError("the image name must contain a tag")
     try:
         ret = docker_client.containers.create(image, *args, **kwargs)
     except ImageNotFound:
         docker_client.images.pull(image, platform=None)
         ret = docker_client.containers.create(image, *args, **kwargs)
     return ret
 
@@ -206,15 +217,15 @@
     Raises:
         FileNotFoundError: Path was not found.
         IsADirectoryError: Path is not a regular file.
     """
     realpath = os.fspath(path)
     exc: Exception
     try:
-        iterator, stats = container.get_archive(realpath, chunk_size=None)  # noqa
+        iterator, stats = container.get_archive(realpath, chunk_size=None)
     except docker.errors.NotFound:
         exc = FileNotFoundError(realpath)
         exc.filename = realpath
         raise exc
 
     if stat.S_ISDIR(stats["mode"]):
         exc = IsADirectoryError(path)
@@ -226,19 +237,20 @@
 
     for chunk in iterator:
         temp_file.write(chunk)
     temp_file.seek(0)
 
     tar_file = tarfile.open(fileobj=temp_file)
     member = tar_file.next()
-    return cast('IO[bytes]', tar_file.extractfile(member))
+    return cast("IO[bytes]", tar_file.extractfile(member))
 
 
-def upload_file(container: Container, path: Union[str, PathLike[str]],
-                data: bytes = None, fileobj: IO[bytes] = None) -> None:
+def upload_file(
+    container: Container, path: Union[str, PathLike[str]], data: bytes = None, fileobj: IO[bytes] = None
+) -> None:
     """Upload a file to the given container
 
     Args:
         container: Docker container.
         path: Path to upload the file to.
         data: Bytes of data to upload. Cannot be set with fileobj.
         fileobj: File object to uplaod. Cannot be set with data.
@@ -280,15 +292,15 @@
                 tar.addfile(tarinfo, fileobj)
             except (OSError, AttributeError):
                 # Failed to extract info, writing and reading from temp file.
                 with TemporaryFile("w+b") as temp_file:
                     shutil.copyfileobj(fileobj, temp_file)
                     temp_file.seek(0)
                     temp_file.flush()
-                    tarinfo = tar.gettarinfo(arcname=filename, fileobj=temp_file)  # noqa
+                    tarinfo = tar.gettarinfo(arcname=filename, fileobj=temp_file)
                     tar.addfile(tarinfo, temp_file)
     return output.getvalue()
 
 
 class SafeContainerCreator:
     """
     A class that can safely pull and create multiple containers in succession, where if one fails, all the previous
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/aerospike.py` & `yellowbox-0.8.4/yellowbox/extras/aerospike.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 from contextlib import contextmanager
-from typing import Optional
+from typing import Any, Dict, Optional
 
 import aerospike
 from docker import DockerClient
 
 from yellowbox import RunMixin
 from yellowbox.containers import create_and_pull, get_ports
 from yellowbox.retry import RetrySpec
 from yellowbox.subclasses import AsyncRunMixin, SingleContainerService
 from yellowbox.utils import DOCKER_EXPOSE_HOST
 
-__all__ = ['AerospikeService', 'AEROSPIKE_DEFAULT_PORT']
+__all__ = ["AerospikeService", "AEROSPIKE_DEFAULT_PORT"]
 
 AerospikeError = aerospike.exception.AerospikeError  # aerospike doesn't let you import this on its own
 
 AEROSPIKE_DEFAULT_PORT = 3000
 
 
 class AerospikeService(SingleContainerService, RunMixin, AsyncRunMixin):
-    def __init__(self, docker_client: DockerClient, image='aerospike:ce-6.2.0.3', **kwargs):
+    def __init__(self, docker_client: DockerClient, image="aerospike:ce-6.2.0.3", **kwargs):
         container = create_and_pull(docker_client, image, publish_all_ports=True, detach=True)
         self.started = False
         super().__init__(container, **kwargs)
 
-    namespace = 'test'
+    namespace = "test"
 
     def client_port(self):
         return get_ports(self.container)[AEROSPIKE_DEFAULT_PORT]
 
-    def _client(self, config={}) -> aerospike.Client:
+    def _client(self, config: Optional[Dict[str, Any]] = None) -> aerospike.Client:
+        config = config or {}
         config = {
             **config,
-            'hosts': [(DOCKER_EXPOSE_HOST, self.client_port())],
+            "hosts": [(DOCKER_EXPOSE_HOST, self.client_port())],
         }
         return aerospike.client(config)
 
     @contextmanager
-    def client(self, config={}):
+    def client(self, config: Optional[Dict[str, Any]] = None):
         ret = self._client(config)
         try:
             yield ret
         finally:
             ret.close()
 
     def start(self, retry_spec: Optional[RetrySpec] = None, **kwargs):
@@ -55,10 +56,10 @@
     async def astart(self, retry_spec: Optional[RetrySpec] = None, **kwargs) -> None:
         super().start()
         retry_spec = retry_spec or RetrySpec(attempts=15)
         client = await retry_spec.aretry(self._client, AerospikeError)
         await retry_spec.aretry(client.is_connected, AerospikeError)
         self.started = True
 
-    def stop(self, signal='SIGKILL'):
+    def stop(self, signal="SIGKILL"):
         # change in default
         return super().stop(signal)
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/azure_storage.py` & `yellowbox-0.8.4/yellowbox/extras/azure_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,44 +8,44 @@
 from docker import DockerClient
 from docker.models.networks import Network
 
 from yellowbox.containers import create_and_pull, get_ports, short_id
 from yellowbox.retry import RetrySpec
 from yellowbox.subclasses import AsyncRunMixin, RunMixin, SingleContainerService
 
-__all__ = ['AzuriteService', 'BlobStorageService']
+__all__ = ["AzuriteService", "BlobStorageService"]
 
 from yellowbox.utils import DOCKER_EXPOSE_HOST, docker_host_name
 
 BLOB_STORAGE_DEFAULT_PORT = 10000
 DEFAULT_ACCOUNT_KEY = "Eby8vdM02xNOcqFlqUwJPLlmEtlCDXJ1OUzFT50uSRZ6IFsuFq2UVErCz4I6tq/K1SZFPTOtr/KBHBeksoGMGw=="
 DEFAULT_ACCOUNT_NAME = "devstoreaccount1"
 
 
-class _ResourceNotReady(Exception):
+class _ResourceNotReadyError(Exception):
     pass
 
 
 class AzuriteService(SingleContainerService, RunMixin, AsyncRunMixin):
     """
     Starts Azurite, Azure's storage emulator.
     Provides helper functions for preparing the instance for testing.
     TODO: Make account name and key configurable.
     """
+
     account_name = DEFAULT_ACCOUNT_NAME
     account_key = DEFAULT_ACCOUNT_KEY
 
-    def __init__(self, docker_client: DockerClient,
-                 image: str = "mcr.microsoft.com/azure-storage/azurite:latest",
-                 **kwargs):
-        container = create_and_pull(
-            docker_client, image, "azurite-blob --blobHost 0.0.0.0", publish_all_ports=True)
+    def __init__(
+        self, docker_client: DockerClient, image: str = "mcr.microsoft.com/azure-storage/azurite:latest", **kwargs
+    ):
+        container = create_and_pull(docker_client, image, "azurite-blob --blobHost 0.0.0.0", publish_all_ports=True)
         super().__init__(container, **kwargs)
 
-    def stop(self, signal: Union[str, int] = 'SIGKILL'):
+    def stop(self, signal: Union[str, int] = "SIGKILL"):
         """
         We override to change the signal.
         """
         super().stop(signal)
 
     def client_port(self):
         return get_ports(self.container)[BLOB_STORAGE_DEFAULT_PORT]
@@ -53,76 +53,78 @@
     @property
     def connection_string(self):
         """Connection string to connect from host to container"""
         return (
             f"DefaultEndpointsProtocol=http;"
             f"AccountName={self.account_name};"
             f"AccountKey={self.account_key};"
-            f"BlobEndpoint={self.endpoint_url};")
+            f"BlobEndpoint={self.endpoint_url};"
+        )
 
     @property
     def container_connection_string(self):
         """Connection string to connect across containers in the same network"""
         return (
             f"DefaultEndpointsProtocol=http;"
             f"AccountName={self.account_name};"
             f"AccountKey={self.account_key};"
-            f"BlobEndpoint={self.container_endpoint_url};")
+            f"BlobEndpoint={self.container_endpoint_url};"
+        )
 
     @property
     def host_connection_string(self):
         """Connection string to connect across containers through the docker host"""
         return (
             f"DefaultEndpointsProtocol=http;"
             f"AccountName={self.account_name};"
             f"AccountKey={self.account_key};"
-            f"BlobEndpoint={self.host_endpoint_url};")
+            f"BlobEndpoint={self.host_endpoint_url};"
+        )
 
     @property
     def endpoint_url(self):
         """URL for the endpoint from docker host"""
-        return f'http://{DOCKER_EXPOSE_HOST}:{self.client_port()}/{self.account_name}'
+        return f"http://{DOCKER_EXPOSE_HOST}:{self.client_port()}/{self.account_name}"
 
     @property
     def container_endpoint_url(self):
         """URL for the endpoint from another container over a common network"""
-        return f'http://{short_id(self.container)}:{BLOB_STORAGE_DEFAULT_PORT}/{self.account_name}'
+        return f"http://{short_id(self.container)}:{BLOB_STORAGE_DEFAULT_PORT}/{self.account_name}"
 
     @property
     def host_endpoint_url(self):
         """URL for the endpoint from another container through the docker host"""
-        return f'http://{docker_host_name}:{self.client_port()}/{self.account_name}'
+        return f"http://{docker_host_name}:{self.client_port()}/{self.account_name}"
 
     @property
     def account_credentials(self):
         """Azure credentials dict to connect to the service"""
-        return {'account_name': self.account_name, 'account_key': self.account_key}
+        return {"account_name": self.account_name, "account_key": self.account_key}
 
     def _check_ready(self):
         if b"Azurite Blob service successfully listens on" not in self.container.logs():
-            raise _ResourceNotReady
+            raise _ResourceNotReadyError
 
     def start(self, retry_spec: Optional[RetrySpec] = None):
         super().start()
 
         retry_spec = retry_spec or RetrySpec(attempts=10)
 
-        retry_spec.retry(self._check_ready, _ResourceNotReady)
+        retry_spec.retry(self._check_ready, _ResourceNotReadyError)
         return self
 
     async def astart(self, retry_spec: Optional[RetrySpec] = None):
         super().start()
 
         retry_spec = retry_spec or RetrySpec(attempts=10)
 
-        await retry_spec.aretry(self._check_ready, _ResourceNotReady)
+        await retry_spec.aretry(self._check_ready, _ResourceNotReadyError)
         return self
 
-    def connect(self, network: Network, aliases: Optional[List[str]] = None,
-                **kwargs) -> Sequence[str]:
+    def connect(self, network: Network, aliases: Optional[List[str]] = None, **kwargs) -> Sequence[str]:
         # Make sure the id is in the aliases list. Needed for the container
         # connection string.
         if aliases is not None:
             aliases.append(short_id(self.container))
         return super().connect(network, aliases=aliases, **kwargs)
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/fake_gcs.py` & `yellowbox-0.8.4/yellowbox/extras/fake_gcs.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,130 +11,144 @@
 from yellowbox.subclasses import AsyncRunMixin, RunMixin, SingleContainerService
 from yellowbox.utils import DOCKER_EXPOSE_HOST, docker_host_name
 
 FAKE_GCS_DEFAULT_PORT = 4443
 
 
 class FakeGoogleCloudStorage(SingleContainerService, RunMixin, AsyncRunMixin):
-    def __init__(self, docker_client: DockerClient,
-                 image: str = "fsouza/fake-gcs-server:1.42",
-                 scheme: str = 'https',
-                 command: str = '',
-                 **kwargs):
+    def __init__(
+        self,
+        docker_client: DockerClient,
+        image: str = "fsouza/fake-gcs-server:1.42",
+        scheme: str = "https",
+        command: str = "",
+        **kwargs,
+    ):
         # note that fake-gcs-server 1.43.0 has a bug https://github.com/fsouza/fake-gcs-server/issues/1034
-        command = f'-scheme {scheme} {command}'
+        command = f"-scheme {scheme} {command}"
         self.scheme = scheme
         container = create_and_pull(docker_client, image, command, publish_all_ports=True)
         super().__init__(container, **kwargs)
 
     def client_port(self):
         return get_ports(self.container)[FAKE_GCS_DEFAULT_PORT]
 
-    def local_url(self,
-                  scheme: Optional[str] = ...  # type: ignore[assignment]
-                  ):
-        ret = f'{DOCKER_EXPOSE_HOST}:{self.client_port()}'
+    def local_url(self, scheme: Optional[str] = ...):  # type: ignore[assignment]
+        ret = f"{DOCKER_EXPOSE_HOST}:{self.client_port()}"
         if scheme is ...:
             scheme = self.scheme
         if scheme:
-            ret = f'{self.scheme}://{ret}'
+            ret = f"{self.scheme}://{ret}"
         return ret
 
-    def container_url(self, hostname: str,
-                      scheme: Optional[str] = ...  # type: ignore[assignment]
-                      ):
-        ret = f'{hostname}:{FAKE_GCS_DEFAULT_PORT}'
+    def container_url(self, hostname: str, scheme: Optional[str] = ...):  # type: ignore[assignment]
+        ret = f"{hostname}:{FAKE_GCS_DEFAULT_PORT}"
         if scheme is ...:
             scheme = self.scheme
         if scheme:
-            ret = f'{self.scheme}://{ret}'
+            ret = f"{self.scheme}://{ret}"
         return ret
 
-    def host_url(self,
-                 scheme: Optional[str] = ...  # type: ignore[assignment]
-                 ):
-        ret = f'{docker_host_name}:{self.client_port()}'
+    def host_url(self, scheme: Optional[str] = ...):  # type: ignore[assignment]
+        ret = f"{docker_host_name}:{self.client_port()}"
         if scheme is ...:
             scheme = self.scheme
         if scheme:
-            ret = f'{self.scheme}://{ret}'
+            ret = f"{self.scheme}://{ret}"
         return ret
 
     def start(self, retry_spec: Optional[RetrySpec] = None):
         super().start()
-        url = self.local_url() + '/storage/v1/b'
+        url = self.local_url() + "/storage/v1/b"
         retry_spec = retry_spec or RetrySpec(attempts=15)
-        retry_spec.retry(lambda: requests.get(url, verify=False).raise_for_status(),
-                         requests.exceptions.RequestException)
+        retry_spec.retry(
+            lambda: requests.get(url, verify=False).raise_for_status(), requests.exceptions.RequestException
+        )
         return self
 
     async def astart(self, retry_spec: Optional[RetrySpec] = None):
         super().start()
-        url = self.local_url() + '/storage/v1/b'
+        url = self.local_url() + "/storage/v1/b"
         retry_spec = retry_spec or RetrySpec(attempts=15)
-        await retry_spec.aretry(lambda: requests.get(url, verify=False).raise_for_status(),
-                                requests.exceptions.RequestException)
+        await retry_spec.aretry(
+            lambda: requests.get(url, verify=False).raise_for_status(), requests.exceptions.RequestException
+        )
 
     @contextmanager
     def patch_gcloud_aio(self):
         from gcloud.aio.storage import __version__ as gcloud_aio_version
+
         if not gcloud_aio_version.startswith("7."):
             # for newer gcloud_aio, we can just adjust the environment
-            warn("newer gcloud versions should be patched directly with by setting the environent variable "
-                 "STORAGE_EMULATOR_HOST to service.local_url()")
-            prev_env = getenv('STORAGE_EMULATOR_HOST')
-            environ['STORAGE_EMULATOR_HOST'] = self.local_url(None)
+            warn(
+                "newer gcloud versions should be patched directly by setting the environment variable "
+                "STORAGE_EMULATOR_HOST to service.local_url()",
+                stacklevel=1,
+            )
+            prev_env = getenv("STORAGE_EMULATOR_HOST")
+            environ["STORAGE_EMULATOR_HOST"] = self.local_url(None)
             yield
             if prev_env is None:
-                del environ['STORAGE_EMULATOR_HOST']
+                del environ["STORAGE_EMULATOR_HOST"]
             else:
-                environ['STORAGE_EMULATOR_HOST'] = prev_env
+                environ["STORAGE_EMULATOR_HOST"] = prev_env
             return
         import gcloud.aio.storage.storage as gcloud_module
-        previous_state = (gcloud_module.API_ROOT, gcloud_module.API_ROOT_UPLOAD, gcloud_module.VERIFY_SSL,
-                          gcloud_module.STORAGE_EMULATOR_HOST)
-        (gcloud_module.API_ROOT, gcloud_module.API_ROOT_UPLOAD, gcloud_module.VERIFY_SSL,
-         gcloud_module.STORAGE_EMULATOR_HOST) = (
+
+        previous_state = (
+            gcloud_module.API_ROOT,
+            gcloud_module.API_ROOT_UPLOAD,
+            gcloud_module.VERIFY_SSL,
+            gcloud_module.STORAGE_EMULATOR_HOST,
+        )
+        (
+            gcloud_module.API_ROOT,
+            gcloud_module.API_ROOT_UPLOAD,
+            gcloud_module.VERIFY_SSL,
+            gcloud_module.STORAGE_EMULATOR_HOST,
+        ) = (
             self.local_url() + "/storage/v1/b",
             self.local_url() + "/upload/storage/v1/b",
             False,
-            self.local_url(scheme='')
+            self.local_url(scheme=""),
         )
         yield
-        (gcloud_module.API_ROOT, gcloud_module.API_ROOT_UPLOAD, gcloud_module.VERIFY_SSL,
-         gcloud_module.STORAGE_EMULATOR_HOST) = previous_state
+        (
+            gcloud_module.API_ROOT,
+            gcloud_module.API_ROOT_UPLOAD,
+            gcloud_module.VERIFY_SSL,
+            gcloud_module.STORAGE_EMULATOR_HOST,
+        ) = previous_state
 
     def create_bucket(self, bucket_name: str) -> Dict[str, Any]:
         url = self.local_url()
 
-        resp = requests.post(url + "/storage/v1/b", json={
-            'name': bucket_name
-        }, verify=False)
+        resp = requests.post(url + "/storage/v1/b", json={"name": bucket_name}, verify=False)
         resp.raise_for_status()
 
         return resp.json()
 
     def clear_bucket(self, bucket_name: str, prefix: Optional[str] = None) -> Iterable[str]:
         url = self.local_url()
         params = {}
         if prefix:
-            params['prefix'] = prefix
+            params["prefix"] = prefix
         page_token = None
         ret = []
         while True:
             if page_token:
-                params['pageToken'] = page_token
+                params["pageToken"] = page_token
             resp = requests.get(url + f"/storage/v1/b/{bucket_name}/o", params=params, verify=False)
             resp.raise_for_status()
             data = resp.json()
-            for item in data['items']:
-                ret.append(item['name'])
+            for item in data["items"]:
+                ret.append(item["name"])
                 requests.delete(url + f'/storage/v1/b/{bucket_name}/o/{item["name"]}', verify=False).raise_for_status()
-            if 'nextPageToken' in data:
-                page_token = data['next_page_token']
+            if "nextPageToken" in data:
+                page_token = data["next_page_token"]
             else:
                 break
         return ret
 
     def delete_bucket(self, bucket_name: str, force: bool = False, missing_ok: bool = False):
         url = self.local_url()
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/http_server.py` & `yellowbox-0.8.4/yellowbox/extras/http_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 import requests
 from requests import ConnectionError, HTTPError
 
 from yellowbox.retry import RetrySpec
 from yellowbox.service import YellowService
 from yellowbox.utils import docker_host_name
 
-__all__ = ['HttpService', 'RouterHTTPRequestHandler']
-SideEffectResponse = Union[bytes, str, int, 'RouterHTTPRequestHandler']
-SideEffect = Union[Callable[['RouterHTTPRequestHandler'], SideEffectResponse],
-                   SideEffectResponse]
+__all__ = ["HttpService", "RouterHTTPRequestHandler"]
+SideEffectResponse = Union[bytes, str, int, "RouterHTTPRequestHandler"]
+SideEffect = Union[Callable[["RouterHTTPRequestHandler"], SideEffectResponse], SideEffectResponse]
 
 
 class RoutedHandler(NamedTuple):
     method: str
     name: str
     route: Union[Pattern[str], str]
     callback: Callable[[RouterHTTPRequestHandler], None]
@@ -35,25 +34,26 @@
 
 
 class RouterHTTPRequestHandler(BaseHTTPRequestHandler):
     """
     A BaseHTTPRequestHandler that allows adding and deleting routed handlers.
     Also contains some utility argument parsing.
     """
+
     _parse_url: ParseResult
     _body: Optional[bytes]
 
     routes_by_method: ClassVar[DefaultDict[str, Set[RoutedHandler]]]
     route_lock: ClassVar[Lock]
 
     def body(self) -> Optional[bytes]:
         try:
             return self._body
         except AttributeError:
-            raw_body_len = self.headers['Content-Length']
+            raw_body_len = self.headers["Content-Length"]
             if raw_body_len is None:
                 self._body = None
             else:
                 length = int(raw_body_len)
                 self._body = self.rfile.read(length)
             return self._body
 
@@ -103,28 +103,29 @@
         candidates = tuple(self.routes_by_method.get(self.command, ()))
         matched_candidates = []
         for candidate in candidates:
             match = candidate.route_match(parsed.path)
             if match:
                 matched_candidates.append((candidate, match))
         if not matched_candidates:
-            self.send_error(404, 'mock server matched no routes')
+            self.send_error(404, "mock server matched no routes")
             self.end_headers()
         elif len(matched_candidates) > 1:
-            self.send_error(500, 'mock server matched multiple routes: '
-                            + ', '.join(c.name for c, _ in matched_candidates))
+            self.send_error(
+                500, "mock server matched multiple routes: " + ", ".join(c.name for c, _ in matched_candidates)
+            )
             self.end_headers()
         else:
-            (routed, match), = matched_candidates
-            self.log_message(f'routed to {routed.name}')
+            ((routed, match),) = matched_candidates
+            self.log_message(f"routed to {routed.name}")
             self.match = match
             routed.callback(self)
 
     def __getattr__(self, item: str):
-        if item.startswith('do_'):
+        if item.startswith("do_"):
             return self._do
         raise AttributeError(item)
 
 
 class HttpService(YellowService):
     """
     The HttpService class is used to mock http servers. Although it is a YellowService,
@@ -141,64 +142,70 @@
     ...      # within this scope, the path "/hello/world" will return a 200 response with the body "hi there"
     ...      assert requests.get(service.local_url+"/hello/world").text == "hi there"
     ...   # routes can also be set without a function
     ...   with service.patch_route('GET', '/meaning_of_life', '42'):
     ...      assert requests.get(service.local_url+"/meaning_of_life").content == b'42'
     """
 
-    def __init__(self, host='0.0.0.0', port=0, name='anonymous_yellowbox_HTTPService'):
-        self.router_cls = cast(Type[RouterHTTPRequestHandler],
-                               new_class(name + '_RequestHandler', (RouterHTTPRequestHandler,)))
+    def __init__(self, host="0.0.0.0", port=0, name="anonymous_yellowbox_HTTPService"):
+        self.router_cls = cast(
+            Type[RouterHTTPRequestHandler], new_class(name + "_RequestHandler", (RouterHTTPRequestHandler,))
+        )
         self.server = HTTPServer((host, port), self.router_cls)
-        self.server_thread = Thread(name=name + '_thread', target=self.server.serve_forever,
-                                    daemon=True)
+        self.server_thread = Thread(name=name + "_thread", target=self.server.serve_forever, daemon=True)
 
     @property
     def server_port(self):
         return self.server.server_port
 
     @property
     def local_url(self):
-        return f'http://127.0.0.1:{self.server_port}'
+        return f"http://127.0.0.1:{self.server_port}"
 
     @property
     def container_url(self):
-        return f'http://{docker_host_name}:{self.server_port}'
+        return f"http://{docker_host_name}:{self.server_port}"
 
     @staticmethod
     def _to_callback(side_effect: SideEffect):
         def _respond(handler: RouterHTTPRequestHandler, response: SideEffectResponse):
             if response is handler:
                 return  # Assuming the user already handled the response
             if isinstance(response, int):
                 handler.send_error(response)
                 handler.end_headers()
                 return
             handler.send_response(200)
             handler.end_headers()
             if isinstance(response, str):
-                response = bytes(response, 'ascii')
+                response = bytes(response, "ascii")
             if isinstance(response, bytes):
                 handler.wfile.write(response)
             else:
-                raise TypeError(f"got response of type {type(response)}, type must be RouterHTTPRequestHandler, "
-                                f"int, str or bytes")
+                raise TypeError(
+                    f"got response of type {type(response)}, type must be RouterHTTPRequestHandler, "
+                    f"int, str or bytes"
+                )
 
         def callback(handler: RouterHTTPRequestHandler):
             if callable(side_effect):
                 result = side_effect(handler)
                 _respond(handler, result)
             else:
                 _respond(handler, cast(SideEffectResponse, side_effect))
 
         return callback
 
-    def patch_route(self, method, route: Union[str, Pattern[str]],
-                    side_effect: SideEffect = ...,  # type: ignore[assignment]
-                    name: Optional[str] = None):
+    def patch_route(
+        self,
+        method,
+        route: Union[str, Pattern[str]],
+        side_effect: SideEffect = ...,  # type: ignore[assignment]
+        name: Optional[str] = None,
+    ):
         """
         Create a context manager that temporarily adds a route handler to the service.
 
         Args:
             method: The request method to add the route to.
             route: The route to attach the side effect to, all routes must begin with a slash "/".
                 Alternatively, The route may be a regex pattern, in which case the request path must fully match it,
@@ -223,31 +230,30 @@
         if side_effect is ...:
             return partial(self.patch_route, method, route, name=name)
 
         @contextmanager
         def _helper():
             nonlocal name
             callback = self._to_callback(side_effect)
-            name = name or getattr(side_effect, '__name__', None) or str(route)
+            name = name or getattr(side_effect, "__name__", None) or str(route)
             handler = RoutedHandler(method, name, route, callback)
             self.router_cls.add_route(handler)
             try:
                 yield handler
             finally:
                 self.router_cls.del_route(handler)
 
         return _helper()
 
     def start(self, retry_spec: Optional[RetrySpec] = None):
-        with self.patch_route('GET', '/health', 200):
+        with self.patch_route("GET", "/health", 200):
             self.server_thread.start()
             retry_spec = retry_spec or RetrySpec(attempts=10)
             retry_spec.retry(
-                lambda: requests.get(self.local_url + '/health').raise_for_status(),
-                (ConnectionError, HTTPError)
+                lambda: requests.get(self.local_url + "/health").raise_for_status(), (ConnectionError, HTTPError)
             )
         return super(HttpService, self).start()
 
     def stop(self):
         self.server.shutdown()
         self.server_thread.join()
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/kafka.py` & `yellowbox-0.8.4/yellowbox/extras/kafka.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,90 +8,107 @@
 
 from yellowbox.containers import SafeContainerCreator, get_ports
 from yellowbox.networks import anonymous_network
 from yellowbox.retry import RetrySpec
 from yellowbox.subclasses import AsyncRunMixin, RunMixin, SingleEndpointService
 from yellowbox.utils import DOCKER_EXPOSE_HOST, get_free_port
 
-__all__ = ['KafkaService']
+__all__ = ["KafkaService"]
 
 
 class KafkaService(SingleEndpointService, RunMixin, AsyncRunMixin):
-    def __init__(self, docker_client: DockerClient, tag_or_images: Union[str, Tuple[str, str]] = 'latest',
-                 inner_port=0, outer_port=0, **kwargs):
+    def __init__(
+        self,
+        docker_client: DockerClient,
+        tag_or_images: Union[str, Tuple[str, str]] = "latest",
+        inner_port=0,
+        outer_port=0,
+        bitnami_debug: bool = False,
+        **kwargs,
+    ):
         self.inner_port = inner_port or get_free_port()
         self.outer_port = outer_port or get_free_port()
         if isinstance(tag_or_images, str):
             zookeeper_image = f"bitnami/zookeeper:{tag_or_images}"
             broker_image = f"bitnami/kafka:{tag_or_images}"
         else:
             zookeeper_image, broker_image = tag_or_images
 
         # broker must have a known alias at creation time
-        self.static_broker_alias = f'broker-{uuid1()}'
+        self.static_broker_alias = f"broker-{uuid1()}"
 
         creator = SafeContainerCreator(docker_client)
 
+        extra_bitnami_env = {}
+        if bitnami_debug:
+            extra_bitnami_env["BITNAMI_DEBUG"] = "true"
+
         self.zookeeper = creator.create_and_pull(
-            zookeeper_image, detach=True,
+            zookeeper_image,
+            detach=True,
             publish_all_ports=True,
             environment={
-                'ZOOKEEPER_CLIENT_PORT': '2181',
-                'ZOOKEEPER_TICK_TIME': '2000',
-                'ALLOW_ANONYMOUS_LOGIN': 'yes',
-            })
+                "ZOOKEEPER_CLIENT_PORT": "2181",
+                "ZOOKEEPER_TICK_TIME": "2000",
+                "ALLOW_ANONYMOUS_LOGIN": "yes",
+                **extra_bitnami_env,
+            },
+        )
 
         self.broker = creator.create_and_pull(
             broker_image,
             ports={
-                str(self.outer_port): ('0.0.0.0', self.outer_port),
-                str(self.inner_port): ('0.0.0.0', self.inner_port)
+                str(self.outer_port): ("0.0.0.0", self.outer_port),
+                str(self.inner_port): ("0.0.0.0", self.inner_port),
             },
             publish_all_ports=True,
             detach=True,
             environment={
-                'KAFKA_CFG_ADVERTISED_LISTENERS': f'INNER://{self.static_broker_alias}:{self.inner_port},'
-                                                  f'OUTER://localhost:{self.outer_port}',
+                "KAFKA_CFG_ADVERTISED_LISTENERS": f"INNER://{self.static_broker_alias}:{self.inner_port},"
+                f"OUTER://localhost:{self.outer_port}",
                 "KAFKA_CFG_ZOOKEEPER_CONNECT": "zk/2181",
-                'ALLOW_PLAINTEXT_LISTENER': 'yes',
-                'KAFKA_CFG_LISTENER_SECURITY_PROTOCOL_MAP': 'INNER:PLAINTEXT,OUTER:PLAINTEXT',
-                'KAFKA_INTER_BROKER_LISTENER_NAME': 'INNER',
-                'KAFKA_CFG_LISTENERS': f'INNER://:{self.inner_port},OUTER://:{self.outer_port}'
-            })
+                "ALLOW_PLAINTEXT_LISTENER": "yes",
+                "KAFKA_CFG_LISTENER_SECURITY_PROTOCOL_MAP": "INNER:PLAINTEXT,OUTER:PLAINTEXT",
+                "KAFKA_INTER_BROKER_LISTENER_NAME": "INNER",
+                "KAFKA_CFG_LISTENERS": f"INNER://:{self.inner_port},OUTER://:{self.outer_port}",
+                "KAFKA_ENABLE_KRAFT": "false",
+                **extra_bitnami_env,
+            },
+        )
 
         self.network = anonymous_network(docker_client)
         self.network.connect(self.zookeeper, aliases=["zk"])
         self.network.connect(self.broker, aliases=[self.static_broker_alias])
         super().__init__((self.zookeeper, self.broker), **kwargs)
 
     def connection_port(self):
         self.broker.reload()
         ports = get_ports(self.broker)
         return ports[self.outer_port]
 
     def consumer(self, **kwargs) -> ContextManager[KafkaConsumer]:
         port = self.connection_port()
         return cast(
-            'ContextManager[KafkaConsumer]',
-            closing(KafkaConsumer(
-                bootstrap_servers=[f'{DOCKER_EXPOSE_HOST}:{port}'],
-                security_protocol="PLAINTEXT",
-                **kwargs
-            ))
+            "ContextManager[KafkaConsumer]",
+            closing(
+                KafkaConsumer(
+                    bootstrap_servers=[f"{DOCKER_EXPOSE_HOST}:{port}"], security_protocol="PLAINTEXT", **kwargs
+                )
+            ),
         )
 
     def producer(self, **kwargs) -> ContextManager[KafkaProducer]:
         port = self.connection_port()
         return cast(
-            'ContextManager[KafkaProducer]',
-            closing(KafkaProducer(
-                bootstrap_servers=[f'{DOCKER_EXPOSE_HOST}:{port}'],
-                security_protocol="PLAINTEXT",
-                **kwargs
-            ))
+            "ContextManager[KafkaProducer]",
+            closing(
+                KafkaProducer(
+                    bootstrap_servers=[f"{DOCKER_EXPOSE_HOST}:{port}"], security_protocol="PLAINTEXT", **kwargs
+                )
+            ),
         )
 
     def start(self, retry_spec: Optional[RetrySpec] = None):
         super().start()
         retry_spec = retry_spec or RetrySpec(attempts=20)
         with retry_spec.retry(self.consumer, (KafkaError, ConnectionError, ValueError)):
             pass
@@ -99,24 +116,24 @@
 
     async def astart(self, retry_spec: Optional[RetrySpec] = None) -> None:
         super().start()
         retry_spec = retry_spec or RetrySpec(attempts=20)
         with await retry_spec.aretry(self.consumer, (KafkaError, ConnectionError, ValueError)):
             pass
 
-    def stop(self, signal='SIGKILL'):
+    def stop(self, signal="SIGKILL"):
         # difference in default signal
         self.network.disconnect(self.broker)
         self.network.disconnect(self.zookeeper)
         self.network.remove()
         super().stop(signal)
 
     def connect(self, network, *, aliases=(), **kwargs):
         if not isinstance(aliases, list):
             aliases = list(aliases)
         aliases.append(self.static_broker_alias)
-        kwargs['aliases'] = aliases
+        kwargs["aliases"] = aliases
         return super().connect(network, **kwargs)
 
     @property
     def _single_endpoint(self):
         return self.broker
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/logstash.py` & `yellowbox-0.8.4/yellowbox/extras/logstash.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import threading
 from typing import Any, Callable, Dict, Iterator, List, TypeVar, Union, cast
 from weakref import WeakMethod
 
 from yellowbox.subclasses import YellowService
 from yellowbox.utils import docker_host_name
 
-__all__ = ['FakeLogstashService']
+__all__ = ["FakeLogstashService"]
 _logger = logging.getLogger(__name__)
 
 _T = TypeVar("_T")
 
 _STOP_TIMEOUT = 5  # Timeout for stopping the service
 
 # Sent on internal connection to signal closing of background thread
@@ -72,14 +72,15 @@
         >>> s.sendall(b'{"record": "value", "level": "ERROR"}\\n')
         >>> s.close()
         >>> time.sleep(0.01)  # Wait for service to process message
         >>> ls.stop()
         >>> ls.assert_logs("ERROR")
         >>> assert ls.records[0]["record"] == "value"
     """
+
     delimiter: bytes = b"\n"
     encoding: str = "utf-8"
     local_host: str = "localhost"
     container_host: str = docker_host_name
 
     def __init__(self, port: int = 0) -> None:
         """Initialize the service.
@@ -108,17 +109,16 @@
         """
 
         root = socket.socket()
         root.bind(("0.0.0.0", port))
         self._root = root
 
         # Avoiding a cyclic reference.
-        _background = WeakMethod(self._background_thread)  # type: ignore # typeshed bug.
-        self._thread = threading.Thread(target=lambda: _background()(),
-                                        daemon=True)
+        _background = WeakMethod(self._background_thread)
+        self._thread = threading.Thread(target=lambda: _background()(), daemon=True)
 
         self._selector = selectors.DefaultSelector()
 
         # Sockets used for signalling shutdown
         self._rshutdown, self._wshutdown = socket.socketpair()
 
         self.port: int = self._root.getsockname()[1]
@@ -178,36 +178,33 @@
                 for chunk in chunks:
                     record_dict = json.loads(chunk.decode(encoding))
                     self.records.append(record_dict)
             except json.JSONDecodeError:
                 self._selector.unregister(sock)
                 sock.shutdown(socket.SHUT_RDWR)
                 sock.close()
-                _logger.exception("Failed decoding json, closing socket. "
-                                  "Data received: %s", chunk)
+                _logger.exception("Failed decoding json, closing socket. Data received: %s", chunk)
                 return
 
         return process_socket_data
 
     def _background_thread(self):
         """Background thread processing incoming connections and data"""
         while True:
             events = self._selector.select(timeout=5)  # For signal handling
-            for key, mask in events:
+            for key, _mask in events:
                 # Handle closing request
                 if key.fileobj is self._rshutdown:
-                    assert self._rshutdown.recv(
-                        len(_CLOSE_SENTINEL)) == _CLOSE_SENTINEL
+                    assert self._rshutdown.recv(len(_CLOSE_SENTINEL)) == _CLOSE_SENTINEL
                     return
 
                 # Handle new connection
                 if key.fileobj is self._root:
                     new_socket, _ = self._root.accept()
-                    self._selector.register(new_socket, selectors.EVENT_READ,
-                                            self._create_data_callback(new_socket))
+                    self._selector.register(new_socket, selectors.EVENT_READ, self._create_data_callback(new_socket))
                     continue
 
                 # Data received, run callback
                 try:
                     key.data()
                 except Exception:
                     _logger.exception("Unknown error occurred, closing connection.")
@@ -250,16 +247,15 @@
         """
         return self._thread.is_alive()
 
     def filter_records(self, level: Union[str, int]) -> Iterator[Dict[str, Any]]:
         """Filter records in the given level or above."""
         level = _level_to_int(level)
 
-        return (record for record in self.records if
-                logging.getLevelName(record["level"]) >= level)
+        return (record for record in self.records if logging.getLevelName(record["level"]) >= level)
 
     def assert_logs(self, level: Union[str, int]):
         """Asserts that log messages were received in the given level or above.
 
         Resembles unittest.assertLogs.
 
         Args:
@@ -267,25 +263,23 @@
 
         Raises:
             AssertionError: No logs above the given level were received.
         """
         level = _level_to_int(level)
 
         if not any(self.filter_records(level)):
-            raise AssertionError(f"No logs of level {logging.getLevelName(level)} "
-                                 f"or above were received.")
+            raise AssertionError(f"No logs of level {logging.getLevelName(level)} or above were received.")
 
     def assert_no_logs(self, level: Union[str, int]):
         """Asserts that no log messages were received in the given level or above.
 
-         Args:
-             level: Log level by name or number
+        Args:
+            level: Log level by name or number
 
-         Raises:
-             AssertionError: A log above the given level was received.
-         """
+        Raises:
+            AssertionError: A log above the given level was received.
+        """
         level = _level_to_int(level)
 
         record = next(self.filter_records(level), None)
         if record:
-            raise AssertionError(f"A log level {record['level']} was received. "
-                                 f"Message: {record['message']}")
+            raise AssertionError(f"A log level {record['level']} was received. Message: {record['message']}")
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/postgresql.py` & `yellowbox-0.8.4/yellowbox/extras/postgresql.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,80 +9,108 @@
 from yellowbox.containers import create_and_pull
 from yellowbox.extras.sql_base import ConnectionOptions, SQLService, as_default
 from yellowbox.subclasses import SingleContainerService
 
 if TYPE_CHECKING:
     from yellowbox.extras.sql_base import AsDefault
 
-__all__ = ['PostgreSQLService', 'POSTGRES_INTERNAL_PORT']
+__all__ = ["PostgreSQLService", "POSTGRES_INTERNAL_PORT"]
 
 POSTGRES_INTERNAL_PORT = 5432
 
 
 class PostgreSQLService(SQLService, SingleContainerService):
     """
     A postgresSQL service
     """
 
     INTERNAL_PORT = POSTGRES_INTERNAL_PORT
-    DIALECT = 'postgresql'
+    DIALECT = "postgresql"
 
-    def __init__(self, docker_client: DockerClient, image='postgres:latest', *, user='postgres',
-                 password='guest', default_db: str = None, **kwargs):
+    def __init__(
+        self,
+        docker_client: DockerClient,
+        image="postgres:latest",
+        *,
+        user="postgres",
+        password="guest",
+        default_db: str = None,
+        **kwargs,
+    ):
         """
         Args:
             user: the Name of the default user for the database
             password: The password of the default user for the database
             default_db: The name of the default database. Defaults to the user name.
         """
         if default_db is None:
             default_db = user
 
         self.user = user
         self.password = password
         self.default_db = default_db
-        super().__init__(create_and_pull(
-            docker_client, image, publish_all_ports=True, detach=True, environment={
-                'POSTGRES_USER': user,
-                'POSTGRES_PASSWORD': password,
-                'POSTGRES_DB': default_db
-            }
-        ), default_database=default_db, **kwargs)
+        super().__init__(
+            create_and_pull(
+                docker_client,
+                image,
+                publish_all_ports=True,
+                detach=True,
+                environment={"POSTGRES_USER": user, "POSTGRES_PASSWORD": password, "POSTGRES_DB": default_db},
+            ),
+            default_database=default_db,
+            **kwargs,
+        )
 
     def userpass(self):
         return self.user, self.password
 
-    def local_connection_string(self, dialect: Union[str, AsDefault] = as_default,
-                                driver: Union[str, AsDefault, None] = as_default, database: Optional[str] = None,
-                                options: Union[ConnectionOptions, AsDefault] = as_default):
+    def local_connection_string(
+        self,
+        dialect: Union[str, AsDefault] = as_default,
+        driver: Union[str, AsDefault, None] = as_default,
+        database: Optional[str] = None,
+        options: Union[ConnectionOptions, AsDefault] = as_default,
+    ):
         database = database or self.default_db
         return super().local_connection_string(dialect, driver, database=database, options=options)
 
-    def container_connection_string(self, hostname: str, dialect: Union[str, AsDefault] = as_default,
-                                    driver: str = None, database: str = None, options: ConnectionOptions = None):
+    def container_connection_string(
+        self,
+        hostname: str,
+        dialect: Union[str, AsDefault] = as_default,
+        driver: str = None,
+        database: str = None,
+        options: ConnectionOptions = None,
+    ):
         database = database or self.default_db
         return super().container_connection_string(hostname, dialect, driver, database=database, options=options)
 
-    def host_connection_string(self, dialect: Union[str, AsDefault] = as_default, driver: str = None,
-                               database: str = None, options: ConnectionOptions = None):
+    def host_connection_string(
+        self,
+        dialect: Union[str, AsDefault] = as_default,
+        driver: str = None,
+        database: str = None,
+        options: ConnectionOptions = None,
+    ):
         database = database or self.default_db
         return super().host_connection_string(dialect, driver, database=database, options=options)
 
-    @deprecated(version='0.7.2', reason='Use sqlalchemy.create_engine(service.local_connection_string()) instead')
+    @deprecated(version="0.7.2", reason="Use sqlalchemy.create_engine(service.local_connection_string()) instead")
     def engine(self, **kwargs):
         """
         Create an sqlalchemy Engine connected to the service's default db.
         """
         cs = self.local_connection_string()
         return create_engine(cs, **kwargs)
 
-    @deprecated(version='0.7.2',
-                reason='Use sqlalchemy.create_engine(service.local_connection_string()).connect() instead')
+    @deprecated(
+        version="0.7.2", reason="Use sqlalchemy.create_engine(service.local_connection_string()).connect() instead"
+    )
     def connection(self, **kwargs):
         """
         Create an sqlalchemy Connection connected to the service's default db.
         """
         return self.engine().connect(**kwargs)
 
-    def stop(self, signal='SIGINT'):
+    def stop(self, signal="SIGINT"):
         # change in default
         return super().stop(signal)
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/rabbit_mq.py` & `yellowbox-0.8.4/yellowbox/extras/rabbit_mq.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,52 +7,72 @@
 from pika.adapters.utils.connection_workflow import AMQPConnectorException
 from pika.exceptions import AMQPConnectionError
 
 from yellowbox.containers import create_and_pull, get_ports, upload_file
 from yellowbox.retry import RetrySpec
 from yellowbox.subclasses import AsyncRunMixin, RunMixin, SingleContainerService
 
-__all__ = ['RabbitMQService', 'RABBIT_DEFAULT_PORT', 'RABBIT_HTTP_API_PORT']
+__all__ = ["RabbitMQService", "RABBIT_DEFAULT_PORT", "RABBIT_HTTP_API_PORT"]
 
 from yellowbox.utils import DOCKER_EXPOSE_HOST
 
 RABBIT_DEFAULT_PORT = 5672
 RABBIT_HTTP_API_PORT = 15672
 
 
 class RabbitMQService(SingleContainerService, RunMixin, AsyncRunMixin):
-    def __init__(self, docker_client: DockerClient, image='rabbitmq:latest', *, user="guest", password="guest",
-                 virtual_host="/", enable_management=False, **kwargs):
+    def __init__(
+        self,
+        docker_client: DockerClient,
+        image="rabbitmq:latest",
+        *,
+        user="guest",
+        password="guest",
+        virtual_host="/",
+        enable_management=False,
+        **kwargs,
+    ):
         self.user = user
         self.password = password
         self.virtual_host = virtual_host
-        super().__init__(create_and_pull(
-            docker_client, image, publish_all_ports=True, detach=True,
-            ports={RABBIT_HTTP_API_PORT: 0},  # Forward management port by default.
-        ), **kwargs)
+        super().__init__(
+            create_and_pull(
+                docker_client,
+                image,
+                publish_all_ports=True,
+                detach=True,
+                ports={RABBIT_HTTP_API_PORT: 0},  # Forward management port by default.
+            ),
+            **kwargs,
+        )
 
-        upload_file(self.container, '/etc/rabbitmq/rabbitmq.conf',
-                    f'''
+        upload_file(
+            self.container,
+            "/etc/rabbitmq/rabbitmq.conf",
+            f"""
                     default_pass = {password}
                     default_user = {user}
                     default_vhost = {virtual_host}
                     loopback_users = none
-                    '''.encode())
+                    """.encode(),
+        )
 
         self._enable_management = enable_management
 
     def connection_port(self):
         return get_ports(self.container)[RABBIT_DEFAULT_PORT]
 
     def connection(self, **kwargs):
         credentials = PlainCredentials(self.user, self.password)
         connection_params = ConnectionParameters(
-            DOCKER_EXPOSE_HOST, self.connection_port(),
-            credentials=credentials, virtual_host=self.virtual_host,
-            **kwargs
+            DOCKER_EXPOSE_HOST,
+            self.connection_port(),
+            credentials=credentials,
+            virtual_host=self.virtual_host,
+            **kwargs,
         )
         return BlockingConnection(connection_params)
 
     def start(self, retry_spec: Optional[RetrySpec] = None):
         super().start()
         retry_spec = retry_spec or RetrySpec(attempts=30)
         conn = retry_spec.retry(self.connection, (AMQPConnectionError, ConnectionError, AMQPConnectorException))
@@ -84,27 +104,26 @@
 
         self.container.exec_run("rabbitmq-plugins enable rabbitmq_management")
 
     def reset_state(self, force_queue_deletion=False):
         try:
             management_url = self.management_url()
         except RuntimeError as e:
-            raise RuntimeError('management must be enabled for clean_slate') from e
+            raise RuntimeError("management must be enabled for clean_slate") from e
 
-        queues_url = management_url + 'api/queues'
+        queues_url = management_url + "api/queues"
         replies = requests.get(queues_url, auth=(self.user, self.password))
         replies.raise_for_status()
         extant_queues = replies.json()
         delete_params = {}
         if not force_queue_deletion:
-            delete_params['if-unused'] = 'true'
+            delete_params["if-unused"] = "true"
         for queue in extant_queues:
-            name = quote(queue['name'], safe='')
-            vhost = quote(queue['vhost'], safe='')
+            name = quote(queue["name"], safe="")
+            vhost = quote(queue["vhost"], safe="")
             requests.delete(
-                management_url + f'api/queues/{vhost}/{name}',
-                auth=(self.user, self.password), params=delete_params
+                management_url + f"api/queues/{vhost}/{name}", auth=(self.user, self.password), params=delete_params
             ).raise_for_status()
 
-    def stop(self, signal='SIGKILL'):
+    def stop(self, signal="SIGKILL"):
         # change in default
         return super().stop(signal)
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/redis.py` & `yellowbox-0.8.4/yellowbox/extras/redis.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,39 +4,40 @@
 from redis import ConnectionError as RedisConnectionError, Redis
 
 from yellowbox import RunMixin
 from yellowbox.containers import create_and_pull, get_ports, upload_file
 from yellowbox.retry import RetrySpec
 from yellowbox.subclasses import AsyncRunMixin, SingleContainerService
 
-__all__ = ['RedisService', 'REDIS_DEFAULT_PORT', 'DEFAULT_RDB_PATH', 'append_state']
+__all__ = ["RedisService", "REDIS_DEFAULT_PORT", "DEFAULT_RDB_PATH", "append_state"]
 
 from yellowbox.utils import DOCKER_EXPOSE_HOST
 
 REDIS_DEFAULT_PORT = 6379
 DEFAULT_RDB_PATH = "/data/dump.rdb"
 
 _T = TypeVar("_T", bound=ContextManager)
 RedisPrimitive = Union[str, int, float, bytes]
-RedisState = Mapping[str, Union[RedisPrimitive, Mapping[str, RedisPrimitive], Sequence[RedisPrimitive]]]
+RedisState = Mapping[str, Union[RedisPrimitive, Mapping[Union[str, bytes], RedisPrimitive], Sequence[RedisPrimitive]]]
 
 
 def append_state(client: Redis, db_state: RedisState):
     for k, v in db_state.items():
         if isinstance(v, Sequence):
             client.rpush(k, *v)
         elif isinstance(v, Mapping):
-            client.hset(k, mapping=v)  # type: ignore
+            client.hset(k, mapping=v)
         else:
             client.set(k, v)
 
 
 class RedisService(SingleContainerService, RunMixin, AsyncRunMixin):
-    def __init__(self, docker_client: DockerClient, image='redis:latest',
-                 redis_file: Optional[IO[bytes]] = None, **kwargs):
+    def __init__(
+        self, docker_client: DockerClient, image="redis:latest", redis_file: Optional[IO[bytes]] = None, **kwargs
+    ):
         container = create_and_pull(docker_client, image, publish_all_ports=True, detach=True)
         self.started = False
         super().__init__(container, **kwargs)
 
         if redis_file:
             self.set_rdb(redis_file)
 
@@ -52,15 +53,15 @@
     def client(self, *, client_cls: Callable[..., _T], **kwargs) -> _T:
         ...
 
     @overload
     def client(self, **kwargs) -> Redis:
         ...
 
-    def client(self, *, client_cls=Redis, **kwargs) -> Any:  # type: ignore
+    def client(self, *, client_cls=Redis, **kwargs) -> Any:
         port = self.client_port()
         return client_cls(host=DOCKER_EXPOSE_HOST, port=port, **kwargs)
 
     def start(self, retry_spec: Optional[RetrySpec] = None):
         super().start()
         client_cm: ContextManager[Redis] = self.client()
         with client_cm as client:
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/sql_base.py` & `yellowbox-0.8.4/yellowbox/extras/sql_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,67 +10,91 @@
 
 from yellowbox import RetrySpec
 from yellowbox.containers import get_ports
 from yellowbox.subclasses import AsyncRunMixin, RunMixin, SingleEndpointService
 from yellowbox.utils import DOCKER_EXPOSE_HOST, docker_host_name
 
 if TYPE_CHECKING:  # pragma: no cover
+
     class AsDefault(Enum):
         as_default = auto()
 
     as_default = AsDefault.as_default
 else:
     as_default = object()
 
 ConnectionOptions = Union[str, Mapping[str, str]]
 
 
-class Database(ContextManager['Database']):
+class Database(ContextManager["Database"]):
     # represents a database that is ensured to exist
     def __init__(self, name: str, owner: SQLService):
         self.name = name
         self.owner = owner
 
-    def local_connection_string(self, dialect: Union[str, AsDefault] = as_default, driver: Optional[str] = None,
-                                options: Union[ConnectionOptions, None, AsDefault] = as_default):
+    def local_connection_string(
+        self,
+        dialect: Union[str, AsDefault] = as_default,
+        driver: Optional[str] = None,
+        options: Union[ConnectionOptions, None, AsDefault] = as_default,
+    ):
         return self.owner.local_connection_string(dialect, driver, database=self.name, options=options)
 
-    def container_connection_string(self, hostname: str, dialect: Union[str, AsDefault] = as_default,
-                                    driver: Optional[str] = None, options: Optional[ConnectionOptions] = None):
+    def container_connection_string(
+        self,
+        hostname: str,
+        dialect: Union[str, AsDefault] = as_default,
+        driver: Optional[str] = None,
+        options: Optional[ConnectionOptions] = None,
+    ):
         return self.owner.container_connection_string(hostname, dialect, driver, database=self.name, options=options)
 
-    def host_connection_string(self, dialect: Union[str, AsDefault] = as_default, driver: Optional[str] = None,
-                               options: Optional[ConnectionOptions] = None):
+    def host_connection_string(
+        self,
+        dialect: Union[str, AsDefault] = as_default,
+        driver: Optional[str] = None,
+        options: Optional[ConnectionOptions] = None,
+    ):
         return self.owner.host_connection_string(dialect, driver, database=self.name, options=options)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.owner.drop_database(self.name)
 
 
 def _options_to_string(options: Optional[ConnectionOptions]) -> str:
     if options is None:
-        return ''
+        return ""
     if isinstance(options, Mapping):
-        return '?' + '&'.join(f"{k}={str(v).replace(' ', '+')}" for k, v in options.items())
-    if not options.startswith('?'):
-        return '?' + options
+        return "?" + "&".join(f"{k}={str(v).replace(' ', '+')}" for k, v in options.items())
+    if not options.startswith("?"):
+        return "?" + options
     return options
 
 
-class SQLService(SingleEndpointService, RunMixin, AsyncRunMixin, ):
+class SQLService(
+    SingleEndpointService,
+    RunMixin,
+    AsyncRunMixin,
+):
     LOCAL_HOSTNAME = DOCKER_EXPOSE_HOST
     INTERNAL_PORT: int
     DIALECT: str
     DEFAULT_START_RETRYSPEC = RetrySpec(attempts=20)
 
-    def __init__(self, *args, local_driver: Optional[str] = None, local_options: Optional[ConnectionOptions] = None,
-                 default_database: str, **kwargs):
+    def __init__(
+        self,
+        *args,
+        local_driver: Optional[str] = None,
+        local_options: Optional[ConnectionOptions] = None,
+        default_database: str,
+        **kwargs,
+    ):
         super().__init__(*args, **kwargs)
         self.local_driver = local_driver
         self.local_options = local_options
         self.default_database = default_database
 
     @abstractmethod
     def userpass(self) -> Tuple[str, str]:
@@ -87,85 +111,102 @@
 
     def database_exists(self, name: str) -> bool:
         return database_exists(self.local_connection_string(database=name))
 
     def external_port(self) -> int:
         return get_ports(self._single_endpoint)[self.INTERNAL_PORT]
 
-    def local_connection_string(self, dialect: Union[str, AsDefault] = as_default,
-                                driver: Union[str, AsDefault, None] = as_default, *, database: str,
-                                options: Union[ConnectionOptions, AsDefault, None] = as_default) -> str:
+    def local_connection_string(
+        self,
+        dialect: Union[str, AsDefault] = as_default,
+        driver: Union[str, AsDefault, None] = as_default,
+        *,
+        database: str,
+        options: Union[ConnectionOptions, AsDefault, None] = as_default,
+    ) -> str:
         """
         Generate an sqlalchemy-style connection string to the database in the service from the docker host.
         Args:
             dialect: The dialect of the sql server.
             driver: additional driver for sqlalchemy to use.
             database: the name of the database to connect to.
             options: additional options to pass to the connection string.
         """
         if dialect is as_default:
             dialect = self.DIALECT
 
         if driver is as_default:
             driver = self.local_driver
         if driver is not None:
-            dialect += '+' + driver
+            dialect += "+" + driver
 
         if options is as_default:
             options = self.local_options
 
         options = _options_to_string(options)
 
-        return f'{dialect}://{":".join(self.userpass())}@{self.LOCAL_HOSTNAME}:{self.external_port()}/' \
-               f'{database}{options}'
-
-    def container_connection_string(self, hostname: str, dialect: Union[str, AsDefault] = as_default,
-                                    driver: Optional[str] = None, *, database: str,
-                                    options: Optional[ConnectionOptions] = None) -> str:
+        return (
+            f'{dialect}://{":".join(self.userpass())}@{self.LOCAL_HOSTNAME}:{self.external_port()}/'
+            f"{database}{options}"
+        )
+
+    def container_connection_string(
+        self,
+        hostname: str,
+        dialect: Union[str, AsDefault] = as_default,
+        driver: Optional[str] = None,
+        *,
+        database: str,
+        options: Optional[ConnectionOptions] = None,
+    ) -> str:
         """
         Generate an sqlalchemy-style connection string to the database in the service from another container on a
          common network.
         Args:
             hostname: the alias of the container.
             dialect: The dialect of the sql server.
             driver: additional driver for sqlalchemy to use.
             database: the name of the database to connect to.
             options: additional options to pass to the connection string.
         """
         if dialect is as_default:
             dialect = self.DIALECT
 
         if driver is not None:
-            dialect += '+' + driver
+            dialect += "+" + driver
 
         options = _options_to_string(options)
 
-        return f'{dialect}://{":".join(self.userpass())}@{hostname}:{self.INTERNAL_PORT}/' \
-               f'{database}{options}'
+        return f"{dialect}://{':'.join(self.userpass())}@{hostname}:{self.INTERNAL_PORT}/{database}{options}"
 
-    def host_connection_string(self, dialect: Union[str, AsDefault] = as_default, driver: Optional[str] = None,
-                               *, database: str, options: Optional[ConnectionOptions] = None) -> str:
+    def host_connection_string(
+        self,
+        dialect: Union[str, AsDefault] = as_default,
+        driver: Optional[str] = None,
+        *,
+        database: str,
+        options: Optional[ConnectionOptions] = None,
+    ) -> str:
         """
         Generate an sqlalchemy-style connection string to the database in the service from another container.
         Args:
             dialect: The dialect of the sql server.
             driver: additional driver for sqlalchemy to use.
             database: the name of the database to connect to.
             options: additional options to pass to the connection string.
         """
         if dialect is as_default:
             dialect = self.DIALECT
 
         if driver is not None:
-            dialect += '+' + driver
+            dialect += "+" + driver
 
         options = _options_to_string(options)
 
-        return f'{dialect}://{":".join(self.userpass())}@{docker_host_name}:{self.external_port()}/' \
-               f'{database}{options}'
+        return f"{dialect}://{':'.join(self.userpass())}@{docker_host_name}:{self.external_port()}/{database}{options}"
 
     def database(self, name: str) -> Database:
         if not self.database_exists(name):
             self.create_database(name)
         return Database(name, self)
 
     def _connect(self):
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/vault.py` & `yellowbox-0.8.4/yellowbox/extras/vault.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,62 +7,68 @@
 from requests.exceptions import ConnectionError
 
 from yellowbox.containers import create_and_pull, get_ports
 from yellowbox.retry import RetrySpec
 from yellowbox.subclasses import AsyncRunMixin, RunMixin, SingleContainerService
 from yellowbox.utils import DOCKER_EXPOSE_HOST, docker_host_name
 
-__all__ = ['VAULT_DEFAULT_PORT', 'DEV_POLICY', 'VaultService']
+__all__ = ["VAULT_DEFAULT_PORT", "DEV_POLICY", "VaultService"]
 
 VAULT_DEFAULT_PORT = 8200
 
 DEV_POLICY = {
     "path": {
-        "secret/*": {
-            "capabilities": ["read"]
-        },
+        "secret/*": {"capabilities": ["read"]},
     }
 }
 
 
 class VaultService(SingleContainerService, RunMixin, AsyncRunMixin):
     """
     A yellow service for Hashicorp Vault, with hvac as a client. The vault container is in dev mode AND SHOULD ONLY BE
     USED FOR DEVELOPMENT.
     """
 
-    def __init__(self, docker_client: DockerClient, image='vault:latest', root_token: str = 'guest', **kwargs):
+    def __init__(
+        self, docker_client: DockerClient, image="hashicorp/vault:latest", root_token: str = "guest", **kwargs
+    ):
         """
         Args:
             docker_client: the client to use
             image: the image name and tag of the vault image
             root_token: the token string for the new vault container, with root access
             **kwargs: forwarded to SingleContainerService
         """
-        container = create_and_pull(docker_client, image, publish_all_ports=True, detach=True, environment={
-            'VAULT_DEV_ROOT_TOKEN_ID': root_token,
-        })
+        container = create_and_pull(
+            docker_client,
+            image,
+            publish_all_ports=True,
+            detach=True,
+            environment={
+                "VAULT_DEV_ROOT_TOKEN_ID": root_token,
+            },
+        )
         self.started = False
         self.root_token = root_token
         super().__init__(container, **kwargs)
 
     def client_port(self):
         return get_ports(self.container)[VAULT_DEFAULT_PORT]
 
     def local_url(self):
-        return f'http://{DOCKER_EXPOSE_HOST}:{self.client_port()}'
+        return f"http://{DOCKER_EXPOSE_HOST}:{self.client_port()}"
 
     def container_url(self):
-        return f'http://{docker_host_name}:{self.client_port()}'
+        return f"http://{docker_host_name}:{self.client_port()}"
 
     def sibling_container_url(self, container_alias):
-        return f'http://{container_alias}:{VAULT_DEFAULT_PORT}'
+        return f"http://{container_alias}:{VAULT_DEFAULT_PORT}"
 
     @contextmanager
-    def client(self, **kwargs) -> Iterator[hvac.Client]:  # type: ignore
+    def client(self, **kwargs) -> Iterator[hvac.Client]:
         """
         Get a context manager that creates and closes a root-access hvac client
         Args:
             **kwargs: forwarded to hvac.Client constructor
         """
         client = hvac.Client(url=self.local_url(), token=self.root_token, **kwargs)
         try:
@@ -77,30 +83,31 @@
     def start(self, retry_spec: Optional[RetrySpec] = None):
         super().start()
 
         retry_spec = retry_spec or RetrySpec(attempts=10)
 
         retry_spec.retry(self._check_health, (VaultError, ConnectionError))
         with self.client() as client:
-            client.sys.enable_auth_method('userpass')
+            client.sys.enable_auth_method("userpass")
         self.started = True
         return self
 
     async def astart(self, retry_spec: Optional[RetrySpec] = None) -> None:
         super().start(retry_spec)
 
         retry_spec = retry_spec or RetrySpec(attempts=10)
 
         await retry_spec.aretry(self._check_health, (VaultError, ConnectionError))
         with self.client() as client:
-            client.sys.enable_auth_method('userpass')
+            client.sys.enable_auth_method("userpass")
         self.started = True
 
-    def set_users(self, userpass: Iterable[Tuple[str, str]], policy_name='dev',
-                  policy: Optional[Mapping] = DEV_POLICY) -> None:
+    def set_users(
+        self, userpass: Iterable[Tuple[str, str]], policy_name="dev", policy: Optional[Mapping] = DEV_POLICY
+    ) -> None:
         """
         Create and set users with policies
         Args:
             userpass: an iterable of users and passwords to create
             policy_name: the name of the policy to assign to the new users
             policy: if assigned, will create or override `profile_name` with the policy dict provided. Default is a
              policy that can read all secrets
@@ -117,30 +124,31 @@
         Args:
             secrets: a dict of secrets, mapping paths to json objects to store
         """
         with self.client() as client:
             for k, v in secrets.items():
                 client.secrets.kv.create_or_update_secret(k, v)
 
-    def clear_secrets(self, root_path='/') -> None:
+    def clear_secrets(self, root_path="/") -> None:
         """
         permanently remove all secrets and subdirectories from a directory in vault
         Args:
             root_path: the root path to delete, default removes all secrets in the vault
         Notes:
             if a secret is assigned to the directory itself, the secret will not be deleted
         """
-        if not root_path.endswith('/'):
+        if not root_path.endswith("/"):
             raise ValueError('path must end with slash "/"')
         client: hvac.Client
         with self.client() as client:
+
             def clear_recursive(path) -> None:
-                secret_names: List[str] = client.secrets.kv.list_secrets(path)['data']['keys']
+                secret_names: List[str] = client.secrets.kv.list_secrets(path)["data"]["keys"]
                 for name in secret_names:
-                    if name.endswith('/'):
+                    if name.endswith("/"):
                         # is a directory
                         clear_recursive(path + name)
                     else:
                         # is a secret
                         client.secrets.kv.delete_metadata_and_all_versions(path + name)
 
             clear_recursive(root_path)
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/webserver/__init__.py` & `yellowbox-0.8.4/yellowbox/extras/webserver/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 from yellowbox.extras.webserver.class_endpoint import class_http_endpoint, class_ws_endpoint
 from yellowbox.extras.webserver.endpoints import MockHTTPEndpoint, MockWSEndpoint, http_endpoint, ws_endpoint
 from yellowbox.extras.webserver.http_request_capture import ExpectedHTTPRequest
 from yellowbox.extras.webserver.util import iter_side_effects, verbose_http_side_effect
 from yellowbox.extras.webserver.webserver import WebServer
 from yellowbox.extras.webserver.ws_request_capture import ExpectedWSTranscript, Sender
 
-__all__ = ['WebServer', 'http_endpoint', 'ws_endpoint', 'ExpectedHTTPRequest', 'ExpectedWSTranscript', 'Sender',
-           'MockHTTPEndpoint', 'MockWSEndpoint', 'class_ws_endpoint', 'class_http_endpoint', 'iter_side_effects',
-           'verbose_http_side_effect']
+__all__ = [
+    "WebServer",
+    "http_endpoint",
+    "ws_endpoint",
+    "ExpectedHTTPRequest",
+    "ExpectedWSTranscript",
+    "Sender",
+    "MockHTTPEndpoint",
+    "MockWSEndpoint",
+    "class_ws_endpoint",
+    "class_http_endpoint",
+    "iter_side_effects",
+    "verbose_http_side_effect",
+]
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/webserver/class_endpoint.py` & `yellowbox-0.8.4/yellowbox/extras/webserver/class_endpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,88 @@
 from functools import update_wrapper
 from typing import TYPE_CHECKING, Any, Callable, ClassVar, Generic, Optional, TypeVar, overload
 
 from yellowbox.extras.webserver.endpoints import (
-    HTTP_SIDE_EFFECT, METHODS, WS_SIDE_EFFECT, MockHTTPEndpoint, MockWSEndpoint, http_endpoint, ws_endpoint
+    HTTP_SIDE_EFFECT,
+    METHODS,
+    WS_SIDE_EFFECT,
+    MockHTTPEndpoint,
+    MockWSEndpoint,
+    http_endpoint,
+    ws_endpoint,
 )
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class EndpointTemplate(Generic[T]):
     """
     A template for a generic endpoint. To be created before any instance of a subclass of webserver, but to be added to
      all instances.
     """
+
     constructor: ClassVar[Callable]
 
     def __init__(self, *args, side_effect_method, **kwargs):
         self.args = args
         self.kwargs = kwargs
         self.side_effect_method = side_effect_method
         update_wrapper(self, side_effect_method)
 
     def construct(self, instance) -> T:
-        if hasattr(self.side_effect_method, '__get__'):
+        if hasattr(self.side_effect_method, "__get__"):
             side_effect = self.side_effect_method.__get__(instance, type(instance))
         else:
             side_effect = self.side_effect_method
         return self.constructor(*self.args, side_effect, **self.kwargs)
 
     if TYPE_CHECKING:
+
         def __get__(self, instance, owner) -> T:
             ...
 
 
 class HTTPEndpointTemplate(EndpointTemplate[MockHTTPEndpoint]):
     """
     A subclass of EndpointTemplate that is used to create an HTTP endpoint.
     """
+
     constructor = staticmethod(http_endpoint)  # type: ignore[assignment]
 
 
 class WSEndpointTemplate(EndpointTemplate[MockWSEndpoint]):
     """
     A subclass of EndpointTemplate that is used to create a websocket endpoint.
     """
+
     constructor = staticmethod(ws_endpoint)  # type: ignore[assignment]
 
 
 @overload
-def class_http_endpoint(methods: METHODS, rule_string: str, *, auto_read_body: bool = True,
-                        forbid_head_verb: bool = True, name: Optional[str] = None)\
-        -> Callable[[Any], HTTPEndpointTemplate]:
+def class_http_endpoint(
+    methods: METHODS,
+    rule_string: str,
+    *,
+    auto_read_body: bool = True,
+    forbid_head_verb: bool = True,
+    name: Optional[str] = None
+) -> Callable[[Any], HTTPEndpointTemplate]:
     ...
 
 
 @overload
-def class_http_endpoint(methods: METHODS, rule_string: str, side_effect: HTTP_SIDE_EFFECT, *,
-                        auto_read_body: bool = True, forbid_implicit_head_verb: bool = True,
-                        name: Optional[str] = None) -> HTTPEndpointTemplate:
+def class_http_endpoint(
+    methods: METHODS,
+    rule_string: str,
+    side_effect: HTTP_SIDE_EFFECT,
+    *,
+    auto_read_body: bool = True,
+    forbid_implicit_head_verb: bool = True,
+    name: Optional[str] = None
+) -> HTTPEndpointTemplate:
     ...
 
 
 def class_http_endpoint(methods: METHODS, rule_string: str, side_effect: Optional[HTTP_SIDE_EFFECT] = None, **kwargs):
     """
     Creates an HTTP endpoint template. Declare this as a class variable in your webserver subclass to automatically add
      the endpoint to all instances. Can be used as a decorator.
@@ -71,43 +92,49 @@
         side_effect: forwarded to MockHTTPEndpoint
         **kwargs: forwarded to MockHTTPEndpoint
 
     Returns:
         A new http endpoint template
 
     """
+
     def ret(side_effect_method):
         return HTTPEndpointTemplate(methods, rule_string, side_effect_method=side_effect_method, **kwargs)
 
     if side_effect is not None:
         return ret(side_effect)
     return ret
 
 
 @overload
-def class_ws_endpoint(rule_string: str, *, name: Optional[str] = None, allow_abrupt_disconnect: bool = True)\
-        -> Callable[[Any], WSEndpointTemplate]: pass
+def class_ws_endpoint(
+    rule_string: str, *, name: Optional[str] = None, allow_abrupt_disconnect: bool = True
+) -> Callable[[Any], WSEndpointTemplate]:
+    pass
 
 
 @overload
-def class_ws_endpoint(rule_string: str, side_effect: WS_SIDE_EFFECT, *,
-                      name: Optional[str] = None, allow_abrupt_disconnect: bool = True) -> WSEndpointTemplate: pass
+def class_ws_endpoint(
+    rule_string: str, side_effect: WS_SIDE_EFFECT, *, name: Optional[str] = None, allow_abrupt_disconnect: bool = True
+) -> WSEndpointTemplate:
+    pass
 
 
 def class_ws_endpoint(rule_string: str, side_effect: Optional[WS_SIDE_EFFECT] = None, **kwargs):
     """
     Creates a websocket endpoint template. Declare this as a class variable in your webserver subclass to automatically
      add the endpoint to all instances. Can be used as a decorator.
     Args:
         rule_string: forwarded to MockWSEndpoint
         side_effect: forwarded to MockWSEndpoint
 
     Returns:
         A new websocket endpoint template
 
     """
+
     def ret(side_effect_method):
         return WSEndpointTemplate(rule_string, side_effect_method=side_effect_method, **kwargs)
 
     if side_effect is not None:
         return ret(side_effect)
     return ret
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/webserver/endpoints.py` & `yellowbox-0.8.4/yellowbox/extras/webserver/endpoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
 from traceback import print_exc
 from typing import (
-    TYPE_CHECKING, Awaitable, Callable, ContextManager, Iterable, Iterator, List, Optional, Tuple, Union, overload
+    TYPE_CHECKING,
+    Awaitable,
+    Callable,
+    ContextManager,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    overload,
 )
 
 from starlette.requests import Request
 from starlette.responses import PlainTextResponse, Response
 from starlette.routing import BaseRoute, Route
 from starlette.status import HTTP_500_INTERNAL_SERVER_ERROR, WS_1011_INTERNAL_ERROR
 from starlette.websockets import WebSocket, WebSocketDisconnect
@@ -15,16 +25,16 @@
 
 from yellowbox.extras.webserver.http_request_capture import RecordedHTTPRequest, RecordedHTTPRequests
 from yellowbox.extras.webserver.ws_request_capture import RecordedWSTranscripts, RecorderEndpoint
 
 BASE_HTTP_SIDE_EFFECT = Union[Response, Callable[[Request], Awaitable[Response]]]
 BASE_WS_SIDE_EFFECT = Callable[[WebSocket], Awaitable[Optional[int]]]
 
-HTTP_SIDE_EFFECT = Union[BASE_HTTP_SIDE_EFFECT, Callable[['MockHTTPEndpoint'], BASE_HTTP_SIDE_EFFECT]]
-WS_SIDE_EFFECT = Union[BASE_WS_SIDE_EFFECT, Callable[['MockWSEndpoint'], BASE_WS_SIDE_EFFECT]]
+HTTP_SIDE_EFFECT = Union[BASE_HTTP_SIDE_EFFECT, Callable[["MockHTTPEndpoint"], BASE_HTTP_SIDE_EFFECT]]
+WS_SIDE_EFFECT = Union[BASE_WS_SIDE_EFFECT, Callable[["MockWSEndpoint"], BASE_WS_SIDE_EFFECT]]
 METHODS = Union[str, Iterable[str]]
 
 if TYPE_CHECKING:
     from yellowbox.extras.webserver.webserver import WebServer
 
 
 class EndpointPatch(ContextManager):
@@ -34,40 +44,47 @@
 
     def __init__(self, endpoint: Union[MockHTTPEndpoint, MockWSEndpoint], restore_side_effect):
         self.endpoint = endpoint
         self.restore_side_effect = restore_side_effect
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.endpoint.side_effect = self.restore_side_effect
-        self.endpoint.owner._raise_from_pending()
+        self.endpoint.owner.raise_from_pending()
 
 
 @overload
 def bind_side_effect(endpoint: MockHTTPEndpoint, side_effect: HTTP_SIDE_EFFECT) -> BASE_HTTP_SIDE_EFFECT:
     pass
 
 
 @overload
 def bind_side_effect(endpoint: MockWSEndpoint, side_effect: WS_SIDE_EFFECT) -> BASE_WS_SIDE_EFFECT:
     pass
 
 
 def bind_side_effect(endpoint, side_effect):
-    if callable(side_effect) and getattr(side_effect, '__side_effect_factory__', False):
+    if callable(side_effect) and getattr(side_effect, "__side_effect_factory__", False):
         return side_effect(endpoint)
     return side_effect
 
 
 class MockHTTPEndpoint:
     """
     A mock http endpoint for a webserver
     """
 
-    def __init__(self, name: str, methods: METHODS, rule_string: str, side_effect: HTTP_SIDE_EFFECT,
-                 auto_read_body: bool = True, forbid_implicit_head_verb: bool = True):
+    def __init__(
+        self,
+        name: str,
+        methods: METHODS,
+        rule_string: str,
+        side_effect: HTTP_SIDE_EFFECT,
+        auto_read_body: bool = True,
+        forbid_implicit_head_verb: bool = True,
+    ):
         """
         Args:
             name: the name of the endpoint
             methods: the methods by which the endpoint is accessible
             rule_string: the rule-string of the endpoint, as specified by starlette routes
             side_effect: the side effect of the endpoint. This can be either a starlette response, or an async callable
              that accepts a starlette request and returns a starlette response.
@@ -96,91 +113,108 @@
         Change the side effect of the endpoint
         Args:
             side_effect: the new side effect of the endpoint
 
         Returns:
             A context manager that, if exited, restores the endpoint's original side effect
         """
-        self.owner._raise_from_pending()
+        self.owner.raise_from_pending()
         previous_side_effect = self.side_effect
         self.side_effect = bind_side_effect(self, side_effect)
         return EndpointPatch(self, previous_side_effect)
 
     @contextmanager
     def capture_calls(self) -> Iterator[RecordedHTTPRequests]:
         """
         A context manager that records all requests to the endpoint in its scope to a list
         Returns:
              A RecordedHTTPRequests to which the requests are recorded
         """
-        self.owner._raise_from_pending()
+        self.owner.raise_from_pending()
         if not self.auto_read_body:
             raise RuntimeError("cannot capture calls if auto_read_body is disabled")
         calls = RecordedHTTPRequests()
         self._request_captures.append(calls)
         try:
             yield calls
         finally:
             if self._request_captures[-1] is not calls:
-                raise RuntimeError('capture_calls contexts cannot be used in parallel')
+                raise RuntimeError("capture_calls contexts cannot be used in parallel")
             self._request_captures.pop()
-            self.owner._raise_from_pending()
+            self.owner.raise_from_pending()
 
     async def get(self, request: Request):
         # the target of the starlette route
         if not self.owner:
-            raise RuntimeError('endpoint must be assigned to a webserver')
-        if self.owner._pending_exception:
+            raise RuntimeError("endpoint must be assigned to a webserver")
+        if self.owner.pending_exception:
             return PlainTextResponse(
-                f'an exception in the webserver had previously occurred: {self.owner._pending_exception!r}',
-                status_code=HTTP_500_INTERNAL_SERVER_ERROR
+                f"an exception in the webserver had previously occurred: {self.owner.pending_exception!r}",
+                status_code=HTTP_500_INTERNAL_SERVER_ERROR,
             )
         try:
             if isinstance(self.side_effect, Response):
                 ret = self.side_effect
             else:
                 ret = await self.side_effect(request)
-        except Exception as ex:
-            print(f'uncaught exception when handling request: {request.method}'
-                  f' {request.url} [{self.owner.__name__}/{self.__name__}]:')
+        except Exception as ex:  # noqa: BLE001
+            print(
+                f"uncaught exception when handling request: {request.method}"
+                f" {request.url} [{self.owner.__name__}/{self.__name__}]:"
+            )
             print_exc()
-            self.owner._pending_exception = ex
-            return PlainTextResponse(f'handler raised an exception: {ex!r}', status_code=HTTP_500_INTERNAL_SERVER_ERROR)
+            self.owner.pending_exception = ex
+            return PlainTextResponse(f"handler raised an exception: {ex!r}", status_code=HTTP_500_INTERNAL_SERVER_ERROR)
         else:
             if self.auto_read_body:
                 await request.body()
             if self._request_captures:  # recording the request reads its body, which we might not want
                 recorded = await RecordedHTTPRequest.from_request(request)
                 for c in self._request_captures:
                     c.append(recorded)
         return ret
 
     def route(self) -> BaseRoute:
         """
         Returns: a starlette route representing the endpoint
         """
         ret = Route(self.rule_string, self.get, methods=self.methods, name=self.__name__)  # type:ignore[arg-type]
-        if self.forbid_implicit_head_verb and 'HEAD' not in self.methods:
-            ret.methods.discard('HEAD')
+        if self.forbid_implicit_head_verb and "HEAD" not in self.methods:
+            ret.methods.discard("HEAD")
         return ret
 
 
 @overload
-def http_endpoint(methods: METHODS, rule_string: str, *, auto_read_body: bool = True, forbid_head_verb: bool = True,
-                  name: str = None) \
-        -> Callable[[HTTP_SIDE_EFFECT], MockHTTPEndpoint]: ...
+def http_endpoint(
+    methods: METHODS, rule_string: str, *, auto_read_body: bool = True, forbid_head_verb: bool = True, name: str = None
+) -> Callable[[HTTP_SIDE_EFFECT], MockHTTPEndpoint]:
+    ...
 
 
 @overload
-def http_endpoint(methods: METHODS, rule_string: str, side_effect: HTTP_SIDE_EFFECT, *, auto_read_body: bool = True,
-                  forbid_implicit_head_verb: bool = True, name: str = None) -> MockHTTPEndpoint: ...
-
-
-def http_endpoint(methods: METHODS, rule_string: str, side_effect: Optional[HTTP_SIDE_EFFECT] = None, *,
-                  name: Optional[str] = None, **kwargs):
+def http_endpoint(
+    methods: METHODS,
+    rule_string: str,
+    side_effect: HTTP_SIDE_EFFECT,
+    *,
+    auto_read_body: bool = True,
+    forbid_implicit_head_verb: bool = True,
+    name: str = None,
+) -> MockHTTPEndpoint:
+    ...
+
+
+def http_endpoint(
+    methods: METHODS,
+    rule_string: str,
+    side_effect: Optional[HTTP_SIDE_EFFECT] = None,
+    *,
+    name: Optional[str] = None,
+    **kwargs,
+):
     """
     Create a mock HTTP endpoint.
     Args:
         methods: forwarded to MockHTTPEndpoint
         rule_string: forwarded to MockHTTPEndpoint
         side_effect: forwarded to MockHTTPEndpoint
         name: forwarded to MockHTTPEndpoint, if none, an automaitic name is generated.
@@ -199,21 +233,21 @@
         ...
         ... WebServer().add_http_endpoint(bar)
 
     """
 
     def ret(func: HTTP_SIDE_EFFECT):
         nonlocal name
-        if name is None and not getattr(func, '__skip_name_for_side_effect__', False):
+        if name is None and not getattr(func, "__skip_name_for_side_effect__", False):
             try:
                 name = func.__name__  # type: ignore[union-attr]
             except AttributeError:
                 pass
         if name is None:
-            name = f'{methods} {rule_string}'
+            name = f"{methods} {rule_string}"
         return MockHTTPEndpoint(name, methods, rule_string, func, **kwargs)
 
     if side_effect is None:
         return ret
     return ret(side_effect)
 
 
@@ -244,67 +278,71 @@
         self.endpoint = RecorderEndpoint(function=self.get, sinks=self._request_captures)
 
     async def get(self, websocket: WebSocket):
         # this will be the function that our endpoint will eventually route to
         if not self.owner:
             await websocket.close(WS_1011_INTERNAL_ERROR)  # note that this will actually send a 403 code :shrug:
             return
-        if self.owner._pending_exception:
+        if self.owner.pending_exception:
             await websocket.close(WS_1011_INTERNAL_ERROR)  # note that this will actually send a 403 code :shrug:
             return
         try:
             code = await self.side_effect(websocket)
-        except Exception as ex:
+        except Exception as ex:  # noqa: BLE001
             if self.allow_abrupt_disconnect and isinstance(ex, (WebSocketDisconnect, ConnectionClosed)):
                 pass
             else:
-                print(f'uncaught exception when handling ws: {websocket.url} [{self.owner.__name__}/{self.__name__}]:')
+                print(f"uncaught exception when handling ws: {websocket.url} [{self.owner.__name__}/{self.__name__}]:")
                 print_exc()
-                self.owner._pending_exception = ex
+                self.owner.pending_exception = ex
                 await websocket.close(WS_1011_INTERNAL_ERROR)
         else:
             if code is not None:
                 await websocket.close(code)
 
     def patch(self, side_effect: WS_SIDE_EFFECT):
         """
         Change the side effect of the endpoint
         Args:
             side_effect: the new side effect of the endpoint
 
         Returns:
             A context manager that, if exited, restores the endpoint's original side effect
         """
-        self.owner._raise_from_pending()
+        self.owner.raise_from_pending()
         previous_side_effect = self.side_effect
         self.side_effect = bind_side_effect(self, side_effect)
         return EndpointPatch(self, previous_side_effect)
 
     @contextmanager
     def capture_calls(self) -> Iterator[RecordedWSTranscripts]:
-        self.owner._raise_from_pending()
+        self.owner.raise_from_pending()
         calls = RecordedWSTranscripts()
         self._request_captures.append(calls)
         try:
             yield calls
         finally:
             if self._request_captures[-1] is not calls:
-                raise RuntimeError('capture_calls contexts cannot be used in parallel')
+                raise RuntimeError("capture_calls contexts cannot be used in parallel")
             self._request_captures.pop()
-            self.owner._raise_from_pending()
+            self.owner.raise_from_pending()
 
 
 @overload
-def ws_endpoint(rule_string: str, *, name: str = None, allow_abrupt_disconnect: bool = True) \
-        -> Callable[[WS_SIDE_EFFECT], MockWSEndpoint]: pass
+def ws_endpoint(
+    rule_string: str, *, name: str = None, allow_abrupt_disconnect: bool = True
+) -> Callable[[WS_SIDE_EFFECT], MockWSEndpoint]:
+    pass
 
 
 @overload
-def ws_endpoint(rule_string: str, side_effect: WS_SIDE_EFFECT, *, name: str = None,
-                allow_abrupt_disconnect: bool = True) -> MockWSEndpoint: pass
+def ws_endpoint(
+    rule_string: str, side_effect: WS_SIDE_EFFECT, *, name: str = None, allow_abrupt_disconnect: bool = True
+) -> MockWSEndpoint:
+    pass
 
 
 def ws_endpoint(rule_string: str, side_effect: Optional[WS_SIDE_EFFECT] = None, *, name: str = None, **kwargs):
     """
     Create a mock websocket endpoint.
     Args:
         rule_string: forwarded to MockWSEndpoint
@@ -326,15 +364,15 @@
         ...   await ws.close()
         ...
         ... WebServer().add_ws_endpoint(square)
     """
 
     def ret(func: WS_SIDE_EFFECT):
         nonlocal name
-        if name is None and not getattr(func, '__skip_name_for_side_effect__', False):
+        if name is None and not getattr(func, "__skip_name_for_side_effect__", False):
             try:
                 name = func.__name__
             except AttributeError:
                 pass
         if name is None:
             name = rule_string
         return MockWSEndpoint(name, rule_string, func, **kwargs)
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/webserver/http_request_capture.py` & `yellowbox-0.8.4/yellowbox/extras/webserver/http_request_capture.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,29 @@
 
 
 class ExpectedHTTPRequest(ScopeExpectation):
     """
     An expected HTTP request
     """
 
-    def __init__(self, headers: Optional[Mapping[str, Collection[str]]] = None,
-                 headers_submap: Optional[Mapping[str, Collection[str]]] = None,
-                 path: Optional[Union[str, Pattern[str]]] = None, path_params: Optional[Mapping[str, Any]] = None,
-                 path_params_submap: Optional[Mapping[str, Any]] = None,
-                 query_params: Optional[Mapping[str, Collection[str]]] = None,
-                 query_params_submap: Optional[Mapping[str, Collection[str]]] = None, method: Optional[str] = None,
-                 body: Optional[bytes] = None, text: Optional[str] = None, json: Any = _missing,
-                 content_predicate: Optional[Union[Callable[[bytes], bool], Tuple[Callable[[bytes], Any], Any]]]
-                 = None):
+    def __init__(
+        self,
+        headers: Optional[Mapping[str, Collection[str]]] = None,
+        headers_submap: Optional[Mapping[str, Collection[str]]] = None,
+        path: Optional[Union[str, Pattern[str]]] = None,
+        path_params: Optional[Mapping[str, Any]] = None,
+        path_params_submap: Optional[Mapping[str, Any]] = None,
+        query_params: Optional[Mapping[str, Collection[str]]] = None,
+        query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
+        method: Optional[str] = None,
+        body: Optional[bytes] = None,
+        text: Optional[str] = None,
+        json: Any = _missing,
+        content_predicate: Optional[Union[Callable[[bytes], bool], Tuple[Callable[[bytes], Any], Any]]] = None,
+    ):
         """
         Args:
             headers: If specified, expects the request to have these headers exactly
             headers_submap: If specified expects the request to have at least the headers specified
             path: If specified, expected the request url (after the host) to either be equal to this (in case of string)
              or to fully match the regex pattern provided
             path_params: If specified, expects the request to have exactly these path parameters, as provided by the
@@ -46,29 +52,25 @@
             json: If specified, expects the JSON-decoded content of the request to be equal to the specified value.
              Cannot be used alongside other content-testing parameters
             content_predicate: If specified, must be either a callable that accepts a bytes object, or a tuple of a
              callable that accepts a bytes object and another value, and expects the return value of the callable with
              the content of the request to evaluate to either True or the second element of the tuple, if one is
              provided. Cannot be used alongside other content-testing parameters
         """
-        super().__init__(headers, headers_submap, path, path_params, path_params_submap, query_params,
-                         query_params_submap)
+        super().__init__(
+            headers, headers_submap, path, path_params, path_params_submap, query_params, query_params_submap
+        )
 
         if method is None:
             self.method = None
         else:
             self.method = method.upper()
 
-        if (
-                (body is not None)
-                + (text is not None)
-                + (json is not _missing)
-                + (content_predicate is not None)
-        ) >= 2:
-            raise ValueError('only one of content, text, json must be set')
+        if ((body is not None) + (text is not None) + (json is not _missing) + (content_predicate is not None)) >= 2:
+            raise ValueError("only one of content, text, json must be set")
 
         self.body_decode: Optional[Callable[[bytes], Any]]
         self.data: Optional[Any]
         if body is not None:
             self.body_decode = lambda x: x
             self.data = body
         elif text is not None:
@@ -93,44 +95,45 @@
 
         Returns:
             True if the request matches, or a MismatchReason object with the reason why otherwise.
         """
         reasons = list(self.scope_mismatch_reasons(recorded))
 
         if self.method and self.method != recorded.method:
-            reasons.append(reason_is_ne('body', self.method, recorded.method))
+            reasons.append(reason_is_ne("body", self.method, recorded.method))
 
         if self.body_decode is not None:
             try:
                 body = self.body_decode(recorded.content)
-            except Exception as e:
-                reasons.append(f'failed to parse content: {e!r}')
+            except Exception as e:  # noqa: BLE001
+                reasons.append(f"failed to parse content: {e!r}")
             else:
                 if self.data != body:
-                    reasons.append(reason_is_ne('content', self.data, body))
+                    reasons.append(reason_is_ne("content", self.data, body))
 
         if reasons:
-            return MismatchReason(', '.join(reasons))
+            return MismatchReason(", ".join(reasons))
         return True
 
     def __repr__(self):
         args = self._repr_map()
         if self.method is not None:
-            args['method'] = self.method
+            args["method"] = self.method
         if self.body_decode is not None:
-            args['content'] = self.data
+            args["content"] = self.data
 
-        return 'ExpectedHTTPRequest(' + ', '.join(f'{k}={v!r}' for (k, v) in args.items()) + ')'
+        return "ExpectedHTTPRequest(" + ", ".join(f"{k}={v!r}" for (k, v) in args.items()) + ")"
 
 
 @dataclass
 class RecordedHTTPRequest:
     """
     A recorded HTTP request, received by a starlette application.
     """
+
     headers: Mapping[str, Sequence[str]]
     method: str
     path: str
     path_params: Mapping[str, Any]
     query_params: Mapping[str, Sequence[str]]
     content: bytes
 
@@ -145,203 +148,211 @@
             the recorded recorded request
 
         Notes:
             this method waits for and reads the request body
         """
         headers = {}
         for k, v in request.headers.items():
-            k = k.lower()
-            if k not in headers:
-                headers[k] = [v]
+            k_lower = k.lower()
+            if k_lower not in headers:
+                headers[k_lower] = [v]
             else:
-                headers[k].append(v)
+                headers[k_lower].append(v)
 
         query_args = {}
         for k, v in request.query_params.multi_items():
             if k not in query_args:
                 query_args[k] = [v]
             else:
                 query_args[k].append(v)
 
-        return cls(
-            headers,
-            request.method,
-            request.url.path,
-            request.path_params,
-            query_args,
-            await request.body()
-        )
+        return cls(headers, request.method, request.url.path, request.path_params, query_args, await request.body())
 
 
 class RecordedHTTPRequests(List[RecordedHTTPRequest]):
     """
     A list of recorded HTTP requests, in the order they were received
     """
 
     def assert_not_requested(self):
         """
         asserts that no requests were recorded.
         """
         if self:
-            raise AssertionError(f'{len(self)} requests, latest: {self[-1]}')
+            raise AssertionError(f"{len(self)} requests, latest: {self[-1]}")
 
     def assert_requested(self):
         """
         asserts that at least one request was recorded.
         """
         if not self:
-            raise AssertionError('No requests were made')
+            raise AssertionError("No requests were made")
 
     def assert_requested_once(self):
         """
         asserts that exactly one request was recorded.
         """
         if not self:
-            raise AssertionError('No requests were made')
+            raise AssertionError("No requests were made")
         if len(self) > 1:
-            raise AssertionError('Multiple requests were made:'
-                                 + ''.join(f'\n\t{existing}' for existing in self))
+            raise AssertionError("Multiple requests were made:" + "".join(f"\n\t{existing}" for existing in self))
 
     @overload
     def assert_requested_with(self, expected: ExpectedHTTPRequest):
         ...
 
     @overload
-    def assert_requested_with(self, *, headers: Optional[Mapping[str, Collection[str]]] = None,
-                              headers_submap: Optional[Mapping[str, Collection[str]]] = None,
-                              path: Optional[Union[str, Pattern[str]]] = None,
-                              path_params: Optional[Mapping[str, Any]] = None,
-                              path_params_submap: Optional[Mapping[str, Any]] = None,
-                              query_params: Optional[Mapping[str, Collection[str]]] = None,
-                              query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
-                              method: Optional[str] = None, body: Optional[bytes] = None,
-                              text: Optional[str] = None, json: Any = _missing,
-                              content_predicate:
-                              Optional[Union[Callable[[bytes], bool], Tuple[Callable[[bytes], Any], Any]]] = None):
+    def assert_requested_with(
+        self,
+        *,
+        headers: Optional[Mapping[str, Collection[str]]] = None,
+        headers_submap: Optional[Mapping[str, Collection[str]]] = None,
+        path: Optional[Union[str, Pattern[str]]] = None,
+        path_params: Optional[Mapping[str, Any]] = None,
+        path_params_submap: Optional[Mapping[str, Any]] = None,
+        query_params: Optional[Mapping[str, Collection[str]]] = None,
+        query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
+        method: Optional[str] = None,
+        body: Optional[bytes] = None,
+        text: Optional[str] = None,
+        json: Any = _missing,
+        content_predicate: Optional[Union[Callable[[bytes], bool], Tuple[Callable[[bytes], Any], Any]]] = None,
+    ):
         ...
 
     def assert_requested_with(self, expected: Optional[ExpectedHTTPRequest] = None, **kwargs):
         """
         Asserts that the latest request recorded matches an expected request
         Args:
             expected: an expected request.
             **kwargs: if an expected request is not provided, then a new expected request is constructed by forwarding
              the keyword arguments to the constructor of ExpectedHTTPRequest.
         """
         if expected and kwargs:
-            raise TypeError('method can be called with either expected or keyword args, but not both')
+            raise TypeError("method can be called with either expected or keyword args, but not both")
         if not expected:
             if not kwargs:
-                raise TypeError('either expected or keyword args must be provided')
+                raise TypeError("either expected or keyword args must be provided")
             expected = ExpectedHTTPRequest(**kwargs)
 
         if not self:
-            raise AssertionError('No requests were made')
+            raise AssertionError("No requests were made")
         match = expected.matches(self[-1])
         if not match:
             raise AssertionError(str(match))
 
     @overload
     def assert_requested_once_with(self, expected: ExpectedHTTPRequest):
         ...
 
     @overload
-    def assert_requested_once_with(self, *, headers: Optional[Mapping[str, Collection[str]]] = None,
-                                   headers_submap: Optional[Mapping[str, Collection[str]]] = None,
-                                   path: Optional[Union[str, Pattern[str]]] = None,
-                                   path_params: Optional[Mapping[str, Any]] = None,
-                                   path_params_submap: Optional[Mapping[str, Any]] = None,
-                                   query_params: Optional[Mapping[str, Collection[str]]] = None,
-                                   query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
-                                   method: Optional[str] = None, body: Optional[bytes] = None,
-                                   text: Optional[str] = None, json: Any = _missing,
-                                   content_predicate:
-                                   Optional[Union[Callable[[bytes], bool], Tuple[Callable[[bytes], Any], Any]]] = None):
+    def assert_requested_once_with(
+        self,
+        *,
+        headers: Optional[Mapping[str, Collection[str]]] = None,
+        headers_submap: Optional[Mapping[str, Collection[str]]] = None,
+        path: Optional[Union[str, Pattern[str]]] = None,
+        path_params: Optional[Mapping[str, Any]] = None,
+        path_params_submap: Optional[Mapping[str, Any]] = None,
+        query_params: Optional[Mapping[str, Collection[str]]] = None,
+        query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
+        method: Optional[str] = None,
+        body: Optional[bytes] = None,
+        text: Optional[str] = None,
+        json: Any = _missing,
+        content_predicate: Optional[Union[Callable[[bytes], bool], Tuple[Callable[[bytes], Any], Any]]] = None,
+    ):
         ...
 
     def assert_requested_once_with(self, expected: Optional[ExpectedHTTPRequest] = None, **kwargs):
         """
         Asserts that there is only one request, and that it matches an expected request
         Args:
             expected: an expected request.
             **kwargs: if an expected request is not provided, then a new expected request is constructed by forwarding
              the keyword arguments to the constructor of ExpectedHTTPRequest.
         """
         if expected and kwargs:
-            raise TypeError('method can be called with either expected or keyword args, but not both')
+            raise TypeError("method can be called with either expected or keyword args, but not both")
         if not expected:
             if not kwargs:
-                raise TypeError('either expected or keyword args must be provided')
+                raise TypeError("either expected or keyword args must be provided")
             expected = ExpectedHTTPRequest(**kwargs)
 
         if not self:
-            raise AssertionError('No requests were made')
+            raise AssertionError("No requests were made")
         if len(self) > 1:
-            raise AssertionError('Multiple requests were made:'
-                                 + ''.join(f'\n\t{existing}' for existing in self))
+            raise AssertionError("Multiple requests were made:" + "".join(f"\n\t{existing}" for existing in self))
         match = expected.matches(self[0])
         if not match:
             raise AssertionError(str(match))
 
     @overload
     def assert_any_request(self, expected: ExpectedHTTPRequest):
         ...
 
     @overload
-    def assert_any_request(self, *, headers: Optional[Mapping[str, Collection[str]]] = None,
-                           headers_submap: Optional[Mapping[str, Collection[str]]] = None,
-                           path: Optional[Union[str, Pattern[str]]] = None,
-                           path_params: Optional[Mapping[str, Any]] = None,
-                           path_params_submap: Optional[Mapping[str, Any]] = None,
-                           query_params: Optional[Mapping[str, Collection[str]]] = None,
-                           query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
-                           method: Optional[str] = None, body: Optional[bytes] = None,
-                           text: Optional[str] = None, json: Any = _missing,
-                           content_predicate:
-                           Optional[Union[Callable[[bytes], bool], Tuple[Callable[[bytes], Any], Any]]] = None):
+    def assert_any_request(
+        self,
+        *,
+        headers: Optional[Mapping[str, Collection[str]]] = None,
+        headers_submap: Optional[Mapping[str, Collection[str]]] = None,
+        path: Optional[Union[str, Pattern[str]]] = None,
+        path_params: Optional[Mapping[str, Any]] = None,
+        path_params_submap: Optional[Mapping[str, Any]] = None,
+        query_params: Optional[Mapping[str, Collection[str]]] = None,
+        query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
+        method: Optional[str] = None,
+        body: Optional[bytes] = None,
+        text: Optional[str] = None,
+        json: Any = _missing,
+        content_predicate: Optional[Union[Callable[[bytes], bool], Tuple[Callable[[bytes], Any], Any]]] = None,
+    ):
         ...
 
     def assert_any_request(self, expected: Optional[ExpectedHTTPRequest] = None, **kwargs):
         """
         Asserts that at least one request recorded matches an expected request
         Args:
             expected: an expected request.
             **kwargs: if an expected request is not provided, then a new expected request is constructed by forwarding
              the keyword arguments to the constructor of ExpectedHTTPRequest.
         """
         if expected and kwargs:
-            raise TypeError('method can be called with either expected or keyword args, but not both')
+            raise TypeError("method can be called with either expected or keyword args, but not both")
         if not expected:
             if not kwargs:
-                raise TypeError('either expected or keyword args must be provided')
+                raise TypeError("either expected or keyword args must be provided")
             expected = ExpectedHTTPRequest(**kwargs)
 
         if not self:
-            raise AssertionError('No requests were made')
+            raise AssertionError("No requests were made")
         whynots: List[Tuple[RecordedHTTPRequest, MismatchReason]] = []
         for req in self:
             match = expected.matches(req)
             if match:
                 return
             assert isinstance(match, MismatchReason)
             whynots.append((req, match))
-        raise AssertionError(f'expected request {expected}, but no requests match:',
-                             ''.join(f'\n\t {existing}- {whynot}' for (existing, whynot) in whynots))
+        raise AssertionError(
+            f"expected request {expected}, but no requests match:",
+            "".join(f"\n\t {existing}- {whynot}" for (existing, whynot) in whynots),
+        )
 
     def assert_has_requests(self, *expected_requests: ExpectedHTTPRequest):
         """
         Asserts that all of the expected requests exclusively match a one of the recorded requests, in sequential order.
         Args:
             *expected_requests: the expected requests.
         Notes:
             The matched requests must be sequential relative to the expected requests, but they needn't be contiguous.
              This means that if requests A,B are expected, then the recorded request sequence A,C,B matches it.
         """
         if not expected_requests:
-            raise TypeError('at least one expected request must be provided')
+            raise TypeError("at least one expected request must be provided")
 
         if len(self) < len(expected_requests):
             raise AssertionError(f"could not find request to match {expected_requests[0]}")
         # match greedily
         expected_iter = iter(expected_requests)
         next_expected = next(expected_iter)
         for request in self:
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/webserver/request_capture.py` & `yellowbox-0.8.4/yellowbox/extras/webserver/request_capture.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import re
 from collections import Counter
 from typing import Any, Collection, Iterable, Iterator, Mapping, Optional, Pattern, Tuple, TypeVar, Union
 
 from yellowbox.extras.webserver.util import MismatchReason, lower_keys, reason_is_ne
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 _missing = object()
-K = TypeVar('K')
-V = TypeVar('V')
+K = TypeVar("K")
+V = TypeVar("V")
 
 
 def _is_submap_of(submap: Mapping[K, V], supermap: Mapping[K, V]):
     """
     checks whether a map is a submap of another map
     Args:
         submap: the submap to check
@@ -23,17 +23,17 @@
 
     Notes:
         Mapping A is a submap of Mapping B iff every pair in A also exists in B
     """
     for k, v in submap.items():
         other_v = supermap.get(k, _missing)  # type:ignore[arg-type]
         if other_v is _missing:
-            return MismatchReason(f'expected key {k}, none found (found keys {list(supermap.keys())})')
+            return MismatchReason(f"expected key {k}, none found (found keys {list(supermap.keys())})")
         if other_v != v:
-            return MismatchReason(f'expected key {k} to have value {v}, got {other_v}')
+            return MismatchReason(f"expected key {k} to have value {v}, got {other_v}")
     return True
 
 
 def _is_submultimap_of(submultimap: Mapping[K, Collection[V]], supermultimap: Mapping[K, Collection[V]]):
     """
     checks whether a map is a submultimap of another map
     Args:
@@ -45,24 +45,25 @@
 
     Notes:
         Mapping A is a submap of Mapping B iff for every key k in A, Counter(B[k]) >= Counter(A[k])
     """
     for k, v in submultimap.items():
         other_v = supermultimap.get(k, _missing)
         if other_v is _missing:
-            return MismatchReason(f'expected key {k}, none found')
+            return MismatchReason(f"expected key {k}, none found")
         if not isinstance(other_v, Iterable):
-            return MismatchReason(f'expected key {k} to be in iterable {other_v}')
+            return MismatchReason(f"expected key {k} to be in iterable {other_v}")
         diff = Counter(other_v)
         diff.subtract(Counter(v))
         missing_value = next((k for (k, v) in diff.items() if v < 0), _missing)
         if missing_value is not _missing:
             expected = sum(i == missing_value for i in v)
-            return MismatchReason(f'expected value {missing_value!r} to appear {expected} times in key {k}'
-                                  f', got {other_v}')
+            return MismatchReason(
+                f"expected value {missing_value!r} to appear {expected} times in key {k} got {other_v}"
+            )
     return True
 
 
 def _to_expected_map(name: str, exact: Optional[T], submap: Optional[T]) -> Optional[Tuple[T, bool]]:
     """
     A utility function to convert two parameters one representing an exact-match expectation and one a submap
      expectation, into a single value.
@@ -81,16 +82,17 @@
             raise TypeError(f'at most one of "{name}" and "{name}_submap" can be provided')
         return exact, False
     if submap is not None:
         return submap, True
     return None
 
 
-def _matches_expected_map(name: str, expected: Optional[Tuple[Mapping[K, V], bool]], recorded: Mapping[K, V]) \
-        -> Optional[str]:
+def _matches_expected_map(
+    name: str, expected: Optional[Tuple[Mapping[K, V], bool]], recorded: Mapping[K, V]
+) -> Optional[str]:
     """
     Matches a map against the return value of _to_expected_map
     Args:
         name: the name of the field being matched
         expected: the expected value, as returned by _to_expected_map
         recorded: the recorded value to match
 
@@ -99,23 +101,23 @@
     """
     if expected is None:
         return None
     expected_value, is_subset = expected
     if is_subset:
         submap_match = _is_submap_of(expected_value, recorded)
         if not submap_match:
-            return f'{name} mismatch: {submap_match}'
-    else:
-        if expected_value != recorded:
-            return reason_is_ne(name, expected_value, recorded)
+            return f"{name} mismatch: {submap_match}"
+    elif expected_value != recorded:
+        return reason_is_ne(name, expected_value, recorded)
     return None
 
 
-def _matches_expected_multimap(name: str, expected: Optional[Tuple[Mapping[K, Collection[V]], bool]],
-                               recorded: Mapping[K, Collection[V]]) -> Optional[str]:
+def _matches_expected_multimap(
+    name: str, expected: Optional[Tuple[Mapping[K, Collection[V]], bool]], recorded: Mapping[K, Collection[V]]
+) -> Optional[str]:
     """
     Matches a multimap against the return value of _to_expected_map
     Args:
         name: the name of the field being matched
         expected: the expected value, as returned by _to_expected_map
         recorded: the recorded value to match
 
@@ -124,18 +126,17 @@
     """
     if expected is None:
         return None
     expected_value, is_subset = expected
     if is_subset:
         submap_match = _is_submultimap_of(expected_value, recorded)
         if not submap_match:
-            return f'{name} mismatch: {submap_match}'
-    else:
-        if expected_value != recorded:
-            return reason_is_ne(name, expected_value, recorded)
+            return f"{name} mismatch: {submap_match}"
+    elif expected_value != recorded:
+        return reason_is_ne(name, expected_value, recorded)
     return None
 
 
 def _repr_map(name: str, expected: Optional[Tuple[T, bool]]):
     """
     A utility function to convert the return value of _to_expected_map back to the provided parameters needed to
      construct it.
@@ -146,60 +147,63 @@
     Returns:
         a mapping of the parameters that would result in this expectation if passed to the constructor
     """
     if expected is None:
         return {}
     expected_value, is_subset = expected
     if is_subset:
-        return {f'{name}_submap': expected_value}
+        return {f"{name}_submap": expected_value}
     else:
         return {name: expected_value}
 
 
 class ScopeExpectation:
     """
     A utility mixin class representing an expected http scope, common to both HTTP and websockets.
     """
 
-    def __init__(self, headers: Optional[Mapping[str, Collection[str]]] = None,
-                 headers_submap: Optional[Mapping[str, Collection[str]]] = None,
-                 path: Optional[Union[str, Pattern[str]]] = None, path_params: Optional[Mapping[str, Any]] = None,
-                 path_params_submap: Optional[Mapping[str, Any]] = None,
-                 query_params: Optional[Mapping[str, Collection[str]]] = None,
-                 query_params_submap: Optional[Mapping[str, Collection[str]]] = None, ):
-        self.headers = _to_expected_map('headers', lower_keys(headers), lower_keys(headers_submap))
+    def __init__(
+        self,
+        headers: Optional[Mapping[str, Collection[str]]] = None,
+        headers_submap: Optional[Mapping[str, Collection[str]]] = None,
+        path: Optional[Union[str, Pattern[str]]] = None,
+        path_params: Optional[Mapping[str, Any]] = None,
+        path_params_submap: Optional[Mapping[str, Any]] = None,
+        query_params: Optional[Mapping[str, Collection[str]]] = None,
+        query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
+    ):
+        self.headers = _to_expected_map("headers", lower_keys(headers), lower_keys(headers_submap))
         if isinstance(path, str):
             self.path_pattern = re.compile(re.escape(path))
         else:
             self.path_pattern = path
-        self.path_params = _to_expected_map('path_params', path_params, path_params_submap)
-        self.query_params = _to_expected_map('query_params', query_params, query_params_submap)
+        self.path_params = _to_expected_map("path_params", path_params, path_params_submap)
+        self.query_params = _to_expected_map("query_params", query_params, query_params_submap)
 
     def scope_mismatch_reasons(self, recorded) -> Iterator[str]:
-        header_match = _matches_expected_multimap('header', self.headers, recorded.headers)
+        header_match = _matches_expected_multimap("header", self.headers, recorded.headers)
         if header_match:
             yield header_match
 
-        if (self.path_pattern is not None
-                and self.path_pattern.fullmatch(str(recorded.path)) is None):
-            yield reason_is_ne('path', self.path_pattern.pattern, recorded.path)
+        if self.path_pattern is not None and self.path_pattern.fullmatch(str(recorded.path)) is None:
+            yield reason_is_ne("path", self.path_pattern.pattern, recorded.path)
 
-        path_params_match = _matches_expected_map('path_params', self.path_params, recorded.path_params)
+        path_params_match = _matches_expected_map("path_params", self.path_params, recorded.path_params)
         if path_params_match:
             yield path_params_match
 
-        query_params_match = _matches_expected_multimap('query_params', self.query_params, recorded.query_params)
+        query_params_match = _matches_expected_multimap("query_params", self.query_params, recorded.query_params)
         if query_params_match:
             yield query_params_match
 
     def _repr_map(self):
         """
         Returns: a mapping of the parameters used to create this mixin instance
         """
         args = {
-            **_repr_map('headers', self.headers),
-            **_repr_map('path_params', self.path_params),
-            **_repr_map('query_params', self.query_params),
+            **_repr_map("headers", self.headers),
+            **_repr_map("path_params", self.path_params),
+            **_repr_map("query_params", self.query_params),
         }
         if self.path_pattern is not None:
-            args['path'] = self.path_pattern
+            args["path"] = self.path_pattern
         return args
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/webserver/util.py` & `yellowbox-0.8.4/yellowbox/extras/webserver/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,27 +16,27 @@
     """
     Create a string that is describes two values being unequal
     Args:
         field: the name of the mismatched field
         expected: the expected value
         got: the actual value
     """
-    return f'{field} mismatch: expected {expected}, got {got}'
+    return f"{field} mismatch: expected {expected}, got {got}"
 
 
 class MismatchReason(str):
     """
     A falsish object, signifying a failure to match, with a reason.
     """
 
     def __bool__(self):
         return False
 
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 def iter_side_effects(side_effects: Iterable[Union[Callable[..., Awaitable[T]], T]]) -> Callable[..., Awaitable[T]]:
     """
     Args:
         side_effects: An iterable of side effects.
 
@@ -58,27 +58,30 @@
 
     # we don't want the inner function's __name__ to be the endpoint's name
     ret.__skip_name_for_side_effect__ = True  # type: ignore[attr-defined]
 
     return ret
 
 
-def _DEFAULT_MESSAGE_FACTORY(endpoint: MockHTTPEndpoint, request: Request, response: Response) -> str:
-    client = f'{request.client.host}:{request.client.port}'
+def _default_verbose_message_factory(endpoint: MockHTTPEndpoint, request: Request, response: Response) -> str:
+    client = f"{request.client.host}:{request.client.port}"
     relative_path = request.url.path
     if request.url.query:
-        relative_path += f'?{request.url.query}'
-    return f'{datetime.now().isoformat(sep=" ", timespec="seconds")} {endpoint.owner.__name__}:{endpoint.__name__} ' \
-           f'{client} - {request.method} {relative_path} {response.status_code} ({len(response.body)} bytes)'
+        relative_path += f"?{request.url.query}"
+    return (
+        f'{datetime.now().isoformat(sep=" ", timespec="seconds")} {endpoint.owner.__name__}:{endpoint.__name__} '
+        f"{client} - {request.method} {relative_path} {response.status_code} ({len(response.body)} bytes)"
+    )
 
 
-def verbose_http_side_effect(side_effect: BASE_HTTP_SIDE_EFFECT,
-                             format_function: Callable[[MockHTTPEndpoint, Request, Response], str]
-                             = _DEFAULT_MESSAGE_FACTORY,
-                             file=sys.stdout) -> HTTP_SIDE_EFFECT:
+def verbose_http_side_effect(
+    side_effect: BASE_HTTP_SIDE_EFFECT,
+    format_function: Callable[[MockHTTPEndpoint, Request, Response], str] = _default_verbose_message_factory,
+    file=sys.stdout,
+) -> HTTP_SIDE_EFFECT:
     """
     Wrap a side effect so that it prints the arguments and return value on each call.
     """
 
     def side_effect_factory(endpoint: MockHTTPEndpoint):
         async def side_effect_wrapper(request: Request):
             if isinstance(side_effect, Response):
@@ -97,12 +100,12 @@
             side_effect_wrapper.__skip_name_for_side_effect__ = True  # type: ignore[attr-defined]
         return side_effect_wrapper
 
     side_effect_factory.__side_effect_factory__ = True  # type: ignore[attr-defined]
     return side_effect_factory
 
 
-V = TypeVar('V')
+V = TypeVar("V")
 
 
 def lower_keys(d: Optional[Mapping[AnyStr, V]]) -> Optional[Dict[AnyStr, V]]:
     return {k.lower(): v for k, v in d.items()} if d else None
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/webserver/webserver.py` & `yellowbox-0.8.4/yellowbox/extras/webserver/webserver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
 from threading import Lock, Thread
 from time import sleep
 from typing import ContextManager, Iterator, Mapping, Optional, Union, overload
 
-from requests import ConnectionError, HTTPError, get
+from requests import ConnectionError, RequestException, get
 from starlette.applications import Starlette
 from starlette.responses import PlainTextResponse
 from starlette.routing import Route, WebSocketRoute
 from uvicorn import Config, Server
 
 from yellowbox import YellowService
 from yellowbox.extras.webserver.class_endpoint import HTTPEndpointTemplate, WSEndpointTemplate
 from yellowbox.extras.webserver.endpoints import (
-    HTTP_SIDE_EFFECT, METHODS, WS_SIDE_EFFECT, MockHTTPEndpoint, MockWSEndpoint, http_endpoint, ws_endpoint
+    HTTP_SIDE_EFFECT,
+    METHODS,
+    WS_SIDE_EFFECT,
+    MockHTTPEndpoint,
+    MockWSEndpoint,
+    http_endpoint,
+    ws_endpoint,
 )
 from yellowbox.retry import RetrySpec
 from yellowbox.utils import docker_host_name
 
 
 class HandlerError(Exception):
     """
@@ -26,14 +32,15 @@
     """
 
 
 class WebServer(YellowService):
     """
     An easy-to-modify HTTP and websocket server, wrapping a starlette application
     """
+
     _PORT_ACCESS_MAX_RETRIES = 100  # the maximum number of attempts to make when accessing a binding port.
     _PORT_ACCESS_INTERVAL = 0.01  # retry interval between attempts when accessing a binding port.
 
     _CLASS_ENDPOINT_TEMPLATES: Mapping[str, Union[HTTPEndpointTemplate, WSEndpointTemplate]] = {}
 
     def __init__(self, name: str, port: int = 0, **kwargs):
         """
@@ -44,26 +51,26 @@
         """
         self.__name__ = name
         self._app = Starlette(debug=True)
         self._route_lock = Lock()
 
         # since the main thread won't catch errors in handlers, this class will store any error raised while handling,
         #  and raise them in the main thread as soon as we can
-        self._pending_exception: Optional[Exception] = None
+        self.pending_exception: Optional[Exception] = None
 
-        if 'log_config' not in kwargs:
-            kwargs['log_config'] = None
+        if "log_config" not in kwargs:
+            kwargs["log_config"] = None
 
-        kwargs.setdefault('host', '0.0.0.0')
+        kwargs.setdefault("host", "0.0.0.0")
 
         self._port = port
 
         config = Config(self._app, **kwargs, port=self._port)
         self._server = Server(config)
-        self._serve_thread = Thread(name=f'{name}_thread', target=self._server.run)
+        self._serve_thread = Thread(name=f"{name}_thread", target=self._server.run)
 
     @property
     def port(self) -> int:
         """
         Returns:
             The port the service is bound to, if the service is binding to anything.
 
@@ -71,86 +78,103 @@
             Will only return 0 if the port was not provided during construction and the service thread is not running
             If the service is starting up, this property will block until the port is bound, or raise an error if
             blocked for longer than 1 second.
         """
         if self._port or not self._serve_thread.is_alive():
             return self._port
         for _ in range(self._PORT_ACCESS_MAX_RETRIES):
-            servers = getattr(self._server, 'servers', None)
+            servers = getattr(self._server, "servers", None)
             if servers:
-                sockets = getattr(servers[0], 'sockets', None)
+                sockets = getattr(servers[0], "sockets", None)
                 if sockets:
                     socket = sockets[0]
                     break
             sleep(self._PORT_ACCESS_INTERVAL)
         else:
-            raise RuntimeError('timed out when getting binding port')
+            raise RuntimeError("timed out when getting binding port")
         self._port = socket.getsockname()[1]
         return self._port
 
     @overload
     def add_http_endpoint(self, endpoint: MockHTTPEndpoint) -> MockHTTPEndpoint:
         ...
 
     @overload
-    def add_http_endpoint(self, methods: METHODS, rule_string: str, side_effect: HTTP_SIDE_EFFECT, *,
-                          auto_read_body: bool = True, forbid_implicit_head_verb: bool = True, name: str = None) \
-            -> MockHTTPEndpoint:
+    def add_http_endpoint(
+        self,
+        methods: METHODS,
+        rule_string: str,
+        side_effect: HTTP_SIDE_EFFECT,
+        *,
+        auto_read_body: bool = True,
+        forbid_implicit_head_verb: bool = True,
+        name: str = None,
+    ) -> MockHTTPEndpoint:
         ...
 
     def add_http_endpoint(self, *args, **kwargs) -> MockHTTPEndpoint:
         """
         Add an http endpoint to the server
         Args:
             *args: either a single mock http endpoint, or parameters forwarded to http_endpoint construct one
             **kwargs: forwarded to http_endpoint to construct an endpoint
 
         Returns:
             the http endpoint added to the server
         """
-        self._raise_from_pending()
+        self.raise_from_pending()
         if len(args) == 1 and not kwargs:
-            ep, = args
+            (ep,) = args
         else:
             ep = http_endpoint(*args, **kwargs)
         if ep.owner is not None:
-            raise RuntimeError('an endpoint cannot be added twice')
+            raise RuntimeError("an endpoint cannot be added twice")
         with self._route_lock:
-            self._app.routes.append(
-                ep.route()
-            )
+            self._app.routes.append(ep.route())
         ep.owner = self
         return ep
 
     def remove_http_endpoint(self, endpoint: MockHTTPEndpoint):
         """
         Remove an http endpoint previously added to the server
         Args:
             endpoint: the endpoint to remove
         """
-        self._raise_from_pending()
+        self.raise_from_pending()
         if endpoint.owner is not self:
-            raise RuntimeError('endpoint is not added to the server')
+            raise RuntimeError("endpoint is not added to the server")
         with self._route_lock:
-            for i, route in enumerate(self._app.router.routes):
-                if isinstance(route, Route) and route.endpoint == endpoint.get:
-                    break
-            else:
-                raise RuntimeError('endpoint is not found in the server')
+            i = next(
+                (
+                    i
+                    for i, route in enumerate(self._app.routes)
+                    if isinstance(route, Route) and route.endpoint == endpoint.get
+                ),
+                None,
+            )
+            if i is None:
+                raise RuntimeError("endpoint is not found in the server")
             self._app.router.routes.pop(i)
             endpoint.owner = None
 
     @overload
     def patch_http_endpoint(self, endpoint: MockHTTPEndpoint) -> ContextManager[MockHTTPEndpoint]:
         ...
 
     @overload
-    def patch_http_endpoint(self, methods: METHODS, rule_string: str, side_effect: HTTP_SIDE_EFFECT, *,
-                            auto_read_body: bool = True, forbid_implicit_head_verb: bool = True, name: str = None) \
-            -> ContextManager[MockHTTPEndpoint]:
+    def patch_http_endpoint(
+        self,
+        methods: METHODS,
+        rule_string: str,
+        side_effect: HTTP_SIDE_EFFECT,
+        *,
+        auto_read_body: bool = True,
+        forbid_implicit_head_verb: bool = True,
+        name: str = None,
+    ) -> ContextManager[MockHTTPEndpoint]:
         ...
 
     @contextmanager  # type:ignore[misc]
     def patch_http_endpoint(self, *args, **kwargs) -> Iterator[MockHTTPEndpoint]:
         """
         A context manager to add and then remove an http endpoint
         Args:
@@ -167,69 +191,74 @@
             self.remove_http_endpoint(ep)
 
     @overload
     def add_ws_endpoint(self, endpoint: MockWSEndpoint) -> MockWSEndpoint:
         ...
 
     @overload
-    def add_ws_endpoint(self, rule_string: str, side_effect: WS_SIDE_EFFECT, *, name: str = None,
-                        allow_abrupt_disconnect: bool = True) -> MockWSEndpoint:
+    def add_ws_endpoint(
+        self, rule_string: str, side_effect: WS_SIDE_EFFECT, *, name: str = None, allow_abrupt_disconnect: bool = True
+    ) -> MockWSEndpoint:
         ...
 
     def add_ws_endpoint(self, *args, **kwargs):
         """
         Add a websocket endpoint to the server
         Args:
             *args: either a single mock ws endpoint, or parameters forwarded to ws_endpoint construct one
             **kwargs: forwarded to ws_endpoint to construct an endpoint
 
         Returns:
             the websocket endpoint added to the server
         """
-        self._raise_from_pending()
+        self.raise_from_pending()
         if len(args) == 1 and not kwargs:
-            ep, = args
+            (ep,) = args
         else:
             ep = ws_endpoint(*args, **kwargs)
 
         if ep.owner is not None:
-            raise RuntimeError('an endpoint cannot be added twice')
+            raise RuntimeError("an endpoint cannot be added twice")
 
         with self._route_lock:
-            self._app.routes.append(
-                WebSocketRoute(ep.rule_string, ep.endpoint, name=ep.__name__)
-            )
+            self._app.routes.append(WebSocketRoute(ep.rule_string, ep.endpoint, name=ep.__name__))
         ep.owner = self
         return ep
 
     def remove_ws_endpoint(self, endpoint: MockWSEndpoint):
         """
         Remove a websocket endpoint previously added to the server
         Args:
             endpoint: the endpoint to remove
         """
-        self._raise_from_pending()
+        self.raise_from_pending()
         if endpoint.owner is not self:
-            raise RuntimeError('endpoint is not added to the server')
+            raise RuntimeError("endpoint is not added to the server")
         with self._route_lock:
-            for i, route in enumerate(self._app.router.routes):
-                if isinstance(route, WebSocketRoute) and route.app == endpoint.endpoint:
-                    break
-            else:
-                raise RuntimeError('endpoint is not found in the server')
+            i = next(
+                (
+                    i
+                    for (i, route) in enumerate(self._app.router.routes)
+                    if isinstance(route, WebSocketRoute) and route.app == endpoint.endpoint
+                ),
+                None,
+            )
+            if i is None:
+                raise RuntimeError("endpoint is not found in the server")
             self._app.router.routes.pop(i)
             endpoint.owner = None
 
     @overload
     def patch_ws_endpoint(self, endpoint: MockWSEndpoint) -> ContextManager[MockWSEndpoint]:
         ...
 
     @overload
-    def patch_ws_endpoint(self, rule_string: str, side_effect: WS_SIDE_EFFECT, *, name: str = None,
-                          allow_abrupt_disconnect: bool = True) -> ContextManager[MockWSEndpoint]:
+    def patch_ws_endpoint(
+        self, rule_string: str, side_effect: WS_SIDE_EFFECT, *, name: str = None, allow_abrupt_disconnect: bool = True
+    ) -> ContextManager[MockWSEndpoint]:
         ...
 
     @contextmanager  # type:ignore[misc]
     def patch_ws_endpoint(self, *args, **kwargs):
         """
         A context manager to add and then remove a ws endpoint
         Args:
@@ -241,47 +270,47 @@
         """
         ep = self.add_ws_endpoint(*args, **kwargs)
         try:
             yield ep
         finally:
             self.remove_ws_endpoint(ep)
 
-    def local_url(self, schema: Optional[str] = 'http') -> str:
+    def local_url(self, schema: Optional[str] = "http") -> str:
         """
         Get the url to access this server from the local machine
         Args:
             schema: the optional schema of the url, defaults to http
         """
         if schema is None:
-            return f'localhost:{self.port}'
-        return f'{schema}://localhost:{self.port}'
+            return f"localhost:{self.port}"
+        return f"{schema}://localhost:{self.port}"
 
-    def container_url(self, schema='http') -> str:
+    def container_url(self, schema="http") -> str:
         """
         Get the url to access this server from a docker container running in the local machine
         Args:
             schema: the optional schema of the url, defaults to http
         """
         if schema is None:
-            return f'{docker_host_name}:{self.port}'
-        return f'{schema}://{docker_host_name}:{self.port}'
+            return f"{docker_host_name}:{self.port}"
+        return f"{schema}://{docker_host_name}:{self.port}"
 
     def start(self, retry_spec: Optional[RetrySpec] = None) -> WebServer:
         if self._serve_thread.is_alive():
-            raise RuntimeError('thread cannot be started twice')
+            raise RuntimeError("thread cannot be started twice")
         self._serve_thread.start()
-        with self.patch_http_endpoint('GET', '/__yellowbox/ping', side_effect=PlainTextResponse('')):
+        with self.patch_http_endpoint("GET", "/__yellowbox/ping", side_effect=PlainTextResponse("")):
             retry_spec = retry_spec or RetrySpec(interval=0.1, timeout=5)
             retry_spec.retry(
-                lambda: get(self.local_url() + '/__yellowbox/ping').raise_for_status(),
-                (ConnectionError, HTTPError)
+                lambda: get(self.local_url() + "/__yellowbox/ping", timeout=1.0).raise_for_status(),
+                (ConnectionError, RequestException),
             )
 
         # add all the class endpoints
-        for name, template in type(self)._CLASS_ENDPOINT_TEMPLATES.items():
+        for name, template in type(self)._CLASS_ENDPOINT_TEMPLATES.items():  # noqa: SLF001
             ep: Union[MockHTTPEndpoint, MockWSEndpoint]
             if isinstance(template, HTTPEndpointTemplate):
                 ep = template.construct(self)
                 self.add_http_endpoint(ep)
             else:
                 assert isinstance(template, WSEndpointTemplate)
                 ep = template.construct(self)
@@ -290,38 +319,38 @@
 
         return super().start()
 
     def stop(self):
         self._server.should_exit = True
         self._serve_thread.join()
         super().stop()
-        self._raise_from_pending()
+        self.raise_from_pending()
 
     def is_alive(self) -> bool:
-        self._raise_from_pending()
+        self.raise_from_pending()
         return self._serve_thread.is_alive()
 
-    def _raise_from_pending(self):
+    def raise_from_pending(self):
         # if there is a pending exception, this will raise it
-        if self._pending_exception:
-            pending = self._pending_exception
-            self._pending_exception = None
+        if self.pending_exception:
+            pending = self.pending_exception
+            self.pending_exception = None
             raise HandlerError() from pending
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         _cls_endpoints = {}
         for base in cls.__bases__:
-            base_http_templates = getattr(base, '_CLASS_ENDPOINT_TEMPLATES', None)
+            base_http_templates = getattr(base, "_CLASS_ENDPOINT_TEMPLATES", None)
             if base_http_templates:
                 overlapping_keys = base_http_templates.keys() & _cls_endpoints.keys()
                 if overlapping_keys:
-                    raise TypeError(f'overlapping cls endpoints: {overlapping_keys}')
+                    raise TypeError(f"overlapping cls endpoints: {overlapping_keys}")
                 _cls_endpoints.update(base_http_templates)
 
         for k, v in vars(cls).items():
             if isinstance(v, (HTTPEndpointTemplate, WSEndpointTemplate)):
                 if k in _cls_endpoints:
-                    raise TypeError(f'cls endpoint {k} already defined')
+                    raise TypeError(f"cls endpoint {k} already defined")
                 _cls_endpoints[k] = v
 
         cls._CLASS_ENDPOINT_TEMPLATES = _cls_endpoints
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/webserver/ws_request_capture.py` & `yellowbox-0.8.4/yellowbox/extras/webserver/ws_request_capture.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 from __future__ import annotations
 
+import builtins
 from dataclasses import dataclass
 from enum import Enum, auto
-from typing import Any, Collection, Dict, Iterable, List, Mapping, Optional, Pattern, Sequence, Tuple, Union, overload
+from typing import (
+    Any,
+    Collection,
+    Dict,
+    Iterable,
+    List,
+    Mapping,
+    Optional,
+    Pattern,
+    Sequence,
+    Tuple,
+    Union,
+    overload,
+)
 
 from starlette.requests import HTTPConnection
 from starlette.websockets import WebSocket
 
 from yellowbox.extras.webserver.request_capture import ScopeExpectation
 from yellowbox.extras.webserver.util import MismatchReason, reason_is_ne
 
@@ -28,38 +42,38 @@
         super().__init__(scope, receive, send)
         self.transcript: RecordedWSTranscript = RecordedWSTranscript.from_connection(self)
         for sink in sinks:
             sink.append(self.transcript)
 
     async def receive(self):
         message = await super().receive()
-        message_type = message.get('type')
+        message_type = message.get("type")
         if message_type == "websocket.receive":
             # by asgi uvicorn implementation (def asgi_receive), a message will always contain exactly one of
             #  'text' or 'bytes'
-            data = message.get('text')
+            data = message.get("text")
             if data is None:
-                data = message.get('bytes')
+                data = message.get("bytes")
             self.transcript.append(RecordedWSMessage(data, Sender.Client))
         elif message_type == "websocket.disconnect":
-            self.transcript.close = (Sender.Client, message.get('code', 1000))
+            self.transcript.close = (Sender.Client, message.get("code", 1000))
         return message
 
     async def send(self, message):
         message_type = message["type"]
         if message_type == "websocket.accept":
             self.transcript.accepted = True
         elif message_type == "websocket.close":
-            self.transcript.close = (Sender.Server, message.get('code', 1000))
+            self.transcript.close = (Sender.Server, message.get("code", 1000))
         elif message_type == "websocket.send":
             # by asgi uvicorn implementation (def asgi_receive), a message will always contain exactly one of
             #  'text' or 'data'
-            data = message.get('text')
+            data = message.get("text")
             if data is None:
-                data = message.get('bytes')
+                data = message.get("bytes")
             self.transcript.append(RecordedWSMessage(data, Sender.Server))
         await super().send(message)
 
 
 class RecorderEndpoint:
     """
     An entrypoint app that records websocket conversations
@@ -83,47 +97,54 @@
 
     Examples:
         >>> import re
         ... expected_message = Sender.Server(re.compile('[a-z][a-z][0-9]'))
         ... message = RecordedWSMessage('tk1', Sender.Server)
         ... assert expected_message.matches(message)
     """
+
     Server = auto()
     Client = auto()
 
-    def __call__(self, data: Union[Pattern[str], Pattern[bytes], str, bytes, ellipsis]) \
-            -> ExpectedWSMessage:  # noqa: F821
+    def __call__(self, data: Union[Pattern[str], Pattern[bytes], str, bytes, builtins.ellipsis]) -> ExpectedWSMessage:
         """
         Create an expected message, originating from this caller
         Args:
             data: the expected data of the message. Can be either a bytes or string for an exact match, a compiled
              pattern for a full match, or ellipsis to match any data.
         """
         return ExpectedWSMessage(data, self)
 
 
 @dataclass
 class RecordedWSMessage:
     """
     A recorded websocket message, with a sender and value sent
     """
+
     data: Union[bytes, str]
     sender: Sender
 
     def __repr__(self):
-        return f'RecordedWSMessage({self.data!r}, Sender.{self.sender.name})'
+        return f"RecordedWSMessage({self.data!r}, Sender.{self.sender.name})"
 
 
 class RecordedWSTranscript(List[RecordedWSMessage]):
     """
     A transcript of a single websocket connection
     """
 
-    def __init__(self, arg: Iterable[RecordedWSMessage], headers: Dict[str, List[str]], path: str,
-                 path_params: Dict[str, Any], query_params: Dict[str, List[str]]):
+    def __init__(
+        self,
+        arg: Iterable[RecordedWSMessage],
+        headers: Dict[str, List[str]],
+        path: str,
+        path_params: Dict[str, Any],
+        query_params: Dict[str, List[str]],
+    ):
         """
         Args:
             arg: forwarded to super (List)
             headers: the headers of the connection
             path: the path of the connection request
             path_params: the path params of the connection request, as specified by the route's starlette rule string
             query_params: the query params of the connection request
@@ -143,18 +164,18 @@
         """
         Create an empty transcript from a new http connection
         Args:
             connection: the http connection to use
         """
         headers: Dict[str, List[str]] = {}
         for h_k, h_v in connection.headers.items():
-            h_k = h_k.lower()
-            h_lst = headers.get(h_k)
+            h_k_lower = h_k.lower()
+            h_lst = headers.get(h_k_lower)
             if h_lst is None:
-                headers[h_k] = [h_v]
+                headers[h_k_lower] = [h_v]
             else:
                 h_lst.append(h_v)
         path = connection.url.path
         path_params = connection.path_params
         query_params: Dict[str, List[str]] = {}
         for q_k, q_v in connection.query_params.multi_items():
             q_lst = query_params.get(q_k)
@@ -166,15 +187,15 @@
 
 
 class ExpectedWSMessage:
     """
     A single expected message in a websockets connection
     """
 
-    def __init__(self, data: Union[Pattern[str], Pattern[bytes], str, bytes, ellipsis], sender: Sender):  # noqa: F821
+    def __init__(self, data: Union[Pattern[str], Pattern[bytes], str, bytes, builtins.ellipsis], sender: Sender):
         """
         Args:
             data: the expected data. Can be either a bytes or string for an exact match, a compiled pattern for a full
              match, or ellipsis to match any data.
             sender: The sender to expect the message from.
         """
         self.data = data
@@ -186,48 +207,52 @@
         Args:
             message: the recorded message
 
         Returns:
             True if the message matches, or a mismatch reason otherwise.
         """
         if self.sender != message.sender:
-            return MismatchReason(reason_is_ne('sender', self.sender, message.sender))
+            return MismatchReason(reason_is_ne("sender", self.sender, message.sender))
 
         if self.data is ...:
             return True
         elif isinstance(self.data, Pattern):
             try:
                 match = self.data.fullmatch(message.data)  # type:ignore[arg-type]
             except TypeError:  # this would happen when we try to use byte patterns on strs or vice-versa
                 match = None
             if not match:
-                return MismatchReason(f'expected data to match pattern {self.data.pattern!r}, got {message.data!r}')
+                return MismatchReason(f"expected data to match pattern {self.data.pattern!r}, got {message.data!r}")
             return True
-        else:
-            if self.data != message.data:
-                return MismatchReason(reason_is_ne('data', self.data, message.data))
+        elif self.data != message.data:
+            return MismatchReason(reason_is_ne("data", self.data, message.data))
         return True
 
     def __str__(self):
-        return f'{self.sender.name}({self.data})'
+        return f"{self.sender.name}({self.data})"
 
 
 class ExpectedWSTranscript(ScopeExpectation):
     """
     An expected websocket transcript
     """
 
-    def __init__(self, messages: Sequence[Union[ellipsis, ExpectedWSMessage]] = (...,),  # noqa: F821
-                 headers: Optional[Mapping[str, Collection[str]]] = None,
-                 headers_submap: Optional[Mapping[str, Collection[str]]] = None,
-                 path: Optional[Union[str, Pattern[str]]] = None, path_params: Optional[Mapping[str, Any]] = None,
-                 path_params_submap: Optional[Mapping[str, Any]] = None,
-                 query_params: Optional[Mapping[str, Collection[str]]] = None,
-                 query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
-                 close: Optional[Tuple[Sender, int]] = None, accepted: Optional[bool] = True):
+    def __init__(
+        self,
+        messages: Sequence[Union[builtins.ellipsis, ExpectedWSMessage]] = (...,),
+        headers: Optional[Mapping[str, Collection[str]]] = None,
+        headers_submap: Optional[Mapping[str, Collection[str]]] = None,
+        path: Optional[Union[str, Pattern[str]]] = None,
+        path_params: Optional[Mapping[str, Any]] = None,
+        path_params_submap: Optional[Mapping[str, Any]] = None,
+        query_params: Optional[Mapping[str, Collection[str]]] = None,
+        query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
+        close: Optional[Tuple[Sender, int]] = None,
+        accepted: Optional[bool] = True,
+    ):
         """
         Args:
             messages: the expected messages in the transcript, can begin or end ellipsis to signify that any
                 number of messages can precede or follow the messages to match.
             headers: If specified, expects the request to have these headers exactly
             headers_submap: If specified expects the request to have at least the headers specified
             path: If specified, expected the request url (after the host) to either be equal to this (in case of string)
@@ -239,30 +264,31 @@
             query_params: If specified, expects the request to have these query arguments exactly
             query_params_submap: If specified, expects the request to have at least these query arguments
             close: If specified, must be a tuple of sender and an integer. Expects the transcript to be closed by that
              sender with that code.
             accepted: If specified, will only match transcripts of accepted connections (if True) or rejected
              connections (if False)
         """
-        super().__init__(headers, headers_submap, path, path_params, path_params_submap, query_params,
-                         query_params_submap)
+        super().__init__(
+            headers, headers_submap, path, path_params, path_params_submap, query_params, query_params_submap
+        )
         if messages and messages[0] is ...:
             messages = messages[1:]
             self.any_start = True
         else:
             self.any_start = False
 
         if messages and messages[-1] is ...:
             messages = messages[:-1]
             self.any_end = True
         else:
             self.any_end = False
 
         if any(m is ... for m in messages):
-            raise TypeError('ExpectedWSTranscript can only contain ellipsis at the start and at the end')
+            raise TypeError("ExpectedWSTranscript can only contain ellipsis at the start and at the end")
 
         self.expected_messages: Tuple[ExpectedWSMessage] = messages  # type:ignore[assignment]
         self.accepted = accepted
         self.close = close
 
     def matches(self, recorded: RecordedWSTranscript):
         """
@@ -270,29 +296,29 @@
         Args:
             recorded: the recorded transcript
 
         Returns:
             True if the transcript matches, or a mismatch reason otherwise.
         """
         if recorded.close is None:
-            raise RuntimeError('the transcript is not yet done')
+            raise RuntimeError("the transcript is not yet done")
 
         reasons = list(self.scope_mismatch_reasons(recorded))
 
         if self.close is not None and recorded.close != self.close:
-            reasons.append(reason_is_ne('close_code', self.close, recorded.close))
+            reasons.append(reason_is_ne("close_code", self.close, recorded.close))
         if self.accepted is not None and recorded.accepted != self.accepted:
-            reasons.append(reason_is_ne('accepted', self.accepted, recorded.accepted))
+            reasons.append(reason_is_ne("accepted", self.accepted, recorded.accepted))
 
         if not self.any_start and not self.any_end and len(recorded) != len(self.expected_messages):
-            reasons.append(f'expected exactly {len(self.expected_messages)} messages, found {len(recorded)}')
+            reasons.append(f"expected exactly {len(self.expected_messages)} messages, found {len(recorded)}")
         if len(recorded) < len(self.expected_messages):
-            reasons.append(f'expected at least {len(self.expected_messages)} messages, found only {len(recorded)}')
+            reasons.append(f"expected at least {len(self.expected_messages)} messages, found only {len(recorded)}")
         if reasons:
-            return MismatchReason(', '.join(reasons))
+            return MismatchReason(", ".join(reasons))
         # in order to account for any_start, any_end, we check every subsequence of the recorded transcript
         # we store a list of candidate indices for the subsequence start
         if not self.any_start:
             # the case of (not any_start and not any_end) is covered by the first condition
             indices: Iterable[int] = (0,)
         elif not self.any_end:
             indices = (len(recorded) - len(self.expected_messages),)
@@ -301,156 +327,170 @@
 
         whynots = []
         for start_index in indices:
             for i, expected_message in enumerate(self.expected_messages):
                 rec = recorded[start_index + i]
                 match = expected_message.matches(rec)
                 if not match:
-                    whynots.append(f'{rec} did not match {expected_message}: {match}')
+                    whynots.append(f"{rec} did not match {expected_message}: {match}")
                     break
             else:
                 return True
 
-        return MismatchReason('could not find expected calls' + ''.join('\n\t' + wn for wn in whynots))
+        return MismatchReason("could not find expected calls" + "".join("\n\t" + wn for wn in whynots))
 
 
 class RecordedWSTranscripts(List[RecordedWSTranscript]):
     """
     A list of recorded WS transcripts, in the order that the connections began
     """
 
     def assert_not_requested(self):
         """
         asserts that no connections were recorded.
         """
         if self:
-            raise AssertionError(f'{len(self)} requests were made')
+            raise AssertionError(f"{len(self)} requests were made")
 
     def assert_requested(self):
         """
         asserts that at least one transcript was recorded.
         """
         if not self:
-            raise AssertionError('No requests were made')
+            raise AssertionError("No requests were made")
 
     def assert_requested_once(self):
         """
         asserts that exactly one transcript was recorded.
         """
         if not self:
-            raise AssertionError('No requests were made')
+            raise AssertionError("No requests were made")
         if len(self) > 1:
-            raise AssertionError(f'{len(self)} requests were made')
+            raise AssertionError(f"{len(self)} requests were made")
 
     @overload
     def assert_requested_with(self, expected: ExpectedWSTranscript):
         ...
 
     @overload
-    def assert_requested_with(self, *, messages: Sequence[Union[ellipsis, ExpectedWSMessage]] = (...,),  # noqa: F821
-                              headers: Optional[Mapping[bytes, Collection[bytes]]] = None,
-                              headers_submap: Optional[Mapping[bytes, Collection[bytes]]] = None,
-                              path: Optional[Union[str, Pattern[str]]] = None,
-                              path_params: Optional[Mapping[str, Any]] = None,
-                              path_params_submap: Optional[Mapping[str, Any]] = None,
-                              query_params: Optional[Mapping[str, Collection[str]]] = None,
-                              query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
-                              close: Optional[Tuple[Sender, int]] = None, accepted: Optional[bool] = True):
+    def assert_requested_with(
+        self,
+        *,
+        messages: Sequence[Union[builtins.ellipsis, ExpectedWSMessage]] = (...,),
+        headers: Optional[Mapping[bytes, Collection[bytes]]] = None,
+        headers_submap: Optional[Mapping[bytes, Collection[bytes]]] = None,
+        path: Optional[Union[str, Pattern[str]]] = None,
+        path_params: Optional[Mapping[str, Any]] = None,
+        path_params_submap: Optional[Mapping[str, Any]] = None,
+        query_params: Optional[Mapping[str, Collection[str]]] = None,
+        query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
+        close: Optional[Tuple[Sender, int]] = None,
+        accepted: Optional[bool] = True,
+    ):
         ...
 
     def assert_requested_with(self, expected: Optional[ExpectedWSTranscript] = None, **kwargs):
         """
         Asserts that the latest transcript recorded matches an expected transcript
         Args:
             expected: an expected transcript.
             **kwargs: if an expected request is not provided, then a new expected request is constructed by forwarding
              the keyword arguments to the constructor of ExpectedWSTranscript.
         """
         if expected and kwargs:
-            raise TypeError('method can be called with either expected or keyword args, but not both')
+            raise TypeError("method can be called with either expected or keyword args, but not both")
         if not expected:
             if not kwargs:
-                raise TypeError('either expected or keyword args must be provided')
+                raise TypeError("either expected or keyword args must be provided")
             expected = ExpectedWSTranscript(**kwargs)
 
         if not self:
-            raise AssertionError('No requests were made')
+            raise AssertionError("No requests were made")
         match = expected.matches(self[-1])
         if not match:
             raise AssertionError(str(match))
 
     @overload
     def assert_requested_once_with(self, expected: ExpectedWSTranscript):
         ...
 
     @overload
-    def assert_requested_once_with(self, *,
-                                   messages: Sequence[Union[ellipsis, ExpectedWSMessage]] = (...,),  # noqa: F821
-                                   headers: Optional[Mapping[bytes, Collection[bytes]]] = None,
-                                   headers_submap: Optional[Mapping[bytes, Collection[bytes]]] = None,
-                                   path: Optional[Union[str, Pattern[str]]] = None,
-                                   path_params: Optional[Mapping[str, Any]] = None,
-                                   path_params_submap: Optional[Mapping[str, Any]] = None,
-                                   query_params: Optional[Mapping[str, Collection[str]]] = None,
-                                   query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
-                                   close: Optional[Tuple[Sender, int]] = None, accepted: Optional[bool] = True):
+    def assert_requested_once_with(
+        self,
+        *,
+        messages: Sequence[Union[builtins.ellipsis, ExpectedWSMessage]] = (...,),
+        headers: Optional[Mapping[bytes, Collection[bytes]]] = None,
+        headers_submap: Optional[Mapping[bytes, Collection[bytes]]] = None,
+        path: Optional[Union[str, Pattern[str]]] = None,
+        path_params: Optional[Mapping[str, Any]] = None,
+        path_params_submap: Optional[Mapping[str, Any]] = None,
+        query_params: Optional[Mapping[str, Collection[str]]] = None,
+        query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
+        close: Optional[Tuple[Sender, int]] = None,
+        accepted: Optional[bool] = True,
+    ):
         ...
 
     def assert_requested_once_with(self, expected: Optional[ExpectedWSTranscript] = None, **kwargs):
         """
         Asserts that there is only one transcript, and that it matches an expected transcript
         Args:
             expected: an expected transcript.
             **kwargs: if an expected request is not provided, then a new expected request is constructed by forwarding
              the keyword arguments to the constructor of ExpectedWSTranscript.
         """
         if expected and kwargs:
-            raise TypeError('method can be called with either expected or keyword args, but not both')
+            raise TypeError("method can be called with either expected or keyword args, but not both")
         if not expected:
             if not kwargs:
-                raise TypeError('either expected or keyword args must be provided')
+                raise TypeError("either expected or keyword args must be provided")
             expected = ExpectedWSTranscript(**kwargs)
 
         if not self:
-            raise AssertionError('No requests were made')
+            raise AssertionError("No requests were made")
         if len(self) > 1:
-            raise AssertionError(f'{len(self)} requests were made')
+            raise AssertionError(f"{len(self)} requests were made")
         match = expected.matches(self[0])
         if not match:
             raise AssertionError(str(match))
 
     @overload
     def assert_any_request(self, expected: ExpectedWSTranscript):
         ...
 
     @overload
-    def assert_any_request(self, *, messages: Sequence[Union[ellipsis, ExpectedWSMessage]] = (...,),  # noqa: F821
-                           headers: Optional[Mapping[bytes, Collection[bytes]]] = None,
-                           headers_submap: Optional[Mapping[bytes, Collection[bytes]]] = None,
-                           path: Optional[Union[str, Pattern[str]]] = None,
-                           path_params: Optional[Mapping[str, Any]] = None,
-                           path_params_submap: Optional[Mapping[str, Any]] = None,
-                           query_params: Optional[Mapping[str, Collection[str]]] = None,
-                           query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
-                           close: Optional[Tuple[Sender, int]] = None, accepted: Optional[bool] = True):
+    def assert_any_request(
+        self,
+        *,
+        messages: Sequence[Union[builtins.ellipsis, ExpectedWSMessage]] = (...,),
+        headers: Optional[Mapping[bytes, Collection[bytes]]] = None,
+        headers_submap: Optional[Mapping[bytes, Collection[bytes]]] = None,
+        path: Optional[Union[str, Pattern[str]]] = None,
+        path_params: Optional[Mapping[str, Any]] = None,
+        path_params_submap: Optional[Mapping[str, Any]] = None,
+        query_params: Optional[Mapping[str, Collection[str]]] = None,
+        query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
+        close: Optional[Tuple[Sender, int]] = None,
+        accepted: Optional[bool] = True,
+    ):
         ...
 
     def assert_any_request(self, expected: Optional[ExpectedWSTranscript] = None, **kwargs):
         """
         Asserts that the at least one transcript recorded matches an expected transcript
         Args:
             expected: an expected transcript.
             **kwargs: if an expected request is not provided, then a new expected request is constructed by forwarding
              the keyword arguments to the constructor of ExpectedWSTranscript.
         """
         if expected and kwargs:
-            raise TypeError('method can be called with either expected or keyword args, but not both')
+            raise TypeError("method can be called with either expected or keyword args, but not both")
         if not expected:
             if not kwargs:
-                raise TypeError('either expected or keyword args must be provided')
+                raise TypeError("either expected or keyword args must be provided")
             expected = ExpectedWSTranscript(**kwargs)
 
         if not self:
-            raise AssertionError('No requests were made')
+            raise AssertionError("No requests were made")
         if any(expected.matches(req) for req in self):
             return
-        raise AssertionError('No transcripts match')
+        raise AssertionError("No transcripts match")
```

### Comparing `yellowbox-0.8.3/yellowbox/extras/websocket.py` & `yellowbox-0.8.4/yellowbox/extras/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,26 @@
     cached_property = property  # type: ignore
 
 import re
 import threading
 from functools import partial, wraps
 from threading import RLock
 from typing import (
-    Any, Callable, Dict, Generator, Iterable, Iterator, List, Optional, Pattern, TypeVar, Union, no_type_check
+    Any,
+    Callable,
+    Dict,
+    Generator,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Pattern,
+    TypeVar,
+    Union,
+    no_type_check,
 )
 from urllib.parse import urlparse
 from weakref import WeakMethod
 
 from simple_websocket_server import WebSocket, WebSocketServer
 
 from yellowbox.service import YellowService
@@ -30,14 +41,15 @@
 class _WebsocketTemplate(WebSocket):
     """Template websocket protocol.
 
     Used in WebSocketServer, this class handles incoming connections and
     communicates over a generator to send and receive data. See WebsocketService
     for usage.
     """
+
     _get_generator: Optional[WeakMethod] = None
     """
     A weakmethod to call WebsocketService._get_generator and find the
     generator appropriate for the connected websocket path.
     """
     _generator: "Optional[_GENERAOTR_TYPE]" = None
     """An initialized generator for IO with the websocket"""
@@ -58,32 +70,30 @@
 
             assert self._get_generator
             get_generator = self._get_generator()  # Resolve weakref
             assert get_generator
             generator_function = get_generator(path)
 
             if generator_function is None:
-                logger.info(f"No handler assigned to {path}. "
-                            "Closing connection.")
+                logger.info(f"No handler assigned to {path}. " "Closing connection.")
                 return
 
             self._generator = generator_function(self)
             initialized = True
         except Exception:
             logger.exception("Exception raised on generator start.")
             raise
 
         finally:
             if not initialized:
                 self.close()
 
         self._advance_generator(None)
 
-    def _advance_generator(
-            self, data: Union[bytearray, str, None]) -> None:
+    def _advance_generator(self, data: Union[bytearray, str, None]) -> None:
         """Advance the IO generator. Send it data and wait for output."""
         try:
             try:
                 # First one will send None, rest will send data.
                 msg = self._generator.send(data)  # type: ignore
             except StopIteration as exc:
                 if exc.value:  # type: ignore
@@ -120,66 +130,65 @@
             logger.exception("Exception raised on connection close.")
             raise
         finally:
             generator.close()  # May throw an exception. Ignore it.
 
 
 @no_type_check
-def _to_generator(
-        side_effect: SIDE_EFFECT_TYPE) -> _GEN_FUNCTION_TYPE:
+def _to_generator(side_effect: SIDE_EFFECT_TYPE) -> _GEN_FUNCTION_TYPE:
     """Convert a side effect to an IO generator function.
 
     Args:
         side_effect: See WebsocketService.route().
 
     Returns:
         Generator function, same as the one in WebsocketService.route().
     """
     # Side effect == normal string
     if isinstance(side_effect, (str, bytes, bytearray, memoryview)):
+
         def gen(*args: Any, **kwargs: Any) -> _GENERAOTR_TYPE:
             return side_effect
             yield  # On purpose.
+
         return gen
 
     # Side effect == list of strings
     if isinstance(side_effect, Iterable):
+
         def gen(*args, **kwargs) -> _GENERAOTR_TYPE:
             for item in side_effect:
                 yield item
+
         return gen
 
     assert callable(side_effect)
 
     @wraps(side_effect)  # type: ignore # Mypy GH-10002
     def gen(*args: Any, **kwargs: Any) -> _GENERAOTR_TYPE:
         # Side effect == normal function that returns a string.
         result = side_effect(*args, **kwargs)
-        if result is None or isinstance(result, (str, bytes,
-                                                 bytearray, memoryview)):
+        if result is None or isinstance(result, (str, bytes, bytearray, memoryview)):
             return result
 
         # Side effect == generator function
         return (yield from result)
 
     return gen
 
 
 # Type aliases used all around
 _YIELDTYPES = Union[str, bytes, bytearray, memoryview, None]
 
-_GENERAOTR_TYPE = Generator[_YIELDTYPES,
-                            Union[bytearray, str], _YIELDTYPES]
+_GENERAOTR_TYPE = Generator[_YIELDTYPES, Union[bytearray, str], _YIELDTYPES]
 
 _GEN_FUNCTION_TYPE = Callable[[WebSocket], _GENERAOTR_TYPE]
 
 SIDE_EFFECT_TYPE = Union[
-    _YIELDTYPES, List[_YIELDTYPES],
-    Callable[[WebSocket], Optional[_YIELDTYPES]],
-    _GEN_FUNCTION_TYPE
+    _YIELDTYPES, List[_YIELDTYPES], Callable[[WebSocket], Optional[_YIELDTYPES]], _GEN_FUNCTION_TYPE
 ]
 
 _T = TypeVar("_T")
 
 
 class WebsocketService(YellowService):
     """Yellobox service to handle incoming websocket connections.
@@ -208,14 +217,15 @@
 
         Keep in mind it's non-blocking. The service will run in the background.
 
         An local websocket should connect to `service.local_url` or
         `service.container_url` if communicating with a hosted docker
         container.
     """
+
     port: int
     """Server listening port."""
 
     def __init__(self) -> None:
         """Initialize the service."""
         self._routes: Dict[str, Callable] = {}
         self._re_routes: Dict[Pattern[str], Callable] = {}
@@ -239,25 +249,25 @@
     @cached_property
     def local_url(self) -> str:
         """Local URL for connecting on the same host.
 
         Suffix this with the path. For example, if you wish to connect locally
         to the "/echo" endpoint, connect to `service.local_url + '/echo'`.
         """
-        return f'ws://127.0.0.1:{self.port}'
+        return f"ws://127.0.0.1:{self.port}"
 
     @cached_property
     def container_url(self) -> str:
         """URL for connecting over a locally hosted docker container.
 
         Suffix this with the path. For example, if you wish to connect to the
         "/echo" endpoint from inside a container, connect
         to `service.container_url + '/echo'`.
         """
-        return f'ws://{docker_host_name}:{self.port}'
+        return f"ws://{docker_host_name}:{self.port}"
 
     def is_alive(self) -> bool:
         """Boolean stating if wesocket service is active."""
         return self._thread.is_alive()
 
     # Mypy doesn't support self generics yet without manual binding (bound=)
     # https://mypy.readthedocs.io/en/stable/generics.html#generic-methods-and-generic-self
@@ -298,17 +308,17 @@
         items = reversed(tuple(self._re_routes.items()))  # Thread safety
         for pattern, callback in items:
             if pattern.fullmatch(path):
                 return callback
 
         return None
 
-    def route(self, path: Optional[str] = None, *,
-              regex: Optional[Union[Pattern[str], str]] = None
-              ) -> Callable[[SIDE_EFFECT_TYPE], None]:
+    def route(
+        self, path: Optional[str] = None, *, regex: Optional[Union[Pattern[str], str]] = None
+    ) -> Callable[[SIDE_EFFECT_TYPE], None]:
         """Add a route using a decorator syntax.
 
         Raises an exception if the route already exists.
 
         Example:
 
             >>> @service.route("/echo")
@@ -330,18 +340,22 @@
             raise ValueError("Only one of path or regex can be specified.")
 
         if not (path or regex):
             raise ValueError("path or regex must be specified.")
 
         return partial(self.add, path=path, regex=regex)
 
-    def add(self, side_effect: SIDE_EFFECT_TYPE,
-            path: Optional[str] = None, *,
-            regex: Optional[Union[Pattern[str], str]] = None,
-            _overwrite: bool = False) -> None:
+    def add(
+        self,
+        side_effect: SIDE_EFFECT_TYPE,
+        path: Optional[str] = None,
+        *,
+        regex: Optional[Union[Pattern[str], str]] = None,
+        _overwrite: bool = False,
+    ) -> None:
         """Add a route.
 
         Raises an exception if the route already exists.
 
         Args:
             side_effect: Side effect can be either a string, bytes or bytearray
             to return a single message; iterable of any combination of them to
@@ -367,49 +381,54 @@
             # Prevent variable order confusion.
             raise TypeError("path must be a string.")
 
         gen = _to_generator(side_effect)
 
         # Check and place
         with self._lock:
-            if not _overwrite and (path in self._routes or
-                                   regex in self._re_routes):
+            if not _overwrite and (path in self._routes or regex in self._re_routes):
                 raise RuntimeError(f"Route {path or regex} already exists!")
 
             if path:
                 self._routes[path] = gen
             else:
                 self._re_routes[regex] = gen  # type: ignore
 
     @contextmanager
-    def patch(self, side_effect: SIDE_EFFECT_TYPE,
-              path: Optional[str] = None, *,
-              regex: Optional[Union[Pattern[str], str]] = None) -> Iterator[None]:
+    def patch(
+        self,
+        side_effect: SIDE_EFFECT_TYPE,
+        path: Optional[str] = None,
+        *,
+        regex: Optional[Union[Pattern[str], str]] = None,
+    ) -> Iterator[None]:
         """Temporarily patch a route.
 
         Like `.add()` but uses a context manager for easy removal.
         """
         self.add(side_effect, path, regex=regex)
         try:
             yield
         finally:
             self.remove(path, regex=regex)
 
-    def set(self, side_effect: SIDE_EFFECT_TYPE,
-            path: Optional[str] = None, *,
-            regex: Optional[Union[Pattern[str], str]] = None) -> None:
+    def set(
+        self,
+        side_effect: SIDE_EFFECT_TYPE,
+        path: Optional[str] = None,
+        *,
+        regex: Optional[Union[Pattern[str], str]] = None,
+    ) -> None:
         """Set a route.
 
         Like `add()` but overwrites existing routes.
         """
-        self.add(side_effect=side_effect, path=path,
-                 regex=regex, _overwrite=True)
+        self.add(side_effect=side_effect, path=path, regex=regex, _overwrite=True)
 
-    def remove(self, path: Optional[str] = None, *,
-               regex: Optional[Union[Pattern[str], str]] = None) -> None:
+    def remove(self, path: Optional[str] = None, *, regex: Optional[Union[Pattern[str], str]] = None) -> None:
         """Remove a route.
 
         Args:
             path: Path that was previously inserted. Omit if using regex.
             regex: Regex that was previously inserted. Omit if using path.
         """
         if path and regex:
```

### Comparing `yellowbox-0.8.3/yellowbox/image_build.py` & `yellowbox-0.8.4/yellowbox/image_build.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,83 @@
 import json
-import os
 import sys
 from contextlib import contextmanager
 from json import JSONDecodeError
 from typing import Optional, TextIO
 
 from docker import DockerClient
 from docker.errors import BuildError, DockerException, ImageNotFound
 
 from yellowbox.utils import _get_spinner
 
 
-class DockerfileParseException(BuildError):
+class DockerfileParseError(BuildError):
     pass
 
 
+DockerfileParseException = DockerfileParseError  # legacy alias
+
+
 @contextmanager
-def build_image(docker_client: DockerClient, image_name: str, remove_image: bool = True,
-                file: Optional[TextIO] = sys.stderr, spinner: bool = True, **kwargs):
+def build_image(
+    docker_client: DockerClient,
+    image_name: str,
+    remove_image: bool = True,
+    file: Optional[TextIO] = sys.stderr,
+    spinner: bool = True,
+    **kwargs,
+):
     """
     Create a docker image (similar to docker build command)
     At the end, deletes the image (using rmi command)
     Args:
         docker_client: DockerClient to be used to create the image
         image_name: Name of the image to be created. If no tag is provided, the tag "test" will be added.
         remove_image: boolean, whether or not to delete the image at the end, default as True
         file: a file-like object (stream); defaults to the current sys.stderr. if set to None, will disable printing
         spinner: boolean, whether or not to use spinner (default as True), note that this param is set to False in
         case `file` param is not None
     """
-    if file is None:
-        file = open(os.devnull, 'w')
-    else:
-        spinner = False  # spinner splits into multiple lines in case stream is being printed at the same time
+    spinner = spinner and file is None
+    # spinner splits into multiple lines in case stream is being printed at the same time
     if ":" in image_name:
         image_tag = image_name
     else:
-        image_tag = f'{image_name}:test'
+        image_tag = f"{image_name}:test"
     yaspin_spinner = _get_spinner(spinner)
-    with yaspin_spinner(f'Creating image {image_tag}...'):
-        kwargs = {'tag': image_tag, 'rm': True, 'forcerm': True, **kwargs}
+    with yaspin_spinner(f"Creating image {image_tag}..."):
+        kwargs = {"tag": image_tag, "rm": True, "forcerm": True, **kwargs}
         build_log = docker_client.api.build(**kwargs)
         for msg_b in build_log:
-            msgs = str(msg_b, 'utf-8').splitlines()
+            msgs = str(msg_b, "utf-8").splitlines()
             for msg in msgs:
                 try:
                     parse_msg = json.loads(msg)
-                except JSONDecodeError:
-                    raise DockerException('error at build logs')
-                s = parse_msg.get('stream')
-                if s:
-                    print(s, end='', flush=True, file=file)
+                except JSONDecodeError as e:
+                    raise DockerException("error at build logs") from e
+                s = parse_msg.get("stream")
+                if s and file:
+                    print(s, end="", flush=True, file=file)
                 else:
                     # runtime errors
-                    error_detail = parse_msg.get('errorDetail')
+                    error_detail = parse_msg.get("errorDetail")
                     # parse errors
-                    error_msg = parse_msg.get('message')
+                    error_msg = parse_msg.get("message")
                     # steps of the image creation
-                    status = parse_msg.get('status')
+                    status = parse_msg.get("status")
                     # end of process, will contain the ID of the temporary container created at the end
-                    aux = parse_msg.get('aux')
+                    aux = parse_msg.get("aux")
                     if error_detail is not None:
                         raise BuildError(reason=error_detail, build_log=None)
                     elif error_msg is not None:
-                        raise DockerfileParseException(reason=error_msg, build_log=None)
-                    elif status is not None:
-                        print(status, end='', flush=True, file=file)
-                    elif aux is not None:
-                        print(aux, end='', flush=True, file=file)
+                        raise DockerfileParseError(reason=error_msg, build_log=None)
+                    elif status is not None and file:
+                        print(status, end="", flush=True, file=file)
+                    elif aux is not None and file:
+                        print(aux, end="", flush=True, file=file)
                     else:
                         raise DockerException(parse_msg)
         yield image_tag
         if remove_image:
             try:
                 docker_client.api.remove_image(image_tag)
             except ImageNotFound:
```

### Comparing `yellowbox-0.8.3/yellowbox/networks.py` & `yellowbox-0.8.4/yellowbox/networks.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from docker import DockerClient
 from docker.models.containers import Container
 from docker.models.networks import Network
 
 from yellowbox.containers import get_aliases, is_removed
 from yellowbox.subclasses import ContainerService
 
-__all__ = ['temp_network', 'anonymous_network', 'connect', 'disconnecting']
+__all__ = ["temp_network", "anonymous_network", "connect", "disconnecting"]
 
 _T = TypeVar("_T")
 _NT = TypeVar("_NT", bound=Network)
 
 
 def anonymous_network(client: DockerClient, *args, **kwargs) -> Network:
     name = f"yellowbox-{uuid1()}"
```

### Comparing `yellowbox-0.8.3/yellowbox/retry.py` & `yellowbox-0.8.4/yellowbox/retry.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import asyncio
 from dataclasses import dataclass
 from itertools import count
 from time import perf_counter, sleep
 from typing import Callable, Iterable, Optional, Tuple, Type, TypeVar, Union
 
-_T = TypeVar('_T')
+_T = TypeVar("_T")
 
 
 @dataclass
 class RetrySpec:
     """
     Specifications for a repeated attempts af an arbitrary action that might fail.
     """
@@ -26,18 +26,17 @@
     timeout: Optional[float] = None
     """
     A timeout for all the attempts (including the interval) combined.
     """
 
     def __post_init__(self):
         if self.attempts is self.timeout is None:
-            raise ValueError('RetrySpec must have either a timeout or attempts')
+            raise ValueError("RetrySpec must have either a timeout or attempts")
 
-    def retry(self, func: Callable[[], _T],
-              exceptions: Union[Type[Exception], Tuple[Type[Exception], ...]]) -> _T:
+    def retry(self, func: Callable[[], _T], exceptions: Union[Type[Exception], Tuple[Type[Exception], ...]]) -> _T:
         """
         Retry running func until it succeeds
 
         Args:
             func: Function to run without arguments.
             exceptions: Single or iterable of exception types to catch. Exceptions raised by `func` not residing
             inside this iterable will be propagated.
@@ -57,27 +56,28 @@
             raise ValueError("Attempts must be greater than zero.")
         else:
             attempt_iterator = range(self.attempts - 1)
 
         if self.timeout:
             time_limit = perf_counter() + self.timeout
         else:
-            time_limit = float('inf')
+            time_limit = float("inf")
 
         for _ in attempt_iterator:
             try:
                 return func()
             except exceptions:
                 if perf_counter() > time_limit:
                     raise
             sleep(self.interval)
         return func()
 
-    async def aretry(self, func: Callable[[], _T],
-                     exceptions: Union[Type[Exception], Tuple[Type[Exception], ...]]) -> _T:
+    async def aretry(
+        self, func: Callable[[], _T], exceptions: Union[Type[Exception], Tuple[Type[Exception], ...]]
+    ) -> _T:
         """
         Retry running func until it succeeds
 
         Args:
             func: Function to run without arguments.
             exceptions: Single or iterable of exception types to catch. Exceptions raised by `func` not residing
             inside this iterable will be propagated.
@@ -97,15 +97,15 @@
             raise ValueError("Attempts must be greater than zero.")
         else:
             attempt_iterator = range(self.attempts - 1)
 
         if self.timeout:
             time_limit = perf_counter() + self.timeout
         else:
-            time_limit = float('inf')
+            time_limit = float("inf")
 
         for _ in attempt_iterator:
             try:
                 return func()
             except exceptions:
                 if perf_counter() > time_limit:
                     raise
```

### Comparing `yellowbox-0.8.3/yellowbox/service.py` & `yellowbox-0.8.4/yellowbox/service.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.3/yellowbox/subclasses.py` & `yellowbox-0.8.4/yellowbox/subclasses.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
+from asyncio import get_running_loop
 from contextlib import asynccontextmanager, contextmanager, nullcontext
+from functools import partial
 from typing import AsyncIterator, ContextManager, Iterator, Optional, Sequence, Type, TypeVar
 
 from docker import DockerClient
 from docker.models.containers import Container
 from docker.models.networks import Network
 
 import yellowbox.networks as networks_mod
@@ -35,21 +39,21 @@
             self, for usage as a context manager.
 
         Notes:
             This method should block until the service is fully operational.
 
         """
         for c in self.containers:
-            if c.status.lower() == 'started':
+            if c.status.lower() == "started":
                 continue
             c.start()
             c.reload()
         return super(ContainerService, self).start()
 
-    def stop(self, signal='SIGTERM'):
+    def stop(self, signal="SIGTERM"):
         for c in reversed(self.containers):
             if not is_alive(c):
                 continue
             c.kill(signal)
             c.wait(timeout=_DEFAULT_TIMEOUT)
             c.reload()
             if self.remove:
@@ -86,15 +90,15 @@
     @property
     @abstractmethod
     def _single_endpoint(self) -> Container:
         pass
 
     @property
     def _endpoint_containers(self) -> Sequence[Container]:
-        return self._single_endpoint,
+        return (self._single_endpoint,)
 
     def connect(self, network: Network, **kwargs) -> Sequence[str]:
         network.connect(self._single_endpoint, **kwargs)
         self._single_endpoint.reload()
         return get_aliases(self._single_endpoint, network)
 
     def disconnect(self, network: Network, **kwargs):
@@ -112,92 +116,119 @@
         return self.containers[0]
 
     @property
     def _single_endpoint(self) -> Container:
         return self.container
 
 
-_T = TypeVar("_T", bound=ContainerService)
+SelfRunMixin = TypeVar("SelfRunMixin", bound="RunMixin")
 
 
-class RunMixin:
+class RunMixin(ContainerService, ABC):
     @classmethod
     def service_name(cls):
         return cls.__name__
 
     @classmethod
     @contextmanager
-    def run(cls: Type[_T], docker_client: DockerClient, *, spinner: bool = True,  # type: ignore
-            retry_spec: Optional[RetrySpec] = None,
-            network: Optional[Network] = None, **kwargs) -> Iterator[_T]:
+    def run(
+        cls: Type[SelfRunMixin],
+        docker_client: DockerClient,
+        *,
+        spinner: bool = True,
+        retry_spec: Optional[RetrySpec] = None,
+        network: Optional[Network] = None,
+        **kwargs,
+    ) -> Iterator[SelfRunMixin]:
         """
         Args:
             docker_client: a DockerClient instance to use when creating the service
             spinner: whether or not to use a yaspin spinner
             retry_spec: forwarded to cls.start
             network: connect service to network
             **kwargs: all keyword arguments are forwarded to the class's constructor
         """
         yaspin_spinner = _get_spinner(spinner)
-        with yaspin_spinner(f"Fetching {cls.service_name()} ..."):  # type: ignore[attr-defined]
+        with yaspin_spinner(f"Fetching {cls.service_name()} ..."):
             service = cls(docker_client, **kwargs)
 
         connect_network: ContextManager[None]
         if network:
             connect_network = networks_mod.connect(network, service)
         else:
             connect_network = nullcontext()
 
         with connect_network:
-            with yaspin_spinner(f"Waiting for {cls.service_name()} to start..."):  # type: ignore[attr-defined]
+            with yaspin_spinner(f"Waiting for {cls.service_name()} to start..."):
                 service.start(retry_spec=retry_spec)
             with service:
                 yield service
 
 
-class AsyncRunMixin(ABC):
+SelfARunMixin = TypeVar("SelfARunMixin", bound="AsyncRunMixin")
+
+
+class AsyncRunMixin(ContainerService, ABC):
     @classmethod
     def service_name(cls):
         return cls.__name__
 
     @abstractmethod
-    async def astart(self: _T, retry_spec: Optional[RetrySpec] = None) -> None:   # type: ignore[misc]
+    async def astart(self, retry_spec: Optional[RetrySpec] = None) -> None:
         """
         Start the service synchronously, but block and wait for startup asynchronously.
         """
-        pass
+
+    async def astop(self, *args, **kwargs) -> None:
+        """
+        Stop the service synchronously, but block and wait for shutdown asynchronously.
+        """
+        loop = get_running_loop()
+        func = partial(self.stop, *args, **kwargs)
+        await loop.run_in_executor(None, func)
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, *args):
+        await self.astop()
 
     @classmethod
     @asynccontextmanager
-    async def arun(cls: Type[_T], docker_client: DockerClient, *, verbose: bool = True,  # type: ignore[misc]
-                   retry_spec: Optional[RetrySpec] = None,
-                   network: Optional[Network] = None, **kwargs) -> AsyncIterator[_T]:
+    async def arun(
+        cls: Type[SelfARunMixin],
+        docker_client: DockerClient,
+        *,
+        verbose: bool = True,
+        retry_spec: Optional[RetrySpec] = None,
+        network: Optional[Network] = None,
+        **kwargs,
+    ) -> AsyncIterator[SelfARunMixin]:
         """
         Same as RunMixin.run, but waits for startup asynchronously.
 
         Args:
             docker_client: a DockerClient instance to use when creating the service
             verbose: whether or not to print progress information when setting up the service
             retry_spec: forwarded to cls.start
             network: connect service to network
             **kwargs: all keyword arguments are forwarded to the class's constructor
         """
 
         yaspin_spinner = _get_spinner(verbose)
-        with yaspin_spinner(f"Fetching {cls.service_name()} ..."):  # type: ignore[attr-defined]
+        with yaspin_spinner(f"Fetching {cls.service_name()} ..."):
             service = cls(docker_client, **kwargs)
 
         connect_network: ContextManager[None]
         if network:
             connect_network = networks_mod.connect(network, service)
         else:
             connect_network = nullcontext()
 
         with connect_network:
             if verbose:
-                print(f".   Waiting for {cls.service_name()} to start...")    # type: ignore[attr-defined]
-            await service.astart(retry_spec=retry_spec)    # type: ignore[attr-defined]
+                print(f".   Waiting for {cls.service_name()} to start...")
+            await service.astart(retry_spec=retry_spec)
             if verbose:
-                print(f"{_SPINNER_SUCCESSMSG} "    # type: ignore[attr-defined]
-                      f"{cls.service_name()} started successfully")    # type: ignore[attr-defined]
-            with service:
+                print(f"{_SPINNER_SUCCESSMSG} {cls.service_name()} started successfully")
+            async with service:
                 yield service
```

### Comparing `yellowbox-0.8.3/yellowbox/utils.py` & `yellowbox-0.8.4/yellowbox/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import platform
 from contextlib import AbstractContextManager, closing, contextmanager, nullcontext
 from socket import AF_INET, SO_REUSEADDR, SOCK_STREAM, SOL_SOCKET, socket
 from typing import Callable, Optional, TypeVar
 
 from yaspin import yaspin
 
-_T = TypeVar('_T')
+_T = TypeVar("_T")
 _SPINNER_FAILMSG = "💥 "
 _SPINNER_SUCCESSMSG = "✅ "
 
 
 @contextmanager
 def _spinner(text):
     with yaspin(text=text) as spinner:
@@ -26,25 +26,25 @@
     if not real:
         return lambda text: nullcontext()
     return _spinner
 
 
 def get_free_port():
     with closing(socket(AF_INET, SOCK_STREAM)) as s:
-        s.bind(('', 0))
+        s.bind(("", 0))
         s.setsockopt(SOL_SOCKET, SO_REUSEADDR, 1)
         return s.getsockname()[1]
 
 
 uname = platform.uname().release.lower()
 
-if platform.system() == "Linux" and ('microsoft' not in uname):  # catch WSL
-    docker_host_name = '172.17.0.1'
+if platform.system() == "Linux" and ("microsoft" not in uname):  # catch WSL
+    docker_host_name = "172.17.0.1"
 else:
-    docker_host_name = 'host.docker.internal'
+    docker_host_name = "host.docker.internal"
 
 # if we expose a port in docker, this is where we expect to find it hosted
 # this is almost always just localhost
 # you can set the value here to some value with the YELLOWBOX_DOCKER_EXPOSE_HOST env-var
 # DO NOT manually change this const, instead call update_docker_expose_host
 DOCKER_EXPOSE_HOST = ""
 
@@ -57,15 +57,15 @@
         value: if provided, will use this value instead of inferring a host
 
     Notes:
         This function is called once when yellowbox is imported with a value of the env var
         YELLOWBOX_DOCKER_EXPOSE_HOST
 
     """
-    global DOCKER_EXPOSE_HOST
+    global DOCKER_EXPOSE_HOST  # noqa: PLW0603
 
     if value is None:
         value = "127.0.0.1"
 
     DOCKER_EXPOSE_HOST = value
```

### Comparing `yellowbox-0.8.3/PKG-INFO` & `yellowbox-0.8.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowbox
-Version: 0.8.3
+Version: 0.8.4
 Summary: 
 Home-page: https://github.com/biocatchltd/yellowbox
 License: MIT
 Author: biocatch ltd
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

