# Comparing `tmp/mly_pipeline-0.5.4.1.tar.gz` & `tmp/mly_pipeline-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly_pipeline-0.5.4.1.tar", last modified: Thu Jul  6 14:15:30 2023, max compression
+gzip compressed data, was "mly_pipeline-0.5.5.tar", last modified: Mon Jul 10 15:13:23 2023, max compression
```

## Comparing `mly_pipeline-0.5.4.1.tar` & `mly_pipeline-0.5.5.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 14:15:30.660858 mly_pipeline-0.5.4.1/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      123 2023-06-27 09:51:40.000000 mly_pipeline-0.5.4.1/.gitignore
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-16 13:29:19.000000 mly_pipeline-0.5.4.1/.gitlab-ci.yml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-16 13:28:31.000000 mly_pipeline-0.5.4.1/LICENSE
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6683 2023-07-06 14:15:30.659859 mly_pipeline-0.5.4.1/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.5.4.1/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 14:15:29.564849 mly_pipeline-0.5.4.1/docs/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.5.4.1/docs/Makefile
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 14:15:29.487848 mly_pipeline-0.5.4.1/docs/build/
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 14:15:29.874851 mly_pipeline-0.5.4.1/docs/build/doctrees/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.5.4.1/docs/build/doctrees/HowToUse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.5.4.1/docs/build/doctrees/Installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2074627 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4.1/docs/build/doctrees/environment.pickle
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/build/doctrees/gettingstarted.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/build/doctrees/howtouse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6321 2023-05-18 11:06:49.000000 mly_pipeline-0.5.4.1/docs/build/doctrees/index.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9106 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4.1/docs/build/doctrees/installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    61091 2023-06-13 10:37:26.000000 mly_pipeline-0.5.4.1/docs/build/doctrees/runningasearch.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    74931 2023-05-18 14:02:37.000000 mly_pipeline-0.5.4.1/docs/build/doctrees/settingupasearch.doctree
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 14:15:30.036853 mly_pipeline-0.5.4.1/docs/build/html/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/build/html/Getting Started.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/build/html/GettingStarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4.1/docs/build/html/How to use.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/build/html/HowToUse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/build/html/Installation.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 14:15:30.121853 mly_pipeline-0.5.4.1/docs/build/html/_modules/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.5.4.1/docs/build/html/_modules/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4.1/docs/build/html/_modules/io.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 14:15:30.128854 mly_pipeline-0.5.4.1/docs/build/html/_sources/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4.1/docs/build/html/_sources/How to use.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/build/html/_sources/HowToUse.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4.1/docs/build/html/_sources/Installation.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/build/html/_sources/index.rst.txt
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 14:15:30.583858 mly_pipeline-0.5.4.1/docs/build/html/_static/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/ajax-loader.gif
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/alabaster.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    15228 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/basic.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9827 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/bizstyle.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1141 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/bizstyle.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/css3-mediaqueries.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/css3-mediaqueries_src.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/custom.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8171 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/doctools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      421 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/documentation_options.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/jquery-3.2.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/jquery.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/language_data.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/pygments.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17088 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/searchtools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/underscore-1.3.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/underscore.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.5.4.1/docs/build/html/_static/websupport.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3127 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4.1/docs/build/html/genindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/build/html/gettingstarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/build/html/howtouse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8175 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4.1/docs/build/html/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8623 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4.1/docs/build/html/installation.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1577 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4.1/docs/build/html/objects.inv
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.5.4.1/docs/build/html/py-modindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27464 2023-06-13 10:37:27.000000 mly_pipeline-0.5.4.1/docs/build/html/runningasearch.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3430 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4.1/docs/build/html/search.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    21370 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4.1/docs/build/html/searchindex.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27034 2023-05-18 14:02:37.000000 mly_pipeline-0.5.4.1/docs/build/html/settingupasearch.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 14:15:30.613858 mly_pipeline-0.5.4.1/docs/source/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5973 2023-05-18 14:08:16.000000 mly_pipeline-0.5.4.1/docs/source/conf.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4.1/docs/source/index.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2134 2023-06-13 10:58:33.000000 mly_pipeline-0.5.4.1/docs/source/installation.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14941 2023-05-30 13:25:04.000000 mly_pipeline-0.5.4.1/docs/source/runningasearch.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13940 2023-05-18 14:02:00.000000 mly_pipeline-0.5.4.1/docs/source/settingupasearch.rst
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 14:15:30.650858 mly_pipeline-0.5.4.1/mly_pipeline/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-0.5.4.1/mly_pipeline/__init__.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    28059 2023-06-28 14:28:41.000000 mly_pipeline-0.5.4.1/mly_pipeline/continuous_FAR.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17355 2023-06-27 11:02:28.000000 mly_pipeline-0.5.4.1/mly_pipeline/continuous_FAR_test.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    31496 2023-07-06 13:46:36.000000 mly_pipeline-0.5.4.1/mly_pipeline/initialization.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13344 2023-05-16 13:28:31.000000 mly_pipeline-0.5.4.1/mly_pipeline/make_eff_estimation.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    33496 2023-06-30 13:55:36.000000 mly_pipeline-0.5.4.1/mly_pipeline/manager.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6330 2023-07-05 16:37:33.000000 mly_pipeline-0.5.4.1/mly_pipeline/mly_to_grace.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    21032 2023-06-15 11:06:35.000000 mly_pipeline-0.5.4.1/mly_pipeline/offline_search.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    16729 2023-07-06 09:18:53.000000 mly_pipeline-0.5.4.1/mly_pipeline/search.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    49569 2023-07-06 13:45:58.000000 mly_pipeline-0.5.4.1/mly_pipeline/search_functions.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 14:15:30.658859 mly_pipeline-0.5.4.1/mly_pipeline/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.5.4.1/mly_pipeline/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-07-04 13:10:16.000000 mly_pipeline-0.5.4.1/mly_pipeline/tests/test_skymap_generation.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 14:15:30.656859 mly_pipeline-0.5.4.1/mly_pipeline.egg-info/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6683 2023-07-06 14:15:29.000000 mly_pipeline-0.5.4.1/mly_pipeline.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2630 2023-07-06 14:15:29.000000 mly_pipeline-0.5.4.1/mly_pipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-06 14:15:29.000000 mly_pipeline-0.5.4.1/mly_pipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      194 2023-07-06 14:15:29.000000 mly_pipeline-0.5.4.1/mly_pipeline.egg-info/entry_points.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-06 14:15:29.000000 mly_pipeline-0.5.4.1/mly_pipeline.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-07-06 14:15:29.000000 mly_pipeline-0.5.4.1/mly_pipeline.egg-info/top_level.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      764 2023-07-06 13:48:12.000000 mly_pipeline-0.5.4.1/pyproject.toml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-07-06 14:15:30.660858 mly_pipeline-0.5.4.1/setup.cfg
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.521055 mly_pipeline-0.5.5/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      123 2023-06-27 09:51:40.000000 mly_pipeline-0.5.5/.gitignore
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-16 13:29:19.000000 mly_pipeline-0.5.5/.gitlab-ci.yml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-16 13:28:31.000000 mly_pipeline-0.5.5/LICENSE
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-10 15:13:23.521055 mly_pipeline-0.5.5/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.5.5/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.047051 mly_pipeline-0.5.5/docs/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.5.5/docs/Makefile
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.021050 mly_pipeline-0.5.5/docs/build/
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.196052 mly_pipeline-0.5.5/docs/build/doctrees/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.5.5/docs/build/doctrees/HowToUse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.5.5/docs/build/doctrees/Installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2074627 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/doctrees/environment.pickle
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/doctrees/gettingstarted.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/doctrees/howtouse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6321 2023-05-18 11:06:49.000000 mly_pipeline-0.5.5/docs/build/doctrees/index.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9106 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/doctrees/installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    61091 2023-06-13 10:37:26.000000 mly_pipeline-0.5.5/docs/build/doctrees/runningasearch.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    74931 2023-05-18 14:02:37.000000 mly_pipeline-0.5.5/docs/build/doctrees/settingupasearch.doctree
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.312053 mly_pipeline-0.5.5/docs/build/html/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/Getting Started.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/GettingStarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/How to use.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/HowToUse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/Installation.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.342053 mly_pipeline-0.5.5/docs/build/html/_modules/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.5.5/docs/build/html/_modules/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_modules/io.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.352053 mly_pipeline-0.5.5/docs/build/html/_sources/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_sources/How to use.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/_sources/HowToUse.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_sources/Installation.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/_sources/index.rst.txt
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.430054 mly_pipeline-0.5.5/docs/build/html/_static/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_static/ajax-loader.gif
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_static/alabaster.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    15228 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/_static/basic.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9827 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/_static/bizstyle.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1141 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/_static/bizstyle.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_static/css3-mediaqueries.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/_static/css3-mediaqueries_src.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_static/custom.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8171 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/_static/doctools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      421 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/_static/documentation_options.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.5.5/docs/build/html/_static/jquery-3.2.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/_static/jquery.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/_static/language_data.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/_static/pygments.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17088 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/_static/searchtools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.5.5/docs/build/html/_static/underscore-1.3.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/_static/underscore.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.5.5/docs/build/html/_static/websupport.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3127 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/genindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/gettingstarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/build/html/howtouse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8175 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8623 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/installation.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1577 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/objects.inv
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.5.5/docs/build/html/py-modindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27464 2023-06-13 10:37:27.000000 mly_pipeline-0.5.5/docs/build/html/runningasearch.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3430 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/search.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    21370 2023-06-13 10:58:46.000000 mly_pipeline-0.5.5/docs/build/html/searchindex.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27034 2023-05-18 14:02:37.000000 mly_pipeline-0.5.5/docs/build/html/settingupasearch.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.482055 mly_pipeline-0.5.5/docs/source/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5973 2023-05-18 14:08:16.000000 mly_pipeline-0.5.5/docs/source/conf.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.5/docs/source/index.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2134 2023-06-13 10:58:33.000000 mly_pipeline-0.5.5/docs/source/installation.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14941 2023-05-30 13:25:04.000000 mly_pipeline-0.5.5/docs/source/runningasearch.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13940 2023-05-18 14:02:00.000000 mly_pipeline-0.5.5/docs/source/settingupasearch.rst
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.512055 mly_pipeline-0.5.5/mly_pipeline/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-0.5.5/mly_pipeline/__init__.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    28059 2023-07-10 09:53:54.000000 mly_pipeline-0.5.5/mly_pipeline/continuous_FAR.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17355 2023-06-27 11:02:28.000000 mly_pipeline-0.5.5/mly_pipeline/continuous_FAR_test.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    30861 2023-07-10 11:35:08.000000 mly_pipeline-0.5.5/mly_pipeline/initialization.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13344 2023-05-16 13:28:31.000000 mly_pipeline-0.5.5/mly_pipeline/make_eff_estimation.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    33484 2023-07-07 10:13:32.000000 mly_pipeline-0.5.5/mly_pipeline/manager.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5596 2023-07-10 10:12:27.000000 mly_pipeline-0.5.5/mly_pipeline/mly_to_grace.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    18914 2023-07-10 10:17:57.000000 mly_pipeline-0.5.5/mly_pipeline/offline_search.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17379 2023-07-10 09:45:05.000000 mly_pipeline-0.5.5/mly_pipeline/search.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    49627 2023-07-10 11:35:33.000000 mly_pipeline-0.5.5/mly_pipeline/search_functions.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.519055 mly_pipeline-0.5.5/mly_pipeline/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.5.5/mly_pipeline/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-07-04 13:10:16.000000 mly_pipeline-0.5.5/mly_pipeline/tests/test_skymap_generation.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-10 15:13:23.517055 mly_pipeline-0.5.5/mly_pipeline.egg-info/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-10 15:13:22.000000 mly_pipeline-0.5.5/mly_pipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2630 2023-07-10 15:13:23.000000 mly_pipeline-0.5.5/mly_pipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-10 15:13:22.000000 mly_pipeline-0.5.5/mly_pipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      194 2023-07-10 15:13:22.000000 mly_pipeline-0.5.5/mly_pipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-10 15:13:22.000000 mly_pipeline-0.5.5/mly_pipeline.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-07-10 15:13:22.000000 mly_pipeline-0.5.5/mly_pipeline.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      762 2023-07-10 15:12:37.000000 mly_pipeline-0.5.5/pyproject.toml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-07-10 15:13:23.521055 mly_pipeline-0.5.5/setup.cfg
```

### Comparing `mly_pipeline-0.5.4.1/.gitlab-ci.yml` & `mly_pipeline-0.5.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/LICENSE` & `mly_pipeline-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/PKG-INFO` & `mly_pipeline-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly_pipeline
-Version: 0.5.4.1
+Version: 0.5.5
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.5.4.1/README.md` & `mly_pipeline-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/Makefile` & `mly_pipeline-0.5.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/doctrees/HowToUse.doctree` & `mly_pipeline-0.5.5/docs/build/doctrees/HowToUse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/doctrees/Installation.doctree` & `mly_pipeline-0.5.5/docs/build/doctrees/Installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/doctrees/environment.pickle` & `mly_pipeline-0.5.5/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/doctrees/gettingstarted.doctree` & `mly_pipeline-0.5.5/docs/build/doctrees/gettingstarted.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/doctrees/howtouse.doctree` & `mly_pipeline-0.5.5/docs/build/doctrees/howtouse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/doctrees/index.doctree` & `mly_pipeline-0.5.5/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/doctrees/installation.doctree` & `mly_pipeline-0.5.5/docs/build/doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/doctrees/runningasearch.doctree` & `mly_pipeline-0.5.5/docs/build/doctrees/runningasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/doctrees/settingupasearch.doctree` & `mly_pipeline-0.5.5/docs/build/doctrees/settingupasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/Getting Started.html` & `mly_pipeline-0.5.5/docs/build/html/Getting Started.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/GettingStarted.html` & `mly_pipeline-0.5.5/docs/build/html/GettingStarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/How to use.html` & `mly_pipeline-0.5.5/docs/build/html/How to use.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/HowToUse.html` & `mly_pipeline-0.5.5/docs/build/html/HowToUse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/Installation.html` & `mly_pipeline-0.5.5/docs/build/html/Installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_modules/index.html` & `mly_pipeline-0.5.5/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_modules/io.html` & `mly_pipeline-0.5.5/docs/build/html/_modules/io.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_sources/How to use.rst.txt` & `mly_pipeline-0.5.5/docs/build/html/_sources/How to use.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_sources/HowToUse.rst.txt` & `mly_pipeline-0.5.5/docs/build/html/_sources/HowToUse.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_sources/Installation.rst.txt` & `mly_pipeline-0.5.5/docs/build/html/_sources/Installation.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_sources/index.rst.txt` & `mly_pipeline-0.5.5/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/ajax-loader.gif` & `mly_pipeline-0.5.5/docs/build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/alabaster.css` & `mly_pipeline-0.5.5/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/basic.css` & `mly_pipeline-0.5.5/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/bizstyle.css` & `mly_pipeline-0.5.5/docs/build/html/_static/bizstyle.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/bizstyle.js` & `mly_pipeline-0.5.5/docs/build/html/_static/bizstyle.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/css3-mediaqueries.js` & `mly_pipeline-0.5.5/docs/build/html/_static/css3-mediaqueries.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/css3-mediaqueries_src.js` & `mly_pipeline-0.5.5/docs/build/html/_static/css3-mediaqueries_src.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/doctools.js` & `mly_pipeline-0.5.5/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/jquery-3.2.1.js` & `mly_pipeline-0.5.5/docs/build/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/jquery.js` & `mly_pipeline-0.5.5/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/language_data.js` & `mly_pipeline-0.5.5/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/pygments.css` & `mly_pipeline-0.5.5/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/searchtools.js` & `mly_pipeline-0.5.5/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/underscore-1.3.1.js` & `mly_pipeline-0.5.5/docs/build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/underscore.js` & `mly_pipeline-0.5.5/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/_static/websupport.js` & `mly_pipeline-0.5.5/docs/build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/genindex.html` & `mly_pipeline-0.5.5/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/gettingstarted.html` & `mly_pipeline-0.5.5/docs/build/html/gettingstarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/howtouse.html` & `mly_pipeline-0.5.5/docs/build/html/howtouse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/index.html` & `mly_pipeline-0.5.5/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/installation.html` & `mly_pipeline-0.5.5/docs/build/html/installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/objects.inv` & `mly_pipeline-0.5.5/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/py-modindex.html` & `mly_pipeline-0.5.5/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/runningasearch.html` & `mly_pipeline-0.5.5/docs/build/html/runningasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/search.html` & `mly_pipeline-0.5.5/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/searchindex.js` & `mly_pipeline-0.5.5/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/build/html/settingupasearch.html` & `mly_pipeline-0.5.5/docs/build/html/settingupasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/source/conf.py` & `mly_pipeline-0.5.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/source/index.rst` & `mly_pipeline-0.5.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/source/installation.rst` & `mly_pipeline-0.5.5/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/source/runningasearch.rst` & `mly_pipeline-0.5.5/docs/source/runningasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/docs/source/settingupasearch.rst` & `mly_pipeline-0.5.5/docs/source/settingupasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/mly_pipeline/__init__.py` & `mly_pipeline-0.5.5/mly_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/mly_pipeline/continuous_FAR.py` & `mly_pipeline-0.5.5/mly_pipeline/continuous_FAR.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/mly_pipeline/continuous_FAR_test.py` & `mly_pipeline-0.5.5/mly_pipeline/continuous_FAR_test.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/mly_pipeline/initialization.py` & `mly_pipeline-0.5.5/mly_pipeline/initialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 def _parser():
 
     arguments = ["search_mode"
                  ,"path"
                  ,"output_directory"
                  ,"trigger_directory"
-                 ,"triggerplot_directory"
                  ,"masterDirectory"
                  ,"bufferDirectory"
                  ,"falseAlarmRates"
                  ,"efficiencies"
                  ,"detectors"
                  ,"reset"
                  ,"far"]
