# Comparing `tmp/WaveLinkCord-2.5.1.tar.gz` & `tmp/WavelinkCord-2.5.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WaveLinkCord-2.5.1.tar", last modified: Mon Jul 10 10:01:14 2023, max compression
+gzip compressed data, was "WavelinkCord-2.5.2b0.tar", last modified: Sun Jun 18 13:22:59 2023, max compression
```

## Comparing `WaveLinkCord-2.5.1.tar` & `WavelinkCord-2.5.2b0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 10:01:14.434559 WaveLinkCord-2.5.1/
--rw-rw-rw-   0        0        0     1088 2023-07-10 09:39:49.000000 WaveLinkCord-2.5.1/LICENSE
--rw-rw-rw-   0        0        0     5875 2023-07-10 10:01:14.433560 WaveLinkCord-2.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4918 2023-07-10 09:39:49.000000 WaveLinkCord-2.5.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-10 10:01:14.402553 WaveLinkCord-2.5.1/WaveLinkCord.egg-info/
--rw-rw-rw-   0        0        0     5875 2023-07-10 10:01:14.000000 WaveLinkCord-2.5.1/WaveLinkCord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      643 2023-07-10 10:01:14.000000 WaveLinkCord-2.5.1/WaveLinkCord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 10:01:14.000000 WaveLinkCord-2.5.1/WaveLinkCord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-07-10 10:01:14.000000 WaveLinkCord-2.5.1/WaveLinkCord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-10 10:01:14.000000 WaveLinkCord-2.5.1/WaveLinkCord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      982 2023-07-10 09:44:27.000000 WaveLinkCord-2.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       29 2023-07-10 09:44:34.000000 WaveLinkCord-2.5.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 10:01:14.434559 WaveLinkCord-2.5.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-10 10:01:14.422558 WaveLinkCord-2.5.1/wavelinkcord/
--rw-rw-rw-   0        0        0     1448 2023-07-10 09:45:00.000000 WaveLinkCord-2.5.1/wavelinkcord/__init__.py
--rw-rw-rw-   0        0        0     2630 2023-07-10 09:39:50.000000 WaveLinkCord-2.5.1/wavelinkcord/backoff.py
--rw-rw-rw-   0        0        0     3539 2023-07-10 09:45:12.000000 WaveLinkCord-2.5.1/wavelinkcord/enums.py
--rw-rw-rw-   0        0        0     2936 2023-07-10 09:45:11.000000 WaveLinkCord-2.5.1/wavelinkcord/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-10 10:01:14.355542 WaveLinkCord-2.5.1/wavelinkcord/ext/
-drwxrwxrwx   0        0        0        0 2023-07-10 10:01:14.424558 WaveLinkCord-2.5.1/wavelinkcord/ext/spotify/
--rw-rw-rw-   0        0        0    17347 2023-07-10 09:45:07.000000 WaveLinkCord-2.5.1/wavelinkcord/ext/spotify/__init__.py
--rw-rw-rw-   0        0        0    19670 2023-07-10 09:45:11.000000 WaveLinkCord-2.5.1/wavelinkcord/filters.py
--rw-rw-rw-   0        0        0    17340 2023-07-10 09:45:13.000000 WaveLinkCord-2.5.1/wavelinkcord/node.py
--rw-rw-rw-   0        0        0     3385 2023-07-10 09:45:13.000000 WaveLinkCord-2.5.1/wavelinkcord/payloads.py
--rw-rw-rw-   0        0        0    21430 2023-07-10 09:45:14.000000 WaveLinkCord-2.5.1/wavelinkcord/player.py
--rw-rw-rw-   0        0        0    12158 2023-07-10 09:45:15.000000 WaveLinkCord-2.5.1/wavelinkcord/queue.py
--rw-rw-rw-   0        0        0     9652 2023-07-10 09:45:15.000000 WaveLinkCord-2.5.1/wavelinkcord/tracks.py
-drwxrwxrwx   0        0        0        0 2023-07-10 10:01:14.431558 WaveLinkCord-2.5.1/wavelinkcord/types/
--rw-rw-rw-   0        0        0      825 2023-07-10 09:39:50.000000 WaveLinkCord-2.5.1/wavelinkcord/types/events.py
--rw-rw-rw-   0        0        0      602 2023-07-10 09:39:50.000000 WaveLinkCord-2.5.1/wavelinkcord/types/request.py
--rw-rw-rw-   0        0        0      409 2023-07-10 09:45:10.000000 WaveLinkCord-2.5.1/wavelinkcord/types/state.py
--rw-rw-rw-   0        0        0      325 2023-07-10 09:39:50.000000 WaveLinkCord-2.5.1/wavelinkcord/types/track.py
--rw-rw-rw-   0        0        0     9339 2023-07-10 09:45:16.000000 WaveLinkCord-2.5.1/wavelinkcord/websocket.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:22:59.579206 WavelinkCord-2.5.2b0/
+-rw-rw-rw-   0        0        0     1108 2023-06-18 12:59:01.000000 WavelinkCord-2.5.2b0/LICENSE
+-rw-rw-rw-   0        0        0     5873 2023-06-18 13:22:59.576205 WavelinkCord-2.5.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0     5064 2023-06-18 12:59:01.000000 WavelinkCord-2.5.2b0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-18 13:22:59.447175 WavelinkCord-2.5.2b0/WavelinkCord.egg-info/
+-rw-rw-rw-   0        0        0     5873 2023-06-18 13:22:59.000000 WavelinkCord-2.5.2b0/WavelinkCord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      579 2023-06-18 13:22:59.000000 WavelinkCord-2.5.2b0/WavelinkCord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 13:22:59.000000 WavelinkCord-2.5.2b0/WavelinkCord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-18 13:22:59.000000 WavelinkCord-2.5.2b0/WavelinkCord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-18 13:22:59.000000 WavelinkCord-2.5.2b0/WavelinkCord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1011 2023-06-18 13:00:25.000000 WavelinkCord-2.5.2b0/pyproject.toml
+-rw-rw-rw-   0        0        0       30 2023-06-18 13:00:12.000000 WavelinkCord-2.5.2b0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 13:22:59.580206 WavelinkCord-2.5.2b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 13:22:59.540197 WavelinkCord-2.5.2b0/wavelink/
+-rw-rw-rw-   0        0        0     1463 2023-06-18 12:57:31.000000 WavelinkCord-2.5.2b0/wavelink/__init__.py
+-rw-rw-rw-   0        0        0     2630 2023-06-18 12:18:36.000000 WavelinkCord-2.5.2b0/wavelink/backoff.py
+-rw-rw-rw-   0        0        0     3539 2023-06-18 12:23:34.000000 WavelinkCord-2.5.2b0/wavelink/enums.py
+-rw-rw-rw-   0        0        0     2936 2023-06-18 12:23:33.000000 WavelinkCord-2.5.2b0/wavelink/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:22:59.366157 WavelinkCord-2.5.2b0/wavelink/ext/
+drwxrwxrwx   0        0        0        0 2023-06-18 13:22:59.545199 WavelinkCord-2.5.2b0/wavelink/ext/spotify/
+-rw-rw-rw-   0        0        0    17299 2023-06-18 12:23:27.000000 WavelinkCord-2.5.2b0/wavelink/ext/spotify/__init__.py
+-rw-rw-rw-   0        0        0    19586 2023-06-18 12:18:36.000000 WavelinkCord-2.5.2b0/wavelink/filters.py
+-rw-rw-rw-   0        0        0    17308 2023-06-18 12:23:32.000000 WavelinkCord-2.5.2b0/wavelink/node.py
+-rw-rw-rw-   0        0        0     3369 2023-06-18 12:23:32.000000 WavelinkCord-2.5.2b0/wavelink/payloads.py
+-rw-rw-rw-   0        0        0    21638 2023-06-18 12:23:31.000000 WavelinkCord-2.5.2b0/wavelink/player.py
+-rw-rw-rw-   0        0        0    12123 2023-06-18 12:18:36.000000 WavelinkCord-2.5.2b0/wavelink/queue.py
+-rw-rw-rw-   0        0        0     9628 2023-06-18 12:23:30.000000 WavelinkCord-2.5.2b0/wavelink/tracks.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:22:59.570204 WavelinkCord-2.5.2b0/wavelink/types/
+-rw-rw-rw-   0        0        0      825 2023-06-18 12:18:36.000000 WavelinkCord-2.5.2b0/wavelink/types/events.py
+-rw-rw-rw-   0        0        0      602 2023-06-18 12:18:37.000000 WavelinkCord-2.5.2b0/wavelink/types/request.py
+-rw-rw-rw-   0        0        0      409 2023-06-18 12:23:29.000000 WavelinkCord-2.5.2b0/wavelink/types/state.py
+-rw-rw-rw-   0        0        0      325 2023-06-18 12:18:37.000000 WavelinkCord-2.5.2b0/wavelink/types/track.py
+-rw-rw-rw-   0        0        0     9311 2023-06-18 12:18:36.000000 WavelinkCord-2.5.2b0/wavelink/websocket.py
```

### Comparing `WaveLinkCord-2.5.1/LICENSE` & `WavelinkCord-2.5.2b0/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2019-Current PythonistaGuild, EvieePy
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2019-Current PythonistaGuild, EvieePy
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `WaveLinkCord-2.5.1/PKG-INFO` & `WavelinkCord-2.5.2b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: WaveLinkCord
-Version: 2.5.1
-Summary: A robust and powerful Lavalink wrapper for Nextcord
-Author-email: Zyb3rWolfi <zyb3rwolfi@proton.me>
+Name: WavelinkCord
+Version: 2.5.2b0
+Summary: A robust and powerful Lavalink wrapper for discord.py
+Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `WaveLinkCord-2.5.1/README.rst` & `WavelinkCord-2.5.2b0/README.rst`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-.. image:: https://raw.githubusercontent.com/PythonistaGuild/Wavelink/master/logo.png
-
-
-.. image:: https://img.shields.io/badge/Python-3.10%20%7C%203.11-blue.svg
-    :target: https://www.python.org
-
-
-.. image:: https://img.shields.io/github/license/EvieePy/Wavelink.svg
-    :target: LICENSE
-
-
-.. image:: https://img.shields.io/discord/490948346773635102?color=%237289DA&label=Pythonista&logo=discord&logoColor=white
-   :target: https://discord.gg/RAKc3HF
-
-
-.. image:: https://img.shields.io/pypi/dm/Wavelink?color=black
-    :target: https://pypi.org/project/Wavelink
-    :alt: PyPI - Downloads
-
-
-.. image:: https://img.shields.io/maintenance/yes/2023?color=pink&style=for-the-badge
-    :target: https://github.com/PythonistaGuild/Wavelink/commits/main
-    :alt: Maintenance
-
-
-
-Wavelink is a robust and powerful Lavalink wrapper for `Discord.py <https://github.com/Rapptz/discord.py>`_.
-Wavelink features a fully asynchronous API that's intuitive and easy to use with built in Spotify Support and Node Pool Balancing.
-
-
-**Features:**
-
-- Fully Asynchronous
-- Auto-Play and Looping (With the inbuilt Queue system)
-- Spotify Support
-- Node Balancing and Fail-over
-- Supports Lavalink 3.7+
-
-
-Documentation
----------------------------
-`Official Documentation <https://wavelink.dev/>`_
-
-Support
----------------------------
-For support using WaveLink, please join the official `support server
-<https://discord.gg/RAKc3HF>`_ on `Discord <https://discordapp.com/>`_.
-
-.. image:: https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2
-    :target: https://discord.gg/RAKc3HF
-
-
-Installation
----------------------------
-The following commands are currently the valid ways of installing WaveLink.
-
-**WaveLink 2 requires Python 3.10+**
-
-**Windows**
-
-.. code:: sh
-
-    py -3.10 -m pip install -U Wavelink
-
-**Linux**
-
-.. code:: sh
-
-    python3.10 -m pip install -U Wavelink
-
-Getting Started
-----------------------------
-
-**See also:** `Examples <https://github.com/PythonistaGuild/Wavelink/tree/main/examples>`_
-
-.. code:: py
-
-    import discord
-    import wavelink
-    from discord.ext import commands
-
-
-    class Bot(commands.Bot):
-
-        def __init__(self) -> None:
-            intents = discord.Intents.default()
-            intents.message_content = True
-
-            super().__init__(intents=intents, command_prefix='?')
-
-        async def on_ready(self) -> None:
-            print(f'Logged in {self.user} | {self.user.id}')
-
-        async def setup_hook(self) -> None:
-            # Wavelink 2.0 has made connecting Nodes easier... Simply create each Node
-            # and pass it to NodePool.connect with the client/bot.
-            node: wavelink.Node = wavelink.Node(uri='http://localhost:2333', password='youshallnotpass')
-            await wavelink.NodePool.connect(client=self, nodes=[node])
-
-
-    bot = Bot()
-
-
-    @bot.command()
-    async def play(ctx: commands.Context, *, search: str) -> None:
-        """Simple play command."""
-
-        if not ctx.voice_client:
-            vc: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
-        else:
-            vc: wavelink.Player = ctx.voice_client
-
-        tracks = await wavelink.YouTubeTrack.search(search)
-        if not tracks:
-            await ctx.send(f'No tracks found with query: `{search}`')
-            return
-
-        track = tracks[0]
-        await vc.play(track)
-
-
-    @bot.command()
-    async def disconnect(ctx: commands.Context) -> None:
-        """Simple disconnect command.
-
-        This command assumes there is a currently connected Player.
-        """
-        vc: wavelink.Player = ctx.voice_client
-        await vc.disconnect()
-
-
-Lavalink Installation
----------------------
-
-Head to the official `Lavalink repo <https://github.com/freyacodes/Lavalink>`_ and give it a star!
-
-- Create a folder for storing Lavalink.jar and related files/folders.
-- Copy and paste the example `application.yml <https://github.com/freyacodes/Lavalink#server-configuration>`_ to ``application.yml`` in the folder we created earlier. You can open the yml in Notepad or any simple text editor.
-- Change your password in the ``application.yml`` and store it in a config for your bot.
-- Set local to true in the ``application.yml`` if you wish to use ``wavelink.LocalTrack`` for local machine search options... Otherwise ignore.
-- Save and exit.
-- Install `Java 17(Windows) <https://download.oracle.com/java/17/latest/jdk-17_windows-x64_bin.exe>`_ or **Java 13+** on the machine you are running.
-- Download `Lavalink.jar <https://ci.fredboat.com/viewLog.html?buildId=lastSuccessful&buildTypeId=Lavalink_Build&tab=artifacts&guest=1>`_ and place it in the folder created earlier.
-- Open a cmd prompt or terminal and change directory ``cd`` into the folder we made earlier.
-- Run: ``java -jar Lavalink.jar``
-
+.. image:: https://raw.githubusercontent.com/PythonistaGuild/Wavelink/master/logo.png
+
+
+.. image:: https://img.shields.io/badge/Python-3.10%20%7C%203.11-blue.svg
+    :target: https://www.python.org
+
+
+.. image:: https://img.shields.io/github/license/EvieePy/Wavelink.svg
+    :target: LICENSE
+
+
+.. image:: https://img.shields.io/discord/490948346773635102?color=%237289DA&label=Pythonista&logo=discord&logoColor=white
+   :target: https://discord.gg/RAKc3HF
+
+
+.. image:: https://img.shields.io/pypi/dm/Wavelink?color=black
+    :target: https://pypi.org/project/Wavelink
+    :alt: PyPI - Downloads
+
+
+.. image:: https://img.shields.io/maintenance/yes/2023?color=pink&style=for-the-badge
+    :target: https://github.com/PythonistaGuild/Wavelink/commits/main
+    :alt: Maintenance
+
+
+
+Wavelink is a robust and powerful Lavalink wrapper for `Discord.py <https://github.com/Rapptz/discord.py>`_.
+Wavelink features a fully asynchronous API that's intuitive and easy to use with built in Spotify Support and Node Pool Balancing.
+
+
+**Features:**
+
+- Fully Asynchronous
+- Auto-Play and Looping (With the inbuilt Queue system)
+- Spotify Support
+- Node Balancing and Fail-over
+- Supports Lavalink 3.7+
+
+
+Documentation
+---------------------------
+`Official Documentation <https://wavelink.dev/>`_
+
+Support
+---------------------------
+For support using WaveLink, please join the official `support server
+<https://discord.gg/RAKc3HF>`_ on `Discord <https://discordapp.com/>`_.
+
+.. image:: https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2
+    :target: https://discord.gg/RAKc3HF
+
+
+Installation
+---------------------------
+The following commands are currently the valid ways of installing WaveLink.
+
+**WaveLink 2 requires Python 3.10+**
+
+**Windows**
+
+.. code:: sh
+
+    py -3.10 -m pip install -U Wavelink
+
+**Linux**
+
+.. code:: sh
+
+    python3.10 -m pip install -U Wavelink
+
+Getting Started
+----------------------------
+
+**See also:** `Examples <https://github.com/PythonistaGuild/Wavelink/tree/main/examples>`_
+
+.. code:: py
+
+    import discord
+    import wavelink
+    from discord.ext import commands
+
+
+    class Bot(commands.Bot):
+
+        def __init__(self) -> None:
+            intents = discord.Intents.default()
+            intents.message_content = True
+
+            super().__init__(intents=intents, command_prefix='?')
+
+        async def on_ready(self) -> None:
+            print(f'Logged in {self.user} | {self.user.id}')
+
+        async def setup_hook(self) -> None:
+            # Wavelink 2.0 has made connecting Nodes easier... Simply create each Node
+            # and pass it to NodePool.connect with the client/bot.
+            node: wavelink.Node = wavelink.Node(uri='http://localhost:2333', password='youshallnotpass')
+            await wavelink.NodePool.connect(client=self, nodes=[node])
+
+
+    bot = Bot()
+
+
+    @bot.command()
+    async def play(ctx: commands.Context, *, search: str) -> None:
+        """Simple play command."""
+
+        if not ctx.voice_client:
+            vc: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
+        else:
+            vc: wavelink.Player = ctx.voice_client
+
+        tracks = await wavelink.YouTubeTrack.search(search)
+        if not tracks:
+            await ctx.send(f'No tracks found with query: `{search}`')
+            return
+
+        track = tracks[0]
+        await vc.play(track)
+
+
+    @bot.command()
+    async def disconnect(ctx: commands.Context) -> None:
+        """Simple disconnect command.
+
+        This command assumes there is a currently connected Player.
+        """
+        vc: wavelink.Player = ctx.voice_client
+        await vc.disconnect()
+
+
+Lavalink Installation
+---------------------
+
+Head to the official `Lavalink repo <https://github.com/freyacodes/Lavalink>`_ and give it a star!
+
+- Create a folder for storing Lavalink.jar and related files/folders.
+- Copy and paste the example `application.yml <https://github.com/freyacodes/Lavalink#server-configuration>`_ to ``application.yml`` in the folder we created earlier. You can open the yml in Notepad or any simple text editor.
+- Change your password in the ``application.yml`` and store it in a config for your bot.
+- Set local to true in the ``application.yml`` if you wish to use ``wavelink.LocalTrack`` for local machine search options... Otherwise ignore.
+- Save and exit.
+- Install `Java 17(Windows) <https://download.oracle.com/java/17/latest/jdk-17_windows-x64_bin.exe>`_ or **Java 13+** on the machine you are running.
+- Download `Lavalink.jar <https://ci.fredboat.com/viewLog.html?buildId=lastSuccessful&buildTypeId=Lavalink_Build&tab=artifacts&guest=1>`_ and place it in the folder created earlier.
+- Open a cmd prompt or terminal and change directory ``cd`` into the folder we made earlier.
+- Run: ``java -jar Lavalink.jar``
+
 If you are having any problems installing Lavalink, please join the official Discord Server listed above for help.
