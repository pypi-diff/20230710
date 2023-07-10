# Comparing `tmp/wonambi-7.12.tar.gz` & `tmp/wonambi-7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonambi-7.12.tar", last modified: Mon Jul 10 20:06:47 2023, max compression
+gzip compressed data, was "dist/wonambi-7.6.tar", last modified: Wed Mar  9 20:09:44 2022, max compression
```

## Comparing `wonambi-7.12.tar` & `wonambi-7.6.tar`

### file list

```diff
@@ -1,176 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.627763 wonambi-7.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-10 20:06:37.000000 wonambi-7.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-10 20:06:47.627763 wonambi-7.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-10 20:06:37.000000 wonambi-7.12/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 20:06:47.627763 wonambi-7.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-10 20:06:37.000000 wonambi-7.12/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.607761 wonambi-7.12/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_attr_anat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_attr_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_attr_chan.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_bids_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_detect_agreement.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_detect_ripple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_detect_slowwave.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_detect_spindle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_ioeeg_abf.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_ioeeg_bci2000.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_ioeeg_bids.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_ioeeg_blackrock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_ioeeg_brainvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_ioeeg_edf.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_ioeeg_eeglab.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_ioeeg_egimff.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_ioeeg_fieldtrip.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_ioeeg_ktlx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_ioeeg_micromed.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_ioeeg_moberg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_ioeeg_openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_ioeeg_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_ioeeg_wonambi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_scroll_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_source_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_source_morph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_trans_baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_trans_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_trans_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_trans_frequency_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_trans_math.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_trans_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_trans_montage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_trans_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_utils_simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_viz_plot3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_widget_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_widget_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_widget_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_widget_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_widget_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-10 20:06:37.000000 wonambi-7.12/tests/test_widgets_modal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.611762 wonambi-7.12/wonambi/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.611762 wonambi-7.12/wonambi/attr/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/attr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/attr/anat.py
--rw-r--r--   0 runner    (1001) docker     (123)    92521 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/attr/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/attr/chan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.611762 wonambi-7.12/wonambi/bids/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/bids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/bids/find.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/bids/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/bids/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.611762 wonambi-7.12/wonambi/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/bin/convert.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10891 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/bin/scroll_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16589 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/datatype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.615762 wonambi-7.12/wonambi/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/detect/agreement.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/detect/arousal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/detect/ripple.py
--rw-r--r--   0 runner    (1001) docker     (123)    18370 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/detect/slowwave.py
--rw-r--r--   0 runner    (1001) docker     (123)    78590 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/detect/spindle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/graphoelement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.615762 wonambi-7.12/wonambi/ioeeg/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/abf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/bci2000.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/bids.py
--rw-r--r--   0 runner    (1001) docker     (123)    21447 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/blackrock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/brainvision.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/edf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/eeglab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/egimff.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/fieldtrip.py
--rw-r--r--   0 runner    (1001) docker     (123)    39601 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/ktlx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/lyonrri.py
--rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/micromed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/mnefiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/moberg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/ioeeg/wonambi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.615762 wonambi-7.12/wonambi/source/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/source/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/source/morph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.619762 wonambi-7.12/wonambi/trans/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14884 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/trans/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/trans/baseline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.619762 wonambi-7.12/wonambi/trans/extern/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/trans/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/trans/extern/dpss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/trans/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    26927 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/trans/frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/trans/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/trans/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/trans/montage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/trans/peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/trans/reject.py
--rw-r--r--   0 runner    (1001) docker     (123)    29815 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/trans/select.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.619762 wonambi-7.12/wonambi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/utils/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.619762 wonambi-7.12/wonambi/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/viz/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/viz/plot_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/viz/visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.623762 wonambi-7.12/wonambi/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    90406 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    18790 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/creation.py
--rw-r--r--   0 runner    (1001) docker     (123)    26784 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/detect_dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.603761 wonambi-7.12/wonambi/widgets/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.627763 wonambi-7.12/wonambi/widgets/icons/oxygen/
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/bookmarks-organize.png
--rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/chronometer.png
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/configure.png
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/document-open.png
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/download.png
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/edit-table-cell-merge.png
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/edit-table-delete-column.png
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/edit-table-insert-column-right.png
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/format-line-spacing-normal.png
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/format-line-spacing-triple.png
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/go-down.png
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/go-next-view.png
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/go-next.png
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/go-previous-view.png
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/go-previous.png
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/go-up.png
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/help-about.png
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/mail-mark-task.png
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/window-close.png
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/window-duplicate.png
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/zoom-in.png
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/zoom-next.png
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/zoom-out.png
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/icons/oxygen/zoom-previous.png
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/modal_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    73769 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/notes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20215 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/overview.py
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)    47836 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/traces.py
--rw-r--r--   0 runner    (1001) docker     (123)    23684 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-10 20:06:37.000000 wonambi-7.12/wonambi/widgets/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:47.611762 wonambi-7.12/wonambi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-10 20:06:47.000000 wonambi-7.12/wonambi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-07-10 20:06:47.000000 wonambi-7.12/wonambi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:06:47.000000 wonambi-7.12/wonambi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-10 20:06:47.000000 wonambi-7.12/wonambi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-10 20:06:47.000000 wonambi-7.12/wonambi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 20:06:47.000000 wonambi-7.12/wonambi.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1479 2022-03-09 20:04:14.000000 wonambi-7.6/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3522 2022-03-09 20:09:44.000000 wonambi-7.6/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2507 2022-03-09 20:04:14.000000 wonambi-7.6/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-03-09 20:09:44.000000 wonambi-7.6/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2350 2022-03-09 20:04:14.000000 wonambi-7.6/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/wonambi/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/VERSION
+-rw-rw-r--   0 travis    (2000) travis    (2000)      442 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/wonambi/attr/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1180 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/attr/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11524 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/attr/anat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91106 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/attr/annotations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14041 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/attr/chan.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/wonambi/bids/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/bids/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      695 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/bids/find.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2551 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/bids/structure.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      905 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/bids/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/wonambi/bin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/bin/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4057 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/bin/convert.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    10891 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/bin/scroll_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15438 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/dataset.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16589 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/datatype.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/wonambi/detect/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/detect/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12360 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/detect/agreement.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8461 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/detect/arousal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1284 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/detect/ripple.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17921 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/detect/slowwave.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78590 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/detect/spindle.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6950 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/graphoelement.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/wonambi/ioeeg/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      642 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15329 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/abf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10054 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/bci2000.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7256 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/bids.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21447 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/blackrock.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9480 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/brainvision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14502 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/edf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5120 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/eeglab.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13707 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/egimff.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4767 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/fieldtrip.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39601 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/ktlx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4220 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/lyonrri.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19707 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/micromed.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1027 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/mnefiff.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6052 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/moberg.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13292 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/openephys.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5609 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/text.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2066 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5036 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/ioeeg/wonambi.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/wonambi/source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       52 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/source/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6148 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/source/linear.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1315 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/source/morph.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/wonambi/trans/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      815 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/trans/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14884 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/trans/analyze.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3174 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/trans/baseline.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/wonambi/trans/extern/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/trans/extern/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12481 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/trans/extern/dpss.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5425 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/trans/filter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26927 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/trans/frequency.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7564 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/trans/math.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2126 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/trans/merge.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6224 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/trans/montage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4921 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/trans/peaks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3238 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/trans/reject.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29815 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/trans/select.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/wonambi/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      278 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      986 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/utils/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7251 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/utils/simulate.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/wonambi/viz/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      306 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/viz/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1598 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/viz/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6438 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/viz/plot_3d.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2342 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/viz/visuals.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/wonambi/widgets/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      583 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    90406 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/analysis.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18790 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/channels.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14140 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/creation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26784 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/detect_dialogs.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/wonambi/widgets/icons/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2520 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/bookmarks-organize.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14551 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/chronometer.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2575 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/configure.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2798 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/document-open.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4482 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/download.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1411 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/edit-table-cell-merge.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2743 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/edit-table-delete-column.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3233 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/edit-table-insert-column-right.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      680 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/format-line-spacing-normal.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      798 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/format-line-spacing-triple.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2404 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/go-down.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2001 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/go-next-view.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2425 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/go-next.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2011 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/go-previous-view.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2522 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/go-previous.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2426 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/go-up.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2742 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/help-about.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3352 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/mail-mark-task.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3751 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/window-close.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      638 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/window-duplicate.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3034 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/zoom-in.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3048 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/zoom-next.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2939 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/zoom-out.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3040 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/icons/oxygen/zoom-previous.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16823 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/info.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6155 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/labels.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8926 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/modal_widgets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    73276 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/notes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20215 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/overview.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12211 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/settings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8734 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/spectrum.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47836 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/traces.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23684 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5809 2022-03-09 20:04:14.000000 wonambi-7.6/wonambi/widgets/video.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-09 20:09:44.000000 wonambi-7.6/wonambi.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3522 2022-03-09 20:09:43.000000 wonambi-7.6/wonambi.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3342 2022-03-09 20:09:43.000000 wonambi-7.6/wonambi.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-03-09 20:09:43.000000 wonambi-7.6/wonambi.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       96 2022-03-09 20:09:43.000000 wonambi-7.6/wonambi.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      159 2022-03-09 20:09:43.000000 wonambi-7.6/wonambi.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2022-03-09 20:09:43.000000 wonambi-7.6/wonambi.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `wonambi-7.12/LICENSE` & `wonambi-7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/PKG-INFO` & `wonambi-7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: wonambi
-Version: 7.12
+Version: 7.6
 Summary: Tools for EEG, ECoG, iEEG, especially for sleep
 Home-page: https://github.com/wonambi-python/wonambi
 Author: Gio Piantoni / Jordan O'Byrne
 Author-email: wonambi@gpiantoni.com
 License: GPLv3
 Keywords: neuroscience analysis sleep EEG ECoG
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Visualization
@@ -110,7 +111,9 @@
 
 .. image:: https://codecov.io/gh/wonambi-python/wonambi/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/wonambi-python/wonambi
 
 License
 -------
 The project is licensed under the 3-clause BSD license.
+
+
```

