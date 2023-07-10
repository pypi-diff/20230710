# Comparing `tmp/gspread_asyncio-1.8.1.tar.gz` & `tmp/gspread_asyncio-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspread_asyncio-1.8.1.tar", last modified: Wed Mar 15 01:22:09 2023, max compression
+gzip compressed data, was "gspread_asyncio-1.9.0.tar", last modified: Mon Jul 10 01:17:00 2023, max compression
```

## Comparing `gspread_asyncio-1.8.1.tar` & `gspread_asyncio-1.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:09.885889 gspread_asyncio-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-15 01:21:58.000000 gspread_asyncio-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-03-15 01:22:09.885889 gspread_asyncio-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-03-15 01:21:58.000000 gspread_asyncio-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:09.885889 gspread_asyncio-1.8.1/gspread_asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)   102600 2023-03-15 01:21:58.000000 gspread_asyncio-1.8.1/gspread_asyncio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:09.885889 gspread_asyncio-1.8.1/gspread_asyncio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-03-15 01:22:09.000000 gspread_asyncio-1.8.1/gspread_asyncio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-15 01:22:09.000000 gspread_asyncio-1.8.1/gspread_asyncio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 01:22:09.000000 gspread_asyncio-1.8.1/gspread_asyncio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-15 01:22:09.000000 gspread_asyncio-1.8.1/gspread_asyncio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-15 01:22:09.000000 gspread_asyncio-1.8.1/gspread_asyncio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-15 01:21:58.000000 gspread_asyncio-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 01:22:09.885889 gspread_asyncio-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-15 01:21:58.000000 gspread_asyncio-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 01:17:00.838613 gspread_asyncio-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 01:16:50.000000 gspread_asyncio-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-10 01:17:00.834613 gspread_asyncio-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-10 01:16:50.000000 gspread_asyncio-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 01:17:00.834613 gspread_asyncio-1.9.0/gspread_asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)   106122 2023-07-10 01:16:50.000000 gspread_asyncio-1.9.0/gspread_asyncio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 01:17:00.834613 gspread_asyncio-1.9.0/gspread_asyncio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-10 01:17:00.000000 gspread_asyncio-1.9.0/gspread_asyncio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-10 01:17:00.000000 gspread_asyncio-1.9.0/gspread_asyncio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 01:17:00.000000 gspread_asyncio-1.9.0/gspread_asyncio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 01:17:00.000000 gspread_asyncio-1.9.0/gspread_asyncio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 01:17:00.000000 gspread_asyncio-1.9.0/gspread_asyncio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-10 01:16:50.000000 gspread_asyncio-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 01:17:00.838613 gspread_asyncio-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-10 01:16:50.000000 gspread_asyncio-1.9.0/setup.py
```

### Comparing `gspread_asyncio-1.8.1/LICENSE` & `gspread_asyncio-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gspread_asyncio-1.8.1/PKG-INFO` & `gspread_asyncio-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspread_asyncio
-Version: 1.8.1
+Version: 1.9.0
 Summary: asyncio wrapper for burnash's Google Spreadsheet API library, gspread
 Home-page: https://github.com/dgilman/gspread_asyncio
 Author: David Gilman
 Author-email: dgilman@gilslotd.com
 License: MIT
 Project-URL: Documentation, https://gspread-asyncio.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/dgilman/gspread_asyncio
```

### Comparing `gspread_asyncio-1.8.1/README.md` & `gspread_asyncio-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gspread_asyncio-1.8.1/gspread_asyncio/__init__.py` & `gspread_asyncio-1.9.0/gspread_asyncio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import functools
 import logging
 from typing import TYPE_CHECKING, Callable, Dict, Iterable, List, Optional, Tuple, Union
+import warnings
 
 import gspread
 from gspread.utils import a1_to_rowcol, extract_id_from_url
 import requests
 
 # Copyright 2018-2022 David Gilman
 # Licensed under the MIT license. See LICENSE for details.
@@ -398,15 +399,15 @@
         :returns: The content of the exported file.
         :rtype: bytes
 
         .. _ExportFormat: https://developers.google.com/drive/api/guides/ref-export-formats
 
         .. versionadded:: 1.6
         """
-        return await self.agcp._call(
+        return await self.agcm._call(
             self.gc.export,
             file_id,
             format=format,
         )
 
     @_nowait
     async def import_csv(self, file_id: str, data: str):
@@ -876,19 +877,36 @@
         .. versionadded:: 1.6
         """
         return await self.agcm._call(
             self.ss.reorder_worksheets, (aws.ws for aws in worksheets_in_desired_order)
         )
 
     @property
