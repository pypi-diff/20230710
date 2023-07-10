# Comparing `tmp/wizproxy-0.3.0.tar.gz` & `tmp/wizproxy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizproxy-0.3.0.tar", max compression
+gzip compressed data, was "wizproxy-0.4.0.tar", max compression
```

## Comparing `wizproxy-0.3.0.tar` & `wizproxy-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      747 2023-06-24 18:52:44.129272 wizproxy-0.3.0/LICENSE
--rw-r--r--   0        0        0     4341 2023-07-09 00:54:38.019365 wizproxy-0.3.0/README.md
--rw-r--r--   0        0        0      564 2023-07-09 01:03:28.499986 wizproxy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-24 17:55:10.532607 wizproxy-0.3.0/wizproxy/__init__.py
--rw-r--r--   0        0        0     2102 2023-07-09 01:02:56.982040 wizproxy-0.3.0/wizproxy/__main__.py
--rw-r--r--   0        0        0     3510 2023-07-07 22:10:54.046310 wizproxy-0.3.0/wizproxy/aes.py
--rw-r--r--   0        0        0     2238 2023-07-08 21:38:01.265737 wizproxy-0.3.0/wizproxy/key_chain.py
--rw-r--r--   0        0        0      186 2023-07-08 20:52:07.212214 wizproxy-0.3.0/wizproxy/plugin/__init__.py
--rw-r--r--   0        0        0     3260 2023-07-08 19:14:33.867973 wizproxy-0.3.0/wizproxy/plugin/builtin.py
--rw-r--r--   0        0        0     1364 2023-07-08 17:35:40.141339 wizproxy-0.3.0/wizproxy/plugin/filter.py
--rw-r--r--   0        0        0     3746 2023-07-08 18:58:23.042352 wizproxy-0.3.0/wizproxy/plugin/interface.py
--rw-r--r--   0        0        0      432 2023-07-08 20:51:54.963279 wizproxy-0.3.0/wizproxy/plugin/log.py
--rw-r--r--   0        0        0     1797 2023-07-09 00:39:09.063077 wizproxy-0.3.0/wizproxy/plugin/scapy.py
--rw-r--r--   0        0        0      226 2023-07-08 15:33:47.151413 wizproxy-0.3.0/wizproxy/proto/__init__.py
--rw-r--r--   0        0        0     2475 2023-07-07 22:10:54.053311 wizproxy-0.3.0/wizproxy/proto/bytes.py
--rw-r--r--   0        0        0     1298 2023-07-07 22:10:54.053311 wizproxy-0.3.0/wizproxy/proto/dml.py
--rw-r--r--   0        0        0     1979 2023-07-08 17:28:54.299160 wizproxy-0.3.0/wizproxy/proto/frame.py
--rw-r--r--   0        0        0     2117 2023-07-07 22:10:54.059311 wizproxy-0.3.0/wizproxy/proto/handshake.py
--rw-r--r--   0        0        0     1807 2023-07-08 19:18:39.599952 wizproxy-0.3.0/wizproxy/proxy.py
--rw-r--r--   0        0        0     4019 2023-07-08 17:14:20.768084 wizproxy-0.3.0/wizproxy/session.py
--rw-r--r--   0        0        0     5042 2023-07-08 23:16:29.087736 wizproxy-0.3.0/wizproxy/shard.py
--rw-r--r--   0        0        0     4956 2023-07-07 22:10:54.060311 wizproxy-0.3.0/wizproxy/stream.py
--rw-r--r--   0        0        0     4893 1970-01-01 00:00:00.000000 wizproxy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      747 2023-06-24 18:52:44.129272 wizproxy-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4649 2023-07-10 20:21:23.444091 wizproxy-0.4.0/README.md
+-rw-r--r--   0        0        0      564 2023-07-10 20:22:09.337409 wizproxy-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-24 17:55:10.532607 wizproxy-0.4.0/wizproxy/__init__.py
+-rw-r--r--   0        0        0     2554 2023-07-10 12:44:36.771515 wizproxy-0.4.0/wizproxy/__main__.py
+-rw-r--r--   0        0        0     3510 2023-07-09 20:05:55.402319 wizproxy-0.4.0/wizproxy/aes.py
+-rw-r--r--   0        0        0     2238 2023-07-08 21:38:01.265737 wizproxy-0.4.0/wizproxy/key_chain.py
+-rw-r--r--   0        0        0      186 2023-07-08 20:52:07.212214 wizproxy-0.4.0/wizproxy/plugin/__init__.py
+-rw-r--r--   0        0        0     3422 2023-07-10 19:55:03.579090 wizproxy-0.4.0/wizproxy/plugin/builtin.py
+-rw-r--r--   0        0        0     1364 2023-07-08 17:35:40.141339 wizproxy-0.4.0/wizproxy/plugin/filter.py
+-rw-r--r--   0        0        0     3746 2023-07-08 18:58:23.042352 wizproxy-0.4.0/wizproxy/plugin/interface.py
+-rw-r--r--   0        0        0      432 2023-07-08 20:51:54.963279 wizproxy-0.4.0/wizproxy/plugin/log.py
+-rw-r--r--   0        0        0     2129 2023-07-09 21:18:01.787007 wizproxy-0.4.0/wizproxy/plugin/scapy.py
+-rw-r--r--   0        0        0      226 2023-07-08 15:33:47.151413 wizproxy-0.4.0/wizproxy/proto/__init__.py
+-rw-r--r--   0        0        0     2475 2023-07-07 22:10:54.053311 wizproxy-0.4.0/wizproxy/proto/bytes.py
+-rw-r--r--   0        0        0     1298 2023-07-07 22:10:54.053311 wizproxy-0.4.0/wizproxy/proto/dml.py
+-rw-r--r--   0        0        0     1979 2023-07-08 17:28:54.299160 wizproxy-0.4.0/wizproxy/proto/frame.py
+-rw-r--r--   0        0        0     2117 2023-07-07 22:10:54.059311 wizproxy-0.4.0/wizproxy/proto/handshake.py
+-rw-r--r--   0        0        0     1807 2023-07-08 19:18:39.599952 wizproxy-0.4.0/wizproxy/proxy.py
+-rw-r--r--   0        0        0     4019 2023-07-10 20:05:51.461947 wizproxy-0.4.0/wizproxy/session.py
+-rw-r--r--   0        0        0     5042 2023-07-08 23:16:29.087736 wizproxy-0.4.0/wizproxy/shard.py
+-rw-r--r--   0        0        0     4956 2023-07-07 22:10:54.060311 wizproxy-0.4.0/wizproxy/stream.py
+-rw-r--r--   0        0        0     5201 1970-01-01 00:00:00.000000 wizproxy-0.4.0/PKG-INFO
```

### Comparing `wizproxy-0.3.0/LICENSE` & `wizproxy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wizproxy-0.3.0/README.md` & `wizproxy-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # wizproxy
 
 A packet proxy for exfiltrating and manipulating encrypted Wizard101
 network traffic.
 
