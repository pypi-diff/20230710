# Comparing `tmp/pywa-0.0.1rc17-py3-none-any.whl.zip` & `tmp/pywa-0.0.1rc18-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 32701 bytes, number of entries: 21
+Zip file size: 32688 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx      117 b- defN 23-Jun-27 07:52 pywa/__init__.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Jul-09 17:47 pywa/__version__.py
--rw-rw-r--  2.0 unx    14468 b- defN 23-Jul-09 17:38 pywa/api.py
--rw-rw-r--  2.0 unx    29314 b- defN 23-Jul-09 17:43 pywa/client.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-10 20:48 pywa/__version__.py
+-rw-rw-r--  2.0 unx    14440 b- defN 23-Jul-09 17:48 pywa/api.py
+-rw-rw-r--  2.0 unx    29315 b- defN 23-Jul-09 21:41 pywa/client.py
 -rw-rw-r--  2.0 unx     7191 b- defN 23-Jul-03 08:28 pywa/errors.py
--rw-rw-r--  2.0 unx    21225 b- defN 23-Jul-09 17:29 pywa/filters.py
+-rw-rw-r--  2.0 unx    21211 b- defN 23-Jul-10 20:48 pywa/filters.py
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
--rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-09 17:47 pywa-0.0.1rc17.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4420 b- defN 23-Jul-09 17:47 pywa-0.0.1rc17.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-09 17:47 pywa-0.0.1rc17.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jul-09 17:47 pywa-0.0.1rc17.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-09 17:47 pywa-0.0.1rc17.dist-info/RECORD
-21 files, 128854 bytes uncompressed, 30175 bytes compressed:  76.6%
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-10 20:48 pywa-0.0.1rc18.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4420 b- defN 23-Jul-10 20:48 pywa-0.0.1rc18.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-10 20:48 pywa-0.0.1rc18.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-10 20:48 pywa-0.0.1rc18.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-10 20:48 pywa-0.0.1rc18.dist-info/RECORD
+21 files, 128813 bytes uncompressed, 30162 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: pywa/types/message_status.py
 Comment: 
 
 Filename: pywa/types/others.py
 Comment: 
 
-Filename: pywa-0.0.1rc17.dist-info/LICENSE
+Filename: pywa-0.0.1rc18.dist-info/LICENSE
 Comment: 
 
-Filename: pywa-0.0.1rc17.dist-info/METADATA
+Filename: pywa-0.0.1rc18.dist-info/METADATA
 Comment: 
 
-Filename: pywa-0.0.1rc17.dist-info/WHEEL
+Filename: pywa-0.0.1rc18.dist-info/WHEEL
 Comment: 
 
-Filename: pywa-0.0.1rc17.dist-info/top_level.txt
+Filename: pywa-0.0.1rc18.dist-info/top_level.txt
 Comment: 
 
-Filename: pywa-0.0.1rc17.dist-info/RECORD
+Filename: pywa-0.0.1rc18.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywa/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1rc17"
+__version__ = "0.0.1rc18"
```

## pywa/api.py

```diff
@@ -1,13 +1,10 @@
-import io
-import mimetypes
 import requests
 from typing import Iterable, BinaryIO
 from requests_toolbelt import MultipartEncoder
-
 from pywa.errors import WhatsAppError
 from pywa.types import InlineButton, SectionList, Contact
 
 
 class WhatsAppCloudApi:
     """Internal methods for the WhatsApp client."""
```

## pywa/client.py

```diff
@@ -434,15 +434,15 @@
         Send a document to a WhatsApp user.
 
         Example:
 
             >>> wa.send_document(
             ...     to="1234567890",
             ...     document="https://example.com/example_123.pdf",
-            ...     file_name="exmaple.pdf",
+            ...     file_name="example.pdf",
             ...     caption="Example PDF"
             ... )
 
 
         Args:
             to: The phone ID of the WhatsApp user.
             document: The document to send (either a media ID, URL, file path, bytes, or a open file object).
@@ -532,15 +532,15 @@
             >>> wa.send_sticker(
             ...     to='1234567890',
             ...     sticker='https://example.com/sticker.webp',
             ... )
 
         Args:
             to: The phone ID of the WhatsApp user.
