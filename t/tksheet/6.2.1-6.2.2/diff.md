# Comparing `tmp/tksheet-6.2.1.tar.gz` & `tmp/tksheet-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-6.2.1.tar", last modified: Mon Jun  5 17:39:49 2023, max compression
+gzip compressed data, was "tksheet-6.2.2.tar", last modified: Mon Jul 10 09:13:21 2023, max compression
```

## Comparing `tksheet-6.2.1.tar` & `tksheet-6.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 17:39:49.065009 tksheet-6.2.1/
--rw-rw-rw-   0        0        0     1101 2023-06-05 17:22:27.000000 tksheet-6.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3657 2023-06-05 17:39:49.066009 tksheet-6.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3007 2023-06-05 17:22:27.000000 tksheet-6.2.1/README.md
--rw-rw-rw-   0        0        0       86 2023-06-05 17:39:49.069520 tksheet-6.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-06-05 17:26:19.000000 tksheet-6.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:39:49.060003 tksheet-6.2.1/tksheet/
--rw-rw-rw-   0        0        0     1901 2023-06-05 17:22:27.000000 tksheet-6.2.1/tksheet/__init__.py
--rw-rw-rw-   0        0        0   164453 2023-06-05 17:33:41.000000 tksheet-6.2.1/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0   111843 2023-06-05 17:28:15.000000 tksheet-6.2.1/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0     8880 2023-06-05 17:28:19.000000 tksheet-6.2.1/tksheet/_tksheet_formatters.py
--rw-rw-rw-   0        0        0   333260 2023-06-05 17:29:44.000000 tksheet-6.2.1/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    12733 2023-06-05 17:28:30.000000 tksheet-6.2.1/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0   108771 2023-06-05 17:28:35.000000 tksheet-6.2.1/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5784 2023-06-05 17:28:39.000000 tksheet-6.2.1/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    60025 2023-06-05 17:28:46.000000 tksheet-6.2.1/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:39:49.065009 tksheet-6.2.1/tksheet.egg-info/
--rw-rw-rw-   0        0        0     3657 2023-06-05 17:39:49.000000 tksheet-6.2.1/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-06-05 17:39:49.000000 tksheet-6.2.1/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 17:39:49.000000 tksheet-6.2.1/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-05 17:39:49.000000 tksheet-6.2.1/tksheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 09:13:21.217928 tksheet-6.2.2/
+-rw-rw-rw-   0        0        0     1101 2023-07-09 07:20:56.000000 tksheet-6.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3657 2023-07-10 09:13:21.217928 tksheet-6.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3007 2023-07-09 07:20:56.000000 tksheet-6.2.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-10 09:13:21.218930 tksheet-6.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-07-09 07:23:02.000000 tksheet-6.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:13:21.207333 tksheet-6.2.2/tksheet/
+-rw-rw-rw-   0        0        0     1901 2023-07-09 07:20:56.000000 tksheet-6.2.2/tksheet/__init__.py
+-rw-rw-rw-   0        0        0   165253 2023-07-09 18:18:57.000000 tksheet-6.2.2/tksheet/_tksheet.py
+-rw-rw-rw-   0        0        0   112139 2023-07-09 17:19:23.000000 tksheet-6.2.2/tksheet/_tksheet_column_headers.py
+-rw-rw-rw-   0        0        0     8880 2023-07-09 07:20:56.000000 tksheet-6.2.2/tksheet/_tksheet_formatters.py
+-rw-rw-rw-   0        0        0   334327 2023-07-09 17:31:47.000000 tksheet-6.2.2/tksheet/_tksheet_main_table.py
+-rw-rw-rw-   0        0        0    12733 2023-07-09 07:20:56.000000 tksheet-6.2.2/tksheet/_tksheet_other_classes.py
+-rw-rw-rw-   0        0        0   109067 2023-07-09 17:20:47.000000 tksheet-6.2.2/tksheet/_tksheet_row_index.py
+-rw-rw-rw-   0        0        0     5784 2023-07-09 07:20:56.000000 tksheet-6.2.2/tksheet/_tksheet_top_left_rectangle.py
+-rw-rw-rw-   0        0        0    60025 2023-07-09 07:20:56.000000 tksheet-6.2.2/tksheet/_tksheet_vars.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:13:21.217928 tksheet-6.2.2/tksheet.egg-info/
+-rw-rw-rw-   0        0        0     3657 2023-07-10 09:13:21.000000 tksheet-6.2.2/tksheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-07-10 09:13:21.000000 tksheet-6.2.2/tksheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 09:13:21.000000 tksheet-6.2.2/tksheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-10 09:13:21.000000 tksheet-6.2.2/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-6.2.1/LICENSE.txt` & `tksheet-6.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.1/PKG-INFO` & `tksheet-6.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.2.1
+Version: 6.2.2
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.2.1.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.2.2.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tksheet-6.2.1/README.md` & `tksheet-6.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.1/setup.py` & `tksheet-6.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'tksheet',
   packages = ['tksheet'],
