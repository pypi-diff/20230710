# Comparing `tmp/gustavselfbot-0.0.1.tar.gz` & `tmp/gustavselfbot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gustavselfbot-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gustavselfbot-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gustavselfbot-0.0.1.tar` & `gustavselfbot-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     3185 2023-07-10 21:22:00.617362 gustavselfbot-0.0.1/.gitignore
--rw-r--r--   0        0        0      205 2023-07-10 20:59:21.677937 gustavselfbot-0.0.1/GustavSelfBot/Commands/Functions/__init__.py
--rw-r--r--   0        0        0     1997 2023-07-10 17:55:43.890956 gustavselfbot-0.0.1/GustavSelfBot/Commands/Functions/__ping__.py
--rw-r--r--   0        0        0     3980 2023-07-10 17:55:43.887623 gustavselfbot-0.0.1/GustavSelfBot/Commands/Functions/__quote__.py
--rw-r--r--   0        0        0     1018 2023-07-10 20:59:21.684604 gustavselfbot-0.0.1/GustavSelfBot/Commands/__commands__.py
--rw-r--r--   0        0        0      126 2023-07-10 20:59:21.681270 gustavselfbot-0.0.1/GustavSelfBot/Commands/__init__.py
--rw-r--r--   0        0        0      276 2023-07-10 20:59:21.691270 gustavselfbot-0.0.1/GustavSelfBot/Events/__init__.py
--rw-r--r--   0        0        0     1715 2023-07-10 21:00:11.519135 gustavselfbot-0.0.1/GustavSelfBot/Events/__on_message__.py
--rw-r--r--   0        0        0      184 2023-07-10 18:12:52.724373 gustavselfbot-0.0.1/GustavSelfBot/Events/__on_ready__.py
--rw-r--r--   0        0        0     4232 2023-07-10 20:16:27.414951 gustavselfbot-0.0.1/GustavSelfBot/Events/__on_voice_state_update__.py
--rw-r--r--   0        0        0      654 2023-07-10 20:59:21.697937 gustavselfbot-0.0.1/GustavSelfBot/__bot__.py
--rw-r--r--   0        0        0      265 2023-07-10 21:07:11.012427 gustavselfbot-0.0.1/GustavSelfBot/__config__.py
--rw-r--r--   0        0        0      305 2023-07-10 21:19:07.142511 gustavselfbot-0.0.1/GustavSelfBot/__init__.py
--rw-r--r--   0        0        0     1489 2023-07-10 21:07:11.009094 gustavselfbot-0.0.1/GustavSelfBot/__logging__.py
--rw-r--r--   0        0        0        0 2023-07-10 21:15:47.984536 gustavselfbot-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2023-07-10 21:15:37.160950 gustavselfbot-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.1/_chatlogs/PLACEHOLDER
--rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.1/_recordings/PLACEHOLDER
--rw-r--r--   0        0        0       87 2023-07-10 12:32:13.422010 gustavselfbot-0.0.1/config.json
--rw-r--r--   0        0        0      474 2023-07-10 21:14:15.379041 gustavselfbot-0.0.1/main.py
--rw-r--r--   0        0        0      568 2023-07-10 21:19:07.135844 gustavselfbot-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       42 2023-07-10 21:14:57.950035 gustavselfbot-0.0.1/requirements.txt
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 gustavselfbot-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3185 2023-07-10 21:22:00.617362 gustavselfbot-0.0.2/.gitignore
+-rw-r--r--   0        0        0      380 2023-07-10 21:34:48.787151 gustavselfbot-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      205 2023-07-10 20:59:21.677937 gustavselfbot-0.0.2/GustavSelfBot/Commands/Functions/__init__.py
+-rw-r--r--   0        0        0     1997 2023-07-10 17:55:43.890956 gustavselfbot-0.0.2/GustavSelfBot/Commands/Functions/__ping__.py
+-rw-r--r--   0        0        0     3788 2023-07-10 21:32:30.543724 gustavselfbot-0.0.2/GustavSelfBot/Commands/Functions/__quote__.py
+-rw-r--r--   0        0        0     1017 2023-07-10 21:32:30.510390 gustavselfbot-0.0.2/GustavSelfBot/Commands/__commands__.py
+-rw-r--r--   0        0        0      126 2023-07-10 20:59:21.681270 gustavselfbot-0.0.2/GustavSelfBot/Commands/__init__.py
+-rw-r--r--   0        0        0      276 2023-07-10 20:59:21.691270 gustavselfbot-0.0.2/GustavSelfBot/Events/__init__.py
+-rw-r--r--   0        0        0     1685 2023-07-10 21:32:30.550391 gustavselfbot-0.0.2/GustavSelfBot/Events/__on_message__.py
+-rw-r--r--   0        0        0      184 2023-07-10 18:12:52.724373 gustavselfbot-0.0.2/GustavSelfBot/Events/__on_ready__.py
+-rw-r--r--   0        0        0     4233 2023-07-10 21:32:30.503723 gustavselfbot-0.0.2/GustavSelfBot/Events/__on_voice_state_update__.py
+-rw-r--r--   0        0        0      655 2023-07-10 21:32:30.520390 gustavselfbot-0.0.2/GustavSelfBot/__bot__.py
+-rw-r--r--   0        0        0      265 2023-07-10 21:07:11.012427 gustavselfbot-0.0.2/GustavSelfBot/__config__.py
+-rw-r--r--   0        0        0      305 2023-07-10 21:36:09.392468 gustavselfbot-0.0.2/GustavSelfBot/__init__.py
+-rw-r--r--   0        0        0     1489 2023-07-10 21:07:11.009094 gustavselfbot-0.0.2/GustavSelfBot/__logging__.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:15:47.984536 gustavselfbot-0.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-10 21:15:37.160950 gustavselfbot-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.2/_chatlogs/PLACEHOLDER
+-rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.2/_recordings/PLACEHOLDER
+-rw-r--r--   0        0        0       87 2023-07-10 12:32:13.422010 gustavselfbot-0.0.2/config.json
+-rw-r--r--   0        0        0      474 2023-07-10 21:14:15.379041 gustavselfbot-0.0.2/main.py
+-rw-r--r--   0        0        0      613 2023-07-10 21:32:16.773381 gustavselfbot-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-07-10 21:31:18.695261 gustavselfbot-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 gustavselfbot-0.0.2/PKG-INFO
```

### Comparing `gustavselfbot-0.0.1/.gitignore` & `gustavselfbot-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.1/GustavSelfBot/Commands/Functions/__ping__.py` & `gustavselfbot-0.0.2/GustavSelfBot/Commands/Functions/__ping__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.1/GustavSelfBot/Commands/Functions/__quote__.py` & `gustavselfbot-0.0.2/GustavSelfBot/Commands/Functions/__quote__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,45 +5,37 @@
 from discord.ext import commands
 
 
 async def func_quote(bot: commands.Bot, ctx: commands.Context, message: discord.Message):
     async with aiohttp.ClientSession() as session:
         try:
             async with session.get(
-                    url="https://clashy-besi.ddns.net/api/quote",
-                    headers={"Accept": "application/json"},
+                url="https://clashy-besi.ddns.net/api/quote",
+                headers={"Accept": "application/json"},
             ) as resp:
                 if resp.status == 200:
                     res = await resp.json()
                     quote = res.get("text")
                     author = res.get("author")
 
                     if quote and author:
                         encoded_quote = urllib.parse.quote(quote)
                         encoded_author = urllib.parse.quote(author)
 
                         embed = f"https://embed.rauf.workers.dev/?author={encoded_author}&title=Quote%21&description={encoded_quote}&color=241f31&redirect=https%253A%252F%252Fclashy-besi.ddns.net%252Fapi%252Fquote"
                     else:
