# Comparing `tmp/twitch-archiver-3.0.4.tar.gz` & `tmp/twitch-archiver-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch-archiver-3.0.4.tar", last modified: Mon May  8 13:49:20 2023, max compression
+gzip compressed data, was "twitch-archiver-3.0.5.tar", last modified: Mon Jul 10 06:43:57 2023, max compression
```

## Comparing `twitch-archiver-3.0.4.tar` & `twitch-archiver-3.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:49:20.532226 twitch-archiver-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-08 13:49:20.532226 twitch-archiver-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:49:20.532226 twitch-archiver-3.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:49:20.528226 twitch-archiver-3.0.4/twitch_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-08 13:49:20.000000 twitch-archiver-3.0.4/twitch_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-08 13:49:20.000000 twitch-archiver-3.0.4/twitch_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:49:20.000000 twitch-archiver-3.0.4/twitch_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-08 13:49:20.000000 twitch-archiver-3.0.4/twitch_archiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 13:49:20.000000 twitch-archiver-3.0.4/twitch_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 13:49:20.000000 twitch-archiver-3.0.4/twitch_archiver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:49:20.528226 twitch-archiver-3.0.4/twitcharchiver/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    10322 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    40439 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)    25839 2023-05-08 13:49:09.000000 twitch-archiver-3.0.4/twitcharchiver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:43:57.172767 twitch-archiver-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-10 06:43:47.000000 twitch-archiver-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-07-10 06:43:57.172767 twitch-archiver-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-07-10 06:43:47.000000 twitch-archiver-3.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-10 06:43:47.000000 twitch-archiver-3.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 06:43:57.172767 twitch-archiver-3.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:43:57.168767 twitch-archiver-3.0.5/twitch_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-07-10 06:43:57.000000 twitch-archiver-3.0.5/twitch_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-10 06:43:57.000000 twitch-archiver-3.0.5/twitch_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:43:57.000000 twitch-archiver-3.0.5/twitch_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 06:43:57.000000 twitch-archiver-3.0.5/twitch_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 06:43:57.000000 twitch-archiver-3.0.5/twitch_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 06:43:57.000000 twitch-archiver-3.0.5/twitch_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:43:57.172767 twitch-archiver-3.0.5/twitcharchiver/
+-rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-07-10 06:43:47.000000 twitch-archiver-3.0.5/twitcharchiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-10 06:43:47.000000 twitch-archiver-3.0.5/twitcharchiver/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-10 06:43:47.000000 twitch-archiver-3.0.5/twitcharchiver/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-10 06:43:47.000000 twitch-archiver-3.0.5/twitcharchiver/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-07-10 06:43:47.000000 twitch-archiver-3.0.5/twitcharchiver/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-07-10 06:43:47.000000 twitch-archiver-3.0.5/twitcharchiver/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-10 06:43:47.000000 twitch-archiver-3.0.5/twitcharchiver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-10 06:43:47.000000 twitch-archiver-3.0.5/twitcharchiver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40937 2023-07-10 06:43:47.000000 twitch-archiver-3.0.5/twitcharchiver/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-07-10 06:43:47.000000 twitch-archiver-3.0.5/twitcharchiver/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-07-10 06:43:47.000000 twitch-archiver-3.0.5/twitcharchiver/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25849 2023-07-10 06:43:47.000000 twitch-archiver-3.0.5/twitcharchiver/utils.py
```

### Comparing `twitch-archiver-3.0.4/LICENSE` & `twitch-archiver-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.4/PKG-INFO` & `twitch-archiver-3.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-archiver
-Version: 3.0.4
+Version: 3.0.5
 Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
 Author-email: Brisppy <brisppy@protonmail.com>
 Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
 Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `twitch-archiver-3.0.4/README.md` & `twitch-archiver-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.4/pyproject.toml` & `twitch-archiver-3.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "twitch-archiver"
-version = "3.0.4"
+version = "3.0.5"
 dependencies = [
     "requests>=2.25.1",
     "m3u8>=0.3.12",
 ]
 authors = [
   { name="Brisppy", email="brisppy@protonmail.com" },
 ]
```