-  version = '6.2.1',
+  version = '6.2.2',
   python_requires = '>=3.6',
   license = 'MIT',
   description = 'Tkinter table / sheet widget',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'ragardner',
   author_email = 'github@ragardner.simplelogin.com',
   url = 'https://github.com/ragardner/tksheet',
-  download_url = 'https://github.com/ragardner/tksheet/archive/6.2.1.tar.gz',
+  download_url = 'https://github.com/ragardner/tksheet/archive/6.2.2.tar.gz',
   keywords = ['tkinter', 'table', 'widget', 'sheet', 'grid', 'tk'],
   install_requires = [],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License'
```

### Comparing `tksheet-6.2.1/tksheet/__init__.py` & `tksheet-6.2.2/tksheet/__init__.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.1/tksheet/_tksheet.py` & `tksheet-6.2.2/tksheet/_tksheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -844,14 +844,34 @@
             e.data = args[0]
             e.widget = widget
             return (e,)
 
         funcid = widget._register(func, _substitute, needcleanup=1)
         cmd = '{0}if {{"[{1} %d]" == "break"}} break\n'.format("+" if add else "", funcid)
         widget.tk.call("bind", widget._w, sequence, cmd)
+        
+    def sync_scroll(self, widget: object) -> Sheet:
+        if widget is self:
+            return self
+        self.MT.synced_scrolls.add(widget)
+        if isinstance(widget, Sheet):
+            widget.MT.synced_scrolls.add(self)
+        return self
+        
+    def unsync_scroll(self, widget: None | Sheet = None) -> Sheet:
+        if widget is None:
+            for widget in self.MT.synced_scrolls:
+                if isinstance(widget, Sheet):
+                    widget.MT.synced_scrolls.discard(self)
+            self.MT.synced_scrolls = set()
+        else:
+            if isinstance(widget, Sheet) and self in widget.MT.synced_scrolls:
+                widget.MT.synced_scrolls.discard(self)
+            self.MT.synced_scrolls.discard(widget)
+        return self
 
     def bind(self, binding, func, add=None):
         if binding == "<ButtonPress-1>":
             self.MT.extra_b1_press_func = func
             self.CH.extra_b1_press_func = func
             self.RI.extra_b1_press_func = func
             self.TL.extra_b1_press_func = func
```

### Comparing `tksheet-6.2.1/tksheet/_tksheet_column_headers.py` & `tksheet-6.2.2/tksheet/_tksheet_column_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -708,23 +708,25 @@
             if x >= wend + 15:
                 self.MT.xview_scroll(2, "units")
                 self.xview_scroll(2, "units")
             else:
                 self.MT.xview_scroll(1, "units")
                 self.xview_scroll(1, "units")
             self.fix_xview()