-    def sheet1(self) -> str:
+    async def sheet1(self) -> "AsyncioGspreadWorksheet":
         """:returns: Shortcut property for getting the first worksheet.
-        :rtype: str
+        :rtype: :class:`AsyncioGspreadWorksheet`
+
+        .. warning::
+
+            This is an asynchronous property! It must be awaited.
+
+        .. deprecated:: 1.6
+            use `AsyncioGspreadSpreadsheet.get_sheet1()` instead
         """
-        return self.ss.sheet1
+        warnings.warn(
+            "get_title will be removed in a future version of gspread_asyncio, use .get_sheet1()",
+            DeprecationWarning,
+        )
+        return await self.get_sheet1()
+
+    async def get_sheet1(self) -> "AsyncioGspreadWorksheet":
+        """:returns: Shortcut for getting the first worksheet.
+        :rtype: :class:`AsyncioGspreadWorksheet`
+        """
+        return await self.get_worksheet(0)
 
     @property
     def timezone(self) -> str:
         """:returns: Title of the spreadsheet.
         :rtype: str
 
         .. versionadded:: 1.6
@@ -903,15 +921,20 @@
         return self.ss.title
 
     async def get_title(self) -> str:
         """:returns: Title of the spreadsheet.
         :rtype: str
 
         .. deprecated:: 1.6
+            Use the `.title` property instead.
         """
+        warnings.warn(
+            "get_title will be removed in gspread_asyncio 2.x, use the .title property",
+            DeprecationWarning,
+        )
         return await self.agcm._call(getattr, self.ss, "title")
 
     @_nowait
     async def update_locale(self, locale: str):
         """Update the locale of the spreadsheet.
 
         Can be any of the ISO 639-1 language codes, such as: de, fr, en, ...
@@ -1087,15 +1110,15 @@
             awses.append(aws)
         return awses
 
 
 class AsyncioGspreadWorksheet(object):
     """An :mod:`asyncio` wrapper for :class:`gspread.Worksheet`.
     You **must** obtain instances of this class from
-    :meth:`AsynctioGspreadSpreadsheet.add_worksheet`,
+    :meth:`AsyncioGspreadSpreadsheet.add_worksheet`,
     :meth:`AsyncioGspreadSpreadsheet.get_worksheet`,
     :meth:`AsyncioGspreadSpreadsheet.worksheet`,
     or :meth:`AsyncioGspreadSpreadsheet.worksheets`.
     """
 
     def __init__(self, agcm, ws: gspread.Worksheet):
         self.agcm = agcm
@@ -1751,15 +1774,20 @@
         :meth:`gspread.Worksheet.delete_row`.
 
         :param int index: Index of a row for deletion.
         :param bool nowait: (optional) If true, return a scheduled future instead of
             waiting for the API call to complete.
 
         .. deprecated:: 1.6
+            Use `AsyncioGspreadWorksheet.delete_rows()` instead.
         """
+        warnings.warn(
+            "delete_row will be removed in a future version of gspread, use .delete_rows()",
+            DeprecationWarning,
+        )
         return await self.agcm._call(self.ws.delete_rows, index)
 
     @_nowait
     async def delete_rows(self, index: int, end_index: Optional[int] = None):
         """Deletes multiple rows from the worksheet starting at the specified
         index. Wraps :meth:`gspread.Worksheet.delete_rows`.
 
@@ -1789,22 +1817,35 @@
             If not set, an ID is chosen. If set, the ID must not conflict with
             any existing sheet ID. If set, it must be non-negative.
         :param str new_sheet_name: (optional) The name of the new sheet.
             If empty, a new name is chosen for you.
 
         :returns: a newly created :class:`AsyncioGspreadWorksheet`.
 
+        .. warning::
+
+            This breaks caching assumptions in AsyncioGspreadSpreadsheet.
+            Its use is not recommended and it will be removed in a future version.
+
         .. versionadded:: 1.6