-                        encoded_author = urllib.parse.quote(
-                            bot.user.display_name
-                        )
-                        error_description = urllib.parse.quote(
-                            "An error has occurred while processing the response."
-                        )
+                        encoded_author = urllib.parse.quote(bot.user.display_name)
+                        error_description = urllib.parse.quote("An error has occurred while processing the response.")
                         embed = f"https://embed.rauf.workers.dev/?author={encoded_author}&title=Error%21&description={error_description}&color=a51d2d&redirect=https%253A%252F%252Fclashy-besi.ddns.net%252Fapi%252Fquote"
                 else:
                     encoded_author = urllib.parse.quote(bot.user.display_name)
-                    error_description = urllib.parse.quote(
-                        "An error has occurred while handling the request."
-                    )
+                    error_description = urllib.parse.quote("An error has occurred while handling the request.")
                     embed = f"https://embed.rauf.workers.dev/?author={encoded_author}&title=Error%21&description={error_description}&color=a51d2d&redirect=https%253A%252F%252Fclashy-besi.ddns.net%252Fapi%252Fquote"
         except aiohttp.ClientError:
             encoded_author = urllib.parse.quote(bot.user.display_name)
-            error_description = urllib.parse.quote(
-                "An error has occurred while processing the request."
-            )
+            error_description = urllib.parse.quote("An error has occurred while processing the request.")
             embed = f"https://embed.rauf.workers.dev/?author={encoded_author}&title=Error%21&description={error_description}&color=a51d2d&redirect=https%253A%252F%252Fclashy-besi.ddns.net%252Fapi%252Fquote"
 
         test = f"||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​|||||||||||| {embed}"
 
         await message.add_reaction("👍")
         await message.reply(content=test)