+            self.MT.x_move_synced_scrolls("moveto", self.MT.xview()[0])
             self.MT.main_table_redraw_grid_and_text(redraw_header=True)
         elif x <= 0 and len(xcheck) > 1 and xcheck[0] > 0:
             if x >= -15:
                 self.MT.xview_scroll(-1, "units")
                 self.xview_scroll(-1, "units")
             else:
                 self.MT.xview_scroll(-2, "units")
                 self.xview_scroll(-2, "units")
             self.fix_xview()
+            self.MT.x_move_synced_scrolls("moveto", self.MT.xview()[0])
             self.MT.main_table_redraw_grid_and_text(redraw_header=True)
         col = self.MT.identify_col(x=event.x)
         if col >= self.dragged_col.to_move[0] and col <= self.dragged_col.to_move[-1]:
             xpos = self.MT.col_positions[self.dragged_col.to_move[0]]
         else:
             if col < self.dragged_col.to_move[0]:
                 xpos = self.MT.col_positions[col]
@@ -768,22 +770,24 @@
         if event.x > self.winfo_width() and len(xcheck) > 1 and xcheck[1] < 1:
             try:
                 self.MT.xview_scroll(1, "units")
                 self.xview_scroll(1, "units")
             except Exception:
                 pass
             self.fix_xview()
+            self.MT.x_move_synced_scrolls("moveto", self.MT.xview()[0])
             need_redraw = True
         elif event.x < 0 and self.canvasx(self.winfo_width()) > 0 and xcheck and xcheck[0] > 0:
             try:
                 self.xview_scroll(-1, "units")
                 self.MT.xview_scroll(-1, "units")
             except Exception:
                 pass
             self.fix_xview()
+            self.MT.x_move_synced_scrolls("moveto", self.MT.xview()[0])
             need_redraw = True
         return need_redraw
 
     def fix_xview(self):
         xcheck = self.xview()
         if xcheck and xcheck[0] < 0:
             self.MT.set_xviews("moveto", 0)
@@ -1404,15 +1408,15 @@
         col_pos_exists,
     ):
         try:
             self.configure(
                 scrollregion=(
                     0,
                     0,
-                    last_col_line_pos + self.MT.empty_horizontal,
+                    last_col_line_pos + self.MT.empty_horizontal + 2,
                     self.current_height,
                 )
             )
         except Exception:
             return
         for k, v in self.disp_text.items():
             if k in self.hidd_text:
```

### Comparing `tksheet-6.2.1/tksheet/_tksheet_formatters.py` & `tksheet-6.2.2/tksheet/_tksheet_formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.1/tksheet/_tksheet_main_table.py` & `tksheet-6.2.2/tksheet/_tksheet_main_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         self.existing_dropdown_window = None
         self.closed_dropdown = None
         self.last_selected = tuple()
         self.centre_alignment_text_mod_indexes = (slice(1, None), slice(None, -1))
         self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
         self.grid_cyctup = ("st", "end")
         self.grid_cyc = cycle(self.grid_cyctup)
+        self.synced_scrolls = set()
 
         self.disp_ctrl_outline = {}
         self.disp_text = defaultdict(set)
         self.disp_high = defaultdict(set)
         self.disp_grid = {}
         self.disp_fill_sels = {}
         self.disp_bord_sels = {}
@@ -1290,16 +1291,14 @@
                 self._row_index[r] = v
             self.reselect_from_get_boxes(undo_storage[2])
             self.set_currently_selected(0, undo_storage[3][1], type_="row")
 
         if undo_storage[0] in ("edit_cells", "edit_cells_paste"):
             for (datarn, datacn), v in undo_storage[1].items():
                 self.set_cell_data(datarn, datacn, v)
-            start_row = float("inf")
-            start_col = float("inf")
             if undo_storage[0] == "edit_cells_paste" and self.expand_sheet_if_paste_too_big:
                 if undo_storage[4][0] > 0:
                     self.del_row_positions(
                         len(self.row_positions) - 1 - undo_storage[4][0],
                         undo_storage[4][0],
                     )
                     self.data[:] = self.data[: -undo_storage[4][0]]