@@ -42,21 +41,14 @@
     parser.add_argument('-t', '--trigger_directory', type=str
                         , default = 'trigger_directory'
                         , help = "The name of the"
                         +" directory to be used by mlyPipeline for the storage"
                         +" of the triggers."
                         , required = False)
 
-    parser.add_argument('-tp', '--triggerplot_directory', type=str
-                        , default = 'triggerplot_directory'
-                        , help = "The name of the"
-                        +" directory to be used by mlyPipeline for the storage"
-                        +" of the plots from the triggers."
-                        , required = False)
-
     parser.add_argument('-m', '--masterDirectory', type=str
                         , default = 'masterDirectory'
                         , help = "The name of the"
                         +" directory to be used by mlyPipeline for the storage"
                         +" of the plots from the triggers."
                         , required = False)
 
@@ -442,15 +434,14 @@
 
     # Mode that creates some presets if used
     search_mode  = kwargs["search_mode"],
     # # # Directory organisation 
     
     output_directory = kwargs["output_directory"],
     trigger_directory = kwargs["trigger_directory"],
-    triggerplot_directory = kwargs["triggerplot_directory"],
     masterDirectory = kwargs["masterDirectory"],
     bufferDirectory = kwargs["bufferDirectory"],
     falseAlarmRates = kwargs["falseAlarmRates"],
     efficiencies = kwargs["efficiencies"],
     log = "log",
     
         
