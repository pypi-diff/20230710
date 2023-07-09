# Comparing `tmp/AsyncIRCClient-0.0.7.tar.gz` & `tmp/AsyncIRCClient-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AsyncIRCClient-0.0.7.tar", last modified: Sun Jul  9 08:47:15 2023, max compression
+gzip compressed data, was "AsyncIRCClient-0.0.8.tar", last modified: Sun Jul  9 22:24:54 2023, max compression
```

## Comparing `AsyncIRCClient-0.0.7.tar` & `AsyncIRCClient-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 08:47:15.542828 AsyncIRCClient-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-07-09 08:47:15.538822 AsyncIRCClient-0.0.7/AsyncIRCClient.egg-info/
--rw-rw-rw-   0        0        0     1339 2023-07-09 08:47:15.000000 AsyncIRCClient-0.0.7/AsyncIRCClient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-09 08:47:15.000000 AsyncIRCClient-0.0.7/AsyncIRCClient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 08:47:15.000000 AsyncIRCClient-0.0.7/AsyncIRCClient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-09 08:47:15.000000 AsyncIRCClient-0.0.7/AsyncIRCClient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-09 08:47:15.000000 AsyncIRCClient-0.0.7/AsyncIRCClient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1339 2023-07-09 08:47:15.542828 AsyncIRCClient-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1152 2023-06-09 10:28:03.000000 AsyncIRCClient-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 08:47:15.541828 AsyncIRCClient-0.0.7/async_irc_client/
--rw-rw-rw-   0        0        0       33 2023-06-09 10:25:57.000000 AsyncIRCClient-0.0.7/async_irc_client/__init__.py
--rw-rw-rw-   0        0        0    35307 2023-07-09 08:46:26.000000 AsyncIRCClient-0.0.7/async_irc_client/async_irc_client.py
--rw-rw-rw-   0        0        0       42 2023-07-09 08:47:15.542828 AsyncIRCClient-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      460 2023-07-09 08:46:26.000000 AsyncIRCClient-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:24:54.673731 AsyncIRCClient-0.0.8/
+drwxrwxrwx   0        0        0        0 2023-07-09 22:24:54.668223 AsyncIRCClient-0.0.8/AsyncIRCClient.egg-info/
+-rw-rw-rw-   0        0        0     2116 2023-07-09 22:24:54.000000 AsyncIRCClient-0.0.8/AsyncIRCClient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-09 22:24:54.000000 AsyncIRCClient-0.0.8/AsyncIRCClient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 22:24:54.000000 AsyncIRCClient-0.0.8/AsyncIRCClient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-09 22:24:54.000000 AsyncIRCClient-0.0.8/AsyncIRCClient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-09 22:24:54.000000 AsyncIRCClient-0.0.8/AsyncIRCClient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2116 2023-07-09 22:24:54.673223 AsyncIRCClient-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1929 2023-07-09 22:24:48.000000 AsyncIRCClient-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 22:24:54.672223 AsyncIRCClient-0.0.8/async_irc_client/
+-rw-rw-rw-   0        0        0       33 2023-06-09 10:25:57.000000 AsyncIRCClient-0.0.8/async_irc_client/__init__.py
+-rw-rw-rw-   0        0        0    35769 2023-07-09 22:19:13.000000 AsyncIRCClient-0.0.8/async_irc_client/async_irc_client.py
+-rw-rw-rw-   0        0        0       42 2023-07-09 22:24:54.673731 AsyncIRCClient-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      460 2023-07-09 22:24:48.000000 AsyncIRCClient-0.0.8/setup.py
```

### Comparing `AsyncIRCClient-0.0.7/AsyncIRCClient.egg-info/PKG-INFO` & `AsyncIRCClient-0.0.8/AsyncIRCClient.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncIRCClient
-Version: 0.0.7
+Version: 0.0.8
 Summary: Async IRC Client
 Author: CoreTaxxe
 Author-email: coretaxxe@gmail.com
 Description-Content-Type: text/markdown
 
 # AsyncIRCClient
 Async (Twitch-) IRC client
@@ -30,20 +30,37 @@
         self.send_chat_message(f"Hello World {message.source.nick}")
 
     # mod only command
     @TwitchIRCBot.command("mod_test", mod_only=True)
     async def mod_test_command(self, message: Message) -> None:
         self.send_chat_message(f"Hello World mod {message.source.nick}")
 
+    @TwitchIRCBot.command("alias_test", aliases=["alias_1", "alias_2"])
+    async def alias_test_command(self, message: Message) -> None:
+        self.send_chat_message("Call as alias!")
+
+    # when using case-insensitive commands you may not use 
+    # any other command with the same name as any case-insensitive combination
+    # works with aliases
+    @TwitchIRCBot.command("case_insensitive", case_sensitive=False)
+    async def case_insensitive_command(self, message: Message) -> None:
+        self.send_chat_message("Case insensitive")
+
     # repeat a task
     # runs once the client is ready and after the specified time interval
     # here 1000s
     @TwitchIRCBot.loop(1000)
     async def my_task(self):
         logger.info("Hello World")
 