### Comparing `twitch-archiver-3.0.4/twitch_archiver.egg-info/PKG-INFO` & `twitch-archiver-3.0.5/twitch_archiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-archiver
-Version: 3.0.4
+Version: 3.0.5
 Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
 Author-email: Brisppy <brisppy@protonmail.com>
 Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
 Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `twitch-archiver-3.0.4/twitch_archiver.egg-info/SOURCES.txt` & `twitch-archiver-3.0.5/twitch_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.4/twitcharchiver/__init__.py` & `twitch-archiver-3.0.5/twitcharchiver/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,28 +26,29 @@
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import argparse
 import os
 import sys
+import tempfile
 import textwrap
 
 from pathlib import Path
 from time import sleep
 
 from twitcharchiver.arguments import Arguments
 from twitcharchiver.configuration import Configuration
 from twitcharchiver.exceptions import TwitchAPIError
 from twitcharchiver.logger import Logger
 from twitcharchiver.processing import Processing
 from twitcharchiver.twitch import Twitch
 from twitcharchiver.utils import getenv, send_push, get_latest_version, version_tuple, check_update_available
 
-__version__ = '3.0.4'
+__version__ = '3.0.5'
 
 
 def main():
     """
     Main processing for twitch-archiver.
     """
     parser = argparse.ArgumentParser(argument_default=None, description=textwrap.dedent(f"""\
@@ -160,14 +161,17 @@
     config.load_config(Path(args.get('config_dir'), 'config.ini'))
     log.debug('Settings prior to loading config: %s', config.get_sanitized())
 
     # overwrite different or missing configuration variables
     config.generate_config(args.get())
     log.debug('Settings after loading config: %s', config.get_sanitized())
 
+    # create temp dir for downloads and lock files
+    Path(tempfile.gettempdir(), 'twitch-archiver').mkdir(exist_ok=True)
+
     # prompt if client id or secret empty
     if config.get('client_id') == '' or config.get('client_secret') == '':
         log.info('No client_id or client_secret passed as argument or found in config file.')
         config.set('client_id', input('Your client ID: '))
         config.set('client_secret', input('Your client secret: '))
 
     log.debug('Performing Twitch authentication.')
```

### Comparing `twitch-archiver-3.0.4/twitcharchiver/api.py` & `twitch-archiver-3.0.5/twitcharchiver/api.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.4/twitcharchiver/arguments.py` & `twitch-archiver-3.0.5/twitcharchiver/arguments.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.4/twitcharchiver/configuration.py` & `twitch-archiver-3.0.5/twitcharchiver/configuration.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.4/twitcharchiver/database.py` & `twitch-archiver-3.0.5/twitcharchiver/database.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.4/twitcharchiver/downloader.py` & `twitch-archiver-3.0.5/twitcharchiver/downloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
         # files are downloaded to $TMP, then moved to final destination
         # takes 3:32 to download an hour long VOD to NAS, compared to 5:00 without using $TMP as download cache
         #   a better method would be to have 20 workers downloading, and 20 moving temp
         #   files from storage avoiding any downtime downloading
 
         # create temporary file for downloading to
-        with open(Path(tempfile.gettempdir(), os.urandom(24).hex()), 'wb') as tmp_ts_file:
+        with open(Path(tempfile.gettempdir(), 'twitch-archiver', os.urandom(24).hex()), 'wb') as tmp_ts_file:
             for _ in range(6):
                 if _ > 4:
                     self.log.debug('Maximum retries for segment %s reached.', Path(ts_path).stem)
                     return {1, f'Maximum retries for segment {Path(ts_path).stem} reached.'}
 
                 try:
                     _r = requests.get(ts_url, stream=True, timeout=10)
@@ -164,96 +164,88 @@
 
         return False
 
     def get_chat(self, vod_json, offset=0):
         """Downloads the chat for a specified VOD, returning comments beginning from offset (if provided).
 
         :param vod_json: dict of vod information
-        :param offset: offset in seconds to begin chat retrieval from
+        :param offset: offset in seconds to begin chat retrieval from - none to begin at start
         """
         chat_log = []
-        message_ids = set()
-        prev_page = None
 
         _s = requests.session()
-        _s.headers.update({'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'})
+        _s.headers.update({'Client-Id': 'ue6666qo983tsx6so1t0vnawi233wa'})
 
         # grab initial chat segment containing cursor
-        initial_segment, next_page = self.get_chat_segment(_s, vod_json['vod_id'], offset)
+        initial_segment, cursor = self.get_chat_segment(_s, vod_json['vod_id'], offset=offset)
         chat_log.extend(initial_segment)
-        message_ids.update([m['id'] for m in chat_log])
-        offset = chat_log[-1]['contentOffsetSeconds']
 
         progress = Progress()
 
-        # we use the contentOffset of the last comment grabbed as a rudimentary cursor as Twitch severely restricted
-        # access to the GQL API by implementing 'kasadas' which is far more work to try and bypass than I feel is worth
-        while offset <= vod_json['duration'] and next_page:
-            # break infinite loops
-            if offset == prev_page:
-                offset += 1
-                continue
-
-            prev_page = offset
+        while True:
+            if not cursor:
+                break
 
             try:
-                # grab next chat segment based on offset
-                segment, next_page = self.get_chat_segment(_s, vod_json['vod_id'], offset)
-                chat_log.extend([m for m in segment if m['id'] not in message_ids])
-                message_ids.update([m['id'] for m in chat_log])
-
+                # grab next chat segment along with cursor for next segment
+                segment, cursor = self.get_chat_segment(_s, vod_json['vod_id'], cursor=cursor)
+                chat_log.extend(segment)
                 # vod duration in seconds is used as the total for progress bar
                 # comment offset is used to track what's been done
                 # could be done properly if there was a way to get the total number of comments
                 if not self.quiet:
                     progress.print_progress(int(segment[-1]['contentOffsetSeconds']),
-                                            vod_json['duration'], not offset)
-
-                # move cursor to offset of most recent message, or increment
-                if chat_log[-1]['contentOffsetSeconds'] > offset:
-                    offset = chat_log[-1]['contentOffsetSeconds']
-
-                else:
-                    offset += 1
+                                            vod_json['duration'], not cursor)
 
             except TwitchAPIErrorNotFound:
                 break
 
-        _s.close()
+            finally:
+                _s.close()
 
         self.log.info('Found %s messages.', len(chat_log))
 
         return chat_log
 
-    def get_chat_segment(self, session, vod_id, offset):
+    def get_chat_segment(self, session, vod_id, offset=None, cursor=None):
         """Retrieves a single chat segment.
 
         :param session: requests session to link request to
         :param vod_id: id of vod to retrieve segment from
         :param offset: offset in seconds to begin retrieval from
+        :param cursor: cursor returned by a previous call of this function
         :return: list of comments and cursor if one is returned from twitch
-        :return: True if more pages available
         """
         # build payload
-        _p = [{"operationName": "VideoCommentsByOffsetOrCursor",
-               "variables": {"videoID": vod_id, "contentOffsetSeconds": offset}}]
+        if offset is not None:
+            _p = [{"operationName": "VideoCommentsByOffsetOrCursor",
+                   "variables": {"videoID": vod_id, "contentOffsetSeconds": offset}}]
+
+        else:
+            _p = [{"operationName": "VideoCommentsByOffsetOrCursor",
+                   "variables": {"videoID": vod_id, "cursor": cursor}}]
 
-        _p[0]['extensions'] = \
+        _p[0]['extensions'] =\
             {'persistedQuery': {'version': 1,
                                 'sha256Hash': "b70a3591ff0f4e0313d126c6a1502d79a1c02baebb288227c582044aa76adf6a"}}
 
         for attempt in range(6):
             if attempt > 4:
-                self.log.error('Maximum attempts reached while downloading chat segment at offset: %s.', offset)
+                self.log.error('Maximum attempts reached while downloading chat segment at cursor or offset: %s, %s.',
+                               cursor, offset)
                 raise ChatDownloadError
 
             try:
                 _r = Api.post_request_with_session('https://gql.twitch.tv/gql', session, _p).json()
 
             except RequestError:
                 continue
 
             break
 
         comments = _r[0]['data']['video']['comments']
 
-        return [c['node'] for c in comments['edges']], comments['pageInfo']['hasNextPage']
+        # check if next page exists
+        if comments['pageInfo']['hasNextPage']:
+            return [c['node'] for c in comments['edges']], comments['edges'][-1]['cursor']
+
+        return [c['node'] for c in comments['edges']], None
```

### Comparing `twitch-archiver-3.0.4/twitcharchiver/exceptions.py` & `twitch-archiver-3.0.5/twitcharchiver/exceptions.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.4/twitcharchiver/logger.py` & `twitch-archiver-3.0.5/twitcharchiver/logger.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.4/twitcharchiver/processing.py` & `twitch-archiver-3.0.5/twitcharchiver/processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 import json
 import logging
 import multiprocessing
 import os
 import re
+import signal
 import shutil
 import sys
 import tempfile
 
 from datetime import datetime, timezone
 from glob import glob
 from math import floor
@@ -57,29 +58,33 @@
         self.oauth_token = config['oauth_token']
 
         self.pushbullet_key = config['pushbullet_key']
 
         self.call_twitch = Twitch(self.client_id, self.client_secret, self.oauth_token)
         self.download = Downloader(self.client_id, self.oauth_token, args['threads'], args['quiet'])
 
+        # create signal handler for graceful removal of lock files
+        signal.signal(signal.SIGTERM, signal.default_int_handler)
+
     def get_channel(self, channels):
         """
         Download all vods from a specified channel or list of channels.
         """
         for channel in channels:
             self.log.info("Now archiving channel '%s'.", channel)
             self.log.debug('Fetching user data from Twitch.')
 
             user_data = self.call_twitch.get_api(f'users?login={channel}')['data'][0]
             user_id = user_data['id']
             user_name = user_data['display_name']
+            available_vods = {}
 
             channel_live = False
             stream = Stream(self.client_id, self.client_secret, self.oauth_token)