@@ -475,15 +466,15 @@
     # Time duration of segments to analyse (analysis window).
     duration=1,         
         
     # Number of segments to analyse, keep to 1 for real-time analysis.
     size=1,
     
     # Detectors used for this search
-    detectors = 'HLV',
+    detectors = kwargs['detectors'],
     
     # Frame file prefixes to use
     frames_directory= frames_dict[kwargs['search_mode']],
     
     # The channels to use, INJ is the MDC and NOISE is O3-replay
     channels = channels_dict[kwargs['search_mode']],
 
@@ -499,17 +490,14 @@
     # the time it takes to process one instance of data.)
 
     parallel_scripts=4,
 
     # Number of seconds to wait between each read attempt.
     wait=0.5,
         
-    # Number of times to attempt to read data, before giving up.
-    timeout=20,
-        
     # Number of seconds required for PSD calculation.
     required_buffer=16,  
         
     # Number of seconds before current GPS time to begin search.
     start_lag=92,
         
     # If search time is left behind by that amount of seconds it skips ahead.
@@ -595,15 +583,14 @@
     
 
     )
 
 
     os.system("mkdir " + configuration['path'] +"/"+ configuration['output_directory'])
     os.system("mkdir " + configuration['path'] +"/"+ configuration['trigger_directory'])