@@ -1315,20 +1314,17 @@
             self.reselect_from_get_boxes(undo_storage[2])
             if undo_storage[3]:
                 self.set_currently_selected(
                     undo_storage[3].row,
                     undo_storage[3].column,
                     type_=undo_storage[3].type_,
                 )
-            elif start_row < len(self.row_positions) - 1 and start_col < len(self.col_positions) - 1:
-                self.set_currently_selected(start_row, start_col, type_="cell")
-            if start_row < len(self.row_positions) - 1 and start_col < len(self.col_positions) - 1:
                 self.see(
-                    r=start_row,
-                    c=start_col,
+                    r=undo_storage[3].row,
+                    c=undo_storage[3].column,
                     keep_yscroll=False,
                     keep_xscroll=False,
                     bottom_right_corner=False,
                     check_cell_visibility=True,
                     redraw=False,
                 )
 
@@ -1544,51 +1540,47 @@
                         y = self.row_positions[r + 1] + 1 - winfo_height
                     args = (
                         "moveto",
                         y / (self.row_positions[-1] + self.empty_vertical),
                     )
                     if args[1] > 1:
                         args[1] = args[1] - 1
-                    self.yview(*args)
-                    self.RI.yview(*args)
+                    self.set_yviews(*args, redraw=False)
                     need_redraw = True
             else:
                 if r is not None and not keep_yscroll:
                     args = (
                         "moveto",
                         self.row_positions[r] / (self.row_positions[-1] + self.empty_vertical),
                     )
                     if args[1] > 1:
                         args[1] = args[1] - 1
-                    self.yview(*args)
-                    self.RI.yview(*args)
+                    self.set_yviews(*args, redraw=False)
                     need_redraw = True
         if not xvis:
             if bottom_right_corner:
                 if c is not None and not keep_xscroll:
                     winfo_width = self.winfo_width()
                     if self.col_positions[c + 1] - self.col_positions[c] > winfo_width:
                         x = self.col_positions[c]
                     else:
                         x = self.col_positions[c + 1] + 1 - winfo_width
                     args = (
                         "moveto",
                         x / (self.col_positions[-1] + self.empty_horizontal),
                     )
-                    self.xview(*args)
-                    self.CH.xview(*args)
+                    self.set_xviews(*args, redraw=False)
                     need_redraw = True
             else:
                 if c is not None and not keep_xscroll:
                     args = (
                         "moveto",
                         self.col_positions[c] / (self.col_positions[-1] + self.empty_horizontal),
                     )
-                    self.xview(*args)
-                    self.CH.xview(*args)
+                    self.set_xviews(*args, redraw=False)
                     need_redraw = True
         if redraw and need_redraw:
             self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             return True
         else:
             return False
 
@@ -3278,29 +3270,29 @@
             return None
         return c
 
     def fix_views(self):
         xcheck = self.xview()
         ycheck = self.yview()
         if xcheck and xcheck[0] <= 0:
-            self.xview(*("moveto", 0))
+            self.xview("moveto", 0)
             if self.show_header:
-                self.CH.xview(*("moveto", 0))
+                self.CH.xview("moveto", 0)
         elif len(xcheck) > 1 and xcheck[1] >= 1:
-            self.xview(*("moveto", 1))
+            self.xview("moveto", 1)
             if self.show_header:
-                self.CH.xview(*("moveto", 1))
+                self.CH.xview("moveto", 1)
         if ycheck and ycheck[0] <= 0:
-            self.yview(*("moveto", 0))
+            self.yview("moveto", 0)
             if self.show_index:
-                self.RI.yview(*("moveto", 0))
+                self.RI.yview("moveto", 0)
         elif len(ycheck) > 1 and ycheck[1] >= 1:
-            self.yview(*("moveto", 1))
+            self.yview("moveto", 1)
             if self.show_index:
-                self.RI.yview(*("moveto", 1))
+                self.RI.yview("moveto", 1)
 
     def scroll_if_event_offscreen(self, event):
         need_redraw = False
         if self.data:
             xcheck = self.xview()
             ycheck = self.yview()
             if len(xcheck) > 1 and xcheck[0] > 0 and event.x < 0:
@@ -3329,63 +3321,97 @@
                     self.yview_scroll(1, "units")
                     self.RI.yview_scroll(1, "units")
                 except Exception:
                     pass
                 need_redraw = True
         if need_redraw:
             self.fix_views()
+            self.x_move_synced_scrolls("moveto", self.xview()[0])
+            self.y_move_synced_scrolls("moveto", self.yview()[0])
         return need_redraw
+    
+    def x_move_synced_scrolls(self, *args, redraw=True):
+        for widget in self.synced_scrolls:
+            # try:
+            if hasattr(widget, "MT"):
+                widget.MT.set_xviews(*args, move_synced=False, redraw=redraw)
+            else:
+                widget.xview(*args)
+            # except Exception:
+            #     continue
+                
+    def y_move_synced_scrolls(self, *args, redraw=True):
+        for widget in self.synced_scrolls:
+            # try:
+            if hasattr(widget, "MT"):
+                widget.MT.set_yviews(*args, move_synced=False, redraw=redraw)
+            else:
+                widget.yview(*args)
+            # except Exception:
+            #     continue
 
-    def set_xviews(self, *args):
+    def set_xviews(self, *args, move_synced=True, redraw=True):
         self.xview(*args)
         if self.show_header:
             self.CH.xview(*args)
+        if move_synced:
+            self.x_move_synced_scrolls(*args)
         self.fix_views()
-        self.main_table_redraw_grid_and_text(redraw_header=True if self.show_header else False)
+        if redraw:
+            self.main_table_redraw_grid_and_text(redraw_header=True if self.show_header else False)
 
-    def set_yviews(self, *args):
+    def set_yviews(self, *args, move_synced=True, redraw=True):
         self.yview(*args)
         if self.show_index:
             self.RI.yview(*args)
+        if move_synced:
+            self.y_move_synced_scrolls(*args)
         self.fix_views()
-        self.main_table_redraw_grid_and_text(redraw_row_index=True if self.show_index else False)
+        if redraw:
+            self.main_table_redraw_grid_and_text(redraw_row_index=True if self.show_index else False)
 
     def set_view(self, x_args, y_args):
         self.xview(*x_args)
         if self.show_header:
             self.CH.xview(*x_args)
         self.yview(*y_args)
         if self.show_index:
             self.RI.yview(*y_args)
+        self.x_move_synced_scrolls(*x_args)
+        self.y_move_synced_scrolls(*y_args)
         self.fix_views()
         self.main_table_redraw_grid_and_text(
             redraw_row_index=True if self.show_index else False,
             redraw_header=True if self.show_header else False,
         )
 
     def mousewheel(self, event=None):
         if event.delta < 0 or event.num == 5:
             self.yview_scroll(1, "units")
             self.RI.yview_scroll(1, "units")
+            self.y_move_synced_scrolls("moveto", self.yview()[0])
         elif event.delta >= 0 or event.num == 4:
             if self.canvasy(0) <= 0:
                 return
             self.yview_scroll(-1, "units")
             self.RI.yview_scroll(-1, "units")
+            self.y_move_synced_scrolls("moveto", self.yview()[0])
         self.main_table_redraw_grid_and_text(redraw_row_index=True)
 
     def shift_mousewheel(self, event=None):
         if event.delta < 0 or event.num == 5:
             self.xview_scroll(1, "units")
             self.CH.xview_scroll(1, "units")
+            self.x_move_synced_scrolls("moveto", self.xview()[0])
         elif event.delta >= 0 or event.num == 4:
             if self.canvasx(0) <= 0:
                 return
             self.xview_scroll(-1, "units")
             self.CH.xview_scroll(-1, "units")