```

### Comparing `WaveLinkCord-2.5.1/WaveLinkCord.egg-info/PKG-INFO` & `WavelinkCord-2.5.2b0/WavelinkCord.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: WaveLinkCord
-Version: 2.5.1
-Summary: A robust and powerful Lavalink wrapper for Nextcord
-Author-email: Zyb3rWolfi <zyb3rwolfi@proton.me>
+Name: WavelinkCord
+Version: 2.5.2b0
+Summary: A robust and powerful Lavalink wrapper for discord.py
+Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `WaveLinkCord-2.5.1/wavelinkcord/__init__.py` & `WavelinkCord-2.5.2b0/wavelink/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 __title__ = "WaveLinkCord"
-__author__ = "Zyb3rWolfi"
+__author__ = "PythonistaGuild, EvieePy"
 __license__ = "MIT"
 __copyright__ = "Copyright 2019-Present (c) PythonistaGuild, EvieePy"
-__version__ = "2.5.1"
+__version__ = "2.5.2b"
 
 from .enums import *
 from .exceptions import *
 from .node import *
 from .payloads import *
 from .player import Player as Player
 from .tracks import *
```

### Comparing `WaveLinkCord-2.5.1/wavelinkcord/backoff.py` & `WavelinkCord-2.5.2b0/wavelink/backoff.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.5.1/wavelinkcord/enums.py` & `WavelinkCord-2.5.2b0/wavelink/enums.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.5.1/wavelinkcord/exceptions.py` & `WavelinkCord-2.5.2b0/wavelink/exceptions.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.5.1/wavelinkcord/ext/spotify/__init__.py` & `WavelinkCord-2.5.2b0/wavelink/ext/spotify/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 import re
 import time
 from typing import Any, List, Optional, Type, TypeVar, Union, TYPE_CHECKING
 
 import aiohttp
 from nextcord.ext import commands
 
