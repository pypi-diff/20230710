# Comparing `tmp/mkdocs_calendar_plugin-0.1.0.tar.gz` & `tmp/mkdocs_calendar_plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_calendar_plugin-0.1.0.tar", max compression
+gzip compressed data, was "mkdocs_calendar_plugin-0.2.0.tar", max compression
```

## Comparing `mkdocs_calendar_plugin-0.1.0.tar` & `mkdocs_calendar_plugin-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       25 2023-06-15 17:38:20.501285 mkdocs_calendar_plugin-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-14 09:13:11.740585 mkdocs_calendar_plugin-0.1.0/mkdocs_calendar/__init__.py
--rw-r--r--   0        0        0     2606 2023-06-15 17:59:03.194992 mkdocs_calendar_plugin-0.1.0/mkdocs_calendar/plugin.py
--rw-r--r--   0        0        0     1102 2023-06-15 19:14:35.102202 mkdocs_calendar_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 mkdocs_calendar_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-07-10 17:53:29.809741 mkdocs_calendar_plugin-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 17:53:29.809741 mkdocs_calendar_plugin-0.2.0/mkdocs_calendar/__init__.py
+-rw-r--r--   0        0        0     3230 2023-07-10 17:53:29.809741 mkdocs_calendar_plugin-0.2.0/mkdocs_calendar/plugin.py
+-rw-r--r--   0        0        0     1102 2023-07-10 17:53:29.813741 mkdocs_calendar_plugin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 mkdocs_calendar_plugin-0.2.0/PKG-INFO
```

### Comparing `mkdocs_calendar_plugin-0.1.0/mkdocs_calendar/plugin.py` & `mkdocs_calendar_plugin-0.2.0/mkdocs_calendar/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ################################################################################
 # @brief       : Calendar plugin for MkDocs
 # @author      : Jacques Supcik <jacques.supcik@hefr.ch>
-# @date        : 14. June 2023
+# @date        : 17. June 2023
 # ------------------------------------------------------------------------------
-# @copyright   : Copyright (c) 2022 HEIA-FR / ISC
+# @copyright   : Copyright (c) 2023 HEIA-FR / ISC
 #                Haute école d'ingénierie et d'architecture de Fribourg
 #                Informatique et Systèmes de Communication
 # @attention   : SPDX-License-Identifier: MIT OR Apache-2.0
 ################################################################################
 
 """Calendar plugin for MkDocs"""
 
@@ -25,51 +25,65 @@
 logger = logging.getLogger("mkdocs.plugins." + __name__)
 TAG = "[calendar] -"
 
 
 class CalendarPluginConfig(BaseConfig):
     """Configuration options for the calendar plugin."""
 
-    start = c.Type(date)
-    end = c.Type(date)
+    start = c.Optional(c.Type(date))
+    end = c.Optional(c.Type(date))
     tz = c.Choice(pytz.all_timezones, default="Europe/Zurich")
-    academic_weeks_off = c.Type(list, default=[])
+    weeks_off = c.Type(list, default=[])
+    extra_key = c.Type(str, default="cal")
 
 
 # pylint: disable-next=too-few-public-methods
 class CalendarPlugin(BasePlugin[CalendarPluginConfig]):
     """Calendar plugin for MkDocs"""
 
+    def get_xconfig(self, config, key):
+        """Get the configuration value for the given key."""
+        if "calendar_plugin" in config.extra:
+            extra = config.extra["calendar_plugin"]
+            if key in extra:
+                return extra[key]
+        if key in self.config:
+            return self.config[key]
+        return None
+
     def on_config(self, config):
         """Validate the configuration and add calendar entries to the config."""
         now = datetime.fromtimestamp(time.time(), tz=timezone(self.config["tz"]))
 
-        start_date = self.config["start"]
-        end_date = self.config["end"]
-
-        academic_week = ((now.date() - start_date).days) // 7 + 1
-        try:
-            for i in self.config["academic_weeks_off"]:
-                if academic_week >= i:
-                    academic_week -= 1
-
-        except Exception as e:  # pylint: disable=invalid-name
-            raise PluginError(f"{TAG} : {e}") from e
-
+        start_date = self.get_xconfig(config, "start")
+        end_date = self.get_xconfig(config, "end")
+        weeks_off = self.get_xconfig(config, "weeks_off") or []
         cal = {
-            "start": start_date,
-            "end": end_date,
             "now": now,
+            "today": now.date(),
             "weekday": now.weekday(),
             "week_number": now.isocalendar()[1],
             "iso_weekday": now.isoweekday(),
-            "today": now.date(),
-            "delta": (now.date() - start_date).days,
-            "delta_w": ((now.date() - start_date).days) / 7,
-            "academic_week": academic_week,
-            "aw": academic_week,
-            "remaining": (end_date - now.date()).days,
         }
 
-        config.extra["cal"] = cal
+        if start_date is not None:
+            academic_week = ((now.date() - start_date).days) // 7 + 1
+            try:
+                for i in weeks_off:
+                    if academic_week >= i:
+                        academic_week -= 1
+            except Exception as e:  # pylint: disable=invalid-name
+                raise PluginError(f"{TAG} : {e}") from e
+
+            cal["start"] = start_date
+            cal["delta"] = (now.date() - start_date).days
+            cal["delta_w"] = ((now.date() - start_date).days) / 7
+            cal["academic_week"] = academic_week
+            cal["aw"] = academic_week
+
+        if end_date is not None:
+            cal["end"] = end_date
+            cal["remaining"] = (end_date - now.date()).days
+
+        config.extra[self.config["extra_key"]] = cal
 
         return config
```

### Comparing `mkdocs_calendar_plugin-0.1.0/pyproject.toml` & `mkdocs_calendar_plugin-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-calendar-plugin"
-version = "0.1.0"
+version = "0.2.0"
 description = "An MkDocs plugin to ..."
 authors = ["Jacques Supcik <jacques.supcik@hefr.ch>"]
 repository = "https://github.com/supcik/mkdocs-today-plugin"
 license = "Apache-2"
 readme = "README.md"
 packages = [{ include = "mkdocs_calendar" }]
 keywords = ["mkdocs", "python", "markdown", "wiki"]
```

### Comparing `mkdocs_calendar_plugin-0.1.0/PKG-INFO` & `mkdocs_calendar_plugin-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-calendar-plugin
-Version: 0.1.0
+Version: 0.2.0
 Summary: An MkDocs plugin to ...
 Home-page: https://github.com/supcik/mkdocs-today-plugin
 License: Apache-2
 Keywords: mkdocs,python,markdown,wiki
 Author: Jacques Supcik
 Author-email: jacques.supcik@hefr.ch
 Requires-Python: >=3.10,<4.0
```