### Comparing `wonambi-7.12/README.rst` & `wonambi-7.6/README.rst`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/setup.py` & `wonambi-7.6/setup.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/attr/__init__.py` & `wonambi-7.6/wonambi/attr/__init__.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/attr/anat.py` & `wonambi-7.6/wonambi/attr/anat.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/attr/annotations.py` & `wonambi-7.6/wonambi/attr/annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,31 +125,24 @@
 PHYSIP_STAGE_KEY = {'0': 'NREM3',
                    '1': 'NREM2',
                    '2': 'NREM1',
                    '3': 'REM',
                    '4': 'Wake',
                    '5': 'Artefact'}
 
-PHILLIPS_STAGE_KEY = {'WK': 'Wake',
-                 'N1': 'NREM1',
-                 'N2': 'NREM2',
-                 'N3': 'NREM3',
-                 'RE': 'REM'}
-
 BIDS_STAGE_KEY = {'Wake': 'sleep_wake',
                   'NREM1': 'sleep_N1',
                   'NREM2': 'sleep_N2',
                   'NREM3': 'sleep_N3',
                   'REM': 'sleep_REM',
                   'Artefact': 'artifact',
                   'Movement': 'artifact_motion',
                   'Unknown': '',
                   'Undefined': ''}
 
-
 def parse_iso_datetime(date):
     try:
         return datetime.strptime(date, "%Y-%m-%dT%H:%M:%S")
     except ValueError:
         return datetime.strptime(date, "%Y-%m-%dT%H:%M:%S.%f")
 
 