-import wavelinkcord
-from wavelinkcord import Node, NodePool
+import wavelink
+from wavelink import Node, NodePool
 
 if TYPE_CHECKING:
-    from wavelinkcord import Player, Playable
+    from wavelink import Player, Playable
 
 
 __all__ = ('SpotifySearchType',
            'SpotifyClient',
            'SpotifyTrack',
            'SpotifyRequestError',
            'decode_url')
@@ -75,15 +75,15 @@
         Could return None if the URL is invalid.
 
     Examples
     --------
 
     .. code:: python3
 
-        from wavelinkcord.ext import spotify
+        from wavelink.ext import spotify
 
         ...
 
         decoded = spotify.decode_url("https://open.spotify.com/track/6BDLcvvtyJD2vnXRDi1IjQ?si=e2e5bd7aaf3d4a2a")
 
         if decoded and decoded['type'] is spotify.SpotifySearchType.track:
             track = await spotify.SpotifyTrack.search(query=decoded["id"], type=decoded["type"])
@@ -108,15 +108,15 @@
     track
         Default search type. Unless specified otherwise this will always be the search type.
     album
         Album search type.
     playlist
         Playlist search type.
     unusable
-        Unusable type. This type is returned when wavelinkcord can not be used to play this track.
+        Unusable type. This type is returned when Wavelink can not be used to play this track.
     """
     track = 0
     album = 1
     playlist = 2
     unusable = 3
 
 
@@ -270,15 +270,15 @@
 
         Parameters
         ----------
         query: str
             The song to search for.
         type: Optional[:class:`~SpotifySearchType`]
             An optional enum value to use when searching with Spotify. Defaults to track.
-        node: Optional[:class:`wavelinkcord.Node`]
+        node: Optional[:class:`wavelink.Node`]
             An optional Node to use to make the search with.
 
         Returns
         -------
         List[:class:`SpotifyTrack`]
 
         Examples
@@ -324,15 +324,15 @@
         ----------
         query: str
             The Spotify URL or ID to search for. Must be of type Playlist or Album.
         limit: Optional[int]
             Limit the amount of tracks returned.
         type: :class:`~SpotifySearchType`
             The type of search. Must be either playlist or album. Defaults to playlist.
-        node: Optional[:class:`wavelinkcord.Node`]
+        node: Optional[:class:`wavelink.Node`]
             An optional node to use when querying for tracks. Defaults to the best available.
 
         Examples
         --------
 
         .. code:: python3
 
@@ -365,26 +365,26 @@
 
         if not results:
             raise commands.BadArgument(f"Could not find any songs matching query: {argument}")
 
         return results[0]
 
     async def fulfill(self, *, player: Player, cls: Playable, populate: bool) -> Playable:
-        """Used to fulfill the :class:`wavelinkcord.Player` Auto Play Queue.
+        """Used to fulfill the :class:`wavelink.Player` Auto Play Queue.
 
         .. warning::
 
-            Usually you would not call this directly. Instead you would set :attr:`wavelinkcord.Player.autoplay` to true,
+            Usually you would not call this directly. Instead you would set :attr:`wavelink.Player.autoplay` to true,
             and allow the player to fulfill this request automatically.
 
 
         Parameters
         ----------
-        player: :class:`wavelinkcord.player.Player`
-            If :attr:`wavelinkcord.Player.autoplay` is enabled, this search will fill the AutoPlay Queue with more tracks.
+        player: :class:`wavelink.player.Player`
+            If :attr:`wavelink.Player.autoplay` is enabled, this search will fill the AutoPlay Queue with more tracks.
         cls
             The class to convert this Spotify Track to.
         """
         tracks: list[cls] = await cls.search(f'"{self.isrc}"')
         if not tracks:
             tracks: list[cls] = await cls.search(f'{self.name} - {self.artists[0]}')
 
