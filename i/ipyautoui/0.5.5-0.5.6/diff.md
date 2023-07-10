# Comparing `tmp/ipyautoui-0.5.5.tar.gz` & `tmp/ipyautoui-0.5.6.tar.gz`

## Comparing `ipyautoui-0.5.5.tar` & `ipyautoui-0.5.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/_dev_sys_path_append.py
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/_utils.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/_utils_debounce.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/_version.py
--rw-r--r--   0        0        0    31739 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/autodisplay.py
--rw-r--r--   0        0        0    14178 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/autodisplay_renderers.py
--rw-r--r--   0        0        0    29497 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/autoipywidget.py
--rw-r--r--   0        0        0    21750 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/automapschema.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/automapschema.yaml
--rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/autoui.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/autovjsf.py
--rw-r--r--   0        0        0    14995 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/autowidgets.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/basemodel.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/constants.py
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/env.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/mydocstring_display.py
--rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/test_schema.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/vjsf.vue
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/__init__.py
--rw-r--r--   0        0        0    41006 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/autogrid.py
--rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/buttonbars.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/decision_branch.py
--rw-r--r--   0        0        0    25595 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/editgrid.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/filechooser.py
--rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/filesindir.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/fileupload.py
--rw-r--r--   0        0        0    30632 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/iterable.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/loadproject.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/markdown_widget.py
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/modelrun.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/multiselect_search.py
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/outputlogging.py
--rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/selectdir.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/selectfrom.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/showhide.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/showopenurl.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/title_description.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/urlimagelink.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/widgetcaller_error.py
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/custom/workingdir.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/__init__.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/complex_serialization.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/core_ipywidgets.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/editable_datagrid.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/nested.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/override_ipywidgets.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/root_array.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/root_array_enum.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/root_enum.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/root_simple.py
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/src/ipyautoui/demo_schemas/ruleset.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/.gitignore
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/LICENSE
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/README.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ipyautoui-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/_dev_sys_path_append.py
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/_utils.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/_utils_debounce.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/_version.py
+-rw-r--r--   0        0        0    31739 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/autodisplay.py
+-rw-r--r--   0        0        0    14178 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/autodisplay_renderers.py
+-rw-r--r--   0        0        0    29497 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/autoipywidget.py
+-rw-r--r--   0        0        0    21750 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/automapschema.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/automapschema.yaml
+-rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/autoui.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/autovjsf.py
+-rw-r--r--   0        0        0    14995 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/autowidgets.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/basemodel.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/constants.py
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/env.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/mydocstring_display.py
+-rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/test_schema.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/vjsf.vue
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/__init__.py
+-rw-r--r--   0        0        0    41006 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/autogrid.py
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/buttonbars.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/decision_branch.py
+-rw-r--r--   0        0        0    25595 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/editgrid.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/filechooser.py
+-rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/filesindir.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/fileupload.py
+-rw-r--r--   0        0        0    30632 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/iterable.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/loadproject.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/markdown_widget.py
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/modelrun.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/multiselect_search.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/outputlogging.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/selectandclick.py
+-rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/selectdir.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/showhide.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/showopenurl.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/title_description.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/urlimagelink.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/widgetcaller_error.py
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/custom/workingdir.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/__init__.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/complex_serialization.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/core_ipywidgets.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/editable_datagrid.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/nested.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/override_ipywidgets.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/root_array.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/root_array_enum.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/root_enum.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/root_simple.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/src/ipyautoui/demo_schemas/ruleset.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/.gitignore
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/LICENSE
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/README.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ipyautoui-0.5.6/PKG-INFO
```

### Comparing `ipyautoui-0.5.5/src/ipyautoui/__init__.py` & `ipyautoui-0.5.6/src/ipyautoui/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/_dev_sys_path_append.py` & `ipyautoui-0.5.6/src/ipyautoui/_dev_sys_path_append.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/_utils.py` & `ipyautoui-0.5.6/src/ipyautoui/_utils.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/_utils_debounce.py` & `ipyautoui-0.5.6/src/ipyautoui/_utils_debounce.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/autodisplay.py` & `ipyautoui-0.5.6/src/ipyautoui/autodisplay.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/autodisplay_renderers.py` & `ipyautoui-0.5.6/src/ipyautoui/autodisplay_renderers.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/autoipywidget.py` & `ipyautoui-0.5.6/src/ipyautoui/autoipywidget.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/automapschema.py` & `ipyautoui-0.5.6/src/ipyautoui/automapschema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/automapschema.yaml` & `ipyautoui-0.5.6/src/ipyautoui/automapschema.yaml`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/autoui.py` & `ipyautoui-0.5.6/src/ipyautoui/autoui.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/autovjsf.py` & `ipyautoui-0.5.6/src/ipyautoui/autovjsf.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/autowidgets.py` & `ipyautoui-0.5.6/src/ipyautoui/autowidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/basemodel.py` & `ipyautoui-0.5.6/src/ipyautoui/basemodel.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/constants.py` & `ipyautoui-0.5.6/src/ipyautoui/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,30 @@
     style={"button_color": "lightgreen"},
     # button_style="success",
     tooltip="true",
     layout={"width": BUTTON_WIDTH_MIN, "height": BUTTON_HEIGHT_MIN},
     disabled=True,
 )
 
+FILEUPLD_BUTTON_KWARGS = frozenmap( 
+    icon="upload",
+    description="",
+    button_style="info",
+    layout={"width": "60px"},
+    disabled=False,
+)
+
+IMAGE_BUTTON_KWARGS = frozenmap(
+    icon="image",
+    disabled=False,
+    button_style="info",
+    layout={"width": "44px"},
+    tooltip="images",
+)
+
 FALSE_BUTTON_KWARGS = frozenmap(
     icon="times",
     style={"button_color": "tomato"},
     # button_style="success",
     tooltip="false",
     layout={"width": BUTTON_WIDTH_MIN, "height": BUTTON_HEIGHT_MIN},
     disabled=True,
```