@@ -465,15 +458,15 @@
 
         Parameters
         ----------
         filename : str
             Staging file name.
         source : str
             Name of program where staging was made. One of 'domino', 'alice',
-            'compumedics', 'sandman', 'remlogic', 'phillips', 'grael', 'egi'
+            'compumedics', 'sandman', 'remlogic'
         rater_name : str
             Rater name for imported staging.
         rec_start : datetime
             Date and time (year, month, day, hour, minute, second) of recording
             start. Year is ignored (New Year's Eve celebratory recordings
             unsupported.)
         staging_start : datetime (default: None)
@@ -706,42 +699,14 @@
                     if j.isdigit():
                         idx_epoch_length = i, i + lines[3][i:].index(' ')
                         epoch_length = int(lines[3][slice(*idx_epoch_length)])
                         break
                 if idx_epoch_length is None:
                     epoch_length = 30
 
-        elif source == 'phillips':
-            if not isinstance(staging_start, datetime):
-                dt = rec_start
-                staging_start_str = lines[1].split(',')[1].lower()
-                staging_start = datetime.strptime(staging_start_str, 
-                                                  '%I:%M:%S %p')
-    
-                # best guess in absence of date
-                if staging_start_str[-2:] == 'pm' and rec_start.hour < 12:
-                    dt = rec_start - timedelta(days=1)
-                elif staging_start_str[-2:] == 'am' and rec_start.hour > 12:
-                    dt = rec_start + timedelta(days=1)
-                    
-                staging_start = staging_start.replace(year=dt.year,
-                                                      month=dt.month,
-                                                      day=dt.day)
-                
-            first_second = int((staging_start - rec_start).total_seconds())
-
-            idx_first_line = 0
-            stage_key = PHILLIPS_STAGE_KEY
-            idx_stage = slice(0, 2)
-
-            if epoch_length is None:
-                epoch_length = 30
-                
-            lines = [x.split(',')[2] for x in lines]            
-
         else:
             raise ValueError('Unknown source program for staging file')
 
         offset = first_second % epoch_length
         lg.info('Time offset: ' + str(offset) + ' sec')
 
         if rater_name not in self.raters:
