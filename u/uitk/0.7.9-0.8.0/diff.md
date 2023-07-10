# Comparing `tmp/uitk-0.7.9.tar.gz` & `tmp/uitk-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uitk-0.7.9.tar", last modified: Mon Jul  3 15:11:22 2023, max compression
+gzip compressed data, was "uitk-0.8.0.tar", last modified: Mon Jul 10 17:27:54 2023, max compression
```

## Comparing `uitk-0.7.9.tar` & `uitk-0.8.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 15:11:22.095646 uitk-0.7.9/
--rw-rw-rw-   0        0        0     7815 2023-04-16 12:18:04.000000 uitk-0.7.9/COPYING.LESSER
--rw-rw-rw-   0        0        0       24 2023-03-28 23:38:26.000000 uitk-0.7.9/MANIFEST.in
--rw-rw-rw-   0        0        0     3691 2023-07-03 15:11:22.095646 uitk-0.7.9/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-03 15:11:22.095646 uitk-0.7.9/setup.cfg
--rw-rw-rw-   0        0        0     1535 2023-06-28 02:16:42.000000 uitk-0.7.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:11:22.057646 uitk-0.7.9/uitk/
--rw-rw-rw-   0        0        0     2937 2023-07-03 15:11:19.000000 uitk-0.7.9/uitk/__init__.py
--rw-rw-rw-   0        0        0    11209 2023-07-02 22:36:44.000000 uitk-0.7.9/uitk/events.py
--rw-rw-rw-   0        0        0    79273 2023-07-03 14:51:51.000000 uitk-0.7.9/uitk/switchboard.py
--rw-rw-rw-   0        0        0   100538 2023-07-01 11:42:38.000000 uitk-0.7.9/uitk/switchboard.py.bak
-drwxrwxrwx   0        0        0        0 2023-07-03 15:11:22.086648 uitk-0.7.9/uitk/widgets/
--rw-rw-rw-   0        0        0    19457 2023-07-02 22:38:42.000000 uitk-0.7.9/uitk/widgets/MainWindow.py
--rw-rw-rw-   0        0        0     3204 2023-05-24 20:56:51.000000 uitk-0.7.9/uitk/widgets/__init__.py
--rw-rw-rw-   0        0        0    15978 2023-06-29 12:22:22.000000 uitk-0.7.9/uitk/widgets/attributeWindow.py
--rw-rw-rw-   0        0        0     5597 2023-07-03 11:38:23.000000 uitk-0.7.9/uitk/widgets/checkBox.py
--rw-rw-rw-   0        0        0     7040 2023-07-03 11:08:37.000000 uitk-0.7.9/uitk/widgets/comboBox.py
--rw-rw-rw-   0        0        0     6954 2023-07-02 00:38:56.000000 uitk-0.7.9/uitk/widgets/draggableHeader.py
--rw-rw-rw-   0        0        0    22380 2023-07-03 00:41:20.000000 uitk-0.7.9/uitk/widgets/expandableList.py
--rw-rw-rw-   0        0        0     2494 2023-07-02 00:29:49.000000 uitk-0.7.9/uitk/widgets/label.py
--rw-rw-rw-   0        0        0     3234 2023-07-02 00:30:20.000000 uitk-0.7.9/uitk/widgets/lineEdit.py
--rw-rw-rw-   0        0        0    22049 2023-07-03 11:48:15.000000 uitk-0.7.9/uitk/widgets/menu.py
--rw-rw-rw-   0        0        0     8559 2023-06-23 14:22:44.000000 uitk-0.7.9/uitk/widgets/messageBox.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:11:22.094645 uitk-0.7.9/uitk/widgets/mixins/
--rw-rw-rw-   0        0        0     3028 2023-05-12 17:13:16.000000 uitk-0.7.9/uitk/widgets/mixins/__init__.py
--rw-rw-rw-   0        0        0    11901 2023-07-02 22:55:42.000000 uitk-0.7.9/uitk/widgets/mixins/attributes.py
--rw-rw-rw-   0        0        0     4023 2023-05-12 17:25:02.000000 uitk-0.7.9/uitk/widgets/mixins/convert.py
--rw-rw-rw-   0        0        0     9499 2023-05-20 02:33:14.000000 uitk-0.7.9/uitk/widgets/mixins/docking.py
--rw-rw-rw-   0        0        0    49547 2023-06-29 12:04:05.000000 uitk-0.7.9/uitk/widgets/mixins/style_sheet.py
--rw-rw-rw-   0        0        0     3409 2023-05-12 17:27:14.000000 uitk-0.7.9/uitk/widgets/mixins/tasks.py
--rw-rw-rw-   0        0        0    11111 2023-07-02 22:52:42.000000 uitk-0.7.9/uitk/widgets/mixins/text.py
--rw-rw-rw-   0        0        0     6046 2023-07-01 23:43:08.000000 uitk-0.7.9/uitk/widgets/optionBox.py
--rw-rw-rw-   0        0        0     3278 2023-06-05 16:23:13.000000 uitk-0.7.9/uitk/widgets/progressBar.py
--rw-rw-rw-   0        0        0     2113 2023-07-03 11:07:37.000000 uitk-0.7.9/uitk/widgets/pushButton.py
--rw-rw-rw-   0        0        0     7907 2023-05-28 21:08:35.000000 uitk-0.7.9/uitk/widgets/region.py
--rw-rw-rw-   0        0        0     3655 2023-07-02 00:31:26.000000 uitk-0.7.9/uitk/widgets/textEdit.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:11:22.070645 uitk-0.7.9/uitk.egg-info/
--rw-rw-rw-   0        0        0     3691 2023-07-03 15:11:21.000000 uitk-0.7.9/uitk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4282 2023-05-11 02:02:25.000000 uitk-0.7.9/uitk.egg-info/PKG-INFO.bak
--rw-rw-rw-   0        0        0      948 2023-07-03 15:11:21.000000 uitk-0.7.9/uitk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      767 2023-04-15 12:48:17.000000 uitk-0.7.9/uitk.egg-info/SOURCES.txt.bak
--rw-rw-rw-   0        0        0        1 2023-07-03 15:11:21.000000 uitk-0.7.9/uitk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-03 15:11:21.000000 uitk-0.7.9/uitk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 17:27:54.482700 uitk-0.8.0/
+-rw-rw-rw-   0        0        0     7815 2023-04-16 12:18:04.000000 uitk-0.8.0/COPYING.LESSER
+-rw-rw-rw-   0        0        0       24 2023-03-28 23:38:26.000000 uitk-0.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3691 2023-07-10 17:27:54.481702 uitk-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-10 17:27:54.482700 uitk-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1535 2023-06-28 02:16:42.000000 uitk-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 17:27:54.426702 uitk-0.8.0/uitk/
+-rw-rw-rw-   0        0        0     2937 2023-07-10 17:27:49.000000 uitk-0.8.0/uitk/__init__.py
+-rw-rw-rw-   0        0        0    11209 2023-07-02 22:36:44.000000 uitk-0.8.0/uitk/events.py
+-rw-rw-rw-   0        0        0    79234 2023-07-08 18:06:12.000000 uitk-0.8.0/uitk/switchboard.py
+-rw-rw-rw-   0        0        0    78582 2023-07-07 17:26:57.000000 uitk-0.8.0/uitk/switchboard.py.bak
+drwxrwxrwx   0        0        0        0 2023-07-10 17:27:54.471702 uitk-0.8.0/uitk/widgets/
+-rw-rw-rw-   0        0        0    19457 2023-07-02 22:38:42.000000 uitk-0.8.0/uitk/widgets/MainWindow.py
+-rw-rw-rw-   0        0        0     3204 2023-05-24 20:56:51.000000 uitk-0.8.0/uitk/widgets/__init__.py
+-rw-rw-rw-   0        0        0    15978 2023-06-29 12:22:22.000000 uitk-0.8.0/uitk/widgets/attributeWindow.py
+-rw-rw-rw-   0        0        0     5597 2023-07-03 11:38:23.000000 uitk-0.8.0/uitk/widgets/checkBox.py
+-rw-rw-rw-   0        0        0     9719 2023-07-10 16:56:56.000000 uitk-0.8.0/uitk/widgets/comboBox.py
+-rw-rw-rw-   0        0        0     6954 2023-07-02 00:38:56.000000 uitk-0.8.0/uitk/widgets/draggableHeader.py
+-rw-rw-rw-   0        0        0    22493 2023-07-10 00:53:06.000000 uitk-0.8.0/uitk/widgets/expandableList.py
+-rw-rw-rw-   0        0        0     2494 2023-07-02 00:29:49.000000 uitk-0.8.0/uitk/widgets/label.py
+-rw-rw-rw-   0        0        0     3234 2023-07-02 00:30:20.000000 uitk-0.8.0/uitk/widgets/lineEdit.py
+-rw-rw-rw-   0        0        0    22168 2023-07-07 13:37:31.000000 uitk-0.8.0/uitk/widgets/menu.py
+-rw-rw-rw-   0        0        0     8559 2023-06-23 14:22:44.000000 uitk-0.8.0/uitk/widgets/messageBox.py
+drwxrwxrwx   0        0        0        0 2023-07-10 17:27:54.480701 uitk-0.8.0/uitk/widgets/mixins/
+-rw-rw-rw-   0        0        0     3028 2023-05-12 17:13:16.000000 uitk-0.8.0/uitk/widgets/mixins/__init__.py
+-rw-rw-rw-   0        0        0    11901 2023-07-02 22:55:42.000000 uitk-0.8.0/uitk/widgets/mixins/attributes.py
+-rw-rw-rw-   0        0        0     4023 2023-05-12 17:25:02.000000 uitk-0.8.0/uitk/widgets/mixins/convert.py
+-rw-rw-rw-   0        0        0     9499 2023-05-20 02:33:14.000000 uitk-0.8.0/uitk/widgets/mixins/docking.py
+-rw-rw-rw-   0        0        0    49547 2023-06-29 12:04:05.000000 uitk-0.8.0/uitk/widgets/mixins/style_sheet.py
+-rw-rw-rw-   0        0        0     3409 2023-05-12 17:27:14.000000 uitk-0.8.0/uitk/widgets/mixins/tasks.py
+-rw-rw-rw-   0        0        0    11111 2023-07-02 22:52:42.000000 uitk-0.8.0/uitk/widgets/mixins/text.py
+-rw-rw-rw-   0        0        0     6046 2023-07-10 16:14:24.000000 uitk-0.8.0/uitk/widgets/optionBox.py
+-rw-rw-rw-   0        0        0     3278 2023-06-05 16:23:13.000000 uitk-0.8.0/uitk/widgets/progressBar.py
+-rw-rw-rw-   0        0        0     2113 2023-07-03 11:07:37.000000 uitk-0.8.0/uitk/widgets/pushButton.py
+-rw-rw-rw-   0        0        0     7907 2023-05-28 21:08:35.000000 uitk-0.8.0/uitk/widgets/region.py
+-rw-rw-rw-   0        0        0     3655 2023-07-02 00:31:26.000000 uitk-0.8.0/uitk/widgets/textEdit.py
+drwxrwxrwx   0        0        0        0 2023-07-10 17:27:54.455701 uitk-0.8.0/uitk.egg-info/
+-rw-rw-rw-   0        0        0     3691 2023-07-10 17:27:54.000000 uitk-0.8.0/uitk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4282 2023-05-11 02:02:25.000000 uitk-0.8.0/uitk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0      948 2023-07-10 17:27:54.000000 uitk-0.8.0/uitk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      767 2023-04-15 12:48:17.000000 uitk-0.8.0/uitk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-07-10 17:27:54.000000 uitk-0.8.0/uitk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-10 17:27:54.000000 uitk-0.8.0/uitk.egg-info/top_level.txt
```

### Comparing `uitk-0.7.9/COPYING.LESSER` & `uitk-0.8.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/PKG-INFO` & `uitk-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uitk
-Version: 0.7.9
+Version: 0.8.0
 Home-page: https://github.com/m3trik/uitk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `uitk-0.7.9/setup.py` & `uitk-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/__init__.py` & `uitk-0.8.0/uitk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import importlib
 import pkgutil
 import inspect
 from .switchboard import signals  # Make signals accessible at package root
 
 
 __package__ = "uitk"