+## Disclaimer
+
+**Using this software bears a risk of getting your account banned. At the time of writing, it works with EU servers but that may change in the future.**
+
+When in doubt, always use a burner account first to fish for a ban.
+
 ## How it works
 
 wizproxy sits between a client and a server, receiving and forwarding
 all traffic from both parties to each other.
 
 Initially, client and server establish a session by confirming they
 use the same RSA key pair and making the client generate a symmetric
@@ -98,14 +104,16 @@
 
 > Client X crashed: Invalid signature
 
 This means your client is out of date. Open the patch client and let it run
 to completion, then follow the above setup steps again to inject a custom
 key ring into the updated binary.
 
+If that still doesn't resolve it, the client version is unsupported.
+
 > Is injection supported?
 
 Yes and no.
 
 Injection as in arbitrarily injecting any amount of packets at any given time
 is not supported and, for many use cases where this would be considered, can
 get your account banned.
```

### Comparing `wizproxy-0.3.0/pyproject.toml` & `wizproxy-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wizproxy"
-version = "0.3.0"
+version = "0.4.0"
 description = "A proxy for handling encrypted Wizard101 traffic"
 authors = ["Valentin B. <valentin.be@protonmail.com>"]
 license = "ISC"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `wizproxy-0.3.0/wizproxy/__main__.py` & `wizproxy-0.4.0/wizproxy/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import argparse
 import json
+import platform
+import socket
 from pathlib import Path
 
 import trio
 from loguru import logger
 
 from .key_chain import KeyChain
 from .plugin import ScapyPlugin, VerboseLog
@@ -13,14 +15,24 @@
 
 async def main(args):
     key_chain = KeyChain(
         json.loads((args.keys / "ki_keys.json").read_text()),
         json.loads((args.keys / "injected_keys.json").read_text()),
     )
 
+    if args.host is None and platform.system() == "Windows":
+        # Windows default wildcard interface behaves funky and
+        # "0.0.0.0" causes trouble when the game client attempts
+        # to connect to the proxy.
+        #
+        # This is not an issue under Wine (Linux and macOS), so
+        # we want to use the proper local interface as a default
+        # on Windows.
+        args.host = socket.gethostbyname(socket.gethostname())
+
     async with trio.open_nursery() as nursery:
         proxy = Proxy(args.host, key_chain, nursery)
 
         # If requested, enable the scapy plugin.
         if args.capture:
             scapy = ScapyPlugin.from_file(args.capture)
 
@@ -46,15 +58,14 @@
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "keys", type=Path, help="The directory with the two key JSON files"
     )
     parser.add_argument(
         "--host",
         type=str,
-        default="0.0.0.0",
         help="The host interface to bind shard sockets to",
     )
     parser.add_argument(
         "-l",
         "--login",
         type=str,
         default="login.us.wizard101.com",
```

