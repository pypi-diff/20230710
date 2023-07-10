# Comparing `tmp/spotify_to_musi-2.0.0.tar.gz` & `tmp/spotify_to_musi-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_to_musi-2.0.0.tar", max compression
+gzip compressed data, was "spotify_to_musi-2.0.1.tar", max compression
```

## Comparing `spotify_to_musi-2.0.0.tar` & `spotify_to_musi-2.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1082 2022-04-30 04:14:50.831047 spotify_to_musi-2.0.0/LICENSE
--rw-r--r--   0        0        0     2412 2023-04-22 00:53:35.525411 spotify_to_musi-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1708 2023-04-22 00:53:50.158969 spotify_to_musi-2.0.0/README.md
--rw-r--r--   0        0        0      749 2023-04-19 20:59:57.112853 spotify_to_musi-2.0.0/spotify_to_musi/__init__.py
--rw-r--r--   0        0        0     4137 2023-04-22 00:47:11.473199 spotify_to_musi-2.0.0/spotify_to_musi/__main__.py
--rw-r--r--   0        0        0     3531 2023-04-19 20:53:14.471015 spotify_to_musi-2.0.0/spotify_to_musi/commons.py
--rw-r--r--   0        0        0     1088 2023-04-16 23:05:44.315588 spotify_to_musi-2.0.0/spotify_to_musi/exceptions.py
--rw-r--r--   0        0        0      982 2023-04-22 00:01:10.469619 spotify_to_musi-2.0.0/spotify_to_musi/main.py
--rw-r--r--   0        0        0     5631 2023-04-22 00:14:25.119714 spotify_to_musi-2.0.0/spotify_to_musi/musi.py
--rw-r--r--   0        0        0     5538 2023-04-22 00:01:10.485440 spotify_to_musi-2.0.0/spotify_to_musi/oauth.py
--rw-r--r--   0        0        0     1024 2023-04-22 00:24:41.849747 spotify_to_musi-2.0.0/spotify_to_musi/paths.py
--rw-r--r--   0        0        0        0 2022-05-12 20:01:34.542338 spotify_to_musi-2.0.0/spotify_to_musi/py.typed
--rw-r--r--   0        0        0    12619 2023-04-22 00:01:10.500456 spotify_to_musi-2.0.0/spotify_to_musi/spotify.py
--rw-r--r--   0        0        0     3688 2023-04-22 00:01:10.504904 spotify_to_musi-2.0.0/spotify_to_musi/tracks_cache.py
--rw-r--r--   0        0        0       35 2023-04-16 22:55:23.576124 spotify_to_musi-2.0.0/spotify_to_musi/typings/__init__.py
--rw-r--r--   0        0        0     2469 2023-04-22 00:22:56.472209 spotify_to_musi-2.0.0/spotify_to_musi/typings/core.py
--rw-r--r--   0        0        0     4108 2023-04-22 00:25:10.891189 spotify_to_musi-2.0.0/spotify_to_musi/typings/musi.py
--rw-r--r--   0        0        0     4215 2023-04-19 21:00:48.910481 spotify_to_musi-2.0.0/spotify_to_musi/typings/spotify.py
--rw-r--r--   0        0        0     1611 2023-04-22 00:01:10.537402 spotify_to_musi-2.0.0/spotify_to_musi/typings/youtube.py
--rw-r--r--   0        0        0    10001 2023-04-21 23:58:33.475408 spotify_to_musi-2.0.0/spotify_to_musi/youtube.py
--rw-r--r--   0        0        0    12837 2023-04-22 00:16:02.227785 spotify_to_musi-2.0.0/spotify_to_musi/ytmusic.py
--rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 spotify_to_musi-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-16 03:48:09.943665 spotify_to_musi-2.0.1/LICENSE
+-rw-r--r--   0        0        0     2430 2023-07-10 02:38:27.098202 spotify_to_musi-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1708 2023-06-16 03:48:09.943665 spotify_to_musi-2.0.1/README.md
+-rw-r--r--   0        0        0      749 2023-06-16 03:48:09.945665 spotify_to_musi-2.0.1/spotify_to_musi/__init__.py
+-rw-r--r--   0        0        0     4137 2023-06-16 03:48:54.381698 spotify_to_musi-2.0.1/spotify_to_musi/__main__.py
+-rw-r--r--   0        0        0     3531 2023-06-16 03:48:09.946665 spotify_to_musi-2.0.1/spotify_to_musi/commons.py
+-rw-r--r--   0        0        0     1088 2023-06-16 03:48:09.946665 spotify_to_musi-2.0.1/spotify_to_musi/exceptions.py
+-rw-r--r--   0        0        0      982 2023-06-16 04:09:26.573939 spotify_to_musi-2.0.1/spotify_to_musi/main.py
+-rw-r--r--   0        0        0     5631 2023-06-16 03:48:09.947665 spotify_to_musi-2.0.1/spotify_to_musi/musi.py
+-rw-r--r--   0        0        0     5538 2023-06-16 03:48:09.947665 spotify_to_musi-2.0.1/spotify_to_musi/oauth.py
+-rw-r--r--   0        0        0     1024 2023-06-16 03:48:09.948665 spotify_to_musi-2.0.1/spotify_to_musi/paths.py
+-rw-r--r--   0        0        0        0 2023-06-16 03:48:09.948665 spotify_to_musi-2.0.1/spotify_to_musi/py.typed
+-rw-r--r--   0        0        0    12854 2023-07-10 02:32:19.765776 spotify_to_musi-2.0.1/spotify_to_musi/spotify.py
+-rw-r--r--   0        0        0     3688 2023-06-16 03:48:09.949665 spotify_to_musi-2.0.1/spotify_to_musi/tracks_cache.py
+-rw-r--r--   0        0        0       36 2023-06-16 03:48:09.949665 spotify_to_musi-2.0.1/spotify_to_musi/typings/__init__.py
+-rw-r--r--   0        0        0     2469 2023-06-16 03:48:09.949665 spotify_to_musi-2.0.1/spotify_to_musi/typings/core.py
+-rw-r--r--   0        0        0     4040 2023-07-10 02:25:26.336985 spotify_to_musi-2.0.1/spotify_to_musi/typings/musi.py
+-rw-r--r--   0        0        0     4168 2023-07-10 02:21:53.001750 spotify_to_musi-2.0.1/spotify_to_musi/typings/spotify.py
+-rw-r--r--   0        0        0     1701 2023-07-10 02:28:21.081690 spotify_to_musi-2.0.1/spotify_to_musi/typings/youtube.py
+-rw-r--r--   0        0        0    10001 2023-06-16 03:48:09.951174 spotify_to_musi-2.0.1/spotify_to_musi/youtube.py
+-rw-r--r--   0        0        0    12837 2023-06-16 03:51:19.885367 spotify_to_musi-2.0.1/spotify_to_musi/ytmusic.py
+-rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 spotify_to_musi-2.0.1/PKG-INFO
```

### Comparing `spotify_to_musi-2.0.0/LICENSE` & `spotify_to_musi-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_to_musi-2.0.0/pyproject.toml` & `spotify_to_musi-2.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "spotify-to-musi"
 description = "Transfer Spotify playlists to Musi."