-__version__ = '0.7.9'
+__version__ = '0.8.0'
 __path__ = [os.path.abspath(os.path.dirname(__file__))]
 
 
 # Define a dictionary to map class names to their respective modules
 CLASS_TO_MODULE = {}
 
 # Build the CLASS_TO_MODULE dictionary by iterating over all submodules of the package
```

### Comparing `uitk-0.7.9/uitk/events.py` & `uitk-0.8.0/uitk/events.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/switchboard.py` & `uitk-0.8.0/uitk/switchboard.py.bak`

 * *Files 1% similar despite different names*

```diff
@@ -1700,35 +1700,28 @@
                 k = k.replace("Un", "")
                 state = False
 
             # set the property state for each widget in the list.
             for w in widgets:
                 getattr(w, k)(state)
 
-    def connect_multi(self, widgets, signals, slots, clss=None):
+    def connect_multi(self, ui, widgets, signals, slots):
         """Connect multiple signals to multiple slots at once.
 
         Parameters:
-            widgets (str/obj/list): ie. 'chk000-2' or [tb.menu.chk000, tb.menu.chk001]
+            ui (QWidget): A previously loaded dynamic ui object.
+            widgets (str/list): ie. 'chk000-2' or [tb.menu.chk000, tb.menu.chk001]
             signals (str/list): ie. 'toggled' or ['toggled']
             slots (obj/list): ie. self.cmb002 or [self.cmb002]
-            clss (obj/list): if the widgets arg is given as a string, then the class it belongs to can be explicitly given.
-                    else, the current ui will be used.
+
         Example:
-            connect_('chk000-2', 'toggled', self.cmb002, tb.menu)
-            connect_([tb.menu.chk000, tb.menu.chk001], 'toggled', self.cmb002)
-            connect_(tb.menu.chk015, 'toggled',
-            [lambda state: self.rigging.tb004.setText('Unlock Transforms' if state else 'Lock Transforms'),
-            lambda state: self.rigging_submenu.tb004.setText('Unlock Transforms' if state else 'Lock Transforms')])
+            connect_multi(tb.menu, 'chk000-2', 'toggled', self.cmb002)
         """
         if isinstance(widgets, (str)):