-    os.system("mkdir " + configuration['path'] +"/"+ configuration['triggerplot_directory'])
     os.system("mkdir " + configuration['path'] +"/"+ configuration['log'])
 
     if not ("OFFLINE" in kwargs['search_mode'] and not kwargs['far']):
 
         os.system("mkdir " + configuration['path'] +"/"+ configuration['masterDirectory'])
         os.system("mkdir " + configuration['path'] +"/"+ configuration['masterDirectory'] 
                 +"/temp")
```

### Comparing `mly_pipeline-0.5.4.1/mly_pipeline/make_eff_estimation.py` & `mly_pipeline-0.5.5/mly_pipeline/make_eff_estimation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/mly_pipeline/manager.py` & `mly_pipeline-0.5.5/mly_pipeline/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -777,15 +777,15 @@
             logger.info(f"New FARfile interpolations saced")
 
             if (farfile_to_delete is not None 
                     and farfile_to_delete!="FARfile_"+str(farfile_size)+".pkl"):
                 os.system("rm "+config['falseAlarmRates']+"/FARfile/"+farfile_to_delete)
             
         # Overwriting config farfile when enough files
-        if len(hourly_files)!=0 and (farfile_size) >= 1*365*24*3600 and (config['path']+"/"+config['falseAlarmRates'] not in config['farfile']):
+        if len(hourly_files)!=0 and (farfile_size) >= 1*365*24*3600 and (config['farfile'] != config['falseAlarmRates']+"/FARfile"):
 
             with open('config.json') as json_file:
                 _config = json.load(json_file)
                 _config['farfile'] = config['falseAlarmRates']+"/FARfile"
             with open("config.json", "w") as config_json:
                 json.dump(_config, config_json,indent=4)
                 config_json.close()
```

### Comparing `mly_pipeline-0.5.4.1/mly_pipeline/mly_to_grace.py` & `mly_pipeline-0.5.5/mly_pipeline/mly_to_grace.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,29 +5,27 @@
 # Scipy and numpy env parameters that limit the threads
 os.environ["MKL_NUM_THREADS"] = "1"
 os.environ["NUMEXPR_NUM_THREADS"] = "1"
 os.environ["OMP_NUM_THREADS"] = "1"
 
 import pickle
 import argparse
-import ast
 import numpy as np
+import matplotlib.pyplot as plt
 
-from mly.datatools import DataPod
 from lal import gpstime
 from ligo.gracedb.rest import GraceDb
 
 # # # Managing arguments
 # 
 # List of arguments to pass:
 arguments = [
     "trigger_destination",
     "skymap_directory",
     "triggerfile",
-    "triggerplot_directory",
     "skymap",
 ]
 
 #Construct argument parser
 parser = argparse.ArgumentParser()
 [parser.add_argument(f"--{argument}") for argument in arguments]
 
@@ -128,91 +126,85 @@
 with open(f"{triggerfile[:-5]}_buffer.pkl", 'rb') as obj:
     buffer = pickle.load(obj)
 if kwargs['skymap']==None:
     kwargs['skymap']=0
 else:
     kwargs['skymap'] = int(kwargs['skymap'])
 
-# if isinstance(kwargs['skymap'],str):
-#     if kwargs['skymap'].lower=='true':
-#         kwargs['skymap']==True
-#     elif kwargs['skymap'].lower=='false':
-#         kwargs['skymap']==False
-#     else:
-#         print(kwargs['skymap'])
+gpsstring=triggerfile.split('_')[-2]
+detectors=triggerfile.split('.')[-2].split('_')[-1]
+
+# Renaming the already created tempEventDirectory to one with the gracedb id in the name
+
+temp_eventDirectory = 'tempEventDirectory_'+gpsstring
+# Creating a directory for each event using the graceid from the event creation.
+# Not always works.
+try:
+    eventDirectory = graceEventDict['graceid']+'-'+gpsstring+'-'+detectors
+except Exception as e:
+    print(e)
+    eventDirectory = 'NoGraceID'+'-'+gpsstring+'-'+detectors
+
+# Renaming the event directory
+os.rename(  f"{config['trigger_directory']}/{temp_eventDirectory}"
+          , f"{config['trigger_directory']}/{eventDirectory}")
+
+
+    
+
+
+# Creating the strain plot
+thepod.plot(type_="strain")
+plt.savefig(f"{config['trigger_directory']}/{eventDirectory}/T_{gpsstring}_{detectors}_strain.png")
 
+# Creating the correlation plot
+thepod.plot(type_="correlation")
+plt.savefig(
+    f"{config['trigger_directory']}/{eventDirectory}/T_{gpsstring}_{detectors}_correlation.png")
 
+thepod.plot('tf_map')
+plt.savefig(
+    f"{config['trigger_directory']}/{eventDirectory}/T_{gpsstring}_{detectors}_tfmap.png")
+
+# And if skymap is created we save the plot as png too.
+if kwargs['skymap']:
+    buffer.plot(type_="skymap")
+    plt.savefig(f"{config['trigger_directory']}/{eventDirectory}/T_{gpsstring}_{detectors}_skymap.png")
 
-# # Probably this could go below skymap generation?    
-if kwargs['triggerplot_directory'] != 'None':
-    
-    # Creating a directory for each event using the graceid from the event creation.
-    # Not always works.
-    try:
-        eventDirectory = graceEventDict['graceid']+'-'+triggerfile.split('_')[-2]+'-'+triggerfile.split('_')[-1].split('.')[0]
-    except Exception as e:
-        print(e)
-        eventDirectory = 'NoGraceID'+'-'+triggerfile.split('_')[-2]+'-'+triggerfile.split('_')[-1].split('.')[0]
-    
-    # Making an event directory
-    os.mkdir(f"{kwargs['triggerplot_directory']}/{eventDirectory}")
-    print('triggerplot_checkpoint')
 
 
 if kwargs['skymap']:
 
     from mly.null_energy_map import *
     from ligo.skymap.io import fits
 
     # Create skymap plugin:
     sky_map_plugin = createSkymapPlugin(
         config["nside"], config["fs"], config["duration"])
 
     # Generate Skymap
     buffer.addPlugIn(sky_map_plugin)
     
