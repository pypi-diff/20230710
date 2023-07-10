# Comparing `tmp/yt_dlp_types-0.0.6.tar.gz` & `tmp/yt_dlp_types-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_dlp_types-0.0.6.tar", max compression
+gzip compressed data, was "yt_dlp_types-0.0.7.tar", max compression
```

## Comparing `yt_dlp_types-0.0.6.tar` & `yt_dlp_types-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1087 2023-07-03 15:46:20.349120 yt_dlp_types-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0      128 2023-07-03 19:42:09.982181 yt_dlp_types-0.0.6/README.md
--rw-r--r--   0        0        0      699 2023-07-04 00:35:19.347007 yt_dlp_types-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      513 2023-07-03 20:27:46.133664 yt_dlp_types-0.0.6/yt_dlp-stubs/YoutubeDL.pyi
--rw-r--r--   0        0        0    27804 2023-07-03 19:37:36.027414 yt_dlp_types-0.0.6/yt_dlp-stubs/__init__.pyi
--rw-r--r--   0        0        0      286 2023-07-03 19:24:37.015987 yt_dlp_types-0.0.6/yt_dlp-stubs/_misc.pyi
--rw-r--r--   0        0        0      588 2023-07-03 19:24:38.504986 yt_dlp_types-0.0.6/yt_dlp-stubs/cookies.pyi
--rw-r--r--   0        0        0        0 2023-07-03 19:24:30.422991 yt_dlp_types-0.0.6/yt_dlp-stubs/extractor/__init__.pyi
--rw-r--r--   0        0        0     1917 2023-07-03 19:24:31.719990 yt_dlp_types-0.0.6/yt_dlp-stubs/extractor/common.pyi
--rw-r--r--   0        0        0        0 2023-07-03 19:04:47.210090 yt_dlp_types-0.0.6/yt_dlp-stubs/py.typed
--rw-r--r--   0        0        0       22 2023-07-03 19:24:33.389989 yt_dlp_types-0.0.6/yt_dlp-stubs/utils/__init__.pyi
--rw-r--r--   0        0        0     1331 2023-07-04 00:35:02.147035 yt_dlp_types-0.0.6/yt_dlp-stubs/utils/_utils.pyi
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 yt_dlp_types-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-07-03 15:46:20.349120 yt_dlp_types-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0      430 2023-07-08 05:26:36.074557 yt_dlp_types-0.0.7/README.md
+-rw-r--r--   0        0        0     4970 2023-07-10 02:39:39.428841 yt_dlp_types-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-07-08 05:13:05.821461 yt_dlp_types-0.0.7/yt_dlp-stubs/YoutubeDL.pyi
+-rw-r--r--   0        0        0    27817 2023-07-08 05:13:15.166452 yt_dlp_types-0.0.7/yt_dlp-stubs/__init__.pyi
+-rw-r--r--   0        0        0      286 2023-07-07 01:16:15.602187 yt_dlp_types-0.0.7/yt_dlp-stubs/_misc.pyi
+-rw-r--r--   0        0        0      588 2023-07-08 05:13:17.677450 yt_dlp_types-0.0.7/yt_dlp-stubs/cookies.pyi
+-rw-r--r--   0        0        0        0 2023-07-03 19:24:30.422991 yt_dlp_types-0.0.7/yt_dlp-stubs/extractor/__init__.pyi
+-rw-r--r--   0        0        0     2213 2023-07-10 02:38:33.275035 yt_dlp_types-0.0.7/yt_dlp-stubs/extractor/common.pyi
+-rw-r--r--   0        0        0        0 2023-07-03 19:04:47.210090 yt_dlp_types-0.0.7/yt_dlp-stubs/py.typed
+-rw-r--r--   0        0        0       22 2023-07-08 05:13:08.732458 yt_dlp_types-0.0.7/yt_dlp-stubs/utils/__init__.pyi
+-rw-r--r--   0        0        0     1335 2023-07-08 05:13:12.255455 yt_dlp_types-0.0.7/yt_dlp-stubs/utils/_utils.pyi
+-rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 yt_dlp_types-0.0.7/PKG-INFO
```

### Comparing `yt_dlp_types-0.0.6/LICENSE.txt` & `yt_dlp_types-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yt_dlp_types-0.0.6/yt_dlp-stubs/YoutubeDL.pyi` & `yt_dlp_types-0.0.7/yt_dlp-stubs/YoutubeDL.pyi`

 * *Files identical despite different names*

### Comparing `yt_dlp_types-0.0.6/yt_dlp-stubs/__init__.pyi` & `yt_dlp_types-0.0.7/yt_dlp-stubs/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -143,17 +143,17 @@
     format_sort: NotRequired[Sequence[str] | None]
     #: Force the given format_sort. see "Sorting Formats" for more details.
     format_sort_force: NotRequired[str | None]
     #: Allow multiple video streams to be merged into a single file.
     allow_multiple_video_streams: NotRequired[bool | None]
     #: Allow multiple audio streams to be merged into a single file.
     allow_multiple_audio_streams: NotRequired[bool | None]
-    #: Whether to test if the formats are downloadable. Can be ``True`` (check all), ``False`` (check
-    #: none), ``'selected'`` (check selected formats), or ``None`` (check only if requested by
-    #: extractor).
+    #: Whether to test if the formats are downloadable. Can be ``True`` (check all), ``False``
+    # (check  none), ``'selected'`` (check selected formats), or ``None`` (check only if requested
+    # by extractor).
     check_formats: NotRequired[bool | Literal['selected'] | None]
     #: Print an overview of available video formats and exit.
     listformats: NotRequired[bool | None]
     #: Dictionary of templates for output names. Allowed keys are ``'default'`` and the keys of
     #: ``OUTTMPL_TYPES`` (in ``utils.py``). For compatibility with youtube-dl, a single string can
     #: also be used.
     outtmpl: NotRequired[str | Mapping[str, str] | None]