-            try:  # get_widgets_from_str returns a widget list from a string of object_names.
-                widgets = self.get_widgets_from_str(clss, widgets)
-            except Exception:
-                widgets = self.get_widgets_from_str(self.get_current_ui(), widgets)
+            widgets = self.get_widgets_from_str(ui, widgets)
 
         # if the variables are not of a list type; convert them.
         widgets = ptk.make_iterable(widgets)
         signals = ptk.make_iterable(signals)
         slots = ptk.make_iterable(slots)
 
         for widget in widgets:
```

### Comparing `uitk-0.7.9/uitk/switchboard.py.bak` & `uitk-0.8.0/uitk/switchboard.py`

 * *Files 14% similar despite different names*

```diff
@@ -273,30 +273,35 @@
             # If the given dir is not a full path, treat it as relative to the default path.
             isAbsPath = os.path.isabs(x)
             ui_path = x if isAbsPath else os.path.join(self.default_dir, x)
 
         elif inspect.ismodule(x):
             # Use get_filepath to get the full path to the package.
             ui_path = ptk.get_filepath(x, inc_filename=True)
-
         else:
             raise ValueError(
                 f"Invalid datatype for ui_location: Expected str or module, got {type(x)}"
             )
 
         self.setWorkingDirectory(ui_path)  # Set QUiLoader working path.
         self.ui_files = self._construct_ui_files_dict(ui_path)
         self._ui_location = ui_path
 
     def _construct_ui_files_dict(self, ui_path) -> dict:
         """Build and return a dictionary of UI paths, where the keys are the UI file names and the values
         are the corresponding file paths.
 
+        Parameters:
+            ui_path (str): Path to the directory containing UI files.
+
+        Raises:
+            ValueError: If the input `ui_path` is not of type `str`.
+
         Returns:
-            dict: A dictionary of UI file paths with UI file names as keys.
+            dict: A dictionary mapping from UI file names to their respective paths.
         """
         if not isinstance(ui_path, str):
             raise ValueError(
                 f"Invalid datatype for _construct_ui_files_dict: Expected str, got {type(ui_path)}"
             )
 
         path = ptk.format_path(ui_path, "path")
@@ -346,75 +351,45 @@
                 f"Invalid datatype for widgets_location: Expected str, module, or QWidget(s), got {type(x)}"
             )
 
         self.addPluginPath(widgets_path)  # Set QUiLoader working path.
         self.widget_files = self._construct_widget_files_dict(widgets_path)
         self._widgets_location = widgets_path
 
-    @staticmethod
-    def _get_classes_in_directory(dir_path) -> dict:
-        """Given a directory, return a dictionary with all classes found in .py files in that directory and their respective filepaths.
+    def _construct_widget_files_dict(self, widgets_path) -> dict:
+        """Build and return a dictionary of widget paths or widget objects, where the keys are the widget
+        file names and the values are the corresponding file paths or widget objects.
 
         Parameters:
-            dir_path (str): A directory path containing Python (.py) files.
+            widgets_path (str/list/tuple/set): Path to the directory containing widget files or a collection of widget classes.
 
-        Returns:
-            dict: A dictionary where keys are class names and values are the paths of the Python files they were found in.
-        """
-        classes_dict = {}
-
-        if not os.path.isdir(dir_path):
-            raise ValueError(f"Provided path is not a directory: {dir_path}")
-
-        for filename in os.listdir(dir_path):
-            if filename.endswith(".py"):
-                file_path = os.path.join(dir_path, filename)
-                module_name = os.path.splitext(filename)[0]
-
-                try:
-                    spec = importlib.util.spec_from_file_location(
-                        module_name, file_path
-                    )
-                    module = importlib.util.module_from_spec(spec)
-                    spec.loader.exec_module(module)
-                except (ImportError, SyntaxError):
-                    continue
-
-                for name, obj in inspect.getmembers(module):
-                    if inspect.isclass(obj):
-                        classes_dict[name] = file_path
-
-        return classes_dict
-
-    def _construct_widget_files_dict(self, widgets_path) -> dict:
-        """Build and return a dictionary of widget paths, where the keys are the widget file names and the
-        values are the corresponding file paths or widget objects.
+        Raises:
+            ValueError: If the input `widgets_path` is not of type `str`, `list`, `tuple`, or `set`.
 
         Returns:
-            dict: A dictionary of widget file paths or widget objects with widget file names as keys.
+            dict: A dictionary mapping from widget file names to their respective paths or widget objects.
         """
         widget_dict = {}
 
         # First, add widget files from the default path
         default_path = f"{self.module_dir}/widgets"
         if os.path.isdir(default_path):
-            widget_dict.update(self._get_classes_in_directory(default_path))
+            widget_dict.update(ptk.get_classes_from_dir(default_path))
         else:
             print(f"Warning: Default widgets directory does not exist: {default_path}")
 
         # Then, add widget files from the given path
         if isinstance(widgets_path, str):
-            widget_dict.update(self._get_classes_in_directory(widgets_path))
+            widget_dict.update(ptk.get_classes_from_dir(widgets_path))
 
         elif isinstance(widgets_path, (list, tuple, set)):
             for widget in widgets_path:
                 widget_name = widget.__name__
                 widget_file = inspect.getfile(widget)
                 widget_dict[widget_name] = widget_file
-
         else:
             raise ValueError(
                 f"Invalid datatype for _construct_widget_files_dict: Expected str, list, tuple, or set, got {type(widgets_path)}"
             )
 
         return widget_dict
 
@@ -456,19 +431,24 @@
             )
 
         self.slots_files = self._construct_slots_files_dict(slots_path)
         self._slots_location = slots_path
 
     def _construct_slots_files_dict(self, slots_path) -> dict:
         """Build and return a dictionary of slot class paths, where the keys are the slot class file names
-        and the values are the corresponding file paths. The method supports two types of input for
-        slots_location: a directory path (str) or a class object.
+        and the values are the corresponding file paths or class objects.
+
+        Parameters:
+            slots_path (str/class): Path to the directory containing slot class files or a slot class object.
+
+        Raises:
+            ValueError: If the input `slots_path` is not of type `str` or `class`.
 
         Returns:
-            dict: A dictionary of slot class file paths with slot class file names as keys.
+            dict: A dictionary mapping from slot class file names to their respective paths or class objects.
         """
         if isinstance(slots_path, str):
             slots_filepaths = ptk.get_dir_contents(
                 slots_path, "filepaths", inc_files="*.py"
             )
             slots_files = ptk.get_file_info(slots_filepaths, "filename|filepath")
             return dict(slots_files)
@@ -1736,35 +1716,28 @@
                 k = k.replace("Un", "")
                 state = False
 
             # set the property state for each widget in the list.
             for w in widgets:
                 getattr(w, k)(state)
 
-    def connect_multi(self, widgets, signals, slots, clss=None):
+    def connect_widgets(self, ui, widgets, signals, slots):
         """Connect multiple signals to multiple slots at once.
 
         Parameters:
-            widgets (str/obj/list): ie. 'chk000-2' or [tb.option_menu.chk000, tb.option_menu.chk001]
+            ui (QWidget): A previously loaded dynamic ui object.
+            widgets (str/list): ie. 'chk000-2' or [tb.menu.chk000, tb.menu.chk001]
             signals (str/list): ie. 'toggled' or ['toggled']
             slots (obj/list): ie. self.cmb002 or [self.cmb002]
-            clss (obj/list): if the widgets arg is given as a string, then the class it belongs to can be explicitly given.
-                    else, the current ui will be used.
+
         Example:
-            connect_('chk000-2', 'toggled', self.cmb002, tb.option_menu)
-            connect_([tb.option_menu.chk000, tb.option_menu.chk001], 'toggled', self.cmb002)
-            connect_(tb.option_menu.chk015, 'toggled',
-            [lambda state: self.rigging.tb004.setText('Unlock Transforms' if state else 'Lock Transforms'),
-            lambda state: self.rigging_submenu.tb004.setText('Unlock Transforms' if state else 'Lock Transforms')])
+            connect_widgets(tb.menu, 'chk000-2', 'toggled', self.cmb002)
         """
         if isinstance(widgets, (str)):
-            try:  # get_widgets_from_str returns a widget list from a string of object_names.
-                widgets = self.get_widgets_from_str(clss, widgets)
-            except Exception:
-                widgets = self.get_widgets_from_str(self.get_current_ui(), widgets)
+            widgets = self.get_widgets_from_str(ui, widgets)
 
         # if the variables are not of a list type; convert them.
         widgets = ptk.make_iterable(widgets)
         signals = ptk.make_iterable(signals)
         slots = ptk.make_iterable(slots)
 
         for widget in widgets:
@@ -1940,481 +1913,7 @@
 
     ui.show(app_exec=True)
 
 logging.info(__name__)  # module name
 # --------------------------------------------------------------------------------------------
 # Notes
 # --------------------------------------------------------------------------------------------
-
-# --------------------------------------------------------------------------------------------
-# deprecated:
-# --------------------------------------------------------------------------------------------
-
-
-# def _create_slot_wrapper(self, slot, widget):
-#     """Creates a wrapper function for a slot that includes the widget as a parameter if possible.
-
-#     The wrapper function is designed to handle different widget-specific signal values as keyword arguments.
-#     The signal values are passed to the slot function as keyword arguments based on the type of the widget.
-
-#     If the slot function does not accept the widget or signal-specific keyword argument, it is called with positional arguments as a fallback.
-
-#     Parameters:
-#         slot (callable): The slot function to be wrapped. This is typically a method of a class.
-#         widget (QWidget): The widget that the slot is connected to. This widget is passed to the slot function as a keyword argument,
-#             and its signal value is also passed as a keyword argument.
-
-#     Returns:
-#         callable: The slot wrapper function. This function can be connected to a widget signal and is responsible for calling the original slot function
-#             with the appropriate arguments.
-#     """
-
-#     def slot_wrapper(*args, **kwargs):
-#         parameters = inspect.signature(slot).parameters
-#         has_kwargs = any(p.kind == p.VAR_KEYWORD for p in parameters.values())
-#         has_widget = "widget" in parameters
-#         try:
-#             if has_kwargs or has_widget:
-#                 kwargs["widget"] = widget
-#             slot(*args, **kwargs)
-#         except TypeError:  # slot didn't accept widget in kwargs
-#             if len(args) > 0:  # if there is a value, try to call the slot with it
-#                 slot(args[0])
-#             else:  # no value, so call the slot with no arguments
-#                 slot()
-
-#     return slot_wrapper
-
-
-# def sync_all_widgets(self, *uis, **kwargs):
-#     """Set sync connections for all widgets of the given UI objects.
-
-#     Parameters:
-#         *uis: A tuple of previously loaded dynamic UI objects to sync widgets among.
-#     """
-#     for i, ui1 in enumerate(uis):
-#         for ui2 in uis[i + 1 :]:
-#             for w1 in ui1.widgets:
-#                 try:
-#                     w2 = self.get_widget(w1.name, ui2)
-#                 except AttributeError:
-#                     continue
-
-#                 pair_id = hash((w1, w2))
-#                 if pair_id in self._synced_pairs:
-#                     continue
-
-#                 self.sync_widgets(w1, w2, **kwargs)
-
-# def sync_widgets(self, w1, w2, **kwargs):
-#     """Set the initial signal connections that will call the _sync_attributes function on state changes.
-
-#     Parameters:
-#         w1 (obj): The first widget to sync.
-#         w2 (obj): The second widget to sync.
-#         kwargs: The attribute(s) to sync as keyword arguments.
-#     """
-#     try:  # get the default signal for the given widget.
-#         signals1 = self.get_default_signals(w1)
-#         signals2 = self.get_default_signals(w2)
-
-#         # set sync connections for each of the widgets signals.
-#         for s1, s2 in zip(signals1, signals2):
-#             s1.connect(lambda: self._sync_attributes(w1, w2, **kwargs))
-#             s2.connect(lambda: self._sync_attributes(w2, w1, **kwargs))
-
-#         pair_id = hash((w1, w2))
-#         self._synced_pairs.add(pair_id)
-
-#     except (AttributeError, KeyError):
-#         return
-
-# attributesGetSet = {
-#     "value": "setValue",
-#     "text": "setText",
-#     "icon": "setIcon",
-#     "checkState": "setCheckState",
-#     "isChecked": "setChecked",
-#     "isDisabled": "setDisabled",
-# }
-
-# def _sync_attributes(self, frm, to, attributes=[]):
-#     """Sync the given attributes between the two given widgets.
-#     If a widget does not have an attribute it will be silently skipped.
-
-#     Parameters:
-#         frm (obj): The widget to transfer attribute values from.
-#         to (obj): The widget to transfer attribute values to.
-#         attributes (str/list)(dict): The attribute(s) to sync. ie. a setter attribute 'setChecked' or a dict containing getter:setter pairs. ie. {'isChecked':'setChecked'}
-#     """
-#     if not attributes:
-#         attributes = self.attributesGetSet
-
-#     elif not isinstance(attributes, dict):
-#         attributes = {
-#             next(
-#                 (k for k, v in self.attributesGetSet.items() if v == i), None
-#             ): i  # construct a gettr setter pair dict using only the given setter values.
-#             for i in ptk.make_iterable(attributes)
-#         }
-
-#     _attributes = {}
-#     for gettr, settr in attributes.items():
-#         try:
-#             _attributes[settr] = getattr(frm, gettr)()
-#         except AttributeError:
-#             pass
-
-#     for (
-#         attr,
-#         value,
-#     ) in _attributes.items():  # set the second widget's attributes from the first.
-#         try:
-#             getattr(to, attr)(value)
-#         except AttributeError:
-#             pass
-
-# def sync_widget_values(self, widget, value):
-#     # Get the relatives of the widget's UI
-#     relatives = self.get_ui_relatives(widget.ui)
-
-#     # For each relative UI...
-#     for relative in relatives:
-#         # Get the widget of the same name
-#         relative_widget = getattr(relative, widget.name, None)
-
-#         # If the relative widget exists...
-#         if relative_widget is not None:
-#             # Check the type of the widget and use the appropriate method to set the value
-#             if isinstance(relative_widget, QtWidgets.QLabel):
-#                 relative_widget.setText(value)
-#             elif isinstance(relative_widget, QtWidgets.QSpinBox):
-#                 relative_widget.setValue(value)
-#             # Add more elif statements for other widget types as needed
-
-# def connect_slot(self, widget, slot):
-#     """
-#     Connects a slot to its corresponding signals for a given widget.
-
-#     This function attempts to fetch signals from the slot decorator. If it fails to fetch them,
-#     it resorts to the default signals based on the widget's derived type. For each fetched signal,
-#     the function checks if the signal is a valid attribute of the widget. If it is, it connects
-#     the slot to this signal and appends the slot to the connected slots list.
-
-#     Parameters:
-#         widget (QWidget): A widget for which the slot is connected to the signals.
-#         slot (method): The slot method to connect to the signals.
-
-#     Raises:
-#         TypeError: If the signal name is not a string or if no valid signal was found for the widget.
-#     """
-#     signals = getattr(
-#         slot,
-#         "signals",
-#         ptk.make_iterable(self.default_signals.get(widget.derived_type)),
-#     )
-
-#     def slot_wrapper(*args, **kwargs):
-#         self.slot_history(add=slot)  # update slot history before calling the slot
-#         slot(*args, **kwargs)
-
-#     for signal_name in signals:
-#         if not isinstance(signal_name, str):
-#             raise TypeError(
-#                 f"Signal name must be a string, not '{type(signal_name)}'"
-#             )
-#         signal = getattr(widget, signal_name, None)
-#         if signal:
-#             signal.connect(slot_wrapper)
-#             if widget not in self._connected_slots:
-#                 self._connected_slots[widget] = {}
-#             self._connected_slots[widget][signal_name] = slot_wrapper
-#         else:
-#             self.logger.warning(
-#                 f"No valid signal '{signal_name}' found for {widget.ui.name}.{widget.name}"
-#             )
-
-# def connect_slots(self, ui, widgets=None):
-#     """Connects the signals to their respective slots for the widgets of the given ui.
-
-#     This function ensures that existing signal-slot connections are not repeated.
-#     If a connection already exists, it is not made again.
-
-#     Parameters:
-#         ui (QWidget): The dynamic UI object containing widgets.
-#         widgets (Iterable[QtWidgets.QWidget], optional): A specific set of widgets for which
-#             to connect slots. If not provided, all widgets from the ui are used.
-
-#     Raises:
-#         ValueError: If ui is not an instance of QWidget.
-
-#     Side effect:
-#         If successful, sets `ui.is_connected` to True indicating that
-#         the slots for the UI's widgets are connected.
-#     """
-#     if not isinstance(ui, QtWidgets.QWidget):
-#         raise ValueError(f"Invalid datatype: {type(ui)}")
-
-#     if widgets is None:
-#         if ui.is_connected:
-#             return
-#         widgets = ui.widgets
-
-#     for widget in ptk.make_iterable(widgets):
-#         slot = widget.get_slot()
-#         self.logger.info(f"Widget: {widget}, Slot: {slot}")
-#         if slot:
-#             # Get signals from slot decorator, or default signals if not present
-#             signals = getattr(
-#                 slot, "signals", [self.default_signals.get(widget.derived_type)]
-#             )
-#             for signal_name in signals:
-#                 signal = getattr(widget, signal_name, None)
-#                 self.logger.info(f"Signal Name: {signal_name}, Signal: {signal}")
-#                 if signal:
-#                     if slot not in self._connected_slots[signal]:
-#                         signal.connect(slot)
-#                         self._connected_slots[signal].append(slot)
-
-#                 elif signal_name in self.default_signals:
-#                     signal = getattr(
-#                         widget, self.default_signals[signal_name], None
-#                     )
-
-#                 try:  # append the slot to _slot_history each time the signal is triggered.
-#                     signal.connect(
-#                         lambda *args, s=slot: self._slot_history.append(s)
-#                     )
-#                 except AttributeError:  # signal is NoneType
-#                     pass
-#     ui.is_connected = True
-
-# def show_and_connect(self, ui, connect_on_show=True):
-#     """Register the uiName in history as current,
-#     set slot connections, and show the given ui.
-#     An override for the built-in show method.
-
-#     Parameters:
-#         ui (QWidget): A previously loaded dynamic ui object.
-#         connect_on_show (bool): The the ui as connected.
-#     """
-#     if not isinstance(ui, QtWidgets.QWidget):
-#         raise ValueError(f"Invalid datatype: {type(ui)}")
-
-#     if connect_on_show:
-#         ui.connected = True
-#     ui.__class__.show(ui)
-
-# def setConnections(self, ui):
-#     """Replace any signal connections of a previous ui with the set for the ui of the given name.
-
-#     Parameters:
-#         ui (QWidget): A previously loaded dynamic ui object.
-#     """
-#     if not isinstance(ui, QtWidgets.QWidget):
-#         raise ValueError(f"Invalid datatype: {type(ui)}")
-
-#     prev_ui = self.get_prev_ui(allow_duplicates=True)
-#     if prev_ui:
-#         if prev_ui == ui:
-#             return
-#         elif prev_ui.is_connected and not prev_ui.is_stacked_widget:
-#             self.disconnect_slots(prev_ui)
-
-#     if not ui.is_connected:
-#         self.connect_slots(ui)
-
-#     # sync all widgets within relative uis.
-#     relatives = self.get_ui_relatives(ui)
-#     self.sync_all_widgets(relatives)
-
-# def sync_all_widgets(self, frm, to, **kwargs):
-#     """Extends setSynConnections method to set sync connections
-#     for all widgets of the given pair of ui objects.
-
-#     Parameters:
-#             frm (obj): A previously loaded dynamic ui object to sync widgets from.
-#             to (obj): A previously loaded dynamic ui object to sync widgets to.
-#     """
-#     for w1 in frm.widgets:
-#         try:
-#             w2 = self.get_widget(w1.name, to)
-#         except AttributeError:
-#             continue
-
-#         pair_id = hash((w1, w2))
-#         if pair_id in self._synced_pairs:
-#             continue
-
-#         self.sync_widgets(w1, w2, **kwargs)
-
-# def sync_widgets(self, w1, w2, **kwargs):
-#     """Set the initial signal connections that will call the _sync_attributes function on state changes.
-
-#     Parameters:
-#             w1 (obj): The first widget to sync.
-#             w2 (obj): The second widget to sync.
-#             kwargs = The attribute(s) to sync as keyword arguments.
-#     """
-#     try:
-#         signals1 = self.get_default_signals(
-#             w1
-#         )  # get the default signal for the given widget.
-#         signals2 = self.get_default_signals(w2)
-
-#         for s1, s2 in zip(
-#             signals1, signals2
-#         ):  # set sync connections for each of the widgets signals.
-#             s1.connect(lambda: self._sync_attributes(w1, w2, **kwargs))
-#             s2.connect(lambda: self._sync_attributes(w2, w1, **kwargs))
-
-#         pair_id = hash((w1, w2))
-#         self._synced_pairs.add(pair_id)
-
-#     except (AttributeError, KeyError) as error:
-#         # if w1 and w2: print ('# {}: {}.sync_widgets({}, {}): {}. args: {}, {} #'.format('KeyError' if type(error)==KeyError else 'AttributeError', __name__, w1.objectName(), w2.objectName(), error, w1, w2)) #debug
-#         return
-
-# @staticmethod
-# def get_derived_type(
-#     widget, name=False, module="QtWidgets", inc=[], exc=[], filterByBaseType=False
-# ):
-#     """Get the base class of a custom widget.
-#     If the type is a standard widget, the derived type will be that widget's type.
-
-#     Parameters:
-#             widget (str/obj): QWidget or it's objectName.
-#             name (bool): Return the class or the class name.
-#             module (str): The name of the base class module to check for.
-#             inc (list): Widget types to include. All other will be omitted. Exclude takes dominance over include. Meaning, if the same attribute is in both lists, it will be excluded.
-#             exc (list): Widget types to exclude. ie. ['QWidget', 'QAction', 'QLabel', 'QPushButton', 'QListWidget']
-#             filterByBaseType (bool): When using `inc`, or `exc`; Filter by base class name, or derived class name. ie. 'QLayout'(base) or 'QGridLayout'(derived)
-
-#     Returns:
-#             (obj)(string)(None) class or class name if `name`. ie. 'QPushButton' from a custom widget with class name: 'PushButton'
-#     """
-#     # logging.info(widget.__class__.__mro__) #debug
-#     for c in widget.__class__.__mro__:
-#         if (
-#             c.__module__ == module or c.__module__.split(".")[-1] == module
-#         ):  # check for the first built-in class. ie. 'PySide2.QtWidgets' or 'QtWidgets'
-#             typ = c.__class__.__base__.__name__ if filterByBaseType else c
-#             if not (typ in exc and (typ in inc if inc else typ not in inc)):
-#                 return typ.__name__ if name else typ
-
-
-# @staticmethod
-# def _getUiLevelFromDir(filePath):
-#     """Get the UI level by looking for trailing intergers in it's dir name.
-#     If none are found a default level of 3 (main menu) is used.
-
-#     Parameters:
-#         filePath (str): The directory containing the ui file. ie. 'O:/Cloud/Code/_scripts/uitk/uitk/ui/uiLevel_0/init.ui'
-
-#     Example:
-#         menu types:
-#             level 1: stackedwidget: base menu
-#             level 2: stackedwidget: sub menu
-#             level 3: standard menu
-#     Returns:
-#         (int) If no level is found, a level of 3 (standard menu) will be returned.
-#     """
-#     ui_dir = ptk.format_path(filePath, "dir")
-#     default_level = 3
-#     try:
-#         return int(re.findall(r"\d+\s*$", ui_dir)[0])  # get trailing integers.
-#     except IndexError:  # int not found.
-#         return default_dir
-
-# @staticmethod
-# def unpack_names(name_string):
-#   '''Get a list of individual names from a single name string.
-#   If you are looking to get multiple objects from a name string, call 'get_widgets_from_str' directly instead.
-
-#   Parameters:
-#       name_string = string consisting of widget names separated by commas. ie. 'v000, b004-6'
-
-#   Returns:
-#       unpacked names. ie. ['v000','b004','b005','b006']
-
-#   Example: unpack_names('chk021-23, 25, tb001')
-#   '''
-#   packed_names = [n.strip() for n in name_string.split(',') #build list of all widgets passed in containing '-'
-#                       if '-' in n or n.strip().isdigit()]
-
-#   otherNames = [n.strip() for n in name_string.split(',') #all widgets passed in not containing '-'
-#                       if '-' not in n and not n.strip().isdigit()]
-
-#   unpacked_names=[] #unpack the packed names:
-#   for name in packed_names:
-#       if '-' in name:
-#           name = name.split('-') #ex. split 'b000-8'
-#           prefix = name[0].strip('0123456789') #ex. split 'b' from 'b000'
-#           start = int(name[0].strip('abcdefghijklmnopqrstuvwxyz') or 0) #start range. #ex. '000' #converting int('000') returns None, if case; assign 0.
-#           stop = int(name[1])+1 #end range. #ex. '8' from 'b000-8' becomes 9, for range up to 9 but not including 9.
-#           unpacked_names.extend([str(prefix)+'000'[:-len(str(num))]+str(num) for num in range(start,stop)]) #build list of name strings within given range
-#           last_name = name
-#           last_prefix = prefix
-#       else:
-#           num = name
-#           unpacked_names.extend([str(last_prefix)+'000'[:-len(str(num))]+str(num)])
-
-#   return otherNames+unpacked_names
-
-# def __getattr__(self, attr_name):
-#   found_widget = self.sb._get_widget_from_ui(self, attr_name)
-#   if found_widget:
-#       self.sb.init_widgets(self, found_widget)
-#       return found_widget
-#   raise AttributeError(f'{self.__class__.__name__} has no attribute `{attr_name}`')
-
-# def get_base_name(widget):
-#       '''Query a widgets prefix.
-#       A valid prefix is returned when the given widget's objectName startswith an alphanumeric char,
-#       followed by at least three integers. ex. i000 (alphanum,int,int,int)
-
-#       Parameters:
-#           widget (str/obj): A widget or it's object name.
-
-#       Returns:
-#           (str)
-#       '''
-#       prefix=''
-#       if not isinstance(widget, (str)):
-#           widget = widget.objectName()
-#       for char in widget:
-#           if not char.isdigit():
-#               prefix = prefix+char
-#           else:
-#               break
-
-#       i = len(prefix)
-#       integers = [c for c in widget[i:i+3] if c.isdigit()]
-#       if len(integers)>2 or len(widget)==i:
-#           return prefix
-
-# def set_attributes(self, obj=None, order=['setVisible'], **kwargs):
-#   '''Set attributes for a given object.
-
-#   Parameters:
-#       obj (obj): the child obj, or widgetAction to set attributes for. (default=self)
-#       order (list): List of string keywords. ie. ['move', 'setVisible']. attributes in this list will be set last, in order of the list. an example would be setting move positions after setting resize arguments.
-#       **kwargs = The keyword arguments to set.
-#   '''
-#   if not kwargs:
-#       return
-
-#   obj = obj if obj else self
-
-#   for k in order:
-#       v = kwargs.pop(k, None)
-#       if v:
-#           from collections import OrderedDict
-#           kwargs = OrderedDict(kwargs)
-#           kwargs[k] = v
-
-#   for attr, value in kwargs.items():
-#       try:
-#           getattr(obj, attr)(value)
-
-#       except AttributeError as error:
-#           pass; # logging.info(__name__+':','set_attributes:', obj, order, kwargs, error)
```

### Comparing `uitk-0.7.9/uitk/widgets/MainWindow.py` & `uitk-0.8.0/uitk/widgets/MainWindow.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/__init__.py` & `uitk-0.8.0/uitk/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/attributeWindow.py` & `uitk-0.8.0/uitk/widgets/attributeWindow.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/checkBox.py` & `uitk-0.8.0/uitk/widgets/checkBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/draggableHeader.py` & `uitk-0.8.0/uitk/widgets/draggableHeader.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/expandableList.py` & `uitk-0.8.0/uitk/widgets/expandableList.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,22 +199,22 @@
 
         Parameters:
             x (str, object, dict, list, tuple, set, map): The item or items to add.
             data: Data to associate with the added item or items. Default is None.
             **kwargs: Additional arguments to set on the added item or items.
 
         Returns:
-            widget: The added widget or list of added widgets.
+            widget/list: The added widget or list of added widgets.
         """
         if isinstance(x, dict):
             return [self.add(key, data=val, **kwargs) for key, val in x.items()]
-
         elif isinstance(x, (list, tuple, set)):
             return [self.add(item, **kwargs) for item in x]
-
+        elif isinstance(x, zip):
+            return [self.add(item, data, **kwargs) for item, data in x]
         elif isinstance(x, map):
             return [self.add(item, **kwargs) for item in list(x)]
 
         # get the widget from the value passed to x
         if isinstance(x, str):
             try:
                 widget = getattr(QtWidgets, x)(self)
@@ -225,15 +225,15 @@
         elif isinstance(x, QtWidgets.QWidget) or (
             inspect.isclass(x) and issubclass(x, QtWidgets.QWidget)
         ):
             widget = x(self) if callable(x) else x
 
         else:
             raise TypeError(
-                f"Unsupported item type: expected str, QWidget, a subclass of QWidget, or a collection (list, tuple, set, map, dict), but got '{type(x)}'"
+                f"Unsupported item type: expected str, QWidget, a subclass of QWidget, or a collection (list, tuple, set, map, zip, dict), but got '{type(x)}'"
             )
 
         widget.item_text = lambda i=widget: self.get_item_text(i)
         widget.item_data = lambda i=widget: self.get_item_data(i)
         widget.parent_item_text = lambda i=widget: self.get_parent_item_text(i)
         widget.parent_item_data = lambda i=widget: self.get_parent_item_data(i)
```

### Comparing `uitk-0.7.9/uitk/widgets/label.py` & `uitk-0.8.0/uitk/widgets/label.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/lineEdit.py` & `uitk-0.8.0/uitk/widgets/lineEdit.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/menu.py` & `uitk-0.8.0/uitk/widgets/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,22 +254,25 @@
             row (int): The row index at which to add the widget. Default is the last row.
             col (int): The column index at which to add the widget. Default is 0.
             rowSpan (int): The number of rows the widget should span. Default is 1.
             colSpan (int): The number of columns the widget should span. Default is the total number of columns.
             **kwargs: Additional arguments to set on the added item or items.
 
         Returns:
-            widget: The added widget or list of added widgets.
+            widget/list: The added widget or list of added widgets.
         """
         if isinstance(x, dict):
             return [self.add(key, data=val, **kwargs) for key, val in x.items()]
 
         elif isinstance(x, (list, tuple, set)):
             return [self.add(item, **kwargs) for item in x]
 