```

### Comparing `wonambi-7.12/wonambi/attr/chan.py` & `wonambi-7.6/wonambi/attr/chan.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/bids/find.py` & `wonambi-7.6/wonambi/bids/find.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/bids/structure.py` & `wonambi-7.6/wonambi/bids/structure.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/bids/utils.py` & `wonambi-7.6/wonambi/bids/utils.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/bin/convert.py` & `wonambi-7.6/wonambi/bin/convert.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/bin/scroll_data.py` & `wonambi-7.6/wonambi/bin/scroll_data.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/dataset.py` & `wonambi-7.6/wonambi/dataset.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/datatype.py` & `wonambi-7.6/wonambi/datatype.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/detect/agreement.py` & `wonambi-7.6/wonambi/detect/agreement.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/detect/arousal.py` & `wonambi-7.6/wonambi/detect/arousal.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/detect/ripple.py` & `wonambi-7.6/wonambi/detect/ripple.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/detect/slowwave.py` & `wonambi-7.6/wonambi/detect/slowwave.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Module to detect slow waves.
 
 """
 from logging import getLogger
 from numpy import (argmin, concatenate, diff, hstack, logical_and, newaxis, 
-                   ones, percentile, roll, sign, sum, vstack, where, zeros)
-from scipy.signal import firwin, kaiserord, lfilter
+                   ones, percentile, sign, sum, vstack, where, zeros)
 
 try:
     from PyQt5.QtCore import Qt
     from PyQt5.QtWidgets import QProgressDialog
 except ImportError:
     pass
 
@@ -319,30 +318,15 @@
     Staresina, B. et al. 18(11) 1679-86 (2015).
 
     """
     if opts.invert:
         dat_orig = -dat_orig
 
     sw_in_chan = []
-    
-    # Create a FIR filter
-    nyq_rate = s_freq / 2.0
-    width = 5.0/nyq_rate
-    N, beta = kaiserord(60.0, width)
-    cutoff = opts.lowpass['freq']
-    b = firwin(N, cutoff/nyq_rate, window=('kaiser', beta))
-    
-    # Filter the signal
-    fir = lfilter(b, 1.0, dat_orig)
-    
-    # Apply the phase shift correction
-    delay = int(-0.5 * (N-1))
-    dat_det = roll(fir, delay)
-    
-    #dat_det = transform_signal(dat_orig, s_freq, 'low_butter', opts.lowpass)
+    dat_det = transform_signal(dat_orig, s_freq, 'low_butter', opts.lowpass)
     idx_zx = find_zero_crossings(dat_det, xtype='pos_to_neg') 
     events = find_intervals(idx_zx, s_freq, opts.duration)
 
     if events is not None:
         events = find_peaks_in_slowwwave(dat_det, events)
 
         if events is not None:
```

### Comparing `wonambi-7.12/wonambi/detect/spindle.py` & `wonambi-7.6/wonambi/detect/spindle.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/graphoelement.py` & `wonambi-7.6/wonambi/graphoelement.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/__init__.py` & `wonambi-7.6/wonambi/ioeeg/__init__.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/abf.py` & `wonambi-7.6/wonambi/ioeeg/abf.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/bci2000.py` & `wonambi-7.6/wonambi/ioeeg/bci2000.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/bids.py` & `wonambi-7.6/wonambi/ioeeg/bids.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/blackrock.py` & `wonambi-7.6/wonambi/ioeeg/blackrock.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/brainvision.py` & `wonambi-7.6/wonambi/ioeeg/brainvision.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/edf.py` & `wonambi-7.6/wonambi/ioeeg/edf.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/eeglab.py` & `wonambi-7.6/wonambi/ioeeg/eeglab.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,27 +68,20 @@
             with File(self.filename) as f:
                 EEG = f['EEG']
                 try:
                     self.s_freq = EEG['srate'].value.item()
                 except:
                     self.s_freq = EEG['srate'][()].item()
                 chan_name = read_hdf5_chan_name(f, EEG['chanlocs']['labels'])
-                try:
-                    n_samples = int(EEG['pnts'].value.item())
-                except:
-                    n_samples = int(EEG['pnts'][0].item())
+                n_samples = int(EEG['pnts'].value.item())
 
                 subj_id = read_hdf5_str(EEG['subject'])
                 try:
                     if 'T0' in list(EEG['etc']):
-                        try:
-                            start_time = datetime(*EEG['etc']['T0'])
-                        except:
-                            EEG_starttime = [int(x[0]) for x in EEG['etc']['T0']]
-                            start_time = datetime(*EEG_starttime)
+                        start_time = datetime(*EEG['etc']['T0'])
                     elif 'rec_startdate' in list(EEG['etc']):
                         EEG_starttime = EEG['etc']['rec_startdate']
                         start_time_char = ''.join([chr(x) for x in EEG_starttime])
                         start_time = datetime.fromisoformat(start_time_char)
                     else:
                         start_time = DEFAULT_DATETIME
                 except ValueError:
```

### Comparing `wonambi-7.12/wonambi/ioeeg/egimff.py` & `wonambi-7.6/wonambi/ioeeg/egimff.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/fieldtrip.py` & `wonambi-7.6/wonambi/ioeeg/fieldtrip.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from datetime import datetime
 from logging import getLogger
-from numpy import around, c_, empty, float64, NaN
+from numpy import around, empty
 from scipy.io import loadmat, savemat
 
 from .utils import read_hdf5_chan_name
 from ..utils import MissingDependency
 
 try:
     from h5py import File
 except ImportError as err:
-    File = MissingDependency(err)  
+    File = MissingDependency(err)
+
 
 lg = getLogger(__name__)
 VAR = 'data'
 
 
 class FieldTrip:
     """Basic class to read the data.
@@ -72,21 +73,18 @@
         except NotImplementedError:
 
             with File(self.filename) as f:
 
                 if VAR not in f.keys():
                     raise KeyError('Save the FieldTrip variable as ''{}'''
                                    ''.format(VAR))
-                try:
-                    s_freq = int(f[VAR]['fsample'].value.squeeze())
-                except:
-                    s_freq = int(f[VAR]['fsample'][0].squeeze())
-                
-                
+
+                s_freq = int(f[VAR]['fsample'].value.squeeze())
                 chan_name = read_hdf5_chan_name(f, f[VAR]['label'])
+
                 n_samples = int(around(f[f[VAR]['trial'][0].item()].shape[0]))
 
         return subj_id, start_time, s_freq, chan_name, n_samples, orig
 
     def return_dat(self, chan, begsam, endsam):
         """Return the data as 2D numpy.ndarray.
 