-version = "2.0.0"
+version = "2.0.1"
 readme = "README.md"
 license = "MIT"
 authors = ["Hexiro <mail@hexiro.me>"]
 repository = "https://github.com/hexiro/spotify-to-musi"
 keywords = ["spotify", "music", "musi", "transfer", "cli"]
 classifiers = [
     "Natural Language :: English",
@@ -20,23 +20,23 @@
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries ",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-rich = "^13.3.4"
+rich = ">=12.6.0 <15.0.0"
 rich-click = "^1.6.1"
 aiofiles = "^23.1.0"
-httpx = "^0.24.0"
-pydantic = "^1.10.7"
+httpx = ">=0.23.0 <=0.25.0"
+pydantic = "^2.0.2"
 pyfy = "^2.2.0"
 sanic = "^23.3.0"
 async-cache = "^1.1.1"
-typing-extensions = {version = "^4.5.0", python = "<3.11"}
+typing-extensions = {version = "^4.7.1", python = "<3.11"}
 uvloop = {version = "^0.17.0", platform = "linux"}
 
 [tool.poetry.scripts]
 spotify-to-musi = "spotify_to_musi.__main__:cli"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/hexiro/spotify-to-musi/issues"
```

### Comparing `spotify_to_musi-2.0.0/README.md` & `spotify_to_musi-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/__init__.py` & `spotify_to_musi-2.0.1/spotify_to_musi/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/__main__.py` & `spotify_to_musi-2.0.1/spotify_to_musi/__main__.py`

 * *Files identical despite different names*

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/commons.py` & `spotify_to_musi-2.0.1/spotify_to_musi/commons.py`

 * *Files identical despite different names*

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/exceptions.py` & `spotify_to_musi-2.0.1/spotify_to_musi/exceptions.py`

 * *Files identical despite different names*

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/main.py` & `spotify_to_musi-2.0.1/spotify_to_musi/main.py`

 * *Files identical despite different names*

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/musi.py` & `spotify_to_musi-2.0.1/spotify_to_musi/musi.py`

 * *Files identical despite different names*

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/oauth.py` & `spotify_to_musi-2.0.1/spotify_to_musi/oauth.py`

 * *Files identical despite different names*

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/paths.py` & `spotify_to_musi-2.0.1/spotify_to_musi/paths.py`

 * *Files identical despite different names*

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/spotify.py` & `spotify_to_musi-2.0.1/spotify_to_musi/spotify.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,16 +300,22 @@
     spotify_tracks: list[SpotifyTrack] = []
     for spotify_track_item in spotify_track_items:
         try:
             track = SpotifyTrack(**spotify_track_item["track"])
         # weird spotify api bug where track, artist, and album name is blank
         # (usually because the track is by 'various artists' the spotify thing)
         # but w/o this information we can't fetch the track so just skip it
-        except pydantic.error_wrappers.ValidationError:
-            continue
+        except pydantic.ValidationError as exc:
+            for error in exc.errors():
+                if error["input"] == "":
+                    continue
+                # as in: '[type] name can't be blank'
+                if "blank" in error["msg"]:
+                    continue
+                raise
         else:
             spotify_tracks.append(track)
 
     spotify_tracks = filter_spotify_tracks(spotify_tracks)
     return spotify_tracks
```

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/tracks_cache.py` & `spotify_to_musi-2.0.1/spotify_to_musi/tracks_cache.py`

 * *Files identical despite different names*

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/typings/core.py` & `spotify_to_musi-2.0.1/spotify_to_musi/typings/core.py`

 * *Files identical despite different names*

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/typings/musi.py` & `spotify_to_musi-2.0.1/spotify_to_musi/typings/musi.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,16 +64,16 @@
 
 
 class MusiPlaylist(BaseModel):
     name: str
     tracks: tuple[MusiTrack, ...] = Field(exclude=True)
     ciu: t.Optional[str] = Field(alias="cover_image_url")
     date: int = Field(default_factory=lambda: int(time.time()))
-    ot: t.Literal["custom"] = Field(default="custom", const=True)
-    type: t.Literal["user"] = Field(default="user", const=True)
+    ot: t.Literal["custom"] = Field(default="custom")
+    type: t.Literal["user"] = Field(default="user")
 
     def dict(self: MusiPlaylist, **kwargs: t.Any) -> MusiPlaylistDict:  # type: ignore[override]
         items: list[MusiItemDict] = [track.musi_item(index).dict() for index, track in enumerate(self.tracks)]  # type: ignore
         super_dict = super().dict(**kwargs)
         data = {
             "ot": super_dict["ot"],
             "items": items,
@@ -91,16 +91,16 @@
     items: list[MusiItemDict]
     name: t.Literal["My Library"]
     date: int  # int(time.time())
 
 
 class MusiLibrary(BaseModel):
     tracks: tuple[MusiTrack, ...] = Field(exclude=True)
-    ot: t.Literal["custom"] = Field(default="custom", const=True)
-    name: t.Literal["My Library"] = Field(default="My Library", const=True)
+    ot: t.Literal["custom"] = Field(default="custom")
+    name: str = Field(default="My Library")
     date: int = Field(default_factory=lambda: int(time.time()))
 
     def dict(self: MusiLibrary, **kwargs: t.Any) -> MusiLibraryDict:  # type: ignore[override]
         items: list[MusiItemDict] = [track.musi_item(index).dict() for index, track in enumerate(self.tracks)]  # type: ignore
         super_dict = super().dict(**kwargs)
         return {
             "ot": super_dict["ot"],
```

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/typings/spotify.py` & `spotify_to_musi-2.0.1/spotify_to_musi/typings/spotify.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import typing as t
 
-from pydantic import BaseModel, validator
+from pydantic import field_validator, BaseModel
 
 from spotify_to_musi.exceptions import BlankNameError
 
 
 class SpotifyResponse(t.TypedDict):
     href: str
     items: list[t.Any]  # potentially make this a generic in future
@@ -53,38 +53,39 @@
 class SpotifyArtist(BaseModel):
     href: str
     name: str
     id: str
     type: str
     uri: str
 
-    @validator("name")
+    @field_validator("name")
+    @classmethod
     def validate_name(cls, v: str) -> str:  # noqa: ANN101, N805
         if not v:
             raise BlankNameError("artist")
         return v
 
 
 class SpotifyAlbum(BaseModel):
-    album_group: t.Union[t.Literal["single"], str]  # not sure what other options are
     album_type: t.Union[t.Literal["single"], str]  # not sure what other options are
     artists: list[SpotifyArtist]
     # 'external_urls': ExternalUrls  noqa: ERA001
     href: str
     id: str
     images: list[SpotifyImage]
     is_playable: bool
     name: str
     release_date: str
     release_date_precision: str
     total_tracks: int
     type: t.Union[t.Literal["album"], str]  # not sure what other options are
     uri: str
 
-    @validator("name")
+    @field_validator("name")
+    @classmethod
     def validate_name(cls, v: str) -> str:  # noqa: ANN101, N805
         if not v:
             raise BlankNameError("album")
         return v
 
 
 class SpotifyTrack(BaseModel):
@@ -104,29 +105,30 @@
     # 'uri': str  noqa: ERA001
     album: SpotifyAlbum
     # 'disc_number': int  noqa: ERA001
     # 'external_ids': ExternalIds  noqa: ERA001
     # 'external_urls': ExternalUrls  noqa: ERA001
     # 'preview_url': Optional[str]  noqa: ERA001
 
-    @validator("name")
+    @field_validator("name")
+    @classmethod
     def validate_name(cls, v: str) -> str:  # noqa: ANN101, N805
         if not v:
             raise BlankNameError("track")
         return v
 
     @property
     def duration(self: SpotifyTrack) -> int:
         return self.duration_ms // 1000
 
     @property
     def album_name(self: SpotifyTrack) -> str | None:
         # song is a single and has the single name as the album name,
         # represent this as None internally because it's not really an album
-        if self.album.album_type == "single" or self.album.album_group == "single" or self.album.total_tracks == 1:
+        if self.album.album_type == "single" or self.album.total_tracks == 1:
             return None
 
         return self.album.name
 
 
 class SpotifyPlaylist(BasicSpotifyPlaylist):
     tracks: list[SpotifyTrack]  # type: ignore[assignment]
```

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/typings/youtube.py` & `spotify_to_musi-2.0.1/spotify_to_musi/typings/youtube.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import typing as t
 from dataclasses import field
 
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, field_validator
 from pydantic.dataclasses import dataclass
 
 from spotify_to_musi.typings.core import Artist, Playlist, Track
 
 
 class YouTubeMusicArtist(BaseModel):
     name: str
@@ -24,15 +24,16 @@
     video_id: str
 
 
 class YouTubeMusicSong(_YouTubeMusicResultType):
     album: t.Optional[YouTubeMusicAlbum]
     is_explicit: bool
 
-    @validator("album")
+    @field_validator("name", check_fields=False)  # type: ignore inherited from BaseModel
+    @classmethod
     def must_not_be_single(
         cls, v: YouTubeMusicAlbum, values: dict[str, t.Any]  # noqa: ANN101, N805
     ) -> YouTubeMusicAlbum | None:
         # sourcery skip: assign-if-exp, reintroduce-else
         if v.name == values["title"]:
             return None
```

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/youtube.py` & `spotify_to_musi-2.0.1/spotify_to_musi/youtube.py`

 * *Files identical despite different names*

### Comparing `spotify_to_musi-2.0.0/spotify_to_musi/ytmusic.py` & `spotify_to_musi-2.0.1/spotify_to_musi/ytmusic.py`

 * *Files identical despite different names*

### Comparing `spotify_to_musi-2.0.0/PKG-INFO` & `spotify_to_musi-2.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-to-musi
-Version: 2.0.0
+Version: 2.0.1
 Summary: Transfer Spotify playlists to Musi.
 Home-page: https://github.com/hexiro/spotify-to-musi
 License: MIT
 Keywords: spotify,music,musi,transfer,cli
 Author: Hexiro
 Author-email: mail@hexiro.me
 Requires-Python: >=3.9,<4.0
@@ -14,30 +14,27 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries 
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: async-cache (>=1.1.1,<2.0.0)
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: httpx (>=0.23.0,<=0.25.0)
+Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Requires-Dist: pyfy (>=2.2.0,<3.0.0)
-Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: rich (>=12.6.0,<15.0.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Requires-Dist: sanic (>=23.3.0,<24.0.0)
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version < "3.11"
+Requires-Dist: typing-extensions (>=4.7.1,<5.0.0) ; python_version < "3.11"
 Requires-Dist: uvloop (>=0.17.0,<0.18.0) ; sys_platform == "linux"
 Project-URL: Bug Tracker, https://github.com/hexiro/spotify-to-musi/issues
 Project-URL: Repository, https://github.com/hexiro/spotify-to-musi
 Description-Content-Type: text/markdown
 
 # spotify-to-musi
```