### Comparing `wizproxy-0.3.0/wizproxy/aes.py` & `wizproxy-0.4.0/wizproxy/aes.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.3.0/wizproxy/key_chain.py` & `wizproxy-0.4.0/wizproxy/key_chain.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.3.0/wizproxy/plugin/builtin.py` & `wizproxy-0.4.0/wizproxy/plugin/builtin.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,21 @@
     async def patch_session_accept(self, ctx: Context, frame: Frame):
         frame.payload = ctx.session.session_accept(frame.payload)
 
     @listen(Direction.SERVER_TO_CLIENT, service_id=7, order=3)
     async def redirect_character_selected(self, ctx: Context, frame: Frame):
         msg = MSG_CHARACTERSELECTED.decode(frame.payload)
 
+        # Extract the server that should be proxied and check validity.
+        socket = SocketAddress(msg["IP"], msg["TCPPort"])
+        if not socket.ip and not socket.port:
+            return
+
         # Spawn a new shard to proxy the new server connection.
-        local = await ctx.spawn_shard(SocketAddress(msg["IP"], msg["TCPPort"]))
+        local = await ctx.spawn_shard(socket)
 
         # Fix up the client packet to make it connect to the shard.
         msg["IP"] = local.ip.encode()
         msg["TCPPort"] = local.port
 
         frame.payload = MSG_CHARACTERSELECTED.encode(msg)
```

### Comparing `wizproxy-0.3.0/wizproxy/plugin/filter.py` & `wizproxy-0.4.0/wizproxy/plugin/filter.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.3.0/wizproxy/plugin/interface.py` & `wizproxy-0.4.0/wizproxy/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.3.0/wizproxy/plugin/scapy.py` & `wizproxy-0.4.0/wizproxy/plugin/scapy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+import logging
+from datetime import datetime
 from pathlib import Path
 
+# Silence overly verbose scapy logging except for errors.
+logging.getLogger("scapy.runtime").setLevel(logging.ERROR)
+
 import trio