@@ -102,48 +100,28 @@
         Returns
         -------
         numpy.ndarray
             A 2d matrix, with dimension chan X samples
 
         """
         TRL = 0
-             
         try:
             ft_data = loadmat(self.filename, struct_as_record=True,
                               squeeze_me=True)
-            
-            n_samples = ft_data['shape'][1]
             ft_data = ft_data[VAR]
-            
 
             data = ft_data['trial'].item(TRL)
 
         except NotImplementedError:
             from h5py import File
 
             with File(self.filename) as f:
-                try:
-                    data = f[f[VAR]['trial'][TRL].item()].value.T
-                except:
-                    data = f[f[VAR]['trial'][TRL].item()][:].T
-            n_samples = data.shape[1]
-       
-        dat = data[:, begsam:endsam]
-                    
-        if begsam < 0:
-            pad = empty((dat.shape[0], 0 - begsam))
-            pad.fill(NaN)
-            dat = c_[pad, dat]
-
-        if endsam >= n_samples:
-            pad = empty((dat.shape[0], endsam - n_samples))
-            pad.fill(NaN)
-            dat = c_[dat, pad]
+                data = f[f[VAR]['trial'][TRL].item()].value.T
 
-        return dat[chan, :]
+        return data[chan, begsam:endsam]
 
     def return_markers(self):
         """Return all the markers (also called triggers or events).
 
         Returns
         -------
         list of dict
```

### Comparing `wonambi-7.12/wonambi/ioeeg/ktlx.py` & `wonambi-7.6/wonambi/ioeeg/ktlx.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/lyonrri.py` & `wonambi-7.6/wonambi/ioeeg/lyonrri.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/micromed.py` & `wonambi-7.6/wonambi/ioeeg/micromed.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/mnefiff.py` & `wonambi-7.6/wonambi/ioeeg/mnefiff.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/moberg.py` & `wonambi-7.6/wonambi/ioeeg/moberg.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/openephys.py` & `wonambi-7.6/wonambi/ioeeg/openephys.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/text.py` & `wonambi-7.6/wonambi/ioeeg/text.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/ioeeg/utils.py` & `wonambi-7.6/wonambi/ioeeg/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,15 +71,12 @@
     for l in labels:
         chan_name.append(read_hdf5_str(f[l]))
     
     return chan_name
 
 
 def read_hdf5_str(value):
-    try:
-        datfile = ''.join([chr(str(x)) for x in value.value])
-    except:
-        datfile = ''.join([chr(x[0]) for x in value])
+    datfile = ''.join([chr(x) for x in value.value])
     if datfile == '\x00\x00':
         return ''
     else:
         return datfile
```

### Comparing `wonambi-7.12/wonambi/ioeeg/wonambi.py` & `wonambi-7.6/wonambi/ioeeg/wonambi.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/source/linear.py` & `wonambi-7.6/wonambi/source/linear.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/source/morph.py` & `wonambi-7.6/wonambi/source/morph.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/trans/__init__.py` & `wonambi-7.6/wonambi/trans/__init__.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/trans/analyze.py` & `wonambi-7.6/wonambi/trans/analyze.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/trans/baseline.py` & `wonambi-7.6/wonambi/trans/baseline.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/trans/extern/dpss.py` & `wonambi-7.6/wonambi/trans/extern/dpss.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/trans/filter.py` & `wonambi-7.6/wonambi/trans/filter.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/trans/frequency.py` & `wonambi-7.6/wonambi/trans/frequency.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/trans/math.py` & `wonambi-7.6/wonambi/trans/math.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/trans/merge.py` & `wonambi-7.6/wonambi/trans/merge.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/trans/montage.py` & `wonambi-7.6/wonambi/trans/montage.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/trans/peaks.py` & `wonambi-7.6/wonambi/trans/peaks.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/trans/reject.py` & `wonambi-7.6/wonambi/trans/reject.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/trans/select.py` & `wonambi-7.6/wonambi/trans/select.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/utils/exceptions.py` & `wonambi-7.6/wonambi/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/utils/simulate.py` & `wonambi-7.6/wonambi/utils/simulate.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/viz/base.py` & `wonambi-7.6/wonambi/viz/base.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/viz/plot_3d.py` & `wonambi-7.6/wonambi/viz/plot_3d.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/viz/visuals.py` & `wonambi-7.6/wonambi/viz/visuals.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/__init__.py` & `wonambi-7.6/wonambi/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/analysis.py` & `wonambi-7.6/wonambi/widgets/analysis.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/channels.py` & `wonambi-7.6/wonambi/widgets/channels.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/creation.py` & `wonambi-7.6/wonambi/widgets/creation.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,26 +268,24 @@
 
     submenu_import = menu_annot.addMenu('Import Staging')
     submenu_import.addAction(actions['import_alice'])
     submenu_import.addAction(actions['import_compumedics'])
     submenu_import.addAction(actions['import_deltamed'])
     submenu_import.addAction(actions['import_grael'])
     submenu_import.addAction(actions['import_domino'])