@@ -419,15 +419,15 @@
 
             await player.auto_queue.put_wait(reco)
 
         return tracks[0]
 
 
 class SpotifyClient:
-    """Spotify client passed to :class:`wavelinkcord.Node` for searching via Spotify.
+    """Spotify client passed to :class:`wavelink.Node` for searching via Spotify.
 
     Parameters
     ----------
     client_id: str
         Your spotify application client ID.
     client_secret: str
         Your spotify application secret.
```

### Comparing `WaveLinkCord-2.5.1/wavelinkcord/filters.py` & `WavelinkCord-2.5.2b0/wavelink/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 class BaseFilter(abc.ABC):
 
     def __init__(self, name: str | None = None) -> None:
         self.name: str = name or "Unknown"
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.BaseFilter name={self.name}>"
+        return f"<wavelink.BaseFilter name={self.name}>"
 
     @property
     @abc.abstractmethod
     def _payload(self) -> Any:
         raise NotImplementedError
 
 
@@ -81,15 +81,15 @@
 
         _dict = collections.defaultdict(float)
         _dict.update(bands)
 
         self.bands = [{"band": band, "gain": _dict[band]} for band in range(15)]
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Equalizer name={self.name}>"
+        return f"<wavelink.Equalizer name={self.name}>"
 
     @property
     def _payload(self) -> list[dict[str, float]]:
         return self.bands
 
     @classmethod
     def flat(cls) -> Equalizer:
@@ -167,15 +167,15 @@
 
         self.level: float = level
         self.mono_level: float = mono_level
         self.filter_band: float = filter_band
         self.filter_width: float = filter_width
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Karaoke level={self.level}, mono_level={self.mono_level}, " \
+        return f"<wavelink.Karaoke level={self.level}, mono_level={self.mono_level}, " \
                f"filter_band={self.filter_band}, filter_width={self.filter_width}>"
 
     @property
     def _payload(self) -> dict[str, float]:
         return {
             "level":       self.level,
             "monoLevel":   self.mono_level,
@@ -219,15 +219,15 @@
         super().__init__(name="Timescale")
 
         self.speed: float = speed
         self.pitch: float = pitch
         self.rate: float = rate
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Timescale speed={self.speed}, pitch={self.pitch}, rate={self.rate}>"
+        return f"<wavelink.Timescale speed={self.speed}, pitch={self.pitch}, rate={self.rate}>"
 
     @property
     def _payload(self) -> dict[str, float]:
         return {
             "speed": self.speed,
             "pitch": self.pitch,
             "rate":  self.rate,
@@ -263,15 +263,15 @@
 
         super().__init__(name="Tremolo")
 
         self.frequency: float = frequency
         self.depth: float = depth
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Tremolo frequency={self.frequency}, depth={self.depth}>"
+        return f"<wavelink.Tremolo frequency={self.frequency}, depth={self.depth}>"
 
     @property
     def _payload(self) -> dict[str, float]:
         return {
             "frequency": self.frequency,
             "depth":     self.depth
         }
@@ -306,15 +306,15 @@
 
         super().__init__(name="Vibrato")
 
         self.frequency: float = frequency
         self.depth: float = depth
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Vibrato frequency={self.frequency}, depth={self.depth}>"
+        return f"<wavelink.Vibrato frequency={self.frequency}, depth={self.depth}>"
 
     @property
     def _payload(self) -> dict[str, float]:
         return {
             "frequency": self.frequency,
             "depth":     self.depth
         }
@@ -335,15 +335,15 @@
 
     def __init__(self, speed: float = 5) -> None:
         super().__init__(name="Rotation")
 
         self.speed: float = speed
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Rotation speed={self.speed}>"
+        return f"<wavelink.Rotation speed={self.speed}>"
 
     @property
     def _payload(self) -> dict[str, float]:
         return {
             "rotationHz": self.speed,
         }
 
@@ -371,15 +371,15 @@
         self.cos_scale: float = cos_scale
         self.tan_offset: float = tan_offset
         self.tan_scale: float = tan_scale
         self.offset: float = offset
         self.scale: float = scale
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Distortion " \
+        return f"<wavelink.Distortion " \
                f"sin_offset={self.sin_offset}, " \
                f"sin_scale={self.sin_scale}, cos_offset={self.cos_offset}, " \
                f"cos_scale={self.cos_scale}, tan_offset={self.tan_offset}, " \
                f"tan_scale={self.tan_scale}, offset={self.offset}, " \
                f"scale={self.scale}>"
 
     @property
@@ -440,15 +440,15 @@
 
         self.left_to_left: float = left_to_left
         self.right_to_right: float = right_to_right
         self.left_to_right: float = left_to_right
         self.right_to_left: float = right_to_left
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.ChannelMix " \
+        return f"<wavelink.ChannelMix " \
                f"left_to_left={self.left_to_left}, " \
                f"right_to_right{self.right_to_right}, " \
                f"left_to_right={self.left_to_right}, " \
                f"right_to_left={self.right_to_left}>"
 
     @property
     def _payload(self) -> dict[str, float]:
@@ -513,15 +513,15 @@
         smoothing: float = 20
     ) -> None:
         super().__init__(name="Low Pass")
 
         self.smoothing: float = smoothing
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.LowPass smoothing={self.smoothing}>"
+        return f"<wavelink.LowPass smoothing={self.smoothing}>"
 
     @property
     def _payload(self) -> dict[str, float]:
         return {
             "smoothing": self.smoothing,
         }
 
@@ -530,33 +530,33 @@
     """A filter that can be applied to a track.
 
     This filter accepts an instance of itself as a parameter which allows
     you to keep previous filters while also applying new ones or overwriting old ones.
 
     Parameters
     ----------
-    filter: wavelinkcord.Filter
+    filter: wavelink.Filter
         An instance of this filter class.
-    equalizer: wavelinkcord.Equalizer
+    equalizer: wavelink.Equalizer
         An equalizer to apply to the track.
-    karaoke: wavelinkcord.Karaoke
+    karaoke: wavelink.Karaoke
         A karaoke filter to apply to the track.
-    timescale: wavelinkcord.Timescale
+    timescale: wavelink.Timescale
         A timescale filter to apply to the track.
-    tremolo: wavelinkcord.Tremolo
+    tremolo: wavelink.Tremolo
         A tremolo filter to apply to the track.
-    vibrato: wavelinkcord.Vibrato
+    vibrato: wavelink.Vibrato
         A vibrato filter to apply to the track.
-    rotation: wavelinkcord.Rotation
+    rotation: wavelink.Rotation
         A rotation filter to apply to the track.
-    distortion: wavelinkcord.Distortion
+    distortion: wavelink.Distortion
         A distortion filter to apply to the track.
-    channel_mix: wavelinkcord.ChannelMix
+    channel_mix: wavelink.ChannelMix
         A channel mix filter to apply to the track.
-    low_pass: wavelinkcord.LowPass
+    low_pass: wavelink.LowPass
         A low pass filter to apply to the track.
 
     """
 
     def __init__(
         self,
         _filter: Filter | None = None,
@@ -581,15 +581,15 @@
         self.vibrato: Vibrato | None = vibrato
         self.rotation: Rotation | None = rotation
         self.distortion: Distortion | None = distortion
         self.channel_mix: ChannelMix | None = channel_mix
         self.low_pass: LowPass | None = low_pass
 
     def __repr__(self) -> str:
-        return f"<wavelinkcord.Filter equalizer={self.equalizer}, " \
+        return f"<wavelink.Filter equalizer={self.equalizer}, " \
                f"karaoke={self.karaoke}, timescale={self.timescale}, tremolo={self.tremolo}, " \
                f"vibrato={self.vibrato}, rotation={self.rotation}, distortion={self.distortion}, " \
                f"channel_mix={self.channel_mix}, low_pass={self.low_pass}>"
 
     @property
     def _payload(self) -> dict[str, Any]:
```

### Comparing `WaveLinkCord-2.5.1/wavelinkcord/node.py` & `WavelinkCord-2.5.2b0/wavelink/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 # noinspection PyShadowingBuiltins
 class Node:
-    """The base wavelinkcord Node.
+    """The base Wavelink Node.
 
     The Node is responsible for keeping the Websocket alive, tracking the state of Players
     and fetching/decoding Tracks and Playlists.
 
     .. note::
 
         The Node class should only be created once per Lavalink connection.
@@ -206,18 +206,18 @@
 
             if version.endswith('-SNAPSHOT'):
                 self._major_version = 3
                 return
 
             version_tuple = tuple(int(v) for v in version.split('.'))
             if version_tuple[0] < 3:
-                raise InvalidLavalinkVersion(f'wavelinkcord 2 is not compatible with Lavalink "{version}".')
+                raise InvalidLavalinkVersion(f'Wavelink 2 is not compatible with Lavalink "{version}".')
 
             if version_tuple[0] == 3 and version_tuple[1] < 7:
-                raise InvalidLavalinkVersion('wavelinkcord 2 is not compatible with Lavalink versions under "3.7".')
+                raise InvalidLavalinkVersion('Wavelink 2 is not compatible with Lavalink versions under "3.7".')
 
             self._major_version = version_tuple[0]
 
     async def _send(self,
                     *,
                     method: str,
                     path: str,
@@ -297,15 +297,15 @@
             The type of which playlist should be returned, this must subclass :class:`tracks.Playlist`.
         query: str
             The playlist's identifier. This may be a YouTube playlist URL for example.
 
         Returns
         -------
         Optional[:class:`tracks.Playlist`]:
-            The related wavelinkcord track object or ``None`` if none was found.
+            The related wavelink track object or ``None`` if none was found.
 
         Raises
         ------
         ValueError
             Loading the playlist failed.
         WavelinkException
             An unspecified error occurred when loading the playlist.
@@ -343,15 +343,15 @@
         data = await self._send(method='GET', path='decodetrack', query=f'encodedTrack={encoded_query}')
 
         return cls(data=data)
 
 
 # noinspection PyShadowingBuiltins
 class NodePool:
-    """The wavelinkcord NodePool is responsible for keeping track of all :class:`Node`.
+    """The Wavelink NodePool is responsible for keeping track of all :class:`Node`.
 
     Attributes
     ----------
     nodes: dict[str, :class:`Node`]
         A mapping of :class:`Node` identifier to :class:`Node`.
 
 
@@ -432,20 +432,20 @@
         Raises
         ------
         InvalidNode
             The given id does nto resolve to a :class:`Node` or no :class:`Node` has been connected.
         """
         if id:
             if id not in cls.__nodes:
-                raise InvalidNode(f'A Node with ID "{id}" does not exist on the wavelinkcord NodePool.')
+                raise InvalidNode(f'A Node with ID "{id}" does not exist on the Wavelink NodePool.')
 
             return cls.__nodes[id]
 
         if not cls.__nodes:
-            raise InvalidNode('No Node currently exists on the wavelinkcord NodePool.')
+            raise InvalidNode('No Node currently exists on the Wavelink NodePool.')
 
         nodes = cls.__nodes.values()
         return sorted(nodes, key=lambda n: len(n.players))[0]
 
     @classmethod
     def get_connected_node(cls) -> Node:
         """Get the best available connected :class:`Node`.
@@ -459,15 +459,15 @@
         ------
         InvalidNode
             No Nodes are currently in the connected state.
         """
 
         nodes: list[Node] = [n for n in cls.__nodes.values() if n.status is NodeStatus.CONNECTED]
         if not nodes:
-            raise InvalidNode('There are no Nodes on the wavelinkcord NodePool that are currently in the connected state.')
+            raise InvalidNode('There are no Nodes on the Wavelink NodePool that are currently in the connected state.')
 
         return sorted(nodes, key=lambda n: len(n.players))[0]
 
     @classmethod
     async def get_tracks(cls_,  # type: ignore
                          query: str,
                          /,
```

### Comparing `WaveLinkCord-2.5.1/wavelinkcord/payloads.py` & `WavelinkCord-2.5.2b0/wavelink/payloads.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,20 +34,20 @@
     from .tracks import Playable
     from .types.events import EventOp
 
 __all__ = ('TrackEventPayload', 'WebsocketClosedPayload')
 
 
 class TrackEventPayload:
-    """The wavelinkcord Track Event Payload.
+    """The Wavelink Track Event Payload.
 
     .. warning::
 
         This class should not be created manually, instead you will receive it from the
-        various wavelinkcord track events.
+        various wavelink track events.
 
     Attributes
     ----------
     event: :class:`TrackEventType`
         An enum of the type of event.
     track: :class:`Playable`
         The track associated with this event.
@@ -65,20 +65,20 @@
         self.original: Playable | None = original
         self.player: Player = player
 
         self.reason: str = data.get('reason')
 
 
 class WebsocketClosedPayload:
-    """The wavelinkcord WebsocketClosed Event Payload.
+    """The Wavelink WebsocketClosed Event Payload.
 
     .. warning::
 
         This class should not be created manually, instead you will receive it from the
-        wavelinkcord `on_wavelink_websocket_closed` event.
+        wavelink `on_wavelink_websocket_closed` event.
 
     Attributes
     ----------
     code: :class:`DiscordVoiceCloseType`
         An Enum representing the close code from nextcord.
     reason: Optional[str]
         The reason the Websocket was closed.
```

### Comparing `WaveLinkCord-2.5.1/wavelinkcord/player.py` & `WavelinkCord-2.5.2b0/wavelink/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 VoiceChannel = Union[
     nextcord.VoiceChannel, nextcord.StageChannel
 ]  # todo: VocalGuildChannel?
 
 
 class Player(nextcord.VoiceProtocol):
-    """wavelinkcord Player class.
+    """Wavelink Player class.
 
     This class is used as a :class:`~nextcord.VoiceProtocol` and inherits all its members.
 
 
     .. note::
 
         The Player class come with an in-built queue. See :class:`queue.Queue`.
@@ -85,15 +85,15 @@
     channel: :class:`nextcord.VoiceChannel`
         The channel this player is currently connected to.
     nodes: list[:class:`node.Node`]
         The list of Nodes this player is currently using.
     current_node: :class:`node.Node`
         The Node this player is currently using.
     queue: :class:`queue.Queue`
-        The wavelinkcord built in Queue. See :class:`queue.Queue`. This queue always takes precedence over the auto_queue.
+        The wavelink built in Queue. See :class:`queue.Queue`. This queue always takes precedence over the auto_queue.
         Meaning any songs in this queue will be played before auto_queue songs.
     auto_queue: :class:`queue.Queue`
         The built-in AutoPlay Queue. This queue keeps track of recommended songs only.
         When a song is retrieved from this queue in the AutoPlay event, it is added to the main Queue.history.
     filter: dict[:class:`str`, :class:`Any`]
         The current filters applied.
     """
@@ -177,14 +177,18 @@
 
         if self.queue:
             populate = len(self.auto_queue) < self._auto_threshold
             await self.play(self.queue.get(), populate=populate)
 
             return
 
+        if self.queue.loop_all:
+            await self.play(self.queue.get())
+            return
+
         if not self.auto_queue:
             return
 
         await self.queue.put_wait(await self.auto_queue.get_wait())
         populate = self.auto_queue.is_empty
 
         await self.play(await self.queue.get_wait(), populate=populate)
@@ -382,15 +386,15 @@
                    end: int | None = None,
                    volume: int | None = None,
                    *,
                    populate: bool = False
                    ) -> Playable:
         """|coro|
 
-        Play a wavelinkcord Track.
+        Play a WaveLink Track.
 
         Parameters
         ----------
         track: :class:`tracks.Playable`
             The :class:`tracks.Playable` track to start playing.
         replace: bool
             Whether this track should replace the current track. Defaults to ``True``.
@@ -449,14 +453,20 @@
 
         except InvalidLavalinkResponse as e:
             self._current = None
             self._original = None
             raise e
 
         self._player_state['track'] = resp['track']['encoded']
+
+        if self.queue.loop and self.queue._loaded:
+            pass
+        else:
+            self.queue.history.put(track)
+
         self.queue._loaded = track
 
         return track
 
     async def set_volume(self, value: int) -> None:
         """|coro|
 
@@ -553,15 +563,15 @@
     ) -> None:
         """|coro|
 
         Set the player's filter.
 
         Parameters
         ----------
-        filter: :class:`wavelinkcord.Filter`
+        filter: :class:`wavelink.Filter`
             The filter to apply to the player.
         seek: bool
             Whether to seek the player to its current position
             which will apply the filter immediately. Defaults to ``False``.
         """
 
         assert self._guild is not None
```

### Comparing `WaveLinkCord-2.5.1/wavelinkcord/queue.py` & `WavelinkCord-2.5.2b0/wavelink/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def __str__(self) -> str:
         """String showing all Playable objects appearing as a list."""
         return str([f"'{t}'" for t in self])
 
     def __repr__(self) -> str:
         """Official representation with max_size and member count."""
         return (
-            f"wavelinkcord Queue: members={self.count}")
+            f"Wavelink Queue: members={self.count}")
 
     def __bool__(self) -> bool:
         """Treats the queue as a bool, with it evaluating True when it contains members."""
         return bool(self.count)
 
     def __call__(self, item: Playable | spotify.SpotifyTrack) -> None:
         """Allows the queue instance to be called directly in order to add a member."""
