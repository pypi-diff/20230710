# Comparing `tmp/ytdlp_auf1-2023.1.5-py3-none-any.whl.zip` & `tmp/ytdlp_auf1-2023.7.10-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 7462 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    17038 b- defN 23-Jan-05 18:54 ytdlp_plugins/extractor/auf1.py
--rw-rw-rw-  2.0 fat     1235 b- defN 23-Jan-05 18:55 ytdlp_auf1-2023.1.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2320 b- defN 23-Jan-05 18:55 ytdlp_auf1-2023.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-05 18:55 ytdlp_auf1-2023.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       24 b- defN 23-Jan-05 18:55 ytdlp_auf1-2023.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      505 b- defN 23-Jan-05 18:55 ytdlp_auf1-2023.1.5.dist-info/RECORD
-6 files, 21214 bytes uncompressed, 6544 bytes compressed:  69.2%
+Zip file size: 11802 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    16625 b- defN 23-Jul-10 09:16 yt_dlp_plugins/extractor/auf1.py
+-rw-rw-rw-  2.0 fat    15329 b- defN 23-Jun-03 09:55 yt_dlp_plugins/extractor/dtube.py
+-rw-rw-rw-  2.0 fat     1212 b- defN 23-Jul-10 09:16 ytdlp_auf1-2023.7.10.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2530 b- defN 23-Jul-10 09:16 ytdlp_auf1-2023.7.10.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-10 09:16 ytdlp_auf1-2023.7.10.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       31 b- defN 23-Jul-10 09:16 ytdlp_auf1-2023.7.10.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      602 b- defN 23-Jul-10 09:16 ytdlp_auf1-2023.7.10.dist-info/RECORD
+7 files, 36421 bytes uncompressed, 10730 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
-Filename: ytdlp_plugins/extractor/auf1.py
+Filename: yt_dlp_plugins/extractor/auf1.py
 Comment: 
 
-Filename: ytdlp_auf1-2023.1.5.dist-info/LICENSE
+Filename: yt_dlp_plugins/extractor/dtube.py
 Comment: 
 
-Filename: ytdlp_auf1-2023.1.5.dist-info/METADATA
+Filename: ytdlp_auf1-2023.7.10.dist-info/LICENSE
 Comment: 
 
-Filename: ytdlp_auf1-2023.1.5.dist-info/WHEEL
+Filename: ytdlp_auf1-2023.7.10.dist-info/METADATA
 Comment: 
 
-Filename: ytdlp_auf1-2023.1.5.dist-info/top_level.txt
+Filename: ytdlp_auf1-2023.7.10.dist-info/WHEEL
 Comment: 
 