-    submenu_import.addAction(actions['import_phillips'])
     submenu_import.addAction(actions['import_prana'])
     submenu_import.addAction(actions['import_remlogic'])
     submenu_import.addAction(actions['import_sandman'])
     submenu_import.addAction(actions['import_fasst'])
 
     submenu_import_qual = menu_annot.addMenu('Import Signal Quality')
     submenu_import_qual.addAction(actions['import_alice_qual'])
     submenu_import_qual.addAction(actions['import_compumedics_qual'])
     submenu_import_qual.addAction(actions['import_deltamed_qual'])
     submenu_import_qual.addAction(actions['import_domino_qual'])
-    submenu_import_qual.addAction(actions['import_phillips_qual'])
     submenu_import_qual.addAction(actions['import_prana_qual'])
     submenu_import_qual.addAction(actions['import_remlogic_qual'])
     submenu_import_qual.addAction(actions['import_sandman_qual'])
     
     submenu_import_event = menu_annot.addMenu('Import Events')
     submenu_import_event.addAction(actions['import_events_wonambi'])
     submenu_import_event.addAction(actions['import_events_remlogic'])
```

### Comparing `wonambi-7.12/wonambi/widgets/detect_dialogs.py` & `wonambi-7.6/wonambi/widgets/detect_dialogs.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/bookmarks-organize.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/bookmarks-organize.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/chronometer.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/chronometer.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/configure.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/configure.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/document-open.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/document-open.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/download.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/download.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/edit-table-cell-merge.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/edit-table-cell-merge.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/edit-table-delete-column.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/edit-table-delete-column.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/edit-table-insert-column-right.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/edit-table-insert-column-right.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/format-line-spacing-normal.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/format-line-spacing-normal.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/format-line-spacing-triple.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/format-line-spacing-triple.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/go-down.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/go-down.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/go-next-view.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/go-next-view.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/go-next.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/go-next.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/go-previous-view.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/go-previous-view.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/go-previous.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/go-previous.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/go-up.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/go-up.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/help-about.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/help-about.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/mail-mark-task.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/mail-mark-task.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/window-close.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/window-close.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/window-duplicate.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/window-duplicate.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/zoom-in.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/zoom-in.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/zoom-next.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/zoom-next.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/zoom-out.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/zoom-out.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/icons/oxygen/zoom-previous.png` & `wonambi-7.6/wonambi/widgets/icons/oxygen/zoom-previous.png`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/info.py` & `wonambi-7.6/wonambi/widgets/info.py`

 * *Files 6% similar despite different names*

```diff
@@ -223,14 +223,40 @@
         IOClass, sessions = detect_format(filename)
         if len(sessions) > 1:
             session = select_session(sessions)
             self.dataset = Dataset(filename, bids=bids, session=session + 1)  # temp
         else:
             self.dataset = Dataset(filename, bids=bids)  # temp
 
+#==============================================================================
+#         try:
+#             self.filename = filename
+#             self.dataset = Dataset(filename)
+#         except FileNotFoundError:
+#             msg = 'File ' + basename(filename) + ' cannot be read'
+#             self.parent.statusBar().showMessage(msg)
+#             lg.info(msg)
+#             error_dialog = QErrorMessage()
+#             error_dialog.setWindowTitle('Error opening dataset')
+#             error_dialog.showMessage(msg)
+#             if debug_filename is None:
+#                 error_dialog.exec()
+#             return
+#
+#         except BaseException as err:
+#             self.parent.statusBar().showMessage(str(err))
+#             lg.info('Error ' + str(err))
+#             error_dialog = QErrorMessage()
+#             error_dialog.setWindowTitle('Error opening dataset')
+#             error_dialog.showMessage(str(err))
+#             if debug_filename is None:
+#                 error_dialog.exec()
+#             return
+#==============================================================================
+
         self.action['export'].setEnabled(True)
 
         self.parent.statusBar().showMessage('')
 
         self.parent.update()
 
     def display_dataset(self):
```