@@ -262,22 +262,21 @@
     def get(self) -> Playable | spotify.SpotifyTrack:
         return self._get()
 
     def _get(self) -> Playable | spotify.SpotifyTrack:
         if self.loop and self._loaded:
             return self._loaded
 
-        item = super()._get()
         if self.loop_all and self.is_empty:
             self._queue.extend(self.history._queue)
             self.history.clear()
 
-        self._loaded = item
-        self.history.put(item)
+        item = super()._get()
 
+        self._loaded = item
         return item
 
     def _put(self, item: Playable | spotify.SpotifyTrack) -> None:
         super()._put(item)
         self._wakeup_next()
 
     def _insert(self, index: int, item: Playable | spotify.SpotifyTrack) -> None:
```

### Comparing `WaveLinkCord-2.5.1/wavelinkcord/tracks.py` & `WavelinkCord-2.5.2b0/wavelink/tracks.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     """
 
     def __init__(self, data: dict[str, Any]):
         self.data: dict[str, Any] = data
 
 
 class Playable(metaclass=abc.ABCMeta):
-    """Base ABC Track used in all the wavelinkcord Track types.
+    """Base ABC Track used in all the Wavelink Track types.
 
     Attributes
     ----------
     data: dict[str, Any]
         The raw data received via Lavalink.
     encoded: str
         The encoded Track string.
@@ -85,15 +85,15 @@
         The length of the track in milliseconds.
     duration: int
         An alias for length.
     position: int
         The position the track will start in milliseconds. Defaults to 0.
     title: str
         The Track title.
-    source: :class:`wavelinkcord.TrackSource`
+    source: :class:`wavelink.TrackSource`
         The source this Track was fetched from.
     uri: Optional[str]
         The URI of this track. Could be None.
     author: Optional[str]
         The author of this track. Could be None.
     identifier: Optional[str]
         The Youtube/YoutubeMusic identifier for this track. Could be None.
@@ -181,17 +181,17 @@
                      ) -> Self | list[Self]:
         """Search and retrieve tracks for the given query.
 
         Parameters
         ----------
         query: str
             The query to search for.