@@ -354,28 +354,29 @@
     default_search: NotRequired[str | None]
     #: Whether to process dynamic DASH manifests (default: ``True``).
     dynamic_mpd: NotRequired[bool | None]
     #: A dictionary of arguments to be passed to the extractors. See "EXTRACTOR ARGUMENTS" for
     #: details. Example: ``{'youtube': {'skip': ['dash', 'hls']}}``.
     extractor_args: NotRequired[Mapping[str, Mapping[str, Any]] | None]
     #: Use ``extractor_args``. If ``True`` (default), DASH manifests and related data will be
-    #: downloaded and processed by extractor. You can reduce network I/O by disabling it if you don't
-    #: care about DASH. Only for YouTube.
+    #: downloaded and processed by extractor. You can reduce network I/O by disabling it if you
+    # don't care about DASH. Only for YouTube.
     youtube_include_dash_manifest: NotRequired[bool | None]
     #: Use ``extractor_args``. If ``True`` (default), DASH manifests and related data will be
-    #: downloaded and processed by extractor. You can reduce network I/O by disabling it if you don't
-    #: care about HLS. Only for YouTube.
+    #: downloaded and processed by extractor. You can reduce network I/O by disabling it if you
+    # don't care about HLS. Only for YouTube.
     youtube_include_hls_manifest: NotRequired[bool | None]
     #: Use this encoding instead of the system-specified.
     encoding: NotRequired[str | None]
     #: Whether to resolve and process ``url_results`` further.
     #: * ``False``: Always process. Default for API.
     #: * ``True``: Never process.
     #: * ``'in_playlist'``: Do not process inside playlist/multi-video.
-    #: * ``'discard'``: Always process, but don't return the result from inside playlist/multi-video.
+    #: * ``'discard'``: Always process, but don't return the result from inside
+    #    playlist/multi-video.
     #: * ``'discard_in_playlist'``: Same as ``'discard'``, but only for playlists (not multi_video).
     #:   Default for CLI.
     extract_flat: NotRequired[bool | Literal['in_playlist', 'discard', 'discard_in_playlist']
                               | None]
     #: Whether to download livestreams videos from the start.
     live_from_start: NotRequired[bool | None]
     #: If given, wait for scheduled streams to become available. The value should be a tuple
@@ -436,15 +437,16 @@
     xattr_set_filesize: NotRequired[bool | None]
     #: A function that gets called for every video with the signature
     #: ``(info_dict, *, incomplete: bool) -> str | None``
     #: For backward compatibility with youtube-dl, the signature
     #: ``(info_dict) -> str | None`` is also allowed.
     #: If it returns a message, the video is ignored.
     #: If it returns ``None``, the video is downloaded.
-    #: If it returns utils.NO_DEFAULT, the user is interactively asked whether to download the video.
+    #: If it returns utils.NO_DEFAULT, the user is interactively asked whether to download the
+    #: video.
     #: Raise ``utils.DownloadCancelled(msg)`` to abort remaining downloads when a video is rejected.
     #: ``match_filter_func`` in utils.py is one example for this.
     match_filter: NotRequired[Callable[[InfoDict, bool], str | None]
                               | Callable[[InfoDict], str | None] | None]
     #: A Dictionary with output stream names as keys and their respective color policy as values.
     #: Can also just be a single color policy, in which case it applies to all outputs.
     #: Valid stream names are ``'stdout'`` and ``'stderr'``. Valid color policies are one of
```

### Comparing `yt_dlp_types-0.0.6/yt_dlp-stubs/cookies.pyi` & `yt_dlp_types-0.0.7/yt_dlp-stubs/cookies.pyi`

 * *Files identical despite different names*

### Comparing `yt_dlp_types-0.0.6/yt_dlp-stubs/extractor/common.pyi` & `yt_dlp_types-0.0.7/yt_dlp-stubs/extractor/common.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import Any, Literal, Mapping
+from typing import Any, Literal, Mapping, TypeVar
 import urllib.request
 
 from ..YoutubeDL import YoutubeDL
 from ..utils import ExtractorError
 
 __all__ = ('ExtractorError', 'InfoExtractor')
 
+T = TypeVar('T')
+
 
 class InfoExtractor:
     def __init__(self, downloader: YoutubeDL | None = ...) -> None:
         ...
 
     def _download_json(self,
                        url: str | urllib.request.Request,
@@ -50,7 +52,15 @@
                          query: Mapping[str, str] = ...,
                          expected_status: int | None = ...) -> Any:
         ...
 
     @classmethod
     def _match_id(cls, url: str) -> str:
         ...
+
+    def _configuration_arg(self,
+                           key: str,
+                           default: T = ...,
+                           *,
+                           ie_key: str | None = ...,
+                           casesense: bool = ...) -> Any:
+        ...
```

### Comparing `yt_dlp_types-0.0.6/yt_dlp-stubs/utils/_utils.pyi` & `yt_dlp_types-0.0.7/yt_dlp-stubs/utils/_utils.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __all__ = ('ExtractorError', 'HEADRequest', 'YoutubeDLError', 'int_or_none', 'parse_iso8601',
            'sanitize_filename', 'try_get')
 
 T = TypeVar('T')
 U = TypeVar('U')
 
 
-def try_get(x: T, getter: Callable[[T], U], t: Type[U]) -> U:
+def try_get(x: T, getter: Callable[[T], U], type_: Type[U]) -> U:
     ...
 
 
 def parse_iso8601(s: str, delimiter: str) -> int | None:
     ...
```

