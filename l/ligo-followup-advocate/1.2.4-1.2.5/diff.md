# Comparing `tmp/ligo-followup-advocate-1.2.4.tar.gz` & `tmp/ligo-followup-advocate-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo-followup-advocate-1.2.4.tar", last modified: Tue Jun 20 23:10:47 2023, max compression
+gzip compressed data, was "ligo-followup-advocate-1.2.5.tar", last modified: Mon Jul 10 20:30:31 2023, max compression
```

## Comparing `ligo-followup-advocate-1.2.4.tar` & `ligo-followup-advocate-1.2.5.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.441718 ligo-followup-advocate-1.2.4/
--rw-rw-rw-   0 root         (0) root         (0)    17895 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/COPYING.md
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      880 2023-06-20 23:10:47.441718 ligo-followup-advocate-1.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2855 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.406717 ligo-followup-advocate-1.2.4/ligo/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.442718 ligo-followup-advocate-1.2.4/ligo/followup_advocate/
--rw-rw-rw-   0 root         (0) root         (0)    25817 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-20 23:10:47.442718 ligo-followup-advocate-1.2.4/ligo/followup_advocate/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/jinja.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.410717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2960 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/RAVEN_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/RAVEN_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 23:10:35.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/authors.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/compare_skymaps.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1036 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/em_bright.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     2614 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/initial_body.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/initial_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1439 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/llama_alert_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/llama_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     2447 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/llama_track_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     9889 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1682 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1496 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/medium_latency_grb_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/numbered_pipeline_citations.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/p_astro.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/retraction.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1122 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/skymap_info.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1350 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/update_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/userguide_conclusion.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.411717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 23:10:35.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.405717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.411717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/
--rw-rw-rw-   0 root         (0) root         (0)     1880 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.412717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      987 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.412717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1133/
--rw-rw-rw-   0 root         (0) root         (0)     1877 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1133/event.json
--rw-rw-rw-   0 root         (0) root         (0)        4 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1133/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.412717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.412717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)      515 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.413717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/
--rw-rw-rw-   0 root         (0) root         (0)     1881 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.413717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.414717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/
--rw-rw-rw-   0 root         (0) root         (0)     1876 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.414717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)      610 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.414717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.415717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.415717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E5678/
--rw-rw-rw-   0 root         (0) root         (0)     1918 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E5678/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.415717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E5678/files/
--rw-rw-rw-   0 root         (0) root         (0)     5761 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E5678/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E5678/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.416717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1122/
--rw-rw-rw-   0 root         (0) root         (0)     1936 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1122/event.json
--rw-rw-rw-   0 root         (0) root         (0)      633 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1122/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.416717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1234/
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1234/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1234/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.416717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1235/
--rw-rw-rw-   0 root         (0) root         (0)     3982 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1235/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1235/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.417717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2468/
--rw-rw-rw-   0 root         (0) root         (0)     3956 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2468/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.417717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2468/files/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2468/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2468/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.417717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2469/
--rw-rw-rw-   0 root         (0) root         (0)     3979 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2469/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.417717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2469/files/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2469/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2469/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.417717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5566/
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5566/event.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5566/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.418717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5678/
--rw-rw-rw-   0 root         (0) root         (0)     3955 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5678/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5678/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.418717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5679/
--rw-rw-rw-   0 root         (0) root         (0)     3979 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5679/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5679/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.419717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.424717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/
--rw-rw-rw-   0 root         (0) root         (0)     4609 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml
--rw-rw-rw-   0 root         (0) root         (0)     4607 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/em_bright.json
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)     1832 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files.json
--rw-rw-rw-   0 root         (0) root         (0)     7997 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     5897 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/voevents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.424717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.426717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files/
--rw-rw-rw-   0 root         (0) root         (0)     4476 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)  1065600 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)     4047 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files.json
--rw-rw-rw-   0 root         (0) root         (0)     4911 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     3397 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)      966 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/voevents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.426717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.440718 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/
--rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)     6731 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)     6716 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/coincidence_far.json
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/em_bright.json
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/em_bright.json,0
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/p_astro.json,0
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files.json
--rw-rw-rw-   0 root         (0) root         (0)     7678 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     5616 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)     1585 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/voevents.json
--rw-rw-rw-   0 root         (0) root         (0)     5199 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     2957 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.441718 ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/
--rw-r--r--   0 root         (0) root         (0)      880 2023-06-20 23:10:47.000000 ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7102 2023-06-20 23:10:47.000000 ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 23:10:47.000000 ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-20 23:10:47.000000 ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-06-20 23:10:47.000000 ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-20 23:10:47.000000 ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1793 2023-06-20 23:10:47.442718 ligo-followup-advocate-1.2.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      539 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    68611 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.251220 ligo-followup-advocate-1.2.5/
+-rw-rw-rw-   0 root         (0) root         (0)    17895 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/COPYING.md
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      880 2023-07-10 20:30:31.251220 ligo-followup-advocate-1.2.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.223219 ligo-followup-advocate-1.2.5/ligo/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.251220 ligo-followup-advocate-1.2.5/ligo/followup_advocate/
+-rw-rw-rw-   0 root         (0) root         (0)    26014 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-07-10 20:30:31.251220 ligo-followup-advocate-1.2.5/ligo/followup_advocate/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/jinja.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.227219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/RAVEN_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      944 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/RAVEN_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      741 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/authors.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/compare_skymaps.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/em_bright.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     2614 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/initial_body.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/initial_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/llama_alert_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/llama_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/llama_track_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     9889 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/medium_latency_grb_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/numbered_pipeline_citations.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/p_astro.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/retraction.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1122 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/skymap_info.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1350 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/update_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/userguide_conclusion.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.227219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.223219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.227219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1122/
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1122/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.227219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1122/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1122/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1122/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      987 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1122/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.227219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1133/
+-rw-rw-rw-   0 root         (0) root         (0)     1877 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1133/event.json
+-rw-rw-rw-   0 root         (0) root         (0)        4 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1133/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.227219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1134/
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1134/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.227219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1134/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1134/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1134/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1134/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.227219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1234/
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1234/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.227219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1234/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1234/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1234/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1234/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.227219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1235/
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1235/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.227219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1235/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1235/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1235/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1235/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)      610 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1235/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.227219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E2244/
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E2244/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.231219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E2244/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E2244/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E2244/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E2244/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.231219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E5678/
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E5678/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.231219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E5678/files/
+-rw-rw-rw-   0 root         (0) root         (0)     5761 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E5678/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E5678/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.231219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M1122/
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M1122/event.json
+-rw-rw-rw-   0 root         (0) root         (0)      633 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M1122/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.231219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M1234/
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M1234/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M1234/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.231219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M1235/
+-rw-rw-rw-   0 root         (0) root         (0)     3982 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M1235/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M1235/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.231219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M2468/
+-rw-rw-rw-   0 root         (0) root         (0)     3956 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M2468/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.231219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M2468/files/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M2468/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M2468/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.231219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M2469/
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M2469/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.231219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M2469/files/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M2469/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M2469/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.231219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M5566/
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M5566/event.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M5566/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.231219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M5678/
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M5678/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M5678/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.231219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M5679/
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M5679/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M5679/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.231219 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.239220 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/
+-rw-rw-rw-   0 root         (0) root         (0)     6797 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6795 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/em_bright.json
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)     1832 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     7997 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5897 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/voevents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.239220 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.239220 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/files/
+-rw-rw-rw-   0 root         (0) root         (0)     4476 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)  1065600 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     4911 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     3397 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)      966 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/voevents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.239220 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.251220 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/
+-rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)     8946 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)     8931 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/coincidence_far.json
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/em_bright.json
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/em_bright.json,0
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/p_astro.json,0
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     7678 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5616 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/voevents.json
+-rw-rw-rw-   0 root         (0) root         (0)     5199 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2957 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/ligo/followup_advocate/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:30:31.251220 ligo-followup-advocate-1.2.5/ligo_followup_advocate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      880 2023-07-10 20:30:31.000000 ligo-followup-advocate-1.2.5/ligo_followup_advocate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7102 2023-07-10 20:30:31.000000 ligo-followup-advocate-1.2.5/ligo_followup_advocate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 20:30:31.000000 ligo-followup-advocate-1.2.5/ligo_followup_advocate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-10 20:30:31.000000 ligo-followup-advocate-1.2.5/ligo_followup_advocate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-10 20:30:31.000000 ligo-followup-advocate-1.2.5/ligo_followup_advocate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-10 20:30:31.000000 ligo-followup-advocate-1.2.5/ligo_followup_advocate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2023-07-10 20:30:31.251220 ligo-followup-advocate-1.2.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      539 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-07-10 20:30:18.000000 ligo-followup-advocate-1.2.5/versioneer.py
```

### Comparing `ligo-followup-advocate-1.2.4/COPYING.md` & `ligo-followup-advocate-1.2.5/COPYING.md`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/PKG-INFO` & `ligo-followup-advocate-1.2.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ligo-followup-advocate
-Version: 1.2.4
+Version: 1.2.5
 Summary: LIGO/Virgo/KAGRA Follow-up Advocate Tools
 Home-page: https://git.ligo.org/emfollow/ligo-followup-advocate
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 Maintainer: Brandon Piotrzkowski
 Maintainer-email: brandon.piotrzkowski@ligo.org
 License: GPL-2+
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 License-File: COPYING.md
 
 This package provides tools for LIGO/Virgo/KAGRA follow-up advocates to assist in tasks such as drafting astronomical bulletins for gravitational-wave detections.
```