-            tmp_buffer_dir = Path(tempfile.gettempdir(), os.urandom(24).hex())
+            tmp_buffer_dir = Path(tempfile.gettempdir(), 'twitch-archiver', os.urandom(24).hex())
 
             self.vod_directory = Path(self.directory, user_name)
 
             # setup database
             with Database(Path(self.config_dir, 'vods.db')) as db:
                 # check db version
                 version = db.execute_query('pragma user_version')[0][0]
@@ -109,44 +114,53 @@
                 channel_live = True
                 # ensure enough time has passed for vod api to update before archiving
                 stream_length = time_since_date(datetime.strptime(
                     channel_data[0]['started_at'], '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc).timestamp())
 
                 self.log.debug('Current stream length: %s', stream_length)
 
+                # fetch broadcast vod id
+                latest_vod_id = self.call_twitch.get_live_broadcast_vod_id(channel)
+                if latest_vod_id:
+                    available_vods.update({int(channel_data[0]['id']): latest_vod_id})
+
                 # while we wait for the api to update we must build a temporary buffer of any parts advertised in the
                 # meantime in case there is no vod and thus no way to retrieve them after the fact
-                if stream_length < 300:
-                    self.log.debug('Stream began less than 5m ago, delaying archival start until VOD API updated.')
+                elif stream_length < 60:
+                    self.log.debug('Stream began less than 60s ago, delaying archival start until VOD API updated.')
                     # create temp dir for buffer
                     Path(tmp_buffer_dir).mkdir(parents=True, exist_ok=True)
 
                     stream.unsynced_setup(tmp_buffer_dir)
                     index_uri = self.call_twitch.get_channel_hls_index(channel, self.quality)
 
                     # download new parts every 4s
-                    for i in range(int((300 - stream_length) / 4)):
+                    for i in range(int((60 - stream_length) / 4)):
                         # grab required values
                         start_timestamp = int(datetime.utcnow().timestamp())
                         incoming_segments = m3u8.loads(Api.get_request(index_uri).text).data
 
                         # create buffer and download segments to temp dir
                         stream.build_unsynced_buffer(incoming_segments)
                         stream.download_buffer(tmp_buffer_dir)
 
                         # wait if less than 5s passed since grabbing more parts
                         processing_time = int(datetime.utcnow().timestamp() - start_timestamp)
                         if processing_time < 4:
                             sleep(4 - processing_time)
 
                     # wait any remaining time
-                    sleep((300 - stream_length) % 4)
+                    sleep((60 - stream_length) % 4)
+
+                    # fetch broadcast vod id again
+                    latest_vod_id = self.call_twitch.get_live_broadcast_vod_id(channel)
+                    if latest_vod_id:
+                        available_vods.update({int(channel_data[0]['id']): latest_vod_id})
 
             # retrieve available vods
-            available_vods: dict[int: tuple[int]] = {}
             cursor = ''
             try:
                 while True:
                     _r = self.call_twitch.get_api(f'videos?user_id={user_id}&first=100&type=archive&after={cursor}')
                     if not _r['pagination']:
                         break
 
@@ -203,67 +217,67 @@
 
             # archive stream in non-segmented mode if no paired vod exists, unless we are in no_stream mode or not
             # archiving video.
             if not self.archive_only and channel_live and not live_vod_exists and self.video:
                 self.log.info('Channel live but not being archived to a VOD, running stream archiver.')
                 self.log.debug('Creating lock file for stream.')
 
-                if create_lock(self.config_dir, channel_data[0]['id'] + '-stream-only'):
+                if create_lock(Path(tempfile.gettempdir(), 'twitch-archiver'), channel_data[0]['id'] + '-stream-only'):
                     self.log.info('Lock file present for stream by %s (.lock.%s-stream-only), skipping.',
                                   user_name, channel_data[0]["id"])
+                    continue
+
+                # check if stream in database
+                with Database(Path(self.config_dir, 'vods.db')) as db:
+                    downloaded_streams = [str(i[0]) for i in db.execute_query(
+                        'SELECT stream_id FROM vods WHERE user_id IS ?', {'user_id': user_id})]
+
+                # Check if stream id in database
+                if channel_data[0]['id'] in downloaded_streams:
+                    self.log.info('Ignoring steam as it has already been downloaded.')
 
                 else:
-                    # check if stream in database
-                    with Database(Path(self.config_dir, 'vods.db')) as db:
-                        downloaded_streams = [str(i[0]) for i in db.execute_query(
-                            'SELECT stream_id FROM vods WHERE user_id IS ?', {'user_id': user_id})]
-
-                    # Check if stream id in database
-                    if channel_data[0]['id'] in downloaded_streams:
-                        self.log.info('Ignoring steam as it has already been downloaded.')
+                    try:
+                        # move parts from temp stream buffer to output dir
+                        # gather parts from temp dir
+                        buffered_parts = [Path(p) for p in sorted(glob(str(Path(tmp_buffer_dir, '*.ts'))))]
+                        # create output dir
+                        output_dir = \
+                            str(Path(self.vod_directory,
+                                     f"{sanitize_date(channel_data[0]['started_at'])} - "
+                                     f"{sanitize_text(channel_data[0]['title'])} - STREAM_ONLY", 'parts'))
+                        Path(output_dir).mkdir(parents=True, exist_ok=True)
+
+                        # move parts individually to destination dir
+                        for part in buffered_parts:
+                            dst_part = str(Path(part).name)
+                            safe_move(part, Path(output_dir, dst_part))
+
+                        stream_json = self.get_unsynced_stream(channel_data[0], stream)
+
+                        if stream_json:
+                            # add to database
+                            self.log.debug('Adding stream info to database.')
+                            with Database(Path(self.config_dir, 'vods.db')) as db:
+                                db.execute_query(CREATE_VOD, stream_json)
 
-                    else:
-                        try:
-                            # move parts from temp stream buffer to output dir
-                            # gather parts from temp dir
-                            buffered_parts = [Path(p) for p in sorted(glob(str(Path(tmp_buffer_dir, '*.ts'))))]
-                            # create output dir
-                            output_dir = \
-                                str(Path(self.vod_directory,
-                                         f"{sanitize_date(channel_data[0]['started_at'])} - "
-                                         f"{sanitize_text(channel_data[0]['title'])} - STREAM_ONLY", 'parts'))
-                            Path(output_dir).mkdir(parents=True, exist_ok=True)
-
-                            # move parts individually to destination dir
-                            for part in buffered_parts:
-                                dst_part = str(Path(part).name)
-                                safe_move(part, Path(output_dir, dst_part))
-
-                            stream_json = self.get_unsynced_stream(channel_data[0], stream)
-
-                            if stream_json:
-                                # add to database
-                                self.log.debug('Adding stream info to database.')
-                                with Database(Path(self.config_dir, 'vods.db')) as db:
-                                    db.execute_query(CREATE_VOD, stream_json)
+                        else:
+                            self.log.debug('No stream information returned to channel function, stream downloader'
+                                           ' exited with error.')
 
-                            else:
-                                self.log.debug('No stream information returned to channel function, stream downloader'
-                                               ' exited with error.')
+                    except BaseException as e:
+                        self.log.error('Exception encountered while archiving live-only stream by %s. Error: %s',
+                                       {user_name}, str(e))
+                        return
 
-                        except BaseException as e:
-                            self.log.error('Exception encountered while archiving live-only stream by %s. Error: %s',
-                                           {user_name}, str(e))
-                            return
-
-                        finally:
-                            # remove lock
-                            self.log.debug('Removing lock file.')
-                            if remove_lock(self.config_dir, channel_data[0]['id'] + '-stream-only'):
-                                raise UnlockingError(user_name, stream_id=channel_data[0]['id'])
+                    finally:
+                        # remove lock
+                        self.log.debug('Removing lock file.')
+                        if remove_lock(Path(tempfile.gettempdir(), 'twitch-archiver'), channel_data[0]['id'] + '-stream-only'):
+                            raise UnlockingError(user_name, stream_id=channel_data[0]['id'])
 
             # wipe stream buffer as stream has paired vod
             if Path(tmp_buffer_dir).exists():
                 shutil.rmtree(tmp_buffer_dir)
 
             # exit if vod queue empty
             if not vod_queue:
@@ -285,15 +299,15 @@
                 if channel_data and self.archive_only and stream_id == int(channel_data[0]['id']):
                     self.log.info('Skipping VOD as it is live and no-stream argument provided.')
                     continue
 
                 self.log.debug('Processing VOD %s by %s', vod_id, user_name)
                 self.log.debug('Creating lock file for VOD.')
 
-                if create_lock(self.config_dir, stream_id):
+                if create_lock(Path(tempfile.gettempdir(), 'twitch-archiver'), stream_id):
                     self.log.info('Lock file present for VOD %s (.lock.%s), skipping.', vod_id, stream_id)
                     continue
 
                 # check if vod in database
                 with Database(Path(self.config_dir, 'vods.db')) as db:
                     downloaded_vod = db.execute_query(
                         'SELECT vod_id, video_archived, chat_archived FROM vods WHERE stream_id IS ?',
@@ -334,15 +348,15 @@
 
                             else:
                                 db.execute_query(CREATE_VOD, vod_json)
 
                     finally:
                         # remove lock
                         self.log.debug('Removing lock file.')
-                        if remove_lock(self.config_dir, vod_json['stream_id']):
+                        if remove_lock(Path(tempfile.gettempdir(), 'twitch-archiver'), vod_json['stream_id']):
                             raise UnlockingError(vod_json['user_name'], vod_json['stream_id'], vod_id)
 
                 else:
                     self.log.debug('No VOD information returned to channel function, downloader exited with error.')
                     continue
 
     def get_unsynced_stream(self, channel_data, stream=None):
@@ -391,17 +405,17 @@
 
             self.log.debug('Cleaning up temporary files...')
             cleanup_vod_parts(stream_json['store_directory'])
 
             return stream_json
 
         except KeyboardInterrupt:
-            self.log.debug('User requested stop, halting stream downloader.')
-            if Path(self.config_dir, f'.lock.{channel_data["user_name"]}').exists():
-                remove_lock(self.config_dir, channel_data[0]['id'] + '-stream-only')
+            self.log.debug('Termination signal received, halting stream downloader.')
+            if remove_lock(Path(tempfile.gettempdir(), 'twitch-archiver'), stream_json['stream_id'] + '-stream-only'):
+                raise UnlockingError(stream_json['user_name'], stream_json['stream_id'])
 
             sys.exit(0)
 
         except (RequestError, VodMergeError) as e:
             self.log.debug('Exception downloading or merging stream.\n{e}', exc_info=True)
             send_push(self.pushbullet_key, 'Exception encountered while downloading or merging downloaded stream '
                                            f'by {channel_data["user_name"]}', str(e))
@@ -427,29 +441,29 @@
         vod_json['vod_id'] = vod_json.pop('id')
         vod_json['muted_segments'] = str(vod_json['muted_segments'])
         vod_json['store_directory'] = \
             str(Path(self.vod_directory, f'{sanitize_date(vod_json["created_at"])} - '
                                          f'{sanitize_text(vod_json["title"])} - {vod_id}'))
         vod_json['duration'] = convert_to_seconds(vod_json['duration'])
 
+        workers = []
+
         # get vod status
         vod_live = self.call_twitch.get_vod_status(vod_json['user_id'], vod_json['created_at'])
 
         self.log.info("VOD %s", 'currently or recently live. Running in LIVE mode.' if vod_live else 'offline.')
 
         _r = None
 
         try:
             # begin real-time archiver if VOD still live and real-time archiver enabled
             if self.real_time_archiver and vod_live:
                 stream = Stream(self.client_id, self.client_secret, self.oauth_token)
                 # concurrently grab live pieces and vod chunks
 
-                workers = []
-
                 # the stream module itself has no checks for what to download so this is done here
                 if get_video:
                     workers.append(multiprocessing.Process(target=stream.get_stream, args=(
                         vod_json['user_name'], Path(vod_json['store_directory'], 'parts'), self.quality)))
 
                 workers.append(multiprocessing.Process(target=self.get_vod, args=(
                     vod_json, get_video, get_chat, vod_live)))
@@ -593,37 +607,34 @@
                 # delete temporary .ts parts and merged.ts file
                 self.log.debug('Cleaning up temporary files...')
                 cleanup_vod_parts(vod_json['store_directory'])
 
         # catch user exiting and remove lock file
         except KeyboardInterrupt:
             if vod_live:
-                self.log.debug('User requested stop, terminating download workers...')
+                self.log.debug('Termination signal received, terminating download workers...')
                 for worker in workers:
                     worker.terminate()
                     worker.join()
 
-            if Path(self.config_dir, f'.lock.{vod_json["stream_id"]}').exists():
-                remove_lock(self.config_dir, vod_json['stream_id'])
+            if remove_lock(Path(tempfile.gettempdir(), 'twitch-archiver'), vod_json['stream_id']):
+                raise UnlockingError(vod_json['user_name'], vod_json['stream_id'], vod_id)
 
             sys.exit(0)
 
         # catch halting errors, send notification and remove lock file
         except (RequestError, VodDownloadError, ChatDownloadError, VodMergeError, ChatExportError) as e:
             if vod_live:
                 self.log.debug('Exception encountered, terminating download workers...')
                 for worker in workers:
                     worker.terminate()
                     worker.join()
 
             self.log.error('Error downloading VOD %s.', vod_id, exc_info=True)
             send_push(self.pushbullet_key, f'Error downloading VOD {vod_id} by {vod_json["user_name"]}', str(e))
-            # remove lock file if archiving channel
-            if Path(self.config_dir, f'.lock.{vod_json["stream_id"]}').exists():
-                remove_lock(self.config_dir, vod_json['stream_id'])
 
             # set to None so that channel function knows download failed
             vod_json = None
 
         # catch unhandled exceptions
         except BaseException as e:
             if vod_live:
@@ -631,15 +642,17 @@
                 for worker in workers:
                     worker.terminate()
                     worker.join()
 
             send_push(self.pushbullet_key, f'Exception encountered while downloading VOD {vod_id} by '
                                            f'{vod_json["user_name"]}', str(e))
             self.log.error('Exception encountered while downloading VOD %s.', vod_id, exc_info=True)
-            return
+
+            # set to None so that channel function knows download failed
+            vod_json = None
 
         # this is only used when archiving a channel
         return vod_json
 
     def get_vod(self, vod_json, get_video=True, get_chat=True, vod_live=False):
         """Retrieves a specified VOD.
 
@@ -658,16 +671,15 @@
             self.log.info('Waiting 5m to download initial VOD parts as it was created very recently. Live archiving '
                           'will still function.')
             sleep(300)
 
         if time_since_date(datetime.strptime(
                 vod_json['created_at'], '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc).timestamp()) \
                 < (vod_json['duration'] + 360):
-            self.log.debug('Time since VOD was created + its duration is a point in time < 10 minutes ago. '
-                           'Running in live mode in case not all parts are available yet.')
+            self.log.debug('Running in live mode as VOD has been updated in the last 10 minutes.')
             vod_live = True
 
         # import chat log if it has been partially downloaded
         try:
             with open(Path(vod_json['store_directory'], 'verbose_chat.json'), 'r', encoding='utf8') as chat_file:
                 chat_log = json.loads(chat_file.read())
```

### Comparing `twitch-archiver-3.0.4/twitcharchiver/stream.py` & `twitch-archiver-3.0.5/twitcharchiver/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
 
         :param segment_id: numbered segment to download
         :param output_dir: location to output segment to
         :param tmp_file: name of temporary file
         :param segment_parts: list of parts which make up the segment
         :return: True on error
         """
-        with open(Path(tempfile.gettempdir(), tmp_file), 'wb') as tmp_ts_file:
+        with open(Path(tempfile.gettempdir(), 'twitch-archiver', tmp_file), 'wb') as tmp_ts_file:
             for segment in segment_parts:
                 try:
                     _r = requests.get(segment[0], stream=True, timeout=5)
 
                     if _r.status_code != 200:
                         return True
 
@@ -265,15 +265,15 @@
                 except requests.exceptions.RequestException as e:
                     self.log.debug(
                         'Error downloading VOD stream segment %s : %s. Error: %s', segment_id, segment, str(e))
                     return True
 
         # move finished ts file to destination storage
         try:
-            safe_move(Path(tempfile.gettempdir(), tmp_file), Path(output_dir, str(f'{segment_id:05d}' + '.ts')))
+            safe_move(Path(tempfile.gettempdir(), 'twitch-archiver', tmp_file), Path(output_dir, str(f'{segment_id:05d}' + '.ts')))
             self.log.debug('Live segment: %s completed.', segment_id)
 
         except BaseException as e:
             self.log.debug('Exception while moving stream segment %s. Error: %s', segment_id, str(e))
             return True
 
         return False
```

### Comparing `twitch-archiver-3.0.4/twitcharchiver/twitch.py` & `twitch-archiver-3.0.5/twitcharchiver/twitch.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     def get_playback_access_token(vod_id):
         """Gets a playback access token for a specified vod.
 
         :param vod_id: id of vod to retrieve token for
         :return: playback access token
         """
         # only accepts the default client ID for non-authenticated clients
-        _h = {'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'}
+        _h = {'Client-Id': 'ue6666qo983tsx6so1t0vnawi233wa'}
         _q = """
         {{
             videoPlaybackAccessToken(
                 id: {vod_id},
                 params: {{
                     platform: "web",
                     playerBackend: "mediaplayer",
@@ -98,52 +98,42 @@
             }}
         }}
         """.format(vod_id=vod_id)
         _r = Api.post_request('https://gql.twitch.tv/gql', j={'query': _q}, h=_h)
 
         return _r.json()['data']['videoPlaybackAccessToken']
 
-    @staticmethod
-    def get_latest_channel_broadcast(channel):
-        """Retrieves most recent archived broadcast. More reliable than helix API for VODs created within the last
-        few seconds.
+    def get_live_broadcast_vod_id(self, channel):
+        """Fetches the paired VOD ID for the currently live broadcast.
 
-        :param channel: Name of Twitch channel/user
-        :return: set of most recent values of (stream_id, vod_id)
+        :param channel: name of channel
+        :return: vod id (if any returned)
         """
         # Uses default client header
-        _h = {'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'}
+        _h = {'Client-Id': 'ue6666qo983tsx6so1t0vnawi233wa'}
         _q = [{
-            "extensions": {
-                "persistedQuery": {
-                    "sha256Hash": "8afefb1ed16c4d8e20fa55024a7ed1727f63b6eca47d8d33a28500770bad8479",
-                    "version": 1
+                "extensions": {
+                    "persistedQuery": {
+                        "sha256Hash": "ac644fafd686f2cb0e3864075af7cf3bb33f4e0525bf84921b10eabaa4e048b5",
+                        "version": 1
+                    }
+                },
+                "operationName": "ChannelVideoLength",
+                "variables": {
+                    "channelLogin": f"{channel.lower()}",
                 }
-            },
-            "operationName": "ChannelVideoShelvesQuery",
-            "variables": {
-                "channelLogin": f"{channel.lower()}",
-                "first": 5,
-            }
-        }]
+            }]
 
         _r = Api.post_request('https://gql.twitch.tv/gql', j=_q, h=_h)
-        _d = _r.json()[0]['data']['user']['videoShelves']['edges']
+        channel_video_length = _r.json()[0]['data']['user']['videos']['edges']
 
-        # extract vod and stream ids from thumbnail url (stream id isnt provided with this call) and add to id list.
-        # _d will be empty if no archives available.
-        if _d:
-            # iter over edges as the order may change, or LATEST_BROADCASTS not provided if none found
-            for edge in _d:
-                if edge['node']['type'] == 'LATEST_BROADCASTS':
-                    _thumbnail_url = edge['node']['items'][0]['animatedPreviewURL'].split('/')
-                    _id = (_thumbnail_url[3].split('_')[2], _thumbnail_url[5].split('-')[0])
-                    return _id
+        if channel_video_length:
+            return channel_video_length[0]['node']['id']
 
-        return
+        self.log.debug('No data returned by ChannelVideoLength API.')
 
     def get_vod_index(self, vod_json, quality='best'):
         """Retrieves an index of m3u8 streams for a given VOD.
 
         :param vod_json: vod information retrieved from Twitch
         :param quality: desired quality in the format [resolution]p[framerate] or 'best', 'worst'
         :return: url of m3u8 playlist
@@ -230,15 +220,15 @@
     def get_stream_playback_access_token(channel):
         """Gets a stream access token for a specified channel.
 
         :param channel: channel name to retrieve token for
         :return: playback access token
         """
         # only accepts the default client ID for non-authenticated clients
-        _h = {'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'}
+        _h = {'Client-Id': 'ue6666qo983tsx6so1t0vnawi233wa'}
         _q = """
         {{
             streamPlaybackAccessToken(
                 channelName: "{channel}",
                 params: {{
                     platform: "web",
                     playerBackend: "mediaplayer",
@@ -257,15 +247,15 @@
     @staticmethod
     def get_vod_category(vod_id):
         """Retrieves category for a specified VOD.
 
         :param vod_id: id of twitch vod to retrieve information for
         :return: name of category / game
         """
-        _h = {'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'}
+        _h = {'Client-Id': 'ue6666qo983tsx6so1t0vnawi233wa'}
         _q = [{
             "extensions": {
                 "persistedQuery": {
                     "sha256Hash": "e1edae8122517d013405f237ffcc124515dc6ded82480a88daef69c83b53ac01",
                     "version": 1
                 }
             },
@@ -315,15 +305,15 @@
     @staticmethod
     def get_vod_chapters(vod_id):
         """Retrieves the chapters for a given Twitch VOD.
 
         :param vod_id: id of twitch vod to retrieve chapters for
         :return: list of vod chapters
         """
-        _h = {'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'}
+        _h = {'Client-Id': 'ue6666qo983tsx6so1t0vnawi233wa'}
         _q = [{
             "extensions": {
                 "persistedQuery": {
                     "sha256Hash": "8d2793384aac3773beab5e59bd5d6f585aedb923d292800119e03d40cd0f9b41",
                     "version": 1
                 }
             },
```

### Comparing `twitch-archiver-3.0.4/twitcharchiver/utils.py` & `twitch-archiver-3.0.5/twitcharchiver/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,39 +382,39 @@
     """
     minutes = seconds // 60
     hours = minutes // 60
 
     return f"{hours:02d}h{minutes % 60:02d}m{seconds % 60:02d}s"
 
 
-def create_lock(ini_path, vod_id):
+def create_lock(lock_dir, vod_id):
     """Creates a lock file for a given VOD.
 
-    :param ini_path: path to config directory
+    :param lock_dir: path to directory with lock file
     :param vod_id: id of vod which lock file is created for
     :return: true if lock file creation fails
     """
     try:
-        with open(Path(ini_path, f'.lock.{vod_id}'), 'x', encoding='utf8') as _:
+        with open(Path(lock_dir, f'.lock.{vod_id}'), 'x', encoding='utf8') as _:
             pass
         return
 
     except FileExistsError:
         return True
 
 
-def remove_lock(config_dir, vod_id):
+def remove_lock(lock_dir, vod_id):
     """Removes a given lock file.
 
-    :param config_dir: path to config directory
+    :param lock_dir: path to directory with lock file
     :param vod_id: id of vod which lock file is created for
     :return: error if lock file removal fails
     """
     try:
-        Path(config_dir, f'.lock.{vod_id}').unlink()
+        Path(lock_dir, f'.lock.{vod_id}').unlink()
         return
 
     except Exception as e:
         return e
 
 
 def time_since_date(timestamp):
```