+
+        .. deprecated:: 1.9
+            Use `AsyncioGspreadSpreadsheet.duplicate_sheet` instead.
         """
-        return await self.agcm._call(
+        warnings.warn(
+            "duplicate() will be removed in a future version of gspread_asyncio, use duplicate_sheet()",
+            DeprecationWarning,
+        )
+        dup_ws = await self.agcm._call(
             self.ws.duplicate,
             insert_sheet_index=insert_sheet_index,
             new_sheet_id=new_sheet_id,
             new_sheet_name=new_sheet_name,
         )
+        return AsyncioGspreadWorksheet(self.agcm, dup_ws)
 
     async def find(
         self,
         query: "Union[str, re.Pattern]",
         in_row: Optional[int] = None,
         in_column: Optional[int] = None,
         case_sensitive: bool = True,
@@ -2030,14 +2071,35 @@
         :param str cell: A string with cell coordinates in A1 notation, e.g. ‘D7’.
         :rtype: :class:`str`
 
         .. versionadded:: 1.5
         """
         return await self.agcm._call(self.ws.get_note, cell)
 
+    async def update_notes(self, notes: Dict):
+        """Update multiple notes.
+
+        :param dict notes: A dict of notes with their cell coordinates and respective content
+
+            dict format is:
+
+            * key: the cell coordinates as A1 range format
+            * value: the string content of the cell
+
+            Example::
+
+                {
+                    "D7": "Please read my notes",
+                    "GH42": "this one is too far",
+                }
+
+        .. versionadded: 1.9
+        """
+        return await self.agcm._call(self.ws.update_notes, notes)
+
     async def get_values(
         self,
         range_name: str = None,
         major_dimension: str = None,
         value_render_option: gspread.utils.ValueRenderOption = None,
         date_time_render_option: gspread.utils.DateTimeOption = None,
     ) -> List[List]:
@@ -2196,14 +2258,47 @@
         :param bool nowait: (optional) If true, return a scheduled future instead of waiting for the API call to complete.
 
         .. versionadded:: 1.4
         """
         return await self.agcm._call(self.ws.insert_note, cell, content)
 
     @_nowait
+    async def insert_notes(self, notes: Dict):
+        """Insert multiple notes.
+
+        :param dict notes: A dict of notes with their cells coordinates and respective content
+
+            dict format is:
+
+            * key: the cell coordinates as A1 range format
+            * value: the string content of the cell
+
+            Example::
+
+                {
+                    "D7": "Please read my notes",
+                    "GH42": "this one is too far",
+                }
+
+        .. versionadded:: 1.9
+        """
+        return await self.agcm._call(self.ws.insert_notes, notes)
+
+    @_nowait
+    async def clear_notes(self, ranges: List[str]):
+        """Clear all notes located at the cells in `ranges`.
+
+        :param ranges: List of A1 coordinates to clear notes
+        :type ranges: :class:`~typing.List`\\[:class:`str`\\]
+
+        .. versionadded:: 1.9
+        """
+        return await self.agcm._call(self.ws.clear_notes, ranges)
+
+    @_nowait
     async def insert_row(
         self,
         values: List,
         index: int = 1,
         value_input_option: gspread.utils.ValueInputOption = gspread.utils.ValueInputOption.raw,
         inherit_from_before: bool = False,
     ):
@@ -2425,14 +2520,28 @@
     async def show(self):
         """Show the current worksheet in the UI.
 
         .. versionadded:: 1.6
         """
         return await self.agcm._call(self.ws.show)
 
+    async def hide_gridlines(self):
+        """Hide gridlines on the current worksheet
+
+        .. versionadded:: 1.9
+        """
+        return await self.agcm._call(self.ws.hide_gridlines)
+
+    async def show_gridlines(self):
+        """Show gridlines on the current worksheet
+
+        .. versionadded:: 1.9
+        """
+        return await self.agcm._call(self.ws.show_gridlines)
+
     async def sort(self, specs: List[Tuple[int, str]], range: str = None):
         """Sorts worksheet using given sort orders.
 
         :param list specs: The sort order per column. Each sort order
             represented by a tuple where the first element is a column index
             and the second element is the order itself: 'asc' or 'des'.
         :param str range: The range to sort in A1 notation. By default sorts
```

### Comparing `gspread_asyncio-1.8.1/gspread_asyncio.egg-info/PKG-INFO` & `gspread_asyncio-1.9.0/gspread_asyncio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspread-asyncio
-Version: 1.8.1
+Version: 1.9.0
 Summary: asyncio wrapper for burnash's Google Spreadsheet API library, gspread
 Home-page: https://github.com/dgilman/gspread_asyncio
 Author: David Gilman
 Author-email: dgilman@gilslotd.com
 License: MIT
 Project-URL: Documentation, https://gspread-asyncio.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/dgilman/gspread_asyncio
```

### Comparing `gspread_asyncio-1.8.1/setup.py` & `gspread_asyncio-1.9.0/setup.py`

 * *Files identical despite different names*