+        elif isinstance(x, zip):
+            return [self.add(item, data, **kwargs) for item, data in x]
+
         elif isinstance(x, map):
             return [self.add(item, **kwargs) for item in list(x)]
 
         # get the widget from the value passed to x
         if isinstance(x, str):
             try:
                 widget = getattr(QtWidgets, x)(self)
@@ -280,15 +283,15 @@
         elif isinstance(x, QtWidgets.QWidget) or (
             inspect.isclass(x) and issubclass(x, QtWidgets.QWidget)
         ):
             widget = x(self) if callable(x) else x
 
         else:
             raise TypeError(
-                f"Unsupported item type: expected str, QWidget, a subclass of QWidget, or a collection (list, tuple, set, map, dict), but got '{type(x)}'"
+                f"Unsupported item type: expected str, QWidget, a subclass of QWidget, or a collection (list, tuple, set, map, zip, dict), but got '{type(x)}'"
             )
 
         widget.item_text = lambda i=widget: self.get_item_text(i)
         widget.item_data = lambda i=widget: self.get_item_data(i)
 
         # If no position is specified, place the widget at the last row and first column
         if row is None:
```

### Comparing `uitk-0.7.9/uitk/widgets/messageBox.py` & `uitk-0.8.0/uitk/widgets/messageBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/mixins/__init__.py` & `uitk-0.8.0/uitk/widgets/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/mixins/attributes.py` & `uitk-0.8.0/uitk/widgets/mixins/attributes.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/mixins/convert.py` & `uitk-0.8.0/uitk/widgets/mixins/convert.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/mixins/docking.py` & `uitk-0.8.0/uitk/widgets/mixins/docking.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/mixins/style_sheet.py` & `uitk-0.8.0/uitk/widgets/mixins/style_sheet.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/mixins/tasks.py` & `uitk-0.8.0/uitk/widgets/mixins/tasks.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/mixins/text.py` & `uitk-0.8.0/uitk/widgets/mixins/text.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/optionBox.py` & `uitk-0.8.0/uitk/widgets/optionBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/progressBar.py` & `uitk-0.8.0/uitk/widgets/progressBar.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/pushButton.py` & `uitk-0.8.0/uitk/widgets/pushButton.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/region.py` & `uitk-0.8.0/uitk/widgets/region.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk/widgets/textEdit.py` & `uitk-0.8.0/uitk/widgets/textEdit.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk.egg-info/PKG-INFO` & `uitk-0.8.0/uitk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uitk
-Version: 0.7.9
+Version: 0.8.0
 Home-page: https://github.com/m3trik/uitk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `uitk-0.7.9/uitk.egg-info/PKG-INFO.bak` & `uitk-0.8.0/uitk.egg-info/PKG-INFO.bak`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk.egg-info/SOURCES.txt` & `uitk-0.8.0/uitk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uitk-0.7.9/uitk.egg-info/SOURCES.txt.bak` & `uitk-0.8.0/uitk.egg-info/SOURCES.txt.bak`

 * *Files identical despite different names*