### Comparing `wonambi-7.12/wonambi/widgets/labels.py` & `wonambi-7.6/wonambi/widgets/labels.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/modal_widgets.py` & `wonambi-7.6/wonambi/widgets/modal_widgets.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/notes.py` & `wonambi-7.6/wonambi/widgets/notes.py`

 * *Files 2% similar despite different names*

```diff
@@ -414,18 +414,14 @@
         act = QAction('DeltaMed', self)
         act.triggered.connect(partial(self.import_staging, 'deltamed'))
         actions['import_deltamed'] = act
         
         act = QAction('Grael', self)
         act.triggered.connect(partial(self.import_staging, 'grael'))
         actions['import_grael'] = act
-        
-        act = QAction('Phillips', self)
-        act.triggered.connect(partial(self.import_staging, 'phillips'))
-        actions['import_phillips'] = act
 
         act = QAction('FASST', self)
         act.triggered.connect(self.import_fasst)
         actions['import_fasst'] = act
 
         act = QAction('Domino', self)
         act.triggered.connect(partial(self.import_staging, 'domino',
@@ -457,19 +453,14 @@
                                       as_qual=True))
         actions['import_prana_qual'] = act
 
         act = QAction('DeltaMed', self)
         act.triggered.connect(partial(self.import_staging, 'deltamed',
                                       as_qual=True))
         actions['import_deltamed_qual'] = act
-        
-        act = QAction('Phillips', self)
-        act.triggered.connect(partial(self.import_staging, 'phillips',
-                                      as_qual=True))
-        actions['import_phillips_qual'] = act
 
         act = QAction('Wonambi', self)
         act.triggered.connect(partial(self.import_events, 'wonambi'))
         actions['import_events_wonambi'] = act
 
         act = QAction('RemLogic', self)
         act.triggered.connect(partial(self.import_events, 'remlogic'))
@@ -1221,23 +1212,20 @@
         if self.parent.info.dataset is None:
             msg = 'No dataset loaded'
             self.parent.statusBar().showMessage(msg)
             lg.info(msg)
             return
 
         record_start = self.parent.info.dataset.header['start_time']
-        file_filter = 'Text File (*.txt)'
-        if source == 'phillips':
-            file_filter = 'CSV File (*.csv)'
 
         if test_filename is None:
             filename, _ = QFileDialog.getOpenFileName(self,
                                                       'Load staging file',
                                                       None,
-                                                      file_filter)
+                                                      'Text File (*.txt)')
         else:
             filename = test_filename
 
         if filename == '':
             return
 
         if test_rater is None:
```

### Comparing `wonambi-7.12/wonambi/widgets/overview.py` & `wonambi-7.6/wonambi/widgets/overview.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/settings.py` & `wonambi-7.6/wonambi/widgets/settings.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/spectrum.py` & `wonambi-7.6/wonambi/widgets/spectrum.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/traces.py` & `wonambi-7.6/wonambi/widgets/traces.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/utils.py` & `wonambi-7.6/wonambi/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi/widgets/video.py` & `wonambi-7.6/wonambi/widgets/video.py`

 * *Files identical despite different names*

### Comparing `wonambi-7.12/wonambi.egg-info/PKG-INFO` & `wonambi-7.6/wonambi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: wonambi
-Version: 7.12
+Version: 7.6
 Summary: Tools for EEG, ECoG, iEEG, especially for sleep
 Home-page: https://github.com/wonambi-python/wonambi
 Author: Gio Piantoni / Jordan O'Byrne
 Author-email: wonambi@gpiantoni.com
 License: GPLv3
 Keywords: neuroscience analysis sleep EEG ECoG
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Visualization
@@ -110,7 +111,9 @@
 
 .. image:: https://codecov.io/gh/wonambi-python/wonambi/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/wonambi-python/wonambi
 
 License
 -------
 The project is licensed under the 3-clause BSD license.
+
+
```