### Comparing `ligo-followup-advocate-1.2.4/README.md` & `ligo-followup-advocate-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/__init__.py` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,16 +56,16 @@
         search = gw_event_dict['search']
         if pipeline not in pipelines:
             pipelines.append(pipeline)
         if pipeline not in early_warning_pipelines and \
                 search == 'EarlyWarning':
             early_warning_pipelines.append(pipeline)
     # Sort to get alphabetical order
-    pipelines.sort()
-    early_warning_pipelines.sort()
+    pipelines.sort(key=str.lower)
+    early_warning_pipelines.sort(key=str.lower)
 
     voevents = client.voevents(gracedb_id).json()['voevents']
     if not voevents:
         raise ValueError(
             "{} has no VOEvent to generate circulars from.".format(
                 gracedb_id))
 
@@ -75,43 +75,33 @@
         if pipeline.lower() != 'mbta':
             citation_index[pipeline.lower() + '_earlywarning'] = \
                 max(citation_index.values()) + 1
 
     gpstime = float(preferred_event['gpstime'])
     event_time = astropy.time.Time(gpstime, format='gps').utc
 
-    # Grab latest p_astro and em_bright files
-    superevent_files = client.files(gracedb_id).json()
-    em_brightfilename = 'em_bright'
-    p_astrofilename = 'p_astro'
-    em_brightfiles = []
-    p_astrofiles = []
-
-    for file in superevent_files:
-        if em_brightfilename in file and '.png' not in file:
-            em_brightfiles.append(file)
-        elif p_astrofilename in file and '.png' not in file:
-            p_astrofiles.append(file)
-
-    if em_brightfiles:
-        source_classification = client.files(
-            gracedb_id, em_brightfiles[-1]).json()
-        source_classification = {
-            key: 100 * value for key, value in source_classification.items()}
+    # Grab latest p_astro and em_bright values from lastest VOEvent
+    voevent_text = client.files(gracedb_id, voevents[-1]['filename']).read()
+    root = lxml.etree.fromstring(voevent_text)
+    p_astros = root.find('./What/Group[@name="Classification"]')
+    em_brights = root.find('./What/Group[@name="Properties"]')
+    classifications = {}
+    source_classification = {}
+    # Only try to load if present to prevent errors with .getchildren()
+    if p_astros:
+        for p_astro in p_astros.getchildren():
+            if p_astro.attrib.get('value'):
+                classifications[p_astro.attrib['name']] = \
+                    float(p_astro.attrib['value']) * 100
+    if em_brights:
+        for em_bright in em_brights.getchildren():
+            if em_bright.attrib.get('value'):
+                source_classification[em_bright.attrib['name']] = \
+                    float(em_bright.attrib['value']) * 100
         citation_index['em_bright'] = max(citation_index.values()) + 1