-    skymap_path = f"{kwargs['triggerplot_directory']}/{eventDirectory}/T_{triggerfile.split('_')[-2]}_{triggerfile.split('_')[-1][:-5]}_skymap.fits"
+    skymap_path = f"{config['trigger_directory']}/{eventDirectory}/T_{gpsstring}_{detectors}_skymap.fits"
     
     skymap_fits = buffer.skymap
 
     with open(skymap_path, "w") as f:
         fits.write_sky_map(f.name, skymap_fits, nest=False)
     
     # Upload skymap to grace db:
     if kwargs['trigger_destination'] != 'None':
 
         client.writeLog(graceEventDict['graceid'], 'skymap',  filename=skymap_path, tg_name='sky_loc')
     print('skymap checkpoint')
 
-if kwargs['triggerplot_directory'] != 'None':
 
-    import matplotlib.pyplot as plt
-    
-    gpsstring=triggerfile.split('_')[1]
-    detectors=triggerfile.split('_')[-1][-5]
-    
-    # Creating the strain plot
-    thepod.plot(type_="strain")
-    plt.savefig(f"{kwargs['triggerplot_directory']}/{eventDirectory}/T_{triggerfile.split('_')[-2]}_{triggerfile.split('_')[-1][:-5]}_strain.png")
-    
-    # Creating the correlation plot
-    thepod.plot(type_="correlation")
-    plt.savefig(
-        f"{kwargs['triggerplot_directory']}/{eventDirectory}/T_{triggerfile.split('_')[-2]}_{triggerfile.split('_')[-1][:-5]}_correlation.png")
 
-    thepod.plot('tf_map')
-    plt.savefig(
-        f"{kwargs['triggerplot_directory']}/{eventDirectory}/T_{triggerfile.split('_')[-2]}_{triggerfile.split('_')[-1][:-5]}_tfmap.png")
 
-    # And if skymap is created we save the plot as png too.
-    if kwargs['skymap']==True:
-        buffer.plot(type_="skymap")
-        plt.savefig(f"{kwargs['triggerplot_directory']}/{eventDirectory}/T_{triggerfile.split('_')[-2]}_{triggerfile.split('_')[-1][:-5]}_skymap.png")
 
-    print('plots checkpoint')
 raise SystemExit()
 
 # if __name__ == "__main__":
 
 
 #     main(**kwargs)
```

### Comparing `mly_pipeline-0.5.4.1/mly_pipeline/offline_search.py` & `mly_pipeline-0.5.5/mly_pipeline/offline_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,18 +69,14 @@
 
     trigger_directory: str (path, optional)
         The path of the directory where the search will save the output of the model
         for each instance that was above the threshold value. If not specified
         it doesn't save anything. It is important to have this directory specified if
         you want to send triggers to GraceDB (using mly_to_grace.py).
 