-        node: Optional[:class:`wavelinkcord.Node`]
-            The node to use when searching for tracks. If no :class:`wavelinkcord.Node` is passed,
-            one will be fetched via the :class:`wavelinkcord.NodePool`.
+        node: Optional[:class:`wavelink.Node`]
+            The node to use when searching for tracks. If no :class:`wavelink.Node` is passed,
+            one will be fetched via the :class:`wavelink.NodePool`.
         """
 
         check = yarl.URL(query)
 
         if str(check.host) == 'youtube.com' or str(check.host) == 'www.youtube.com' and check.query.get("list") or \
                 cls.PREFIX == 'ytpl:':
 
@@ -219,15 +219,15 @@
         if issubclass(cls, YouTubePlaylist):
             return results  # type: ignore
 
         return results[0]
 
 
 class GenericTrack(Playable):
-    """Generic wavelinkcord Track.
+    """Generic Wavelink Track.
 
     Use this track for searching for Local songs or direct URLs.
     """
     ...
 
 
 class YouTubeTrack(Playable):
```

### Comparing `WaveLinkCord-2.5.1/wavelinkcord/types/events.py` & `WavelinkCord-2.5.2b0/wavelink/types/events.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.5.1/wavelinkcord/types/request.py` & `WavelinkCord-2.5.2b0/wavelink/types/request.py`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.5.1/wavelinkcord/websocket.py` & `WavelinkCord-2.5.2b0/wavelink/websocket.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 import asyncio
 import logging
 from typing import TYPE_CHECKING, Any, Optional
 
 import aiohttp
 
-import wavelinkcord
+import wavelink
 
 from . import __version__
 from .backoff import Backoff
 from .enums import NodeStatus, TrackEventType
 from .exceptions import *
 from .payloads import TrackEventPayload, WebsocketClosedPayload
 
@@ -75,15 +75,15 @@
     def headers(self) -> dict[str, str]:
         assert self.node.client is not None
         assert self.node.client.user is not None
 
         return {
             'Authorization': self.node.password,
             'User-Id': str(self.node.client.user.id),
-            'Client-Name': f'wavelinkcord/{__version__}'
+            'Client-Name': f'Wavelink/{__version__}'
         }
 
     def is_connected(self) -> bool:
         return self.socket is not None and not self.socket.closed
 
     async def connect(self) -> None:
         if self.node.status is NodeStatus.CONNECTED:
@@ -125,22 +125,22 @@
         self._listener_task = asyncio.create_task(self._listen())
 
     async def _reconnect(self) -> None:
         self.node._status = NodeStatus.CONNECTING
         self.retry = self.backoff.calculate()
 
         if self.retries == 0:
-            logger.error('wavelinkcord 2.0 was unable to connect, and has exhausted the reconnection attempt limit. '
+            logger.error('Wavelink 2.0 was unable to connect, and has exhausted the reconnection attempt limit. '
                          'Please check your Lavalink Node is started and your connection details are correct.')
 
             await self.cleanup()
             return
 
         retries = f'{self.retries} attempt(s) remaining.' if self.retries else ''
-        logger.error(f'wavelinkcord 2.0 was unable to connect, retrying connection in: "{self.retry}" seconds. {retries}')
+        logger.error(f'Wavelink 2.0 was unable to connect, retrying connection in: "{self.retry}" seconds. {retries}')
 
         if self.retries:
             self.retries -= 1
 
         await asyncio.sleep(self.retry)
         await self.connect()
 
@@ -199,15 +199,15 @@
                                  f'<code: {data["code"]}, reason: {data["reason"]}, by_discord: {data["byRemote"]}>')
 
                     payload: WebsocketClosedPayload = WebsocketClosedPayload(data=data, player=player)
 
                     self.dispatch('websocket_closed', payload)
                     continue
 
-                track = await self.node.build_track(cls=wavelinkcord.GenericTrack, encoded=data['encodedTrack'])
+                track = await self.node.build_track(cls=wavelink.GenericTrack, encoded=data['encodedTrack'])
                 payload: TrackEventPayload = TrackEventPayload(
                     data=data,
                     track=track,
                     player=player,
                     original=player._original
                 )
 
@@ -231,16 +231,16 @@
 
                 await player._update_event(data)
                 self.dispatch("player_update", data)
                 logger.debug(f'Websocket Player Update: {data}')
 
             else:
                 logger.info(f'Received unknown payload from Lavalink: <{data}>. '
-                            f'If this continues consider making a ticket on the wavelinkcord GitHub. '
-                            f'https://github.com/PythonistaGuild/wavelinkcord')
+                            f'If this continues consider making a ticket on the Wavelink GitHub. '
+                            f'https://github.com/PythonistaGuild/Wavelink')
 
     def get_player(self, payload: dict[str, Any]) -> Optional['Player']:
         return self.node.players.get(int(payload['guildId']), None)
 
     def dispatch(self, event, *args: Any, **kwargs: Any) -> None:
         self.node.client.dispatch(f"wavelink_{event}", *args, **kwargs)
```

