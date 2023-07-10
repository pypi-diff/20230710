# Comparing `tmp/ex4nicegui-0.1.3.tar.gz` & `tmp/ex4nicegui-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex4nicegui-0.1.3.tar", last modified: Sun Jul  9 18:21:01 2023, max compression
+gzip compressed data, was "ex4nicegui-0.1.4.tar", last modified: Mon Jul 10 14:32:06 2023, max compression
```

## Comparing `ex4nicegui-0.1.3.tar` & `ex4nicegui-0.1.4.tar`

### file list

```diff
@@ -1,47 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 18:21:01.030755 ex4nicegui-0.1.3/
--rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      481 2023-07-09 18:21:01.029730 ex4nicegui-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-07-05 06:11:55.000000 ex4nicegui-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 18:21:00.944546 ex4nicegui-0.1.3/ex4nicegui/
--rw-rw-rw-   0        0        0      366 2023-07-09 18:20:51.000000 ex4nicegui-0.1.3/ex4nicegui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:21:00.961485 ex4nicegui-0.1.3/ex4nicegui/layout/
--rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/layout/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/layout/gridbox.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:21:00.991978 ex4nicegui-0.1.3/ex4nicegui/reactive/
--rw-rw-rw-   0        0        0     1023 2023-07-09 14:56:08.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/__index.py
--rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:21:00.997961 ex4nicegui-0.1.3/ex4nicegui/reactive/draggable/
--rw-rw-rw-   0        0        0     4851 2023-07-05 09:28:02.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/draggable/UseDraggable.js
--rw-rw-rw-   0        0        0     3041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/draggable/UseDraggable.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/draggable/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/drawer.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:21:01.010777 ex4nicegui-0.1.3/ex4nicegui/reactive/echarts/
--rw-rw-rw-   0        0        0  1581614 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/echarts/ECharts.js
--rw-rw-rw-   0        0        0     2685 2023-07-09 14:56:08.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/echarts/ECharts.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/echarts/__init__.py
--rw-rw-rw-   0        0        0     6101 2023-07-09 14:56:08.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/local_file_picker.py
--rw-rw-rw-   0        0        0     1041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/official.py
--rw-rw-rw-   0        0        0    30066 2023-07-09 18:20:32.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/ref.py
--rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/rxui.py
--rw-rw-rw-   0        0        0      803 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/signature.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:21:01.015766 ex4nicegui-0.1.3/ex4nicegui/reactive/useMouse/
--rw-rw-rw-   0        0        0     2722 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/useMouse/UseMouse.js
--rw-rw-rw-   0        0        0     2244 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/useMouse/UseMouse.py
--rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/useMouse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:21:01.019755 ex4nicegui-0.1.3/ex4nicegui/tools/
--rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/tools/__init__.py
--rw-rw-rw-   0        0        0     5024 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/tools/debug.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:21:01.027737 ex4nicegui-0.1.3/ex4nicegui/utils/
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/utils/__init__.py
--rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/utils/common.py
--rw-rw-rw-   0        0        0     4430 2023-07-09 14:56:08.000000 ex4nicegui-0.1.3/ex4nicegui/utils/signals.py
--rw-rw-rw-   0        0        0      910 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:21:00.957503 ex4nicegui-0.1.3/ex4nicegui.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-09 18:21:00.000000 ex4nicegui-0.1.3/ex4nicegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1104 2023-07-09 18:21:00.000000 ex4nicegui-0.1.3/ex4nicegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 18:21:00.000000 ex4nicegui-0.1.3/ex4nicegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-09 18:21:00.000000 ex4nicegui-0.1.3/ex4nicegui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       32 2023-07-09 18:21:00.000000 ex4nicegui-0.1.3/ex4nicegui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-09 18:21:00.000000 ex4nicegui-0.1.3/ex4nicegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 18:21:01.031752 ex4nicegui-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2073 2023-07-09 14:56:08.000000 ex4nicegui-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.405094 ex4nicegui-0.1.4/
+-rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      481 2023-07-10 14:32:06.400107 ex4nicegui-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-07-05 06:11:55.000000 ex4nicegui-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.316329 ex4nicegui-0.1.4/ex4nicegui/
+-rw-rw-rw-   0        0        0      337 2023-07-10 14:31:57.000000 ex4nicegui-0.1.4/ex4nicegui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.331291 ex4nicegui-0.1.4/ex4nicegui/layout/
+-rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/layout/__init__.py
+-rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/layout/gridbox.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.345252 ex4nicegui-0.1.4/ex4nicegui/reactive/
+-rw-rw-rw-   0        0        0      998 2023-07-10 14:31:39.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/__index.py
+-rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.363204 ex4nicegui-0.1.4/ex4nicegui/reactive/draggable/
+-rw-rw-rw-   0        0        0     4851 2023-07-05 09:28:02.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/draggable/UseDraggable.js
+-rw-rw-rw-   0        0        0     3041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/draggable/UseDraggable.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/draggable/__init__.py
+-rw-rw-rw-   0        0        0     1365 2023-07-10 14:31:39.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/drawer.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.380160 ex4nicegui-0.1.4/ex4nicegui/reactive/echarts/
+-rw-rw-rw-   0        0        0  1581614 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/echarts/ECharts.js
+-rw-rw-rw-   0        0        0     2685 2023-07-09 14:56:08.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/echarts/ECharts.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/echarts/__init__.py
+-rw-rw-rw-   0        0        0     6106 2023-07-10 14:31:39.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/local_file_picker.py
+-rw-rw-rw-   0        0        0    30930 2023-07-10 14:31:39.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/officials.py
+-rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/rxui.py
+-rw-rw-rw-   0        0        0      803 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/signature.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.386143 ex4nicegui-0.1.4/ex4nicegui/reactive/useMouse/
+-rw-rw-rw-   0        0        0     2722 2023-07-08 17:55:18.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/useMouse/UseMouse.js
+-rw-rw-rw-   0        0        0     2244 2023-07-08 17:55:18.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/useMouse/UseMouse.py
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/useMouse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.390133 ex4nicegui-0.1.4/ex4nicegui/tools/
+-rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.4/ex4nicegui/tools/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.1.4/ex4nicegui/tools/debug.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.397118 ex4nicegui-0.1.4/ex4nicegui/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/utils/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.4/ex4nicegui/utils/common.py
+-rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.1.4/ex4nicegui/utils/signals.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.327303 ex4nicegui-0.1.4/ex4nicegui.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-10 14:32:05.000000 ex4nicegui-0.1.4/ex4nicegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1052 2023-07-10 14:32:06.000000 ex4nicegui-0.1.4/ex4nicegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 14:32:05.000000 ex4nicegui-0.1.4/ex4nicegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-10 14:32:05.000000 ex4nicegui-0.1.4/ex4nicegui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       32 2023-07-10 14:32:05.000000 ex4nicegui-0.1.4/ex4nicegui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-10 14:32:05.000000 ex4nicegui-0.1.4/ex4nicegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 14:32:06.405094 ex4nicegui-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     2073 2023-07-09 14:56:08.000000 ex4nicegui-0.1.4/setup.py
```

### Comparing `ex4nicegui-0.1.3/LICENSE` & `ex4nicegui-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.3/ex4nicegui/layout/gridbox.py` & `ex4nicegui-0.1.4/ex4nicegui/layout/gridbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.3/ex4nicegui/reactive/__index.py` & `ex4nicegui-0.1.4/ex4nicegui/reactive/__index.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-from .official import (
-    # color_picker,
-    aggrid,
-)
-
-from .ref import (
+from .officials import (
     TableBindableUi as table,
+    AggridBindableUi as aggrid,
     RadioBindableUi as radio,
     SelectBindableUi as select,
     SwitchBindableUi as switch,
     InputBindableUi as input,
     LazyInputBindableUi as lazy_input,
     TextareaBindableUi as textarea,
     LazyTextareaBindableUi as lazy_textarea,
```

### Comparing `ex4nicegui-0.1.3/ex4nicegui/reactive/draggable/UseDraggable.js` & `ex4nicegui-0.1.4/ex4nicegui/reactive/draggable/UseDraggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.3/ex4nicegui/reactive/draggable/UseDraggable.py` & `ex4nicegui-0.1.4/ex4nicegui/reactive/draggable/UseDraggable.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.3/ex4nicegui/reactive/drawer.py` & `ex4nicegui-0.1.4/ex4nicegui/reactive/drawer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from typing_extensions import Literal
 from nicegui import ui
-from ex4nicegui.reactive.ref import DrawerBindableUi
+from ex4nicegui.reactive.officials import DrawerBindableUi
 from signe import effect
+from typing import Union, Optional
 
 _TDrawerSide = Literal["left", "right"]
 
 
 def drawer(
     side: _TDrawerSide = "left",
     overlay=False,
     *,
-    value: bool | None = None,
+    value: Optional[bool] = None,
     fixed: bool = False,
     bordered: bool = True,
     elevated: bool = False,
     top_corner: bool = False,
     bottom_corner: bool = False,
 ):
     kws = {
```

### Comparing `ex4nicegui-0.1.3/ex4nicegui/reactive/echarts/ECharts.js` & `ex4nicegui-0.1.4/ex4nicegui/reactive/echarts/ECharts.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.3/ex4nicegui/reactive/echarts/ECharts.py` & `ex4nicegui-0.1.4/ex4nicegui/reactive/echarts/ECharts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.3/ex4nicegui/reactive/local_file_picker.py` & `ex4nicegui-0.1.4/ex4nicegui/reactive/local_file_picker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Optional, cast
+from typing import Any, Callable, Optional, cast,List
 from typing_extensions import Literal
 from signe import createSignal, effect, computed
 from nicegui import ui, Tailwind
 from pathlib import Path
 
 from signe.types import TGetter
 from ex4nicegui.utils.signals import Ref, effect_refreshable, ReadonlyRef
@@ -27,23 +27,23 @@
         return self
 
 
 def local_file_picker(
     title: Optional[str] = None,
     dir: Optional[str] = None,
     mode: SelectMode = "file",
-    ext: Optional[list[str]] = None,
+    ext: Optional[List[str]] = None,
 ):
     """本地文件目录选择框
 
     Args:
         title (Optional[str], optional): 标题. Defaults to None.
         dir (Optional[str], optional): 起始目录,默认为当前目录. Defaults to None.
         mode (SelectMode, optional): 选择文件或选择目录，'file' | 'dir'. Defaults to "file".
-        ext (Optional[list[str]], optional): 当 `mode` 为 'file' 时,保留指定的文件后缀.例如: ```ext=['.xlsx','.csv']```. Defaults to None.
+        ext (Optional[List[str]], optional): 当 `mode` 为 'file' 时,保留指定的文件后缀.例如: ```ext=['.xlsx','.csv']```. Defaults to None.
 
     Returns:
         _type_: open,result
             open:打开选择框函数
             result: 获取结果的信号函数。
 
     例子:
```

### Comparing `ex4nicegui-0.1.3/ex4nicegui/reactive/ref.py` & `ex4nicegui-0.1.4/ex4nicegui/reactive/officials.py`

 * *Files 2% similar despite different names*

```diff
@@ -600,14 +600,15 @@
             ele._style["color"] = color
             ele.update()
 
     def bind_text(self, ref_ui: ReadonlyRef):
         @effect
         def _():
             self.element.on_text_change(str(ref_ui.value))
+            # self.element.update()
 
         return self
 
 
 class IconBindableUi(SingleValueBindableUi[str, ui.icon]):
     def __init__(
         self,
@@ -797,51 +798,75 @@
 
         ele.on("change", handler=onModelValueChanged)
 
 
 _TAggridValue = Dict
 
 
-class AggridBindableUi(SingleValueBindableUi[_TAggridValue, ui.aggrid]):
-    def __init__(self, value: _TAggridValue, element: ui.aggrid) -> None:
-        super().__init__(value, element)
+class AggridBindableUi(BindableUi[ui.aggrid]):
+    def __init__(
+        self,
+        options: TMaybeRef[Dict],
+        *,
+        html_columns: TMaybeRef[List[int]] = [],
+        theme: TMaybeRef[str] = "balham",
+    ) -> None:
+        kws = {
+            "options": options,
+            "html_columns": html_columns,
+            "theme": theme,
+        }
+
+        value_kws = _convert_kws_ref2value(kws)
+
+        element = ui.aggrid(**value_kws)
+
+        super().__init__(element)
+
+        for key, value in kws.items():
+            if is_ref(value):
+                self.bind_prop(key, value)  # type: ignore
+
+    @staticmethod
+    def from_pandas(df: TMaybeRef):
+        if is_ref(df):
+
+            @ref_computed
+            def cp_convert_df():
+                return utils_common.convert_dataframe(df.value)
+
+            @ref_computed
+            def cp_options():
+                columnDefs = [
+                    {"headerName": col, "field": col}
+                    for col in cp_convert_df.value.columns
+                ]
+                rowData = cp_convert_df.value.to_dict("records")
+                data = {"columnDefs": columnDefs, "rowData": rowData}
+                return data
+
+            return AggridBindableUi(cp_options)
+
+        columnDefs = [{"headerName": col, "field": col} for col in df.columns]  # type: ignore
+        rowData = df.to_dict("records")  # type: ignore
+        options = {"columnDefs": columnDefs, "rowData": rowData}
+        return AggridBindableUi(options)
 
     def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
         if prop == "options":
             return self.bind_options(ref_ui)
 
         return super().bind_prop(prop, ref_ui)
 
-    @overload
-    def bind_options(self, ref_ui: ReadonlyRef[Dict]) -> Self:
-        ...
-
-    @overload
-    def bind_options(self, ref_ui: ReadonlyRef) -> Self:
-        ...
-
-    def bind_options(self, ref_ui: ReadonlyRef):
-        import pandas as pd
-
+    def bind_options(self, ref_ui: ReadonlyRef[List[Dict]]):
         @effect
         def _():
             ele = self.element
-
             data = ref_ui.value
-            if isinstance(data, pd.DataFrame):
-                columnDefs = [{"headerName": col, "field": col} for col in data.columns]
-
-                data = utils_common.convert_dataframe(data)
-
-                rowData = data.to_dict("records")
-
-                data = {"columnDefs": columnDefs, "rowData": rowData}
-
             ele._props["options"].update(data)
-
             ele.update()
 
         return self
 
 
 class TableBindableUi(BindableUi[ui.table]):
     def __init__(
```

### Comparing `ex4nicegui-0.1.3/ex4nicegui/reactive/signature.py` & `ex4nicegui-0.1.4/ex4nicegui/reactive/signature.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.3/ex4nicegui/reactive/useMouse/UseMouse.js` & `ex4nicegui-0.1.4/ex4nicegui/reactive/useMouse/UseMouse.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.3/ex4nicegui/reactive/useMouse/UseMouse.py` & `ex4nicegui-0.1.4/ex4nicegui/reactive/useMouse/UseMouse.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.3/ex4nicegui/tools/debug.py` & `ex4nicegui-0.1.4/ex4nicegui/tools/debug.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,10 @@
 from signe.core.effect import Effect
-from signe.core.signal import Signal
-from ex4nicegui import ref_computed, to_ref, effect
 import ex4nicegui.reactive as rxui
-from ex4nicegui.utils.signals import (
-    ReadonlyRef,
-    DescReadonlyRef,
-    Ref,
-    ref_computed_with_opts,
-)
+from ex4nicegui.utils.signals import ReadonlyRef, DescReadonlyRef, Ref, ref_computed
 from nicegui import ui
 from typing import Callable, Dict, TypeVar, Generic
 
 T = TypeVar("T")
 
 
 def display_ref_vars_ui(vars_dict: Dict):
@@ -42,15 +35,15 @@
 
     all_computed_var_map = {
         getattr(value, "_ReadonlyRef___getter"): var
         for var, value in need_vars_dict.items()
         if isinstance(value, DescReadonlyRef)
     }
 
-    @ref_computed_with_opts(priority_level=9999)
+    @ref_computed(priority_level=9999)
     def cp_rows():
         rows = []
 
         for var, value in need_vars_dict.items():
             if isinstance(value, Effect):
                 row = _handler_Effect_rows(
                     var, value, all_ref_var_map, all_computed_var_map
```

### Comparing `ex4nicegui-0.1.3/ex4nicegui/utils/signals.py` & `ex4nicegui-0.1.4/ex4nicegui/utils/signals.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,36 +111,57 @@
     # getter, setter = createSignal(value, comp)
 
     s = Signal(signe_utils.exec, value, SignalOption(comp))
 
     return cast(Ref[T], Ref(s.getValue, s.setValue, s))
 
 
+@overload
 def ref_computed(
     fn: Callable[[], T],
-    desc="",
     *,
+    desc="",
     debug_trigger: Optional[Callable[..., None]] = None,
     priority_level: int = 1,
 ) -> ReadonlyRef[T]:
-    getter = computed(fn, debug_trigger, priority_level)
-    return cast(DescReadonlyRef[T], DescReadonlyRef(getter, desc))
+    ...
+
+
+@overload
+def ref_computed(
+    fn=None,
+    *,
+    desc="",
+    debug_trigger: Optional[Callable[..., None]] = None,
+    priority_level: int = 1,
+) -> Callable[[Callable[..., T]], ReadonlyRef[T]]:
+    ...
 
 
-def ref_computed_with_opts(
+def ref_computed(
+    fn: Optional[Callable[[], T]] = None,
+    *,
     desc="",
     debug_trigger: Optional[Callable[..., None]] = None,
     priority_level: int = 1,
-):
-    def wrap(fn: Callable[[], T]) -> ReadonlyRef[T]:
-        return ref_computed(
-            fn, desc, debug_trigger=debug_trigger, priority_level=priority_level
-        )
+) -> Union[ReadonlyRef[T], Callable[[Callable[..., T]], ReadonlyRef[T]]]:
+    kws = {
+        "debug_trigger": debug_trigger,
+        "priority_level": priority_level,
+    }
+
+    if fn:
+        getter = computed(fn, **kws)
+        return cast(DescReadonlyRef[T], DescReadonlyRef(getter, desc))
+    else:
+
+        def wrap(fn: Callable[[], T]):
+            return ref_computed(fn, **kws)
 
-    return wrap
+        return wrap
 
 
 class effect_refreshable:
     def __init__(
         self, fn: Callable, refs: Union[ReadonlyRef, Sequence[ReadonlyRef]] = []
     ) -> None:
         self._fn = fn
```

### Comparing `ex4nicegui-0.1.3/ex4nicegui.egg-info/SOURCES.txt` & `ex4nicegui-0.1.4/ex4nicegui.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 ex4nicegui.egg-info/top_level.txt
 ex4nicegui/layout/__init__.py
 ex4nicegui/layout/gridbox.py
 ex4nicegui/reactive/__index.py
 ex4nicegui/reactive/__init__.py
 ex4nicegui/reactive/drawer.py
 ex4nicegui/reactive/local_file_picker.py
-ex4nicegui/reactive/official.py
-ex4nicegui/reactive/ref.py
+ex4nicegui/reactive/officials.py
 ex4nicegui/reactive/rxui.py
 ex4nicegui/reactive/signature.py
 ex4nicegui/reactive/draggable/UseDraggable.js
 ex4nicegui/reactive/draggable/UseDraggable.py
 ex4nicegui/reactive/draggable/__init__.py
 ex4nicegui/reactive/echarts/ECharts.js
 ex4nicegui/reactive/echarts/ECharts.py
@@ -27,9 +26,8 @@
 ex4nicegui/reactive/useMouse/UseMouse.js
 ex4nicegui/reactive/useMouse/UseMouse.py
 ex4nicegui/reactive/useMouse/__init__.py
 ex4nicegui/tools/__init__.py
 ex4nicegui/tools/debug.py
 ex4nicegui/utils/__init__.py
 ex4nicegui/utils/common.py
-ex4nicegui/utils/signals.py
-ex4nicegui/utils/types.py
+ex4nicegui/utils/signals.py
```

### Comparing `ex4nicegui-0.1.3/setup.py` & `ex4nicegui-0.1.4/setup.py`

 * *Files identical despite different names*

