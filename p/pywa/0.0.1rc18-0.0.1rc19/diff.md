# Comparing `tmp/pywa-0.0.1rc18-py3-none-any.whl.zip` & `tmp/pywa-0.0.1rc19-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 32688 bytes, number of entries: 21
+Zip file size: 32686 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx      117 b- defN 23-Jun-27 07:52 pywa/__init__.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Jul-10 20:48 pywa/__version__.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-10 21:35 pywa/__version__.py
 -rw-rw-r--  2.0 unx    14440 b- defN 23-Jul-09 17:48 pywa/api.py
 -rw-rw-r--  2.0 unx    29315 b- defN 23-Jul-09 21:41 pywa/client.py
 -rw-rw-r--  2.0 unx     7191 b- defN 23-Jul-03 08:28 pywa/errors.py
--rw-rw-r--  2.0 unx    21211 b- defN 23-Jul-10 20:48 pywa/filters.py
+-rw-rw-r--  2.0 unx    21046 b- defN 23-Jul-10 21:34 pywa/filters.py
 -rw-rw-r--  2.0 unx     1794 b- defN 23-Jul-02 08:19 pywa/handlers.py
 -rw-rw-r--  2.0 unx      873 b- defN 23-Jul-09 12:48 pywa/utils.py
 -rw-rw-r--  2.0 unx     4449 b- defN 23-Jul-09 13:09 pywa/webhook.py
 -rw-rw-r--  2.0 unx      336 b- defN 23-Jul-07 13:20 pywa/types/__init__.py
 -rw-rw-r--  2.0 unx     9301 b- defN 23-Jul-09 17:41 pywa/types/base_update.py
 -rw-rw-r--  2.0 unx     5653 b- defN 23-Jul-07 13:38 pywa/types/callback.py
 -rw-rw-r--  2.0 unx     4609 b- defN 23-Jul-09 14:47 pywa/types/media.py
 -rw-rw-r--  2.0 unx    11234 b- defN 23-Jul-09 17:38 pywa/types/message.py
 -rw-rw-r--  2.0 unx     1934 b- defN 23-Jul-07 13:28 pywa/types/message_status.py
 -rw-rw-r--  2.0 unx     9156 b- defN 23-Jul-07 13:38 pywa/types/others.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-10 20:48 pywa-0.0.1rc18.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4420 b- defN 23-Jul-10 20:48 pywa-0.0.1rc18.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-10 20:48 pywa-0.0.1rc18.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jul-10 20:48 pywa-0.0.1rc18.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-10 20:48 pywa-0.0.1rc18.dist-info/RECORD
-21 files, 128813 bytes uncompressed, 30162 bytes compressed:  76.6%
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-10 21:35 pywa-0.0.1rc19.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4420 b- defN 23-Jul-10 21:35 pywa-0.0.1rc19.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-10 21:35 pywa-0.0.1rc19.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-10 21:35 pywa-0.0.1rc19.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-10 21:35 pywa-0.0.1rc19.dist-info/RECORD
+21 files, 128648 bytes uncompressed, 30160 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: pywa/types/message_status.py
 Comment: 
 
 Filename: pywa/types/others.py
 Comment: 
 
-Filename: pywa-0.0.1rc18.dist-info/LICENSE
+Filename: pywa-0.0.1rc19.dist-info/LICENSE
 Comment: 
 
-Filename: pywa-0.0.1rc18.dist-info/METADATA
+Filename: pywa-0.0.1rc19.dist-info/METADATA
 Comment: 
 
-Filename: pywa-0.0.1rc18.dist-info/WHEEL
+Filename: pywa-0.0.1rc19.dist-info/WHEEL
 Comment: 
 
-Filename: pywa-0.0.1rc18.dist-info/top_level.txt
+Filename: pywa-0.0.1rc19.dist-info/top_level.txt
 Comment: 
 
-Filename: pywa-0.0.1rc18.dist-info/RECORD
+Filename: pywa-0.0.1rc19.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywa/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1rc18"
+__version__ = "0.0.1rc19"
```

## pywa/filters.py

```diff
@@ -53,33 +53,33 @@
 
 >>> filters.FORWARDED_MANY_TIMES
 """
 
 
 def all_(*filters: Callable[[Wa, T], bool]) -> Callable[[Wa, T], bool]:
     """
-    Filter for messages that pass all the given filters.
+    Filter for updates that pass all the given filters.
 
     >>> all_(TextFilter.startswith("World"), TextFilter.contains("Word"))
     """
     return lambda wa, m: all(f(wa, m) for f in filters)
 
 
 def any_(*filters: Callable[[Wa, T], bool]) -> Callable[[Wa, T], bool]:
     """