-from scapy.layers.inet import Ether, IP, TCP
+from scapy.layers.inet import IP, TCP, Ether
 from scapy.utils import PcapNgWriter
 
 from ..proto import Bytes, Frame, SocketAddress
 from . import Context, Direction, Plugin, listen
 
 
 class ScapyPlugin(Plugin):
@@ -22,29 +27,35 @@
     def __init__(self, writer: PcapNgWriter):
         super().__init__()
 
         self.writer = writer
 
     @classmethod
     def from_file(cls, path: Path):
+        if path.is_dir():
+            now = datetime.now()
+            path = path / now.strftime("wizproxy_%Y-%m-%d_%H-%M-%S.pcapng")
+
         writer = PcapNgWriter(str(path.resolve()))
         return cls(writer)
 
     async def write_to_file(
         self, ctx: Context, source: SocketAddress, dest: SocketAddress, raw: bytes
     ):
         shard = ctx.shard()
 
         packet = (
             Ether()
             / IP(src=source.ip, dst=dest.ip)
             / TCP(sport=source.port, dport=dest.port)
             / raw
         )
-        packet.comment = f"Shard {shard.ip}:{shard.port}, client {ctx.session.sid}"
+        packet.comment = (
+            f"Shard {shard.ip}:{shard.port}, client {ctx.session.sid}".encode()
+        )
 
         await trio.to_thread.run_sync(self.writer.write, packet)
 
     @listen(Direction.CLIENT_TO_SERVER)
     async def clientbound(self, ctx: Context, frame: Frame):
         bytes = Bytes()
         frame.write(bytes)
```

### Comparing `wizproxy-0.3.0/wizproxy/proto/bytes.py` & `wizproxy-0.4.0/wizproxy/proto/bytes.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.3.0/wizproxy/proto/dml.py` & `wizproxy-0.4.0/wizproxy/proto/dml.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.3.0/wizproxy/proto/frame.py` & `wizproxy-0.4.0/wizproxy/proto/frame.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.3.0/wizproxy/proto/handshake.py` & `wizproxy-0.4.0/wizproxy/proto/handshake.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.3.0/wizproxy/proxy.py` & `wizproxy-0.4.0/wizproxy/proxy.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.3.0/wizproxy/session.py` & `wizproxy-0.4.0/wizproxy/session.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.3.0/wizproxy/shard.py` & `wizproxy-0.4.0/wizproxy/shard.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.3.0/wizproxy/stream.py` & `wizproxy-0.4.0/wizproxy/stream.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.3.0/PKG-INFO` & `wizproxy-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizproxy
-Version: 0.3.0
+Version: 0.4.0
 Summary: A proxy for handling encrypted Wizard101 traffic
 License: ISC
 Author: Valentin B.
 Author-email: valentin.be@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,20 @@
 Description-Content-Type: text/markdown
 
 # wizproxy
 
 A packet proxy for exfiltrating and manipulating encrypted Wizard101
 network traffic.
 
+## Disclaimer
+
+**Using this software bears a risk of getting your account banned. At the time of writing, it works with EU servers but that may change in the future.**
+
+When in doubt, always use a burner account first to fish for a ban.
+
 ## How it works
 
 wizproxy sits between a client and a server, receiving and forwarding
 all traffic from both parties to each other.
 
 Initially, client and server establish a session by confirming they
 use the same RSA key pair and making the client generate a symmetric
@@ -115,14 +121,16 @@
 
 > Client X crashed: Invalid signature
 
 This means your client is out of date. Open the patch client and let it run
 to completion, then follow the above setup steps again to inject a custom
 key ring into the updated binary.
 
+If that still doesn't resolve it, the client version is unsupported.
+
 > Is injection supported?
 
 Yes and no.
 
 Injection as in arbitrarily injecting any amount of packets at any given time
 is not supported and, for many use cases where this would be considered, can
 get your account banned.
```