```

### Comparing `gustavselfbot-0.0.1/GustavSelfBot/Commands/__commands__.py` & `gustavselfbot-0.0.2/GustavSelfBot/Commands/__commands__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,7 @@
     log.info(f"Command {message.content.replace('>', '')} called by {ctx.author.display_name} (ID: {ctx.author.id})")
     try:
         await func_quote(bot, ctx, message)
     except discord.errors.ClientException as e:
         log.error(e)
         await ctx.send("Error")
         raise Exception(e)
-
```

### Comparing `gustavselfbot-0.0.1/GustavSelfBot/Events/__on_message__.py` & `gustavselfbot-0.0.2/GustavSelfBot/Events/__on_message__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 
 
 async def func_on_message(bot: commands.Bot, message: discord.Message):
     if bot.user in message.mentions:
         if message.author.id == bot.user.id:
             return
         else:
-            log.info(
-                f"Message received from {message.author.display_name} (ID: {message.author.id}): {message.content}"
-            )
+            log.info(f"Message received from {message.author.display_name} (ID: {message.author.id}): {message.content}")
 
     if message.content.startswith(">"):
         if message.author.id != bot.user.id:
             return
         if message.author.id == bot.user.id:
             if message.content.__contains__("|") or message.content.__contains__("||"):
                 return
```

### Comparing `gustavselfbot-0.0.1/GustavSelfBot/Events/__on_voice_state_update__.py` & `gustavselfbot-0.0.2/GustavSelfBot/Events/__on_voice_state_update__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # import os
 # import asyncio
 import discord
 from discord.ext import commands
+
 # from datetime import datetime
 # from GustavSelfBot import log
 
 
 # async def save_recording(audio_source):
 #     # Save the recorded audio to an MP3 file with a unique filename
 #     timestamp = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
```

### Comparing `gustavselfbot-0.0.1/GustavSelfBot/__bot__.py` & `gustavselfbot-0.0.2/GustavSelfBot/__bot__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import discord
 from discord.ext import commands
 
 from GustavSelfBot import log
 
 from GustavSelfBot.Events import func_on_message
 from GustavSelfBot.Events import func_on_ready
+
 # from GustavSelfBot.Events import func_on_voice_state_update
 
-bot = commands.Bot(command_prefix='>', self_bot=True)
+bot = commands.Bot(command_prefix=">", self_bot=True)
 
 
 @bot.event
 async def on_ready():
     await func_on_ready(bot)
```

### Comparing `gustavselfbot-0.0.1/GustavSelfBot/__logging__.py` & `gustavselfbot-0.0.2/GustavSelfBot/__logging__.py`

 * *Files identical despite different names*