-    Filter for messages that pass any of the given filters.
+    Filter for updates that pass any of the given filters.
 
     >>> any_(TextFilter.contains("Hello"), TextFilter.contains("World"))
     """
     return lambda wa, m: any(f(wa, m) for f in filters)
 
 
 def not_(fil: Callable[[Wa, T], bool]) -> Callable[[Wa, T], bool]:
     """
-    Filter for messages that don't pass the given filter.
+    Filter for updates that don't pass the given filter.
 
     >>> not_(TextFilter.contains("Hello"))
     """
     return lambda wa, m: not fil(wa, m)
 
 
 def from_user(*numbers: str) -> MessageT:
@@ -175,17 +175,15 @@
         >>> TextFilter.match("Hello", "Hi")
 
         Args:
             matches: The text/s to filter for.
             ignore_case: Whether to ignore case when matching (default: ``False``).
         """
         matches = tuple(m.lower() for m in matches) if ignore_case else matches
-        return lambda wa, m: TextFilter._match_type(m) and any(
-            (m.text.lower() if ignore_case else m.text) == t for t in matches
-        )
+        return lambda wa, m: TextFilter._match_type(m) and (m.text.lower() if ignore_case else m.text) in matches
 
     same_as = match  # alias
     matches = match # alias
     equals = match  # alias
 
     @staticmethod
     def contain(*matches: str, ignore_case: bool = False) -> MessageT:
@@ -216,33 +214,29 @@
         >>> TextFilter.startswith("What", "When", ignore_case=True)
 
         Args:
             matches: The text/s to filter for.
             ignore_case: Whether to ignore case when matching (default: ``False``).
         """
         matches = tuple(m.lower() for m in matches) if ignore_case else matches
-        return lambda wa, m: TextFilter._match_type(m) and any(
-            (m.text.lower() if ignore_case else m.text).startswith(t) for t in matches
-        )
+        return lambda wa, m: TextFilter._match_type(m) and (m.text.lower() if ignore_case else m.text).startswith(matches)
 
     @staticmethod
     def endswith(*matches: str, ignore_case: bool = False) -> MessageT:
         """
         Filter for text messages that end with the given text/s.
 
         >>> TextFilter.endswith("Bye", "See you", ignore_case=True)
 
         Args:
             matches: The text/s to filter for.
             ignore_case: Whether to ignore case when matching (default: ``False``).
         """
         matches = tuple(m.lower() for m in matches) if ignore_case else matches
-        return lambda wa, m: TextFilter._match_type(m) and any(
-            (m.text.lower() if ignore_case else m.text).endswith(t) for t in matches
-        )
+        return lambda wa, m: TextFilter._match_type(m) and (m.text.lower() if ignore_case else m.text).endswith(matches)
 
     @staticmethod
     def regex(*patterns: str | re.Pattern, flags: int = 0) -> MessageT:
         """
         Filter for text messages that match the given regex/regexes.
             - Aliases: ``regexes``, ``pattern``, ``patterns``
 
@@ -549,15 +543,15 @@
         >>> CallbackFilter.data_match("back", "return", "exit")
 
         Args:
             matches: The string/s to match.
             ignore_case: Whether to ignore case when matching (default: False).
         """
         matches = tuple(m.lower() for m in matches) if ignore_case else matches
-        return lambda wa, c: any((c.data.lower() if ignore_case else c.data) == m for m in matches)
+        return lambda wa, c: (c.data.lower() if ignore_case else c.data) in matches
 
     data_equals = data_match
     data_same_as = data_match
     data_matches = data_match
 
     @staticmethod
     def data_startswith(*matches: str, ignore_case: bool = False) -> CallbackT:
@@ -567,29 +561,29 @@
         >>> CallbackFilter.data_startswith("id:")
 
         Args:
             matches: The string/s to match.
             ignore_case: Whether to ignore case when matching (default: False).
         """
         matches = tuple(m.lower() for m in matches) if ignore_case else matches
-        return lambda wa, c: any((c.data.lower() if ignore_case else c.data).startswith(m for m in matches))
+        return lambda wa, c: (c.data.lower() if ignore_case else c.data).startswith(matches)
 
     @staticmethod
     def data_endswith(*matches: str, ignore_case: bool = False) -> CallbackT:
         """
         Filter for callbacks their data ends with the given string/s.
 
         >>> CallbackFilter.data_endswith(":true", ":false")
 
         Args:
             matches: The string/s to match.
             ignore_case: Whether to ignore case when matching (default: False).
         """
         matches = tuple(m.lower() for m in matches) if ignore_case else matches