-Filename: ytdlp_auf1-2023.1.5.dist-info/RECORD
+Filename: ytdlp_auf1-2023.7.10.dist-info/top_level.txt
+Comment: 
+
+Filename: ytdlp_auf1-2023.7.10.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ytdlp_plugins/extractor/auf1.py` & `yt_dlp_plugins/extractor/auf1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,469 +1,471 @@
-# coding: utf-8
-import json
-import re
-import time
-from contextlib import suppress
-from shlex import shlex
-from urllib.error import HTTPError
-
-from yt_dlp.extractor.common import InfoExtractor
-from yt_dlp.extractor.peertube import PeerTubeIE
-from yt_dlp.utils import (
-    ExtractorError,
-    OnDemandPagedList,
-    base_url,
-    clean_html,
-    js_to_json,
-    parse_duration,
-    parse_iso8601,
-    traverse_obj,
-    urljoin,
-)
-
-__version__ = "2023.01.05"
-
-
-class JSHLEX(shlex):
-    def __init__(self, instream):
-        super().__init__(
-            instream=instream, infile=None, posix=True, punctuation_chars=False
-        )
-        self.whitespace = ", \t\r\n"
-        self.whitespace_split = True
-
-    def __next__(self):
-        value = super().__next__()
-        try:
-            json.loads(value)
-        except json.JSONDecodeError:
-            quote_escaped = value.replace('"', '\\"')
-            value = f'"{quote_escaped}"'
-        return value
-
-
-# pylint: disable=abstract-method
-class Auf1IE(InfoExtractor):
-    IE_NAME = "auf1"
-    _VALID_URL = r"""(?x)
-                    (?:https?:)?//
-                        (?:www\.)?
-                        (?:auf1\.tv/)
-                        (?P<category>[^/]+/)?
-                        (?P<id>[^/]+)
-                    """
-
-    peertube_extract_url = None
-    _TESTS = [
-        {
-            "url": "https://auf1.tv/nachrichten-auf1/ampelkoalition-eine-abrissbirne-fuer-deutschland/",
-            "info_dict": {
-                "id": "rKjpWNnocoARnj4pQMRKXQ",
-                "title": "Ampelkoalition: Eine Abrissbirne für Deutschland?",
-                "description": "md5:9265dda76d30e842e1f75aa3cb3e3884",
-                "ext": "mp4",
-                "thumbnail": r"re:https://(:?auf1.)?gegenstimme.tv/static/thumbnails/[\w-]+.jpg",
-                "timestamp": 1638446905,
-                "upload_date": "20211202",
-                "uploader": "AUF1.TV",
-                "uploader_id": "25408",
-                "duration": 818,
-                "view_count": int,
-                "like_count": int,
-                "dislike_count": int,
-                "categories": ["News & Politics"],
-            },
-            "params": {"skip_download": True},
-            "expected_warnings": ["JSON API"],
-        },
-        {
-            "url": "https://auf1.tv/nachrichten-auf1/nachrichten-auf1-vom-15-dezember-2022/",
-            "info_dict": {
-                "id": "nVBERN4MzFutVzoXsADf8F",
-                "title": "Nachrichten AUF1 vom 15. Dezember 2022",
-                "description": "md5:bc4def34dcc8401d84c5127c5f759543",
-                "ext": "mp4",
-                "thumbnail": r"re:https://(:?auf1.)?gegenstimme.tv/static/thumbnails/[\w-]+.jpg",
-                "timestamp": 1671121411,
-                "upload_date": "20221215",
-                "uploader": "AUF1.TV",
-                "uploader_id": "25408",
-                "duration": 1825,
-                "view_count": int,
-                "like_count": int,
-                "dislike_count": int,
-                "categories": ["News & Politics"],
-            },
-            "params": {"skip_download": True},
-            "expected_warnings": ["JSON API"],
-        },
-        {  # JSON API without payload.js
-            "url": "https://auf1.tv/stefan-magnet-auf1/"
-            "heiko-schoening-chaos-und-krieg-gehoeren-leider-zu-deren-plan/",
-            "info_dict": {
-                "id": "dVk8Q3VNMLi7b7uhyuSSp6",
-                "ext": "mp4",
-                "title": "Heiko Schöning: „Chaos und Krieg gehören leider zu deren Plan“",
-                "description": "md5:6fb9e7eb469fc544223018a2ff3c998c",
-                "timestamp": int,
-                "uploader": str,
-                "uploader_id": str,
-                "upload_date": "20220307",
-                "channel": str,
-                "channel_url": "contains:/video-channels/auf1.tv",
-                "duration": 2089,
-                "view_count": int,
-                "like_count": int,
-                "dislike_count": int,
-                "tags": [],
-                "categories": ["News & Politics"],
-            },
-            "params": {"skip_download": True},
-            "expected_warnings": [
-                "Retrying due to too many requests.",
-                "The read operation timed out",
-                "JSON API",
-            ],
-        },
-        {
-            # playlist for category
-            "url": "https://auf1.tv/nachrichten-auf1/",
-            "info_dict": {
-                "id": "nachrichten-auf1",
-                "title": "Nachrichten AUF1",
-                "description": "md5:5b1f113270133adfd94f6ae3014e3d6f",
-            },
-            "playlist_mincount": 100,
-            "expected_warnings": [
-                "Retrying due to too many requests.",
-                "The read operation timed out",
-                "JSON API",
-            ],
-        },
-        {
-            # playlist for all videos
-            "url": "https://auf1.tv/videos",
-            "info_dict": {
-                "id": "all_videos",
-                "title": "AUF1.TV - Alle Videos",
-            },
-            "playlist_mincount": 200,
-            "expected_warnings": [
-                "Retrying due to too many requests.",
-                "JSON API",
-            ],
-        },
-    ]
-
-    @staticmethod
-    def parse_url(url: str):
-        if not url:
-            return None
-        match = re.match(r"^https?://([^/]+)/videos/embed/([^?]+)", url)
-        # pylint: disable=consider-using-f-string
-        return "peertube:{}:{}".format(*match.groups()) if match else None
-
-    @staticmethod
-    def sparse_info(metadata):
-        return {
-            "id": metadata.get("public_id", "unknown"),
-            "url": metadata.get("videoUrl"),
-            "title": metadata.get("title"),
-            "description": clean_html(traverse_obj(metadata, "text", "preview_text")),
-            "duration": parse_duration(metadata.get("duration")),
-            "timestamp": parse_iso8601(metadata.get("published_at") or None),
-            "thumbnail": metadata.get("thumbnail_url"),
-        }
-
-    def call_api(self, endpoint, video_id=None, fatal=True):
-        return self._download_json(
-            f"https://auf1.tv/api/{endpoint}",
-            video_id=video_id,
-            fatal=fatal,
-            errnote="JSON API",
-        )
-
-    def call_with_retries(
-        self,
-        operation,
-        http_error_map=None,
-    ):
-        http_error_map = http_error_map or {}
-        max_duration_s = 30.0
-        sleep_duration_s = 5.0
-        attempt_count = 0
-        while True:
-            start = time.time()
-            try:
-                return operation()
-            except ExtractorError as exc:
-                attempt_count += 1
-                errorcode = None
-                if isinstance(exc.cause, HTTPError):
-                    errorcode = exc.cause.code
-                    sleep_duration_s = float(
-                        exc.cause.headers.get("retry-after", sleep_duration_s)
-                    )
-                if max_duration_s < 0.0:
-                    self.report_warning(f"Giving up after {attempt_count} attempts.")
-                elif errorcode == 429:
-                    self.report_warning(
-                        f"Retrying in {sleep_duration_s:.0f} seconds due to too many requests."
-                    )
-                    max_duration_s -= time.time() - start
-                    time.sleep(sleep_duration_s)
-                    continue
-                for errors, exception in http_error_map.items():
-                    if isinstance(errors, int):
-                        errors = {errors}
-                    if errorcode in errors:
-                        raise exception from exc
-                raise
-
-    def peertube_extract(self, url):
-        if self.peertube_extract_url is None:
-            peertube_extractor = self._downloader.get_info_extractor(
-                PeerTubeIE.ie_key()
-            )
-            self.peertube_extract_url = getattr(peertube_extractor, "_real_extract")
-
-        return self.call_with_retries(
-            lambda: self.peertube_extract_url(url),
-        )
-
-    def playlist_from_entries(self, all_videos, **kwargs):
-        entries = []
-        for item in all_videos:
-            public_id = item.get("public_id")
-            if not public_id:
-                continue
-            category = traverse_obj(item, ("show", "public_id"), default="video")
-            entries.append(
-                {
-                    "_type": "url",
-                    "ie_key": self.ie_key(),
-                    **self.sparse_info(item),
-                    "url": f"//auf1.tv/{category}/{public_id}/",
-                }
-            )
-
-        return self.playlist_result(
-            entries,
-            **kwargs,
-        )
-
-    def _payloadjs(self, url, page_id):
-        webpage = self._download_webpage(url, page_id)
-        payloadjs_url = self._search_regex(
-            r'href="([^"]+/_?payload.js)"', webpage, "payload url"
-        )
-        payloadjs_url = urljoin(base_url(url), payloadjs_url)
-        payload_js = self._download_webpage(
-            payloadjs_url, page_id, note="Downloading payload.js"
-        )
-
-        match = re.match(
-            r"""(?x)
-                .*
-                \(function\ *\( (?P<vars>[^)]*) \)
-                \{\ *return\ * (?P<metadata>\{.+}) .*}
-                \( (?P<values>.*) \){2}
-            """,
-            payload_js,
-        )
-        if match is None:
-            raise ExtractorError("Failed parsing payload.js")
-
-        variables, metadata, values = match.groups()
-        var_mapping = dict(zip(variables.split(","), JSHLEX(values)))
-
-        control_character_mapping = dict.fromkeys(range(32))
-        js_string = js_to_json(metadata, vars=var_mapping).translate(
-            control_character_mapping
-        )
-        return json.loads(js_string)
-
-    def _metadata(self, url, *, page_id, method="api"):
-        if method == "api":
-            return self.call_with_retries(
-                lambda: self.call_api(f"getContent/{page_id}", page_id),
-                http_error_map={500: ExtractorError("JSON API failed (500)")},
-            )
-        payload = self._payloadjs(url, page_id)
-        return payload["data"].popitem()[1]
-
-    def _real_extract(self, url):
-        category, page_id = self._match_valid_url(url).groups()
-
-        # single video
-        if category:
-            try:
-                metadata = self._metadata(url, page_id=page_id, method="api")
-            except ExtractorError as exc:
-                self.report_warning(exc, page_id)
-                metadata = self._metadata(url, page_id=page_id, method="payloadjs")
-            peertube_url = self.parse_url(metadata.get("videoUrl"))
-            return (
-                self.peertube_extract(peertube_url)
-                if peertube_url
-                else self.sparse_info(metadata)
-            )
-
-        # video playlist
-        if page_id == "videos":
-            return self.playlist_from_entries(
-                self.call_with_retries(
-                    lambda: self.call_api("getVideos", video_id="all_videos"),
-                ),
-                playlist_id="all_videos",
-                playlist_title="AUF1.TV - Alle Videos",
-            )
-
-        try:
-            metadata = self.call_with_retries(
-                lambda: self.call_api(f"getShow/{page_id}", page_id),
-            )
-        except ExtractorError as exc:
-            self.report_warning(exc, page_id)
-            metadata = self._metadata(url, page_id=page_id, method="payloadjs")
-
-        return self.playlist_from_entries(
-            metadata.get("contents"),
-            playlist_id=page_id,
-            playlist_title=metadata.get("name"),
-            description=clean_html(metadata.get("description")),
-        )
-
-
-# pylint: disable=abstract-method
-class Auf1RadioIE(InfoExtractor):
-    IE_NAME = "auf1:radio"
-    _VALID_URL = r"""(?x)
-                    https?://
-                        (?:www\.)?
-                        auf1\.radio
-                        (?: / 
-                            (?P<category>[^/]+/)?
-                            (?P<id>[^/]+)
-                        )?
-                        /?
-                    """
-
-    _TESTS = [
-        {
-            "url": "https://auf1.radio/nachrichten-auf1/worte-der-hoffnung-ein-sammelband-der-mut-macht/",
-            "md5": "3a0d00dd473f46b387678621420fad8e",
-            "info_dict": {
-                "id": "worte-der-hoffnung-ein-sammelband-der-mut-macht",
-                "ext": "mp3",
-                "title": "Worte der Hoffnung: Ein Sammelband, der Mut macht",
-                "description": "md5:3102f277e87e1baafc7f09242b66a071",
-                "duration": 70,
-                "timestamp": 1669539605,
-                "upload_date": "20221127",
-                "thumbnail": "re:https://auf1.*.jpg",
-            },
-        },
-        {
-            # playlist for category
-            "url": "https://auf1.radio/nachrichten-auf1/",
-            "info_dict": {
-                "id": "nachrichten-auf1",
-                "title": "Nachrichten AUF1",
-            },
-            "playlist_mincount": 50,
-        },
-        {
-            # playlist for all media
-            "url": "https://auf1.radio/",
-            "info_dict": {
-                "id": "all",
-                "title": "all",
-            },
-            "playlist_mincount": 50,
-        },
-    ]
-
-    MP3_FORMAT = {
-        "ext": "mp3",
-        "acodec": "mp3",
-        "vcodec": "none",
-        "asr": 48000,
-        "tbr": 64,
-        "abr": 64,
-        "format": "MP2/3 (MPEG audio layer 2/3)",
-    }
-
-    def call_api(self, endpoint, **kwargs):
-        kwargs.setdefault("errnote", "JSON API")
-        return self._download_json(
-            f"https://auf1.radio/api/{endpoint}",
-            **kwargs,
-        )
-
-    def formats(self, url: str, duration):
-        format_info = {"url": url}
-        if url.endswith(".mp3"):
-            format_info.update(self.MP3_FORMAT)
-            if duration:
-                format_info["filesize_approx"] = duration * 8000
-        return [format_info]
-
-    def entry_from_info(self, info, media_id):
-        return {
-            "id": info.get("content_public_id", media_id),
-            "title": info["title"],
-            "description": info.get("summary"),
-            "duration": info.get("duration"),
-            "timestamp": parse_iso8601(info.get("created_at")),
-            "thumbnail": info.get("thumbnail")
-            and f"https://auf1.tv/images/{info['thumbnail']}",
-            "formats": self.formats(info.get("audio_url"), info.get("duration")),
-        }
-
-    def entries_from_playlist(self, playlist_id):
-        endpoint = "" if playlist_id == "all" else "getShow/"
-
-        def fetch(page, _last_page):
-            page_note = (
-                f"{page+1}/{_last_page}" if isinstance(_last_page, int) else page + 1
-            )
-            return self.call_api(
-                f"{endpoint}{playlist_id}",
-                query={"page": page + 1},
-                video_id=playlist_id,
-                note=f"Downloading page {page_note}",
-            )
-
-        first_page = fetch(0, None)
-        last_page = first_page.get("last_page", "NA")
-        page_size = first_page.get("per_page", len(first_page.get("data", ())))
-        playlist_title = playlist_id
-        with suppress(KeyError, IndexError):
-            if playlist_id != "all":
-                playlist_title = first_page["data"][0]["show_name"]
-
-        def load_page(index):
-            info = fetch(index, last_page) if index > 0 else first_page
-            for media_info in info["data"]:
-                audiofile = media_info.get("audiofile")
-                if audiofile:
-                    media_info["audio_url"] = f"https://auf1.radio/storage/{audiofile}"
-                yield self.entry_from_info(media_info, playlist_id)
-
-        return self.playlist_result(
-            entries=OnDemandPagedList(load_page, page_size),
-            playlist_id=playlist_id,
-            playlist_title=playlist_title,
-            playlist_count=first_page.get("total", "NA"),
-        )
-
-    def _real_extract(self, url):
-        category, page_id = self._match_valid_url(url).groups()
-
-        if category:
-            info = self.call_api(f"get/{page_id}", video_id=page_id)
-            if not info:
-                raise ExtractorError("not available")
-            return self.entry_from_info(info, page_id)
-
-        return self.entries_from_playlist(page_id or "all")
+# coding: utf-8
+import json
+import re
+import time
+from contextlib import suppress
+from shlex import shlex
+from urllib.error import HTTPError
+
+from yt_dlp.extractor.common import InfoExtractor
+from yt_dlp.extractor.peertube import PeerTubeIE
+from yt_dlp.utils import (
+    ExtractorError,
+    OnDemandPagedList,
+    base_url,
+    clean_html,
+    js_to_json,
+    parse_duration,
+    parse_iso8601,
+    traverse_obj,
+    urljoin,
+)
+
+__version__ = "2023.07.10"
+
+
+class JSHLEX(shlex):
+    def __init__(self, instream):
+        super().__init__(
+            instream=instream, infile=None, posix=True, punctuation_chars=False
+        )
+        self.whitespace = ", \t\r\n"
+        self.whitespace_split = True
+
+    def __next__(self):
+        value = super().__next__()
+        try:
+            json.loads(value)
+        except json.JSONDecodeError:
+            quote_escaped = value.replace('"', '\\"')
+            value = f'"{quote_escaped}"'
+        return value
+
+
+# pylint: disable=abstract-method
+class Auf1IE(InfoExtractor):
+    IE_NAME = "auf1"
+    _VALID_URL = r"""(?x)
+                    (?:https?:)?//
+                        (?:www\.)?
+                        (?:auf1\.tv/)
+                        (?P<category>[^/]+/)?
+                        (?P<id>[^/]+)
+                    """
+
+    peertube_extract_url = None
+    _TESTS = [
+        {
+            "url": "https://auf1.tv/nachrichten-auf1/ampelkoalition-eine-abrissbirne-fuer-deutschland/",
+            "info_dict": {
+                "id": "rKjpWNnocoARnj4pQMRKXQ",
+                "title": "Ampelkoalition: Eine Abrissbirne für Deutschland?",
+                "description": "md5:9265dda76d30e842e1f75aa3cb3e3884",
+                "ext": "mp4",
+                "thumbnail": r"re:https://videos\.auf1\.tv/static/thumbnails/[\w-]+\.jpg",
+                "timestamp": 1638446905,
+                "upload_date": "20211202",
+                "uploader": "AUF1.TV",
+                "uploader_id": "25408",
+                "duration": 818,
+                "view_count": int,
+                "like_count": int,
+                "dislike_count": int,
+                "categories": ["News & Politics"],
+            },
+            "params": {"skip_download": True},
+            "expected_warnings": ["JSON API"],
+        },
+        {
+            "url": "https://auf1.tv/nachrichten-auf1/nachrichten-auf1-vom-15-dezember-2022/",
+            "info_dict": {
+                "id": "nVBERN4MzFutVzoXsADf8F",
+                "title": "Nachrichten AUF1 vom 15. Dezember 2022",
+                "description": "md5:bc4def34dcc8401d84c5127c5f759543",
+                "ext": "mp4",
+                "thumbnail": r"re:https://videos\.auf1\.tv/static/thumbnails/[\w-]+\.jpg",
+                "timestamp": 1671121411,
+                "upload_date": "20221215",
+                "uploader": "AUF1.TV",
+                "uploader_id": "25408",
+                "duration": 1825,
+                "view_count": int,
+                "like_count": int,
+                "dislike_count": int,
+                "categories": ["News & Politics"],
+            },
+            "params": {"skip_download": True},
+            "expected_warnings": ["JSON API"],
+        },
+        {  # JSON API without payload.js
+            "url": "https://auf1.tv/stefan-magnet-auf1/"
+            "heiko-schoening-chaos-und-krieg-gehoeren-leider-zu-deren-plan/",
+            "info_dict": {
+                "id": "dVk8Q3VNMLi7b7uhyuSSp6",
+                "ext": "mp4",
+                "title": "Heiko Schöning: „Chaos und Krieg gehören leider zu deren Plan“",
+                "description": "md5:6fb9e7eb469fc544223018a2ff3c998c",
+                "timestamp": int,
+                "uploader": str,
+                "uploader_id": str,
+                "upload_date": "20220307",
+                "channel": str,
+                "channel_url": "contains:/video-channels/auf1.tv",
+                "duration": 2089,
+                "view_count": int,
+                "like_count": int,
+                "dislike_count": int,
+                "tags": [],
+                "categories": ["News & Politics"],
+            },
+            "params": {"skip_download": True},
+            "expected_warnings": [
+                "Retrying due to too many requests.",
+                "The read operation timed out",
+                "JSON API",
+            ],
+        },
+        {
+            # playlist for category
+            "url": "https://auf1.tv/nachrichten-auf1/",
+            "info_dict": {
+                "id": "nachrichten-auf1",
+                "title": "Nachrichten AUF1",
+                "description": "md5:dcb992e2bb7fd020a417634b949f2951",
+            },
+            "playlist_mincount": 100,
+            "expected_warnings": [
+                "Retrying due to too many requests.",
+                "The read operation timed out",
+                "JSON API",
+            ],
+        },
+        {
+            # playlist for all videos
+            "url": "https://auf1.tv/videos",
+            "info_dict": {
+                "id": "all_videos",
+                "title": "AUF1.TV - Alle Videos",
+            },
+            "playlist_mincount": 200,
+            "expected_warnings": [
+                "Retrying due to too many requests.",
+                "JSON API",
+            ],
+        },
+    ]
+
+    @staticmethod
+    def parse_url(url: str):
+        if not url:
+            return None
+        match = re.match(r"^https?://([^/]+)/videos/embed/([^?]+)", url)
+        # pylint: disable=consider-using-f-string
+        return "peertube:{}:{}".format(*match.groups()) if match else None
+
+    @staticmethod
+    def sparse_info(metadata):
+        return {
+            "id": metadata.get("public_id", "unknown"),
+            "url": metadata.get("videoUrl"),
+            "title": metadata.get("title"),
+            "description": clean_html(traverse_obj(metadata, "text", "preview_text")),
+            "duration": parse_duration(metadata.get("duration")),
+            "timestamp": parse_iso8601(metadata.get("published_at") or None),
+            "thumbnail": metadata.get("thumbnail_url"),
+        }
+
+    def call_api(self, endpoint, video_id=None, fatal=True):
+        return self._download_json(
+            f"https://auf1.tv/api/{endpoint}",
+            video_id=video_id,
+            fatal=fatal,
+            errnote="JSON API",
+        )
+
+    def call_with_retries(
+        self,
+        operation,
+        http_error_map=None,
+    ):
+        http_error_map = http_error_map or {}
+        max_duration_s = 30.0
+        sleep_duration_s = 5.0
+        attempt_count = 0
+        while True:
+            start = time.time()
+            try:
+                return operation()
+            except ExtractorError as exc:
+                attempt_count += 1
+                errorcode = None
+                if isinstance(exc.cause, HTTPError):
+                    errorcode = exc.cause.code
+                    sleep_duration_s = float(
+                        exc.cause.headers.get("retry-after", sleep_duration_s)
+                    )
+                if max_duration_s < 0.0:
+                    self.report_warning(f"Giving up after {attempt_count} attempts.")
+                elif errorcode == 429:
+                    self.report_warning(
+                        f"Retrying in {sleep_duration_s:.0f} seconds due to too many requests."
+                    )
+                    max_duration_s -= time.time() - start
+                    time.sleep(sleep_duration_s)
+                    continue
+                for errors, exception in http_error_map.items():
+                    if isinstance(errors, int):
+                        errors = {errors}
+                    if errorcode in errors:
+                        raise exception from exc
+                raise
+
+    def peertube_extract(self, url):
+        if self.peertube_extract_url is None:
+            peertube_extractor = self._downloader.get_info_extractor(
+                PeerTubeIE.ie_key()
+            )
+            self.peertube_extract_url = getattr(peertube_extractor, "_real_extract")
+
+        return self.call_with_retries(
+            lambda: self.peertube_extract_url(url),
+        )
+
+    def playlist_from_entries(self, all_videos, **kwargs):
+        entries = []
+        for item in all_videos:
+            public_id = item.get("public_id")
+            if not public_id:
+                continue
+            category = traverse_obj(item, ("show", "public_id"), default="video")
+            entries.append(
+                {
+                    "_type": "url",
+                    "ie_key": self.ie_key(),
+                    **self.sparse_info(item),
+                    "url": f"//auf1.tv/{category}/{public_id}/",
+                }
+            )
+
+        return self.playlist_result(
+            entries,
+            **kwargs,
+        )
+
+    def _payloadjs(self, url, page_id):
+        webpage = self._download_webpage(url, page_id)
+        payloadjs_url = self._search_regex(
+            r'href="([^"]+/_?payload.js)"', webpage, "payload url"
+        )
+        payloadjs_url = urljoin(base_url(url), payloadjs_url)
+        payload_js = self._download_webpage(
+            payloadjs_url, page_id, note="Downloading payload.js"
+        )
+
+        match = re.match(
+            r"""(?x)
+                .*
+                \(function\ *\( (?P<vars>[^)]*) \)
+                \{\ *return\ * (?P<metadata>\{.+}) .*}
+                \( (?P<values>.*) \){2}
+            """,
+            payload_js,
+        )
+        if match is None:
+            raise ExtractorError("Failed parsing payload.js")
+
+        variables, metadata, values = match.groups()
+        var_mapping = dict(zip(variables.split(","), JSHLEX(values)))
+
+        control_character_mapping = dict.fromkeys(range(32))
+        js_string = js_to_json(metadata, vars=var_mapping).translate(
+            control_character_mapping
+        )
+        return json.loads(js_string)
+
+    def _metadata(self, url, *, page_id, method="api"):
+        if method == "api":
+            return self.call_with_retries(
+                lambda: self.call_api(f"getContent/{page_id}", page_id),
+                http_error_map={500: ExtractorError("JSON API failed (500)")},
+            )
+        payload = self._payloadjs(url, page_id)
+        return payload["data"].popitem()[1]
+
+    def _real_extract(self, url):
+        category, page_id = self._match_valid_url(url).groups()
+
+        # single video
+        if category:
+            try:
+                metadata = self._metadata(url, page_id=page_id, method="api")
+            except ExtractorError as exc:
+                self.report_warning(exc, page_id)
+                metadata = self._metadata(url, page_id=page_id, method="payloadjs")
+            peertube_url = self.parse_url(
+                traverse_obj(metadata, ("videoUrl",), ("videoUrls", "peertube"))
+            )
+            return (
+                self.peertube_extract(peertube_url)
+                if peertube_url
+                else self.sparse_info(metadata)
+            )
+
+        # video playlist
+        if page_id == "videos":
+            return self.playlist_from_entries(
+                self.call_with_retries(
+                    lambda: self.call_api("getVideos", video_id="all_videos"),
+                ),
+                playlist_id="all_videos",
+                playlist_title="AUF1.TV - Alle Videos",
+            )
+
+        try:
+            metadata = self.call_with_retries(
+                lambda: self.call_api(f"getShow/{page_id}", page_id),
+            )
+        except ExtractorError as exc:
+            self.report_warning(exc, page_id)
+            metadata = self._metadata(url, page_id=page_id, method="payloadjs")
+
+        return self.playlist_from_entries(
+            metadata.get("contents"),
+            playlist_id=page_id,
+            playlist_title=metadata.get("name"),
+            description=clean_html(metadata.get("description")),
+        )
+
+
+# pylint: disable=abstract-method
+class Auf1RadioIE(InfoExtractor):
+    IE_NAME = "auf1:radio"
+    _VALID_URL = r"""(?x)
+                    https?://
+                        (?:www\.)?
+                        auf1\.radio
+                        (?: / 
+                            (?P<category>[^/]+/)?
+                            (?P<id>[^/]+)
+                        )?
+                        /?
+                    """
+
+    _TESTS = [
+        {
+            "url": "https://auf1.radio/nachrichten-auf1/worte-der-hoffnung-ein-sammelband-der-mut-macht/",
+            "md5": "3a0d00dd473f46b387678621420fad8e",
+            "info_dict": {
+                "id": "worte-der-hoffnung-ein-sammelband-der-mut-macht",
+                "ext": "mp3",
+                "title": "Worte der Hoffnung: Ein Sammelband, der Mut macht",
+                "description": "md5:3102f277e87e1baafc7f09242b66a071",
+                "duration": 70,
+                "timestamp": 1669539605,
+                "upload_date": "20221127",
+                "thumbnail": "re:https://auf1.*.jpg",
+            },
+        },
+        {
+            # playlist for category
+            "url": "https://auf1.radio/nachrichten-auf1/",
+            "info_dict": {
+                "id": "nachrichten-auf1",
+                "title": "Nachrichten AUF1",
+            },
+            "playlist_mincount": 50,
+        },
+        {
+            # playlist for all media
+            "url": "https://auf1.radio/",
+            "info_dict": {
+                "id": "all",
+                "title": "all",
+            },
+            "playlist_mincount": 50,
+        },
+    ]
+
+    MP3_FORMAT = {
+        "ext": "mp3",
+        "acodec": "mp3",
+        "vcodec": "none",
+        "asr": 48000,
+        "tbr": 64,
+        "abr": 64,
+        "format": "MP2/3 (MPEG audio layer 2/3)",
+    }
+
+    def call_api(self, endpoint, **kwargs):
+        kwargs.setdefault("errnote", "JSON API")
+        return self._download_json(
+            f"https://auf1.radio/api/{endpoint}",
+            **kwargs,
+        )
+
+    def formats(self, url: str, duration):
+        format_info = {"url": url}
+        if url.endswith(".mp3"):
+            format_info.update(self.MP3_FORMAT)
+            if duration:
+                format_info["filesize_approx"] = duration * 8000
+        return [format_info]
+
+    def entry_from_info(self, info, media_id):
+        return {
+            "id": info.get("content_public_id", media_id),
+            "title": info["title"],
+            "description": info.get("summary"),
+            "duration": info.get("duration"),
+            "timestamp": parse_iso8601(info.get("created_at")),
+            "thumbnail": info.get("thumbnail")
+            and f"https://auf1.tv/images/{info['thumbnail']}",
+            "formats": self.formats(info.get("audio_url"), info.get("duration")),
+        }
+
+    def entries_from_playlist(self, playlist_id):
+        endpoint = "" if playlist_id == "all" else "getShow/"
+
+        def fetch(page, _last_page):
+            page_note = (
+                f"{page+1}/{_last_page}" if isinstance(_last_page, int) else page + 1
+            )
+            return self.call_api(
+                f"{endpoint}{playlist_id}",
+                query={"page": page + 1},
+                video_id=playlist_id,
+                note=f"Downloading page {page_note}",
+            )
+
+        first_page = fetch(0, None)
+        last_page = first_page.get("last_page", "NA")
+        page_size = first_page.get("per_page", len(first_page.get("data", ())))
+        playlist_title = playlist_id
+        with suppress(KeyError, IndexError):
+            if playlist_id != "all":
+                playlist_title = first_page["data"][0]["show_name"]
+
+        def load_page(index):
+            info = fetch(index, last_page) if index > 0 else first_page
+            for media_info in info["data"]:
+                audiofile = media_info.get("audiofile")
+                if audiofile:
+                    media_info["audio_url"] = f"https://auf1.radio/storage/{audiofile}"
+                yield self.entry_from_info(media_info, playlist_id)
+
+        return self.playlist_result(
+            entries=OnDemandPagedList(load_page, page_size),
+            playlist_id=playlist_id,
+            playlist_title=playlist_title,
+            playlist_count=first_page.get("total", "NA"),
+        )
+
+    def _real_extract(self, url):
+        category, page_id = self._match_valid_url(url).groups()
+
+        if category:
+            info = self.call_api(f"get/{page_id}", video_id=page_id)
+            if not info:
+                raise ExtractorError("not available")
+            return self.entry_from_info(info, page_id)
+
+        return self.entries_from_playlist(page_id or "all")
```

## Comparing `ytdlp_auf1-2023.1.5.dist-info/LICENSE` & `ytdlp_auf1-2023.7.10.dist-info/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-This is free and unencumbered software released into the public domain.
-
-Anyone is free to copy, modify, publish, use, compile, sell, or
-distribute this software, either in source code form or as a compiled
-binary, for any purpose, commercial or non-commercial, and by any
-means.
-
-In jurisdictions that recognize copyright laws, the author or authors
-of this software dedicate any and all copyright interest in the
-software to the public domain. We make this dedication for the benefit
-of the public at large and to the detriment of our heirs and
-successors. We intend this dedication to be an overt act of
-relinquishment in perpetuity of all present and future rights to this
-software under copyright law.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
-OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-OTHER DEALINGS IN THE SOFTWARE.
-
-For more information, please refer to <http://unlicense.org/>
+This is free and unencumbered software released into the public domain.
+
+Anyone is free to copy, modify, publish, use, compile, sell, or
+distribute this software, either in source code form or as a compiled
+binary, for any purpose, commercial or non-commercial, and by any
+means.
+
+In jurisdictions that recognize copyright laws, the author or authors
+of this software dedicate any and all copyright interest in the
+software to the public domain. We make this dedication for the benefit
+of the public at large and to the detriment of our heirs and
+successors. We intend this dedication to be an overt act of
+relinquishment in perpetuity of all present and future rights to this
+software under copyright law.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+OTHER DEALINGS IN THE SOFTWARE.
+
+For more information, please refer to <https://unlicense.org/>
```

## Comparing `ytdlp_auf1-2023.1.5.dist-info/METADATA` & `ytdlp_auf1-2023.7.10.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 Metadata-Version: 2.1
 Name: ytdlp-auf1