-    else:
-        source_classification = {}
-
-    if p_astrofiles:
-        classifications = client.files(
-            gracedb_id, p_astrofiles[-1]).json()
-        classifications = {
-            key: 100 * value for key, value in classifications.items()}
-    else:
-        classifications = {}
 
     skymaps = {}
     for voevent in voevents:
         voevent_text = client.files(gracedb_id, voevent['filename']).read()
         root = lxml.etree.fromstring(voevent_text)
         alert_type = root.find(
             './What/Param[@name="AlertType"]').attrib['value'].lower()
@@ -535,15 +525,15 @@
     ----------
     graceid: str
         ID of the trigger used by GraceDB
     filename: str
         File name of sky map
     client: class
         REST API client for HTTP connection
-    cls: list
+    cls: array-like
         List of percentage of minimal credible area used to check whether the
         areas are close to an ellipse, returning the values of the final item
     ratio_ellipse_cl_areas: float
         Ratio between ellipse area and minimal credible area from cl
     """
     if filename.endswith('.gz'):
         # Try using the multi-res sky map if it exists
@@ -551,22 +541,30 @@
             new_filename = filename.replace('.fits.gz', '.multiorder.fits')
             skymap = read_map_gracedb(graceid, new_filename, client)
         except (IOError, rest.HTTPError):
             skymap = read_map_gracedb(graceid, filename, client)
     else:
         skymap = read_map_gracedb(graceid, filename, client)
 
-    use_ellipse = True
-    for cl in cls:
-        result = crossmatch(skymap, contours=[cl / 100])
-        greedy_area = result.contour_areas[0]
-        ra, dec, a, b, pa, ellipse_area = find_ellipse(skymap, cl=cl)
-        use_ellipse = (ellipse_area <= ratio_ellipse_cl_areas * greedy_area and
-                       use_ellipse)
-    return use_ellipse, ra, dec, a, b, pa, ellipse_area, greedy_area
+    # Convert to an array if necessary
+    if np.isscalar(cls):
+        cls = [cls]
+    cls = np.asarray(cls)
+
+    # Pass array of contour inteverals to get areas
+    result = crossmatch(skymap, contours=cls / 100)
+    greedy_areas = np.asarray(result.contour_areas)
+    ra, dec, a, b, pa, ellipse_areas = find_ellipse(skymap, cl=cls)
+    a, b = np.asarray(a), np.asarray(b)
+
+    # Only use ellipse if every confidence interval passes
+    use_ellipse = \
+        np.all(ellipse_areas <= ratio_ellipse_cl_areas * greedy_areas)
+    return (use_ellipse, ra, dec, a[-1], b[-1], pa, ellipse_areas[-1],
+            greedy_areas[-1])
 
 
 def _update_raven_parameters(gracedb_id, kwargs, client):
     """Update kwargs with parameters for RAVEN coincidence"""
 
     event = client.superevent(gracedb_id).json()
```

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/jinja.py` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/jinja.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/RAVEN_circular.jinja2` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/RAVEN_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/RAVEN_subject.jinja2` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/RAVEN_subject.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/authors.jinja2` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/authors.jinja2`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% from 'macros.jinja2' import oxford_commas %}
+{% from 'macros.jinja2' import grbmission, oxford_commas %}
 {% filter rewrap %}
 {% if authors %}
 {{oxford_commas(authors)}} report{% if authors|length == 1 %}s{% endif %} on behalf of the LIGO Scientific Collaboration, the Virgo Collaboration, and the KAGRA Collaboration{% if llama and not icecube_alert %} in conjunction with the IceCube Collaboration (http://icecube.wisc.edu/){% endif %} report:
 {% else %}
-The LIGO Scientific Collaboration, the Virgo Collaboration, and the KAGRA Collaboration{% if llama and not icecube_alert %} along with the IceCube Collaboration (http://icecube.wisc.edu/){% endif %} report:
+The LIGO Scientific Collaboration, the Virgo Collaboration, and the KAGRA Collaboration{% if subthreshold_targeted %} along with the {{grbmission(external_pipeline)}} Collaboration{% elif llama and not icecube_alert %} along with the IceCube Collaboration (http://icecube.wisc.edu/){% endif %} report:
 {% endif %}
 {% endfilter %}
```

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/em_bright.jinja2` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/em_bright.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/initial_body.jinja2` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/initial_body.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/llama_alert_circular.jinja2` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/llama_alert_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/llama_track_circular.jinja2` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/llama_track_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/macros.jinja2` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/macros.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/retraction.jinja2` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/retraction.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/skymap_info.jinja2` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/skymap_info.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/update_circular.jinja2` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/templates/update_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/event.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1122/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1122/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1133/event.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1133/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/event.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1134/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1134/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/event.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1234/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files/initial.data` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1234/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/event.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1235/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/files/initial.data` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1235/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E1235/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/event.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E2244/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E2244/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E5678/event.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E5678/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E5678/files/initial.data` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/E5678/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1122/event.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M1122/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1122/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M1122/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1234/event.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M1234/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1234/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1235/event.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M1235/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1235/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M1235/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2468/event.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M2468/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2468/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M2468/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2469/event.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M2469/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2469/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M2469/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5566/event.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M5566/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5566/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M5566/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5678/event.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M5678/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5678/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M5678/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5679/event.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M5679/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5679/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/M5679/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml`

 * *Files 6% similar despite different names*

#### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml`

```diff
@@ -1,39 +1,39 @@
 <?xml version="1.0" encoding="utf-8"?>
-<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S1234-1-EarlyWarning">
+<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S2468-1-Initial">
   <Who>
-    <Date>2018-06-28T03:07:02</Date>
+    <Date>2023-04-30T18:55:35</Date>
     <Author>
       <contactName>LIGO Scientific Collaboration and Virgo Collaboration</contactName>
     </Author>
   </Who>
   <What>
     <Param name="internal" dataType="int" value="1">
       <Description>Indicates whether this event should be distributed to LSC/Virgo members only</Description>
     </Param>
     <Param name="Pkt_Ser_Num" dataType="string" value="1"/>
-    <Param name="SupereventID" dataType="string" value="S1234" ucd="meta.id">
+    <Param name="SupereventID" dataType="string" value="S2468" ucd="meta.id">
       <Description>Identifier in GraceDB</Description>
     </Param>
-    <Param name="AlertType" dataType="string" value="EarlyWarning" ucd="meta.version" unit="">
+    <Param name="AlertType" dataType="string" value="Initial" ucd="meta.version" unit="">
       <Description>VOEvent alert type</Description>
     </Param>
     <Param name="Retraction" dataType="string" value="false" ucd="meta.code" unit="">
       <Description>Set to true if the event is retracted.</Description>
     </Param>
     <Param name="HardwareInj" dataType="int" value="0" ucd="meta.number" unit="">
       <Description>Indicates that this event is a hardware injection if 1, no if 0</Description>
     </Param>
     <Param name="Vetted" dataType="int" value="0" ucd="meta.number" unit="">
       <Description>Indicates whether this candidate has undergone basic vetting by humans</Description>
     </Param>
     <Param name="OpenAlert" dataType="int" value="0" ucd="meta.number" unit="">
       <Description>Indicates that this event is an open alert if 1, no if 0</Description>
     </Param>
-    <Param name="SupereventPage" dataType="string" value="https://gracedb-playground.ligo.org/superevents/S1234/view/" ucd="meta.ref.url">
+    <Param name="SupereventPage" dataType="string" value="https://gracedb-playground.ligo.org/superevents/S2468/view/" ucd="meta.ref.url">
       <Description>Web page for evolving status of this GW candidate</Description>
     </Param>
     <Param name="Instruments" dataType="string" value="H1,L1" ucd="meta.code">
       <Description>List of instruments used in analysis to identify this event</Description>
     </Param>
     <Param name="FAR" dataType="float" value="9.11069936486e-14" ucd="arith.rate;stat.falsealarm" unit="Hz">
       <Description>False alarm rate for GW candidates with this strength or greater</Description>
@@ -43,32 +43,30 @@
     </Param>
     <Param name="Pipeline" dataType="string" value="gstlal" ucd="meta.code" unit="">
       <Description>Low-latency data analysis pipeline</Description>
     </Param>
     <Param name="Search" dataType="string" value="MDC" ucd="meta.code" unit="">
       <Description>Specific low-latency search</Description>
     </Param>
-    <Param dataType="int" name="Significant" ucd="meta.number" value="1">
-      <Description>Indicates that this event is a significant alert if 1, no if 0</Description>
-    </Param>
-    <Group type="GW_SKYMAP" name="BAYESTAR">
-      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S1234/files/bayestar.fits.gz" ucd="meta.ref.url" unit="">
+    <Group type="GW_SKYMAP" name="cWB">
+      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S2468/files/cwb.multiorder.fits" ucd="meta.ref.url" unit="">
+        <Description>Sky Map FITS basic auth protected</Description>
         <Description>Sky Map FITS</Description>
       </Param>
     </Group>
   </What>
   <WhereWhen>
     <ObsDataLocation>
       <ObservatoryLocation id="LIGO Virgo"/>
       <ObservationLocation>
         <AstroCoordSystem id="UTC-FK5-GEO"/>
         <AstroCoords coord_system_id="UTC-FK5-GEO">
           <Time>
             <TimeInstant>
-              <ISOTime>2018-06-28T03:08:04.911085</ISOTime>
+              <ISOTime>2023-04-30T18:50:35.276956</ISOTime>
             </TimeInstant>
           </Time>
         </AstroCoords>
       </ObservationLocation>
     </ObsDataLocation>
   </WhereWhen>
   <How>
```

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml`

 * *Files 23% similar despite different names*

#### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml`

```diff
@@ -1,24 +1,24 @@
 <?xml version="1.0" encoding="utf-8"?>
-<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S1234-2-Initial">
+<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S1234-1-EarlyWarning">
   <Who>
-    <Date>2018-06-28T03:20:02</Date>
+    <Date>2018-06-28T03:07:02</Date>
     <Author>
       <contactName>LIGO Scientific Collaboration and Virgo Collaboration</contactName>
     </Author>
   </Who>
   <What>
     <Param name="internal" dataType="int" value="1">
       <Description>Indicates whether this event should be distributed to LSC/Virgo members only</Description>
     </Param>
     <Param name="Pkt_Ser_Num" dataType="string" value="1"/>
     <Param name="SupereventID" dataType="string" value="S1234" ucd="meta.id">
       <Description>Identifier in GraceDB</Description>
     </Param>
-    <Param name="AlertType" dataType="string" value="Initial" ucd="meta.version" unit="">
+    <Param name="AlertType" dataType="string" value="EarlyWarning" ucd="meta.version" unit="">
       <Description>VOEvent alert type</Description>
     </Param>
     <Param name="Retraction" dataType="string" value="false" ucd="meta.code" unit="">
       <Description>Set to true if the event is retracted.</Description>
     </Param>
     <Param name="HardwareInj" dataType="int" value="0" ucd="meta.number" unit="">
       <Description>Indicates that this event is a hardware injection if 1, no if 0</Description>
@@ -47,18 +47,45 @@
     <Param name="Search" dataType="string" value="MDC" ucd="meta.code" unit="">
       <Description>Specific low-latency search</Description>
     </Param>
     <Param dataType="int" name="Significant" ucd="meta.number" value="1">
       <Description>Indicates that this event is a significant alert if 1, no if 0</Description>
     </Param>
     <Group type="GW_SKYMAP" name="BAYESTAR">
-      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S1234/files/bayestar.multiorder.fits" ucd="meta.ref.url" unit="">
+      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S1234/files/bayestar.fits.gz" ucd="meta.ref.url" unit="">
         <Description>Sky Map FITS</Description>
       </Param>
     </Group>
+    <Group name="Classification" type="Classification">
+      <Param name="BNS" value="0.95" ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is a binary neutron star merger (both objects lighter than 3 solar masses)</Description>
+      </Param>
+      <Param name="NSBH" value="0.01" ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is a neutron star-black merger (secondary lighter than 3 solar masses)</Description>
+      </Param>
+      <Param name="BBH" value="0." ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is a binary black hole merger (both objects heavier than 3 solar masses)</Description>
+      </Param>
+      <Param name="Terrestrial" value="0.04" ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is terrestrial (i.e., a background noise fluctuation or a glitch)</Description>
+      </Param>
+      <Description>Source classification: binary neutron star (BNS), neutron star-black hole (NSBH), binary black hole (BBH), or terrestrial (noise)</Description>
+    </Group>
+    <Group name="Properties" type="Properties">
+      <Param name="HasNS" value="1.0" ucd="stat.probability" dataType="float">
+        <Description>Probability that at least one object in the binary has a mass that is less than 3 solar masses</Description>
+      </Param>
+      <Param name="HasRemnant" value="1.0" ucd="stat.probability" dataType="float">
+        <Description>Probability that a nonzero mass was ejected outside the central remnant object</Description>
+      </Param>
+      <Param name="HasMassGap" value="0.2" ucd="stat.probability" dataType="float">
+        <Description>Probability that the source has at least one object between 3 and 5 solar masses</Description>
+      </Param>
+      <Description>Qualitative properties of the source, conditioned on the assumption that the signal is an astrophysical compact binary merger</Description>
+    </Group>
   </What>
   <WhereWhen>
     <ObsDataLocation>
       <ObservatoryLocation id="LIGO Virgo"/>
       <ObservationLocation>
         <AstroCoordSystem id="UTC-FK5-GEO"/>
         <AstroCoords coord_system_id="UTC-FK5-GEO">
```

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/logs.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/superevent.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/voevents.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml`

 * *Files 23% similar despite different names*

#### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml`

```diff
@@ -1,21 +1,21 @@
 <?xml version="1.0" encoding="utf-8"?>
-<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S2468-1-Initial">
+<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S1234-2-Initial">
   <Who>
-    <Date>2023-04-30T18:55:35</Date>
+    <Date>2018-06-28T03:20:02</Date>
     <Author>
       <contactName>LIGO Scientific Collaboration and Virgo Collaboration</contactName>
     </Author>
   </Who>
   <What>
     <Param name="internal" dataType="int" value="1">
       <Description>Indicates whether this event should be distributed to LSC/Virgo members only</Description>
     </Param>
     <Param name="Pkt_Ser_Num" dataType="string" value="1"/>
-    <Param name="SupereventID" dataType="string" value="S2468" ucd="meta.id">
+    <Param name="SupereventID" dataType="string" value="S1234" ucd="meta.id">
       <Description>Identifier in GraceDB</Description>
     </Param>
     <Param name="AlertType" dataType="string" value="Initial" ucd="meta.version" unit="">
       <Description>VOEvent alert type</Description>
     </Param>
     <Param name="Retraction" dataType="string" value="false" ucd="meta.code" unit="">
       <Description>Set to true if the event is retracted.</Description>
@@ -25,15 +25,15 @@
     </Param>
     <Param name="Vetted" dataType="int" value="0" ucd="meta.number" unit="">
       <Description>Indicates whether this candidate has undergone basic vetting by humans</Description>
     </Param>
     <Param name="OpenAlert" dataType="int" value="0" ucd="meta.number" unit="">
       <Description>Indicates that this event is an open alert if 1, no if 0</Description>
     </Param>
-    <Param name="SupereventPage" dataType="string" value="https://gracedb-playground.ligo.org/superevents/S2468/view/" ucd="meta.ref.url">
+    <Param name="SupereventPage" dataType="string" value="https://gracedb-playground.ligo.org/superevents/S1234/view/" ucd="meta.ref.url">
       <Description>Web page for evolving status of this GW candidate</Description>
     </Param>
     <Param name="Instruments" dataType="string" value="H1,L1" ucd="meta.code">
       <Description>List of instruments used in analysis to identify this event</Description>
     </Param>
     <Param name="FAR" dataType="float" value="9.11069936486e-14" ucd="arith.rate;stat.falsealarm" unit="Hz">
       <Description>False alarm rate for GW candidates with this strength or greater</Description>
@@ -43,30 +43,59 @@
     </Param>
     <Param name="Pipeline" dataType="string" value="gstlal" ucd="meta.code" unit="">
       <Description>Low-latency data analysis pipeline</Description>
     </Param>
     <Param name="Search" dataType="string" value="MDC" ucd="meta.code" unit="">
       <Description>Specific low-latency search</Description>
     </Param>
-    <Group type="GW_SKYMAP" name="cWB">
-      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S2468/files/cwb.multiorder.fits" ucd="meta.ref.url" unit="">
-        <Description>Sky Map FITS basic auth protected</Description>
+    <Param dataType="int" name="Significant" ucd="meta.number" value="1">
+      <Description>Indicates that this event is a significant alert if 1, no if 0</Description>
+    </Param>
+    <Group type="GW_SKYMAP" name="BAYESTAR">
+      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S1234/files/bayestar.multiorder.fits" ucd="meta.ref.url" unit="">
         <Description>Sky Map FITS</Description>
       </Param>
     </Group>
+    <Group name="Classification" type="Classification">
+      <Param name="BNS" value="0.95" ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is a binary neutron star merger (both objects lighter than 3 solar masses)</Description>
+      </Param>
+      <Param name="NSBH" value="0.01" ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is a neutron star-black merger (secondary lighter than 3 solar masses)</Description>
+      </Param>
+      <Param name="BBH" value="0." ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is a binary black hole merger (both objects heavier than 3 solar masses)</Description>
+      </Param>
+      <Param name="Terrestrial" value="0.04" ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is terrestrial (i.e., a background noise fluctuation or a glitch)</Description>
+      </Param>
+      <Description>Source classification: binary neutron star (BNS), neutron star-black hole (NSBH), binary black hole (BBH), or terrestrial (noise)</Description>
+    </Group>
+    <Group name="Properties" type="Properties">
+      <Param name="HasNS" value="1.0" ucd="stat.probability" dataType="float">
+        <Description>Probability that at least one object in the binary has a mass that is less than 3 solar masses</Description>
+      </Param>
+      <Param name="HasRemnant" value="1.0" ucd="stat.probability" dataType="float">
+        <Description>Probability that a nonzero mass was ejected outside the central remnant object</Description>
+      </Param>
+      <Param name="HasMassGap" value="0.2" ucd="stat.probability" dataType="float">
+        <Description>Probability that the source has at least one object between 3 and 5 solar masses</Description>
+      </Param>
+      <Description>Qualitative properties of the source, conditioned on the assumption that the signal is an astrophysical compact binary merger</Description>
+    </Group>
   </What>
   <WhereWhen>
     <ObsDataLocation>
       <ObservatoryLocation id="LIGO Virgo"/>
       <ObservationLocation>
         <AstroCoordSystem id="UTC-FK5-GEO"/>
         <AstroCoords coord_system_id="UTC-FK5-GEO">
           <Time>
             <TimeInstant>
-              <ISOTime>2023-04-30T18:50:35.276956</ISOTime>
+              <ISOTime>2018-06-28T03:08:04.911085</ISOTime>
             </TimeInstant>
           </Time>
         </AstroCoords>
       </ObservationLocation>
     </ObsDataLocation>
   </WhereWhen>
   <How>
```

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/logs.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/superevent.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/voevents.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S2468/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml`

 * *Files 16% similar despite different names*

#### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml`

```diff
@@ -79,14 +79,41 @@
     </Group>
     <Group type="GW_SKYMAP" name="BAYESTAR">
       <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S5678/files/bayestar.multiorder.fits" ucd="meta.ref.url" unit="">
         <Description>Sky Map FITS basic auth protected</Description>
         <Description>Sky Map FITS</Description>
       </Param>
     </Group>
+    <Group name="Classification" type="Classification">
+      <Param name="BNS" value="0." ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is a binary neutron star merger (both objects lighter than 3 solar masses)</Description>
+      </Param>
+      <Param name="NSBH" value="0.6778160323909137" ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is a neutron star-black merger (secondary lighter than 3 solar masses)</Description>
+      </Param>
+      <Param name="BBH" value="0." ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is a binary black hole merger (both objects heavier than 3 solar masses)</Description>
+      </Param>
+      <Param name="Terrestrial" value="0.32218396760908624" ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is terrestrial (i.e., a background noise fluctuation or a glitch)</Description>
+      </Param>
+      <Description>Source classification: binary neutron star (BNS), neutron star-black hole (NSBH), binary black hole (BBH), or terrestrial (noise)</Description>
+    </Group>
+    <Group name="Properties" type="Properties">
+      <Param name="HasNS" value="1.0" ucd="stat.probability" dataType="float">
+        <Description>Probability that at least one object in the binary has a mass that is less than 3 solar masses</Description>
+      </Param>
+      <Param name="HasRemnant" value="0.0" ucd="stat.probability" dataType="float">
+        <Description>Probability that a nonzero mass was ejected outside the central remnant object</Description>
+      </Param>
+      <Param name="HasMassGap" value="0.0" ucd="stat.probability" dataType="float">
+        <Description>Probability that the source has at least one object between 3 and 5 solar masses</Description>
+      </Param>
+      <Description>Qualitative properties of the source, conditioned on the assumption that the signal is an astrophysical compact binary merger</Description>
+    </Group>
   </What>
   <WhereWhen>
     <ObsDataLocation>
       <ObservatoryLocation id="LIGO Virgo"/>
       <ObservationLocation>
         <AstroCoordSystem id="UTC-FK5-GEO"/>
         <AstroCoords coord_system_id="UTC-FK5-GEO">
```

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml`

 * *Files 19% similar despite different names*

#### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml`

```diff
@@ -79,14 +79,41 @@
     </Group>
     <Group type="GW_SKYMAP" name="LALInference">
       <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S5678/files/bilby.fits.gz,0" ucd="meta.ref.url" unit="">
         <Description>Sky Map FITS basic auth protected</Description>
         <Description>Sky Map FITS</Description>
       </Param>
     </Group>
+    <Group name="Classification" type="Classification">
+      <Param name="BNS" value="0." ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is a binary neutron star merger (both objects lighter than 3 solar masses)</Description>
+      </Param>
+      <Param name="NSBH" value="0.6778160323909137" ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is a neutron star-black merger (secondary lighter than 3 solar masses)</Description>
+      </Param>
+      <Param name="BBH" value="0." ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is a binary black hole merger (both objects heavier than 3 solar masses)</Description>
+      </Param>
+      <Param name="Terrestrial" value="0.32218396760908624" ucd="stat.probability" dataType="float">
+        <Description>Probability that the source is terrestrial (i.e., a background noise fluctuation or a glitch)</Description>
+      </Param>
+      <Description>Source classification: binary neutron star (BNS), neutron star-black hole (NSBH), binary black hole (BBH), or terrestrial (noise)</Description>
+    </Group>
+    <Group name="Properties" type="Properties">
+      <Param name="HasNS" value="1.0" ucd="stat.probability" dataType="float">
+        <Description>Probability that at least one object in the binary has a mass that is less than 3 solar masses</Description>
+      </Param>
+      <Param name="HasRemnant" value="0.0" ucd="stat.probability" dataType="float">
+        <Description>Probability that a nonzero mass was ejected outside the central remnant object</Description>
+      </Param>
+      <Param name="HasMassGap" value="0.0" ucd="stat.probability" dataType="float">
+        <Description>Probability that the source has at least one object between 3 and 5 solar masses</Description>
+      </Param>
+      <Description>Qualitative properties of the source, conditioned on the assumption that the signal is an astrophysical compact binary merger</Description>
+    </Group>
   </What>
   <WhereWhen>
     <ObsDataLocation>
       <ObservatoryLocation id="LIGO Virgo"/>
       <ObservationLocation>
         <AstroCoordSystem id="UTC-FK5-GEO"/>
         <AstroCoords coord_system_id="UTC-FK5-GEO">
```

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/logs.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/superevent.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/voevents.json` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/data/S5678/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/test_tool.py` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/test/test_tool.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo/followup_advocate/tool.py` & `ligo-followup-advocate-1.2.5/ligo/followup_advocate/tool.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/PKG-INFO` & `ligo-followup-advocate-1.2.5/ligo_followup_advocate.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ligo-followup-advocate
-Version: 1.2.4
+Version: 1.2.5
 Summary: LIGO/Virgo/KAGRA Follow-up Advocate Tools
 Home-page: https://git.ligo.org/emfollow/ligo-followup-advocate
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 Maintainer: Brandon Piotrzkowski
 Maintainer-email: brandon.piotrzkowski@ligo.org
 License: GPL-2+
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 License-File: COPYING.md
 
 This package provides tools for LIGO/Virgo/KAGRA follow-up advocates to assist in tasks such as drafting astronomical bulletins for gravitational-wave detections.
```

### Comparing `ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/SOURCES.txt` & `ligo-followup-advocate-1.2.5/ligo_followup_advocate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/setup.cfg` & `ligo-followup-advocate-1.2.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 maintainer = Brandon Piotrzkowski
 maintainer_email = brandon.piotrzkowski@ligo.org
 url = https://git.ligo.org/emfollow/ligo-followup-advocate
 classifiers = 
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 	Operating System :: POSIX
-	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
 	Topic :: Scientific/Engineering :: Astronomy
 	Topic :: Scientific/Engineering :: Physics
 scripts = bin/ligo-followup-advocate
 
 [options]
 packages = find:
-python_requires = >= 3.8
+python_requires = >= 3.9
 tests_require = 
 	pytest >= 3.0
 	pytest-mock
 
 [options.entry_points]
 console_scripts = 
 	ligo-followup-advocate = ligo.followup_advocate.tool:main
```

### Comparing `ligo-followup-advocate-1.2.4/setup.py` & `ligo-followup-advocate-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.4/versioneer.py` & `ligo-followup-advocate-1.2.5/versioneer.py`

 * *Files identical despite different names*