-    triggerplot_directory: str (path, optional)
-        The path of the file where the search will save a plot of the timeseries data
-        for each instance that was above the threshold value and issued a trigger.
-
     trigger_destination: {'test, 'playground', 'dev1', None}
         The GraceDB domain for the triggers to be uploaded. Each option represent
         a corresponding url. If equals to None, it will not issue an GraceDB event.
         
     splitter: list
         A way to split the search into different parallel jobs. The list must have
         two parameters. The first is the amount of scripts this search is split into.
@@ -331,110 +327,80 @@
             
             threshold = far(config['farfile']+"/"+"FARfile_interpolation_inverse.pkl"
                                 ,config['far_config']['threshold'], inverse = True)
             # If result us above threshold, do all even relate actions 
 
             # Perform time- and frequency-domain parameter estimation.
             # It adds parameter estimation to events.
-            pe_t0 = time.time()
+
             mly_output = runTimeFrequencyParameterEstimation(thepod,  mly_output)
 
             if mly_output["scores"]["combined"] >= threshold:
                 
-                print("the output: ",mly_output)
+                mly_output['trigger']=True
+                
+                # Making the directory of the trigger
+                eventDirectory = "T_"+str(mly_output['gpstime'])
+
+                if os.path.exists(f"{config['trigger_directory']}/{eventDirectory}"):
+                    shutil.rmtree(f"{config['trigger_directory']}/{eventDirectory}")
+                
+                os.mkdir(f"{config['trigger_directory']}/{eventDirectory}")
+
+
                 # Saving trigger into the trigger_directory
-                with open(f"{config['trigger_directory']}/T_{mly_output['gpstime']}_{detectors}.json", "w") as mly_json:
-                    json.dump(mly_output, mly_json)
+                with open(f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_{detectors}.json", "w") as mly_json:
+                    json.dump(mly_output, mly_json,indent=4)
                     mly_json.close()
 
                 # Saving trigger DataPod into the trigger_directory
-                with open(f"{config['trigger_directory']}/T_{mly_output['gpstime']}_{detectors}.pkl", 'wb') as mly_pkl:
+                with open(f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_{detectors}.pkl", 'wb') as mly_pkl:
                     pickle.dump(thepod, mly_pkl, 4)
                     
                 # Saving trigger background DataPod into the trigger_directory
-                with open(f"{config['trigger_directory']}/T_{mly_output['gpstime']}_{detectors}_buffer.pkl", 'wb') as mly_pkl:
+                with open(f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_{detectors}_buffer.pkl", 'wb') as mly_pkl:
                     pickle.dump(buffer_pod, mly_pkl, 4)
-                                    
-                # Saving output to output directory. Notice that the name starts with T_ for triggers
-                # if config["output_directory"] != None:
-                #     with open(f"{config['output_directory']}/T_{mly_output['gpstime']}_{detectors}.json", "w") as mly_json:
-                #         json.dump(mly_output, mly_json)
-                #         mly_json.close()
-                mly_output['trigger']=True
-                mly_output_list.append(mly_output)
-
 
-
-                eventDirectory = "T_"+str(mly_output['gpstime'])
-
-                if os.path.exists(f"{config['triggerplot_directory']}/{eventDirectory}"):
-                    shutil.rmtree(f"{config['triggerplot_directory']}/{eventDirectory}")
-
-                os.mkdir(f"{config['triggerplot_directory']}/{eventDirectory}")
+                # Creating the strain plot
+                thepod.plot(type_="strain")
+                plt.savefig(f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_strain.png")
+                plt.clf()
+                # Creating the correlation plot
+                thepod.plot(type_="correlation")
+                plt.savefig(
+                    f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_correlation.png")
+                plt.clf()
 
 
                 if config['skymap']:
 
                     # Create skymap plugin:
                     sky_map_plugin = createSkymapPlugin(
                         config["nside"], config["fs"], config["duration"])
 
                     # Generate Skymap
                     buffer_pod.addPlugIn(sky_map_plugin)
                     
-                    skymap_path = f"{config['triggerplot_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_skymap.fits"
+                    skymap_path = f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_skymap.fits"
                     
                     skymap_fits = buffer_pod.skymap
 
                     with open(skymap_path, "w") as f:
                         fits.write_sky_map(f.name, skymap_fits, nest=False)
-
-                if config['triggerplot_directory'] != 'None':
-
-                    # Saving trigger into the triggerplot_directory
-                    with open(f"{config['triggerplot_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_{detectors}.json", "w") as mly_json:
-                        json.dump(mly_output, mly_json,indent=4)
-                        mly_json.close()
-
-                    # Saving trigger DataPod into the trigger_directory
-                    with open(f"{config['triggerplot_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_{detectors}.pkl", 'wb') as mly_pkl:
-                        pickle.dump(thepod, mly_pkl, 4)
-                        
-                    # Saving trigger background DataPod into the trigger_directory
-                    with open(f"{config['triggerplot_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_{detectors}_buffer.pkl", 'wb') as mly_pkl:
-                        pickle.dump(buffer_pod, mly_pkl, 4)
                         
-                    # Creating the strain plot
-                    thepod.plot(type_="strain")
-                    plt.savefig(f"{config['triggerplot_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_strain.png")
-                    plt.clf()
-                    # Creating the correlation plot
-                    thepod.plot(type_="correlation")
-                    plt.savefig(
-                        f"{config['triggerplot_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_correlation.png")
-                    plt.clf()
-
                     # And if skymap is created we save the plot as png too.
-                    if config['skymap']==True:
-                        buffer_pod.plot(type_="skymap")
-                        plt.savefig(f"{config['triggerplot_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_skymap.png")
-                        plt.clf()
-
-
+                    buffer_pod.plot(type_="skymap")
+                    plt.savefig(f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_skymap.png")
+                                            
 
             else:
 
-                # # Saving output to output directory. Notice that the name starts with T_ for triggers
-                # if config["output_directory"] != None:
-                #     with open(f"{config['output_directory']}/N_{mly_output['gpstime']}_{detectors}.json", "w") as mly_json:
-                #         json.dump(mly_output, mly_json)
-                #         mly_json.close()
                 mly_output['trigger']=False
-                mly_output_list.append(mly_output)
-            
+
+            mly_output_list.append(mly_output)
             sys.stdout.flush()
 
 
         tempFrame = pd.DataFrame(columns = ['gpstime','far','snr','ifos'
                                                     ,'coincidence','coherency'
                                                     ,'combined','central_time','duration','central_freq','bandwidth'
                                                     ,'trigger'])
```

### Comparing `mly_pipeline-0.5.4.1/mly_pipeline/search.py` & `mly_pipeline-0.5.5/mly_pipeline/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 from tensorflow.keras.models import load_model
 from tensorflow.config import threading
 
 threading.set_inter_op_parallelism_threads(1)
 threading.set_intra_op_parallelism_threads(1)
 
+
 from mly.datatools import DataPod
 from mly.validators import Validator
 from mly.null_energy_map import *
 
 from .search_functions import *
 
 
@@ -81,18 +82,14 @@
 
     trigger_directory: str (path, optional)
         The path of the directory where the search will save the output of the model
         for each instance that was above the threshold value. If not specified
         it doesn't save anything. It is important to have this directory specified if
         you want to send triggers to GraceDB (using mly_to_grace.py).
 
-    triggerplot_directory: str (path, optional)
-        The path of the file where the search will save a plot of the timeseries data
-        for each instance that was above the threshold value and issued a trigger.
-
     trigger_destination: {'test, 'playground', 'dev1', None}
         The GraceDB domain for the triggers to be uploaded. Each option represent
         a corresponding url. If equals to None, it will not issue an GraceDB event.
         
     splitter: list
         A way to split the search into different parallel jobs. The list must have
         two parameters. The first is the amount of scripts this search is split into.
@@ -188,14 +185,15 @@
     # GPS index counts how many gps times have been searched by this script alone:
     gps_index = 0 
     
     subconfig = config.copy()
     for key in ['detectors','fs','duration','restriction','prefixes','frames','channels','size']:
         subconfig.pop(key,None)
     
+    logger.debug(f"PROCESSES before main loop: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
     # # # Main Loop
     while (1):  
         
         # Get GPS time for this script to search
         gps_time, gps_index = calculateRequiredGPSTime(config, gps_index, initial_gps_time)
         logger.info(f"S{config['script_index']} - Requested / Difference from current GPS time: {gps_time} / {gpstime.gps_time_now() - gps_time}")
@@ -225,14 +223,16 @@
         buffer_pod = DataPod(
             np.array(buffers),
             detectors = config["detectors"], 
             fs = config["fs"], 
             gps = len(config["detectors"])*[float(gps_time)] 
         )
         
+        logger.debug(f"PROCESSES before validation: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+
 
         result, thepod = Validator.falseAlarmTest(
                                         models = models,
                                         duration = config["duration"],
                                         fs =  config["fs"],
                                         size = 1,
                                         detectors = config["detectors"],
@@ -242,14 +242,16 @@
                                         mapping = mapping,
                                         strides = None,
                                         plugins = ["correlation_30",'snr'],
                                         restriction = None,
                                         podreturn = True,
                                         **subconfig
                                     )
+        logger.debug(f"PROCESSES after validation: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+
         # Change format of detector name to include 1 (ex. H->H1)
         ifos = [f"{detector}1" for detector in config["detectors"]] 
         
         # Create mly_output dictionary, GraceDB event file basis
         
         interpolated_FAR_t0=time.time()
         interpolated_FAR_trials = 0
@@ -266,15 +268,15 @@
                                         ,result["total"][0], inverse = False)
                     break
                 except Exception as e:
                     interpolated_FAR_trials+=1
                     if interpolated_FAR_trials >= 3:
                         raise e
         logger.info(f"S{config['script_index']} - Loading interpolated_FAR time: ,{time.time()-interpolated_FAR_t0}, {interpolated_FAR_trials}")
-
+        logger.debug(f"PROCESSES after interpolation loading: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
         mly_output = {
             "gpstime": result["GPSH"][0],
             "far": interpolated_FAR,
             "ifos": ifos,
             "scores": {
                 "coincidence": result["scores1"][0],
@@ -316,66 +318,67 @@
 
         # Perform time- and frequency-domain parameter estimation.
         # It adds parameter estimation to events.
         pe_t0 = time.time()
         mly_output = runTimeFrequencyParameterEstimation(thepod,  mly_output)
         logger.info(f"PE time {time.time()- pe_t0}s")
         # If result us above threshold, do all even relate actions 
-        if mly_output["scores"]["combined"] >= threshold:
+                
+        logger.debug(f"PROCESSES after runTimeFrequencyParameterEstimation : {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
+        if mly_output["scores"]["combined"] >= threshold:
 
+            eventDirectory = 'tempEventDirectory_'+str(mly_output['gpstime'])
+            os.mkdir(f"{config['trigger_directory']}/{eventDirectory}")
 
             # Saving trigger into the trigger_directory
-            with open(f"{config['trigger_directory']}/T_{mly_output['gpstime']}_{detectors}.json", "w") as mly_json:
+            with open(f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_{detectors}.json", "w") as mly_json:
                 json.dump(mly_output, mly_json,indent=4)
                 mly_json.close()
-            
 
             # Saving trigger DataPod into the trigger_directory
-            with open(f"{config['trigger_directory']}/T_{mly_output['gpstime']}_{detectors}.pkl", 'wb') as mly_pkl:
+            with open(f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_{detectors}.pkl", 'wb') as mly_pkl:
                 pickle.dump(thepod, mly_pkl, 4)
                 
             # Saving trigger background DataPod into the trigger_directory
-            with open(f"{config['trigger_directory']}/T_{mly_output['gpstime']}_{detectors}_buffer.pkl", 'wb') as mly_pkl:
+            with open(f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_{detectors}_buffer.pkl", 'wb') as mly_pkl:
                 pickle.dump(buffer_pod, mly_pkl, 4)
                                 
             # Sending trigger to GraceDB 
             logger.debug(f"PROCESSES before run mlytograce: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']])}")
 
-            print(config['skymap'],type(config['skymap']))
-
-            with open( f"{config['trigger_directory']}/T_{mly_output['gpstime']}_{detectors}.out"
+            with open( f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_{detectors}.out"
             ,"wb") as out:
                 # Using subprocess to create mly_to grace function and run it independently.
                 p = subprocess.Popen(["python","-m","mly_pipeline.mly_to_grace", "--triggerfile"
-                                      ,f"{config['trigger_directory']}/T_{mly_output['gpstime']}_{detectors}.json"
+                                      ,f"{config['trigger_directory']}/{eventDirectory}/T_{mly_output['gpstime']}_{detectors}.json"
                                       ,"--trigger_destination", str(config['trigger_destination'])
-                                      ,"--triggerplot_directory",config['triggerplot_directory']
                                       ,"--skymap", str(int(config['skymap']))]
                                       #+" > "+f"{config['trigger_directory']}/T_{mly_output['gpstime']}_{detectors}.out &"
                                       ,stdout=out, stderr=out,shell=False)
             
             logger.info(f"S{config['script_index']} - TRIGGER follow-up script initialised for: "+str(mly_output['gpstime']))
                 
-
             # Saving output to output directory. Notice that the name starts with T_ for triggers
             if config["output_directory"] != None:
                 with open(f"{config['output_directory']}T_{mly_output['gpstime']}_{detectors}.json", "w") as mly_json:
                     json.dump(mly_output, mly_json,indent=4)
                     mly_json.close()
             
             logger.debug(f"PROCESSES after run mlytograce: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']])}")
 
         # If result is below threshold, we just save the output. Note that the name starts with N_
         elif config["output_directory"] != None:
             
             with open(f"{config['output_directory']}N_{mly_output['gpstime']}_{detectors}.json", "w") as mly_json:
                 json.dump(mly_output, mly_json, indent=4)
                 mly_json.close()
-                
+        
+        logger.debug(f"PROCESSES after saving: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+
         # If fileSystem parameter is provided, we save the second processed by the model in
         # the file system directory.
         if config["masterDirectory"]!=None:
             podToFileSystem(thepod, masterDirectory = config["masterDirectory"])
 
         # If bufferDirectory is provided, we save the buffer_pod in the 
         # buffer directory.
```

### Comparing `mly_pipeline-0.5.4.1/mly_pipeline/search_functions.py` & `mly_pipeline-0.5.5/mly_pipeline/search_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 import json, pickle, sys, time, os, argparse
 
+# Scipy and numpy env parameters that limit the threads
+os.environ["MKL_NUM_THREADS"] = "1"
+os.environ["NUMEXPR_NUM_THREADS"] = "1"
+os.environ["OMP_NUM_THREADS"] = "1"
+
 import numpy             as np
 import matplotlib.pyplot as plt
 
 from os                import path
 from math              import ceil
 from gwpy.timeseries   import TimeSeries, StateVector, TimeSeriesDict
 from gwpy.segments     import SegmentList, Segment
@@ -16,18 +21,15 @@
 from ast               import literal_eval as make_tuple
 
 from mly.datatools import DataPod
 from mly.validators import Validator
 from mly.plugins import *
 
 
-# Scipy and numpy env parameters that limit the threads
-os.environ["MKL_NUM_THREADS"] = "1"
-os.environ["NUMEXPR_NUM_THREADS"] = "1"
-os.environ["OMP_NUM_THREADS"] = "1"
+
 
 def checkDetectorArguments(config):
     
     """Injests command line arguments dictionary and outputs runtime config
         dictionary with error checked detector parameters.
         
        Parameters
@@ -200,46 +202,14 @@
     else:
         # Raiser error if no trigger directory inputted:
         raise FileNotFoundError("You need to specify a directory where the triggers \
  will be saved using the following syntax when running the command --trigger_directory <value>.")
     
     return config
 
-def checkTriggerPlotDirectoryArguments(config):
-    
-    """Injests command line arguments dictionary and outputs runtime config
-        dictionary with error checked trigger plot directory parameters.
-       
-       Parameters
-       ----------
-       
-       config: dict
-           Dictionary containing program runtime variables
-    
-       Returns
-       ------- 
-       
-       config: dict
-           Dictionary containing program runtime variables
-    """
-    
-    #Check trigger plot directory:
-    if config['triggerplot_directory'] != None:
-        if os.path.isdir(config['triggerplot_directory']):
-            # Set config trigger directory if trigger directory argument
-            # present and directory exists.
-            config["triggerplot_directory"] = config["triggerplot_directory"]
-        else:
-             # Raise error if triggerplot directory does not exist.
-            raise FileNotFoundError(f"{config['triggerplot_directory']} is not a valid path")
-    else:
-        # If output directory does not exist set trigger plot directory to None.
-        config["triggerplot_directory"] = None
-    
-    return config
 
 def checktriggerDestinationArguments(config):
     
     """Injests command line arguments dictionary and outputs runtime config
         dictionary with error checked trigger_destination parameters.
        
        Parameters
@@ -349,14 +319,49 @@
 
     elif "OFFLINE" not in config["search_mode"]:
 
         raise ValueError("time_reference must be the current unix time in numerical or string format")
 
     return config
 
+
+def checkSkymapArguments(config):
+    
+    """Injests command line arguments dictionary and outputs runtime config
+        dictionary with error checked output directory parameters.
+       
+       Parameters
+       ----------
+       
+       config: dict 
+           Dictionary containing comand line arguments
+           
+       config: dict
+           Dictionary containing program runtime variables
+    
+       Returns
+       -------
+    
+       config: dict 
+           Dictionary containing comand line arguments
+           
+       config: dict
+           Dictionary containing program runtime variables
+    """
+    
+    # Check output directory:
+    if config['skymap']==None:
+        config['skymap']=0
+    
+    if not isinstance(config['skymap'],int):
+        raise TypeError("skymap option must be 1 for true or 0 for false")
+    else:
+
+        return config
+
 def checkSkymapArguments(config):
     
     """Injests command line arguments dictionary and outputs runtime config
         dictionary with error checked output directory parameters.
        
        Parameters
        ----------
@@ -561,15 +566,14 @@
     
     check_functions = [
         checkDetectorArguments, 
         checkChannelArguments, 
         checkThresholdArguments,
         checkOutputDirectoryArguments,
         checkTriggerDirectoryArguments,
-        checkTriggerPlotDirectoryArguments,
         checktriggerDestinationArguments,
         checkSplitArguments,
         checkTimeReferenceArguments,
         checkSkymapArguments,
         checkMasterDirectoryArguments,
         checkBufferDirectoryArguments,
         
@@ -637,15 +641,15 @@
         config['prefix'] = prefix_name_list[0]
         return config
     else:
         raise ValueError("Prefix names are not consistent in frames")
 
 
     
-def readFrameFile(frames, channel, state_vector_channel , start_gps = None, end_gps = None, wait = 0.5, timeout = 10, count=0):
+def readFrameFile(frames, channel, state_vector_channel , start_gps = None, end_gps = None, wait = 0.5, timeout = 5, count=0):
     
     """A wrapper function for TimeSeries.read from gwpy. It reads the channels
     from the frames provided. If the reading fails for any reason it 
     waits <wait> time and tries again, up to <timeout> times.
     
     Parameters
     ----------
@@ -676,41 +680,45 @@
         If data are fetched sucessfully it returns a gwpy TimeSeries
         
     None: 
         If data are not fetched after <timeout> attemts
 
     """
 
-    channels = [channel, state_vector_channel]
-
+    if state_vector_channel is not None:
+        channels = [channel, state_vector_channel]
+    else:
+        channels = [channel]
+    
     try:
         
         try:
             data = TimeSeriesDict.read(frames, channels, start = start_gps, end = end_gps)
-
+            
         except Exception as ex:
-
             raise(ex)
         
-        
+        if state_vector_channel is not None:
 
-        state_vector_status = StateVector(data[state_vector_channel]).boolean[:,0:2].value.all()
+            state_vector_status = StateVector(data[state_vector_channel]).boolean[:,0:2].value.all()
 
-        if state_vector_status:
-            return data[channel]
+            if state_vector_status:
+                return data[channel]
 
+            else:
+                    
+                raise Exception(f"State vector is {state_vector_status}")
         else:
-            raise Exception(f"State vector is {state_vector_status}")
 
-        
+            return data[channel]
+            
     except Exception as e:
 
         time.sleep(wait)
-        count += 1;
-        
+        count += 1
         if count < timeout:
             return readFrameFile(frames, channel, state_vector_channel, start_gps, end_gps 
                                     , wait = wait, timeout=timeout, count = count)
             
         else:
             print(e)
             print("Could not find frames.")
@@ -911,16 +919,16 @@
     start = config['segment_list'][0]
     end = config['segment_list'][1]
 
     config = find_observing_run(config,interval = [start,end])
     print("looked for observing run")
 
     detector_active_flag = {'H1': 'H1:DMT-ANALYSIS_READY:1'
-                        ,'L1': 'L1:DMT-ANALYSIS_READY:1'
-                        ,'V1': 'V1:ITF_SCIENCE:1'}
+                           ,'L1': 'L1:DMT-ANALYSIS_READY:1'
+                           ,'V1': 'V1:ITF_SCIENCE:1'}
 
     detector_segments = []
 
     for det in detectors:
         individual_detector_segment = query_segments(detector_active_flag[det+'1'], start, end)['active']
         print(det, individual_detector_segment)
         for flag in inclusion_flags:
@@ -1029,20 +1037,20 @@
 
         #Combine path to frame file with prefix variable for readability:
         prefix = config['frames_directory'][detector_initial] + detector_initial+"-"+detector_initial+"1_"+config['prefix']
 
         #Generate names of fram files to be read:
         frames = [f"{prefix}{gps_time + i}-1.gwf" for i in range(config["required_buffer"] + 1)]
 
-        
+        state_vector = config["state_vector_channels"][detector_initial] if (config["state_vector_channels"] is not None) else None
         #Search for frame files, return None if not found
         strain = readFrameFile(
             frames, 
             config["channels"][detector_initial],
-            config["state_vector_channels"][detector_initial],
+            state_vector,
             wait = config["wait"],
             timeout = int((config["num_scripts"]*1.5)/config["wait"]) # Using up to 1.5 times the time available in one loop of time. 
         )
 
         if strain != None:
             #Resample all strain data:
             strain = strain.resample(config["fs"]).value[int(config["fs"]*0.5):-int(config["fs"]*0.5)]
@@ -1119,14 +1127,15 @@
     
     We don't use checking functions to save time in low latency searces.
     """
     
     detectors = pod.detectors
     for det in detectors:
         _gps = pod.gps[pod.detectors.index(det)]
+        if _gps==0.0: continue # Correction to avoid saving virgo
         _pod = DataPod(pod.strain[pod.detectors.index(det)]
                        ,detectors = [det]
                        ,fs = pod.fs
                        ,gps = [_gps])
         
         _pod.save(masterDirectory+'temp/'+det+'/'+str(_gps)+'_1')
```

### Comparing `mly_pipeline-0.5.4.1/mly_pipeline/tests/__init__.py` & `mly_pipeline-0.5.5/mly_pipeline/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/mly_pipeline/tests/test_skymap_generation.py` & `mly_pipeline-0.5.5/mly_pipeline/tests/test_skymap_generation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/mly_pipeline.egg-info/PKG-INFO` & `mly_pipeline-0.5.5/mly_pipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly-pipeline
-Version: 0.5.4.1
+Version: 0.5.5
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.5.4.1/mly_pipeline.egg-info/SOURCES.txt` & `mly_pipeline-0.5.5/mly_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.4.1/pyproject.toml` & `mly_pipeline-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61", "setuptools-scm>=3.4.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mly_pipeline"
-version = "0.5.4.1"
+version = "0.5.5"
 authors = [
     {name = "Vasileios SKliris", email = "sklirisv@cardiff.ac.uk"},
 ]
 description = "Search pipeline to run online and offline GW searches with mly package."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["ml", "gravitational waves", "bursts"]
```