-Version: 2023.1.5
+Version: 2023.7.10
 Summary: yt-dlp extractor for auf1.tv
 Home-page: https://github.com/flashdagger/ytdlp-plugins/tree/auf1
 Author: flashdagger
 Author-email: flashdagger@googlemail.com
 License: The Unlicense
 Keywords: yt-dlp,youtube-dl,auf1,extractors,plugins
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
 Classifier: Topic :: Multimedia :: Video
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ytdlp-plugins (>=2021.11.17)
+Requires-Dist: yt-dlp (>=2023.01.06)
+
+> **_NOTE_:**  
+> 
+> Since version 2023.01.06 yt-dlp supports plugins from python packages.
+> The ytdlp-plugins package is no longer necessary.
+> 
+> For further details see https://github.com/yt-dlp/yt-dlp#plugins
 
 # auf1.tv and auf1.radio support for yt-dlp
 
 ## installation
 
 You can install ytdlp-auf1 via pip:
 
@@ -41,15 +48,15 @@
 
   `python3 -m pip install -U https://github.com/flashdagger/ytdlp-plugins/archive/refs/heads/auf1.zip`
 
 Note that on some systems, you may need to use `py` or `python` instead of `python3`
 
 ## example: show the 20 recent titles from channel
 
-`python3 -m ytdlp_plugins -e --playlist-items 1-20 https://auf1.tv/videos`
+`python3 -m yt_dlp -e --playlist-items 1-20 https://auf1.tv/videos`
 
 ## yt-dlp
 
 [yt-dlp](https://github.com/yt-dlp/yt-dlp) is a [youtube-dl](https://github.com/ytdl-org/youtube-dl) fork based on the now
 inactive [youtube-dlc](https://github.com/blackjack4494/yt-dlc). The main focus of this project is adding new features
 and patches while also keeping up to date with the original project
```