### Comparing `ipyautoui-0.5.5/src/ipyautoui/demo.py` & `ipyautoui-0.5.6/src/ipyautoui/demo.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/env.py` & `ipyautoui-0.5.6/src/ipyautoui/env.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/mydocstring_display.py` & `ipyautoui-0.5.6/src/ipyautoui/mydocstring_display.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/test_schema.py` & `ipyautoui-0.5.6/src/ipyautoui/test_schema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/vjsf.vue` & `ipyautoui-0.5.6/src/ipyautoui/vjsf.vue`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/autogrid.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/autogrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/buttonbars.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/buttonbars.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # jupyter:
 #   jupytext:
 #     formats: py:light
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
-#       jupytext_version: 1.14.0
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # +
@@ -163,15 +163,15 @@
     print("-----")
     actions.fns_onrevert_add_action(f)
     actions.fns_onrevert_add_action(f1)
     actions.fn_revert()
 
 
 # +
-class SaveButtonBar(w.HBox, SaveActions):
+class SaveButtonBar(SaveActions, w.HBox):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._init_form()
         self._init_controls()
 
     def _init_form(self):
         self.tgl_unsaved_changes = w.ToggleButton(
```

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/decision_branch.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/decision_branch.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/editgrid.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/editgrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/filechooser.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/filechooser.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/filesindir.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/filesindir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/fileupload.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/fileupload.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/iterable.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/iterable.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/loadproject.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/loadproject.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/markdown_widget.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/markdown_widget.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/modelrun.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/modelrun.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/multiselect_search.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/multiselect_search.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/outputlogging.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/outputlogging.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/selectdir.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/selectdir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/showhide.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/showhide.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/showopenurl.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/showopenurl.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/title_description.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/title_description.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/urlimagelink.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/urlimagelink.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/widgetcaller_error.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/widgetcaller_error.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/custom/workingdir.py` & `ipyautoui-0.5.6/src/ipyautoui/custom/workingdir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/__init__.py` & `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/complex_serialization.py` & `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/complex_serialization.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/core_ipywidgets.py` & `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/editable_datagrid.py` & `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/nested.py` & `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/nested.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/nested_editable_datagrid.py` & `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/nested_editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py` & `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/root_array_enum.py` & `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/root_array_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/root_enum.py` & `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/root_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/src/ipyautoui/demo_schemas/ruleset.py` & `ipyautoui-0.5.6/src/ipyautoui/demo_schemas/ruleset.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/.gitignore` & `ipyautoui-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/LICENSE` & `ipyautoui-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/README.md` & `ipyautoui-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/pyproject.toml` & `ipyautoui-0.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.5/PKG-INFO` & `ipyautoui-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyautoui
-Version: 0.5.5
+Version: 0.5.6
 Summary: wrapper that sits on top of ipywidgets and other ipy widget libraries to template / automate the creation of widget forms. Uses pydantic to create defined data-container and serialisation to JSON. Includes example patterns for adding new custom widgets.
 Project-URL: Homepage, https://github.com/maxfordham/ipyautoui
 Author-email: John Gunstone <gunstone.john@gmail.com>
 License-File: LICENSE
 Keywords: ipyautoui
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