-        return lambda wa, c: any((c.data.lower() if ignore_case else c.data).endswith(m for m in matches))
+        return lambda wa, c: (c.data.lower() if ignore_case else c.data).endswith(matches)
 
     @staticmethod
     def data_contain(*matches: str, ignore_case: bool = False) -> CallbackT:
         """
         Filter for callbacks their data contains the given string/s.
             - Aliases: ``data_contains``, ``data_include``, ``data_includes``
```

## Comparing `pywa-0.0.1rc18.dist-info/LICENSE` & `pywa-0.0.1rc19.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywa-0.0.1rc18.dist-info/METADATA` & `pywa-0.0.1rc19.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 0.0.1rc18
+Version: 0.0.1rc19
 Summary: Python wrapper for the WhatsApp Cloud API
 Download-URL: https://pypi.org/project/pywa/
 Author: David Lev
 Author-email: davidlev@telegmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/david-lev/pywa#readme
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
```

## Comparing `pywa-0.0.1rc18.dist-info/RECORD` & `pywa-0.0.1rc19.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 pywa/__init__.py,sha256=u98CpT0wYk8-XDPUGB_hW-a_23agBkzTSzfwmoqnsE0,117
-pywa/__version__.py,sha256=Ifv_aiJHNqitXC2u_HQuKwd6bRW6jAXmmZunuaCprsg,26
+pywa/__version__.py,sha256=X4Zu_d6IDlLaJ4dU_U08K496PYIf5zbTpoaQW75fkCc,26
 pywa/api.py,sha256=334CM6QSpzUbJ5-2BKXZg6ZZWyl09VImxMgbKNwUHOk,14440
 pywa/client.py,sha256=joguy-5GgmKvw_2KD8YGzJXb_V0o7DOmKJeP9a8YfVQ,29315
 pywa/errors.py,sha256=ErB0UGIpIOF5vZXK39WmiSrB_PSYvTJL8PLIp90vTjU,7191
-pywa/filters.py,sha256=AwMO34POFm7QDw9FPCMFVOFdIG3fSLm9ZKIWEO-Gt6w,21211
+pywa/filters.py,sha256=thOtWYSeFFmLkTJ-cegfQmOfFT5dxV3PnI9DQo6HY6Y,21046
 pywa/handlers.py,sha256=DTlKr-yvVKpTgh3F0Gsq78gT5XhBIo_VVnYHz3lu25w,1794
 pywa/utils.py,sha256=vIPGDuXFo80xAhv88mboE-rU-uDEv594cAxEPsMrIZg,873
 pywa/webhook.py,sha256=XJEJRKLk8Dg4eJ1qE5_B3bUXu0ugt-0cjWe8C9tbvH4,4449
 pywa/types/__init__.py,sha256=HwhabvWT9b1bgPLnvXBDOmYNTh-FYjCC-ot-rh8xqzo,336
 pywa/types/base_update.py,sha256=Jd3JW8nhFd2ss0ftBjr8mEKw1gVhxlOcbKosPdQwPhA,9301
 pywa/types/callback.py,sha256=J7xDPPeGaU_JPpbdyJXJtmVu7hTMMlyquqQI9p95F5w,5653
 pywa/types/media.py,sha256=4T5yOsoZwFmJaTUZf49VnMsXACsGLq1crC6wzSBqanA,4609
 pywa/types/message.py,sha256=zNKvifHA3P89TOxKoV4dLnt-B9jbu7whlP8gdu304Xo,11234
 pywa/types/message_status.py,sha256=wgUlrgTCaKKqEZgVaZt_yYY_PKyJMhBGz-Rh3WaXSB0,1934
 pywa/types/others.py,sha256=UeXSWEY1pekZDVBDacbUsXff_OmYbxbAe9P2o_am4es,9156
-pywa-0.0.1rc18.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
-pywa-0.0.1rc18.dist-info/METADATA,sha256=3r6gTUhe18dWuTQtlRsx8qu7_FpqNfwM89aUw1QgPPg,4420
-pywa-0.0.1rc18.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pywa-0.0.1rc18.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
-pywa-0.0.1rc18.dist-info/RECORD,,
+pywa-0.0.1rc19.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
+pywa-0.0.1rc19.dist-info/METADATA,sha256=f44Ly70xc5gSUSjFI8GJMB8gHKvT2j7Mgkwy8yZVPc4,4420
+pywa-0.0.1rc19.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pywa-0.0.1rc19.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
+pywa-0.0.1rc19.dist-info/RECORD,,
```