-            sticker: The sticker to send (either a media ID, URL, file path, bytes, or a open file object).
+            sticker: The sticker to send (either a media ID, URL, file path, bytes, or an open file object).
             reply_to_message_id: The message ID to reply to (optional).
 
         Returns:
             The message ID of the sent message.
         """
         _, sticker = self._resolve_media_param(media=sticker, mime_type="image/webp", file_name="sticker.webp")
         return self.api.send_media(
```

## pywa/filters.py

```diff
@@ -284,16 +284,16 @@
 
         Args:
             cmds: The command/s to filter for (e.g. "start", "hello").
             prefixes: The prefix/s to filter for (default: "!", i.e. "!start").
             ignore_case: Whether to ignore case when matching (default: ``False``).
         """
         cmds = tuple(c.lower() for c in cmds) if ignore_case else cmds
-        return lambda wa, m: TextFilter._match_type(m) and any(
-            m.text[0] in prefixes and (m.text[1:].lower() if ignore_case else m.text[1:]).startswith(c for c in cmds)
+        return lambda wa, m: TextFilter._match_type(m) and (
+            m.text[0] in prefixes and (m.text[1:].lower() if ignore_case else m.text[1:]).startswith(cmds)
         )
     commands = command  # alias
     cmd = command  # alias
     cmds = command  # alias
 
 
 class ImageFilter(_MediaWithCaptionFilter):
```

## Comparing `pywa-0.0.1rc17.dist-info/LICENSE` & `pywa-0.0.1rc18.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywa-0.0.1rc17.dist-info/METADATA` & `pywa-0.0.1rc18.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 0.0.1rc17
+Version: 0.0.1rc18
 Summary: Python wrapper for the WhatsApp Cloud API
 Download-URL: https://pypi.org/project/pywa/
 Author: David Lev
 Author-email: davidlev@telegmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/david-lev/pywa#readme
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
```

## Comparing `pywa-0.0.1rc17.dist-info/RECORD` & `pywa-0.0.1rc18.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 pywa/__init__.py,sha256=u98CpT0wYk8-XDPUGB_hW-a_23agBkzTSzfwmoqnsE0,117
-pywa/__version__.py,sha256=DlFrhUG4bi9E-87CieAzje8rjSKLjHTgQ3wNJ8fl9T8,26
-pywa/api.py,sha256=rx6ceDInJ_1srH65PNNub7CYwb9BHM7_dXAuC0OF9FQ,14468
-pywa/client.py,sha256=3ioAyAwVD320CPbEJP07kfkGzog4JEXTB0Gge3cbF_A,29314
+pywa/__version__.py,sha256=Ifv_aiJHNqitXC2u_HQuKwd6bRW6jAXmmZunuaCprsg,26
+pywa/api.py,sha256=334CM6QSpzUbJ5-2BKXZg6ZZWyl09VImxMgbKNwUHOk,14440
+pywa/client.py,sha256=joguy-5GgmKvw_2KD8YGzJXb_V0o7DOmKJeP9a8YfVQ,29315
 pywa/errors.py,sha256=ErB0UGIpIOF5vZXK39WmiSrB_PSYvTJL8PLIp90vTjU,7191
-pywa/filters.py,sha256=Iqcah-FLKkAbeKdSHEm33bGOPe-2E-eDa7-1DrXFKnc,21225
+pywa/filters.py,sha256=AwMO34POFm7QDw9FPCMFVOFdIG3fSLm9ZKIWEO-Gt6w,21211
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
-pywa-0.0.1rc17.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
-pywa-0.0.1rc17.dist-info/METADATA,sha256=ncFGGg_nCInvGdfHKC5lUpY2DXkz9m3bG3SZ9fRaluo,4420
-pywa-0.0.1rc17.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pywa-0.0.1rc17.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
-pywa-0.0.1rc17.dist-info/RECORD,,
+pywa-0.0.1rc18.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
+pywa-0.0.1rc18.dist-info/METADATA,sha256=3r6gTUhe18dWuTQtlRsx8qu7_FpqNfwM89aUw1QgPPg,4420
+pywa-0.0.1rc18.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pywa-0.0.1rc18.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
+pywa-0.0.1rc18.dist-info/RECORD,,
```