+            self.x_move_synced_scrolls("moveto", self.xview()[0])
         self.main_table_redraw_grid_and_text(redraw_header=True)
 
     def get_txt_w(self, txt, font=None):
         self.txt_measure_canvas.itemconfig(
             self.txt_measure_canvas_text,
             text=txt,
             font=self.table_font if font is None else font,
```

### Comparing `tksheet-6.2.1/tksheet/_tksheet_other_classes.py` & `tksheet-6.2.2/tksheet/_tksheet_other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.1/tksheet/_tksheet_row_index.py` & `tksheet-6.2.2/tksheet/_tksheet_row_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -664,23 +664,25 @@
             if y >= hend + 15:
                 self.MT.yview_scroll(2, "units")
                 self.yview_scroll(2, "units")
             else:
                 self.MT.yview_scroll(1, "units")
                 self.yview_scroll(1, "units")
             self.fix_yview()
+            self.MT.y_move_synced_scrolls("moveto", self.MT.yview()[0])
             self.MT.main_table_redraw_grid_and_text(redraw_row_index=True)
         elif y <= 0 and len(ycheck) > 1 and ycheck[0] > 0:
             if y >= -15:
                 self.MT.yview_scroll(-1, "units")
                 self.yview_scroll(-1, "units")
             else:
                 self.MT.yview_scroll(-2, "units")
                 self.yview_scroll(-2, "units")
             self.fix_yview()
+            self.MT.y_move_synced_scrolls("moveto", self.MT.yview()[0])
             self.MT.main_table_redraw_grid_and_text(redraw_row_index=True)
         row = self.MT.identify_row(y=event.y)
         if row >= self.dragged_row.to_move[0] and row <= self.dragged_row.to_move[-1]:
             ypos = self.MT.row_positions[self.dragged_row.to_move[0]]
         else:
             if row < self.dragged_row.to_move[0]:
                 ypos = self.MT.row_positions[row]
@@ -724,22 +726,24 @@
         if event.y > self.winfo_height() and len(ycheck) > 1 and ycheck[1] < 1:
             try:
                 self.MT.yview_scroll(1, "units")
                 self.yview_scroll(1, "units")
             except Exception:
                 pass
             self.fix_yview()
+            self.MT.y_move_synced_scrolls("moveto", self.MT.yview()[0])
             need_redraw = True
         elif event.y < 0 and self.canvasy(self.winfo_height()) > 0 and ycheck and ycheck[0] > 0:
             try:
                 self.yview_scroll(-1, "units")
                 self.MT.yview_scroll(-1, "units")
             except Exception:
                 pass
             self.fix_yview()
+            self.MT.y_move_synced_scrolls("moveto", self.MT.yview()[0])
             need_redraw = True
         return need_redraw
 
     def fix_yview(self):
         ycheck = self.yview()
         if ycheck and ycheck[0] < 0:
             self.MT.set_yviews("moveto", 0)
@@ -1349,15 +1353,15 @@
     ):
         try:
             self.configure(
                 scrollregion=(
                     0,
                     0,
                     self.current_width,
-                    last_row_line_pos + self.MT.empty_vertical,
+                    last_row_line_pos + self.MT.empty_vertical + 2,
                 )
             )
         except Exception:
             return
         for k, v in self.disp_text.items():
             if k in self.hidd_text:
                 self.hidd_text[k] = self.hidd_text[k] | self.disp_text[k]
```

### Comparing `tksheet-6.2.1/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.2.2/tksheet/_tksheet_top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.1/tksheet/_tksheet_vars.py` & `tksheet-6.2.2/tksheet/_tksheet_vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.2.1/tksheet.egg-info/PKG-INFO` & `tksheet-6.2.2/tksheet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.2.1
+Version: 6.2.2
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.2.1.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.2.2.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