+    # repeat a task at given time
+    # is 1 second delayed to prevent double trigger inaccuracies
+    @TwitchIRCBot.loop(time="08:36")
+    async def my_timed_task(self):
+        logger.info("Hello World at 08:36")
+
 
 if __name__ == "__main__":
     MyBot(oauth_token="YOURTOKEN", nick_name="BOTNAME", channel="CHANNELNAME").run()
 
 
 ```
```

### Comparing `AsyncIRCClient-0.0.7/PKG-INFO` & `AsyncIRCClient-0.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncIRCClient
-Version: 0.0.7
+Version: 0.0.8
 Summary: Async IRC Client
 Author: CoreTaxxe
 Author-email: coretaxxe@gmail.com
 Description-Content-Type: text/markdown
 
 # AsyncIRCClient
 Async (Twitch-) IRC client
@@ -30,20 +30,37 @@
         self.send_chat_message(f"Hello World {message.source.nick}")
 
     # mod only command
     @TwitchIRCBot.command("mod_test", mod_only=True)
     async def mod_test_command(self, message: Message) -> None:
         self.send_chat_message(f"Hello World mod {message.source.nick}")
 
+    @TwitchIRCBot.command("alias_test", aliases=["alias_1", "alias_2"])
+    async def alias_test_command(self, message: Message) -> None:
+        self.send_chat_message("Call as alias!")
+
+    # when using case-insensitive commands you may not use 
+    # any other command with the same name as any case-insensitive combination
+    # works with aliases
+    @TwitchIRCBot.command("case_insensitive", case_sensitive=False)
+    async def case_insensitive_command(self, message: Message) -> None:
+        self.send_chat_message("Case insensitive")
+
     # repeat a task
     # runs once the client is ready and after the specified time interval
     # here 1000s
     @TwitchIRCBot.loop(1000)
     async def my_task(self):
         logger.info("Hello World")
 
+    # repeat a task at given time
+    # is 1 second delayed to prevent double trigger inaccuracies
+    @TwitchIRCBot.loop(time="08:36")
+    async def my_timed_task(self):
+        logger.info("Hello World at 08:36")
+
 
 if __name__ == "__main__":
     MyBot(oauth_token="YOURTOKEN", nick_name="BOTNAME", channel="CHANNELNAME").run()
 
 
 ```
```

### Comparing `AsyncIRCClient-0.0.7/async_irc_client/async_irc_client.py` & `AsyncIRCClient-0.0.8/async_irc_client/async_irc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,14 +308,22 @@
         """
         restart timer
         :return: None
         """
         self.cancel()
         self.start()
 
+    def set_timeout(self, timeout: int) -> None:
+        """
+        set timer timeout.
+        :param timeout: timeout
+        :return: None
+        """
+        self._timeout = timeout
+
 
 class AsyncIRCClientProtocol(asyncio.Protocol):
 
     def __init__(self, on_connection_made: Union[Callable, None] = None,
                  on_connection_lost: Union[Callable, None] = None, on_data_received: Union[Callable, None] = None):
         """
         protocol constructor
@@ -560,14 +568,17 @@
 
     async def on_client_joined(self, message: Message) -> None:
         """called when client joined (JOIN)"""
 
     async def on_user_join(self, message: Message) -> None:
         """called if any user joins the channel (JOIN)"""
 
+    async def on_client_left(self, message: Message) -> None:
+        """called when client left (PART)"""
+
     async def on_user_left(self, message: Message) -> None:
         """called on user leaves or gets banned (PART)"""
 
     async def on_irc_capabilities(self, message: Message) -> None:
         """called when receiving command and tag capabilities (CAP) """
 
     async def on_user_state(self, message: Message) -> None:
@@ -711,24 +722,24 @@
                 :return: None
                 """
                 if wait_first:
                     while True:
                         if time is None:
                             await asyncio.sleep(seconds)
                         else:
-                            await asyncio.sleep(get_time_difference(time))
+                            await asyncio.sleep(get_time_difference(time) + 1)
                         await function(*args, **kwargs)
                 else:
                     while True:
                         await function(*args, **kwargs)
 
                         if time is None:
                             await asyncio.sleep(seconds)
                         else:
-                            await asyncio.sleep(get_time_difference(time))
+                            await asyncio.sleep(get_time_difference(time) + 1)
 
             TwitchIRCBot.tasks.append(wrapper)
 
             return wrapper
 
         return decorator
 
@@ -894,14 +905,17 @@
                 elif parsed_message.parameters == "twitch.tv/commands":
                     self._has_commands = True
                 callback = self.on_irc_capabilities
 
             case "JOIN":
                 callback = self.on_client_joined if parsed_message.source.nick == self._nick_name else self.on_user_join
 
+            case "PART":
+                callback = self.on_client_left if parsed_message.source.nick == self._nick_name else self.on_user_left
+
             case "NOTICE":
                 callback = self.on_notice
 
             case "CLEARCHAT":
                 callback = self.on_clear_chat
 
             case "HOSTTARGET":
```

