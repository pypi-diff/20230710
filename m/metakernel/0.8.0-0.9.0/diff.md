# Comparing `tmp/metakernel-0.8.0.zip` & `tmp/metakernel-0.9.0.zip`

## zipinfo {}

```diff
@@ -1,122 +1,124 @@
-Zip file size: 172214 bytes, number of entries: 120
--rw-r--r--  2.0 unx      240 b- defN 14-Oct-11 05:18 metakernel-0.8.0/CONTRIBUTORS.rst
--rw-r--r--  2.0 unx      415 b- defN 14-Dec-12 09:18 metakernel-0.8.0/MANIFEST.in
--rw-r--r--  2.0 unx     1407 b- defN 15-Jan-31 16:10 metakernel-0.8.0/HISTORY.rst
--rw-r--r--  2.0 unx     1658 b- defN 15-Jan-15 19:01 metakernel-0.8.0/README.rst
--rw-r--r--  2.0 unx     1714 b- defN 15-Jan-10 08:31 metakernel-0.8.0/Makefile
--rw-r--r--  2.0 unx      199 b- defN 15-Jan-31 16:12 metakernel-0.8.0/setup.cfg
--rw-r--r--  2.0 unx      216 b- defN 15-Jan-10 17:19 metakernel-0.8.0/LICENSE.txt
--rw-r--r--  2.0 unx     2632 b- defN 15-Jan-31 16:12 metakernel-0.8.0/PKG-INFO
--rw-r--r--  2.0 unx     1540 b- defN 15-Jan-29 19:07 metakernel-0.8.0/setup.py
--rw-r--r--  2.0 unx      220 b- defN 15-Jan-25 21:43 metakernel-0.8.0/metakernel/display.py
--rw-r--r--  2.0 unx      994 b- defN 14-Oct-11 05:18 metakernel-0.8.0/metakernel/config.py
--rw-r--r--  2.0 unx     7953 b- defN 15-Jan-10 17:16 metakernel-0.8.0/metakernel/magic.py
--rw-r--r--  2.0 unx     6746 b- defN 14-Dec-12 09:47 metakernel-0.8.0/metakernel/replwrap.py
--rw-r--r--  2.0 unx    22516 b- defN 15-Jan-31 13:31 metakernel-0.8.0/metakernel/_metakernel.py
--rw-r--r--  2.0 unx      325 b- defN 15-Jan-31 16:10 metakernel-0.8.0/metakernel/__init__.py
--rw-r--r--  2.0 unx    10775 b- defN 15-Jan-10 13:55 metakernel-0.8.0/metakernel/parser.py
--rw-r--r--  2.0 unx    89499 b- defN 14-Dec-12 09:18 metakernel-0.8.0/metakernel/pexpect.py
--rw-r--r--  2.0 unx     6826 b- defN 14-Dec-12 09:18 metakernel-0.8.0/metakernel/process_metakernel.py
--rw-r--r--  2.0 unx        0 b- defN 14-Dec-12 09:18 metakernel-0.8.0/metakernel/utils/__init__.py
--rw-r--r--  2.0 unx      448 b- defN 15-Jan-29 19:07 metakernel-0.8.0/metakernel/utils/kernel.py
--rwxr-xr-x  2.0 unx    21508 b- defN 14-Nov-22 15:23 metakernel-0.8.0/metakernel/tests/test_expect.py
--rw-r--r--  2.0 unx     2608 b- defN 15-Jan-10 17:03 metakernel-0.8.0/metakernel/tests/test_magic.py
--rwxr-xr-x  2.0 unx     1638 b- defN 14-Nov-11 19:38 metakernel-0.8.0/metakernel/tests/_echo_wait.py
--rwxrwxrwx  2.0 unx      600 b- defN 14-Nov-16 12:37 metakernel-0.8.0/metakernel/tests/test_process_metakernel.py
--rw-r--r--  2.0 unx     3209 b- defN 14-Nov-10 08:13 metakernel-0.8.0/metakernel/tests/test_parser.py
--rw-r--r--  2.0 unx        0 b- defN 14-Oct-11 05:18 metakernel-0.8.0/metakernel/tests/__init__.py
--rw-r--r--  2.0 unx       48 b- defN 14-Nov-11 19:38 metakernel-0.8.0/metakernel/tests/_list100.py
--rw-r--r--  2.0 unx     2833 b- defN 14-Dec-12 10:34 metakernel-0.8.0/metakernel/tests/test_replwrap.py
--rw-r--r--  2.0 unx     2094 b- defN 14-Dec-12 09:18 metakernel-0.8.0/metakernel/tests/utils.py
--rw-r--r--  2.0 unx     7379 b- defN 14-Nov-10 08:13 metakernel-0.8.0/metakernel/tests/test_metakernel.py
--rw-r--r--  2.0 unx      788 b- defN 14-Oct-11 05:18 metakernel-0.8.0/metakernel/magics/run_magic.py
--rw-r--r--  2.0 unx     4666 b- defN 14-Oct-11 05:18 metakernel-0.8.0/metakernel/magics/spell_magic.py
--rw-r--r--  2.0 unx      984 b- defN 14-Oct-11 05:18 metakernel-0.8.0/metakernel/magics/plot_magic.py
--rw-r--r--  2.0 unx     9679 b- defN 15-Jan-25 21:43 metakernel-0.8.0/metakernel/magics/parallel_magic.py
--rw-r--r--  2.0 unx      568 b- defN 14-Dec-12 09:18 metakernel-0.8.0/metakernel/magics/get_magic.py
--rw-r--r--  2.0 unx      539 b- defN 14-Nov-09 20:30 metakernel-0.8.0/metakernel/magics/restart_magic.py
--rw-r--r--  2.0 unx     3153 b- defN 14-Nov-22 19:23 metakernel-0.8.0/metakernel/magics/shell_magic.py
--rw-r--r--  2.0 unx     2851 b- defN 14-Dec-03 21:19 metakernel-0.8.0/metakernel/magics/kernel_magic.py
--rw-r--r--  2.0 unx      799 b- defN 14-Oct-11 05:18 metakernel-0.8.0/metakernel/magics/load_magic.py
--rw-r--r--  2.0 unx     4838 b- defN 15-Jan-29 19:06 metakernel-0.8.0/metakernel/magics/python_magic.py
--rw-r--r--  2.0 unx      599 b- defN 14-Dec-12 09:18 metakernel-0.8.0/metakernel/magics/set_magic.py
--rw-r--r--  2.0 unx     4123 b- defN 15-Jan-10 09:15 metakernel-0.8.0/metakernel/magics/help_magic.py
--rw-r--r--  2.0 unx     1405 b- defN 14-Oct-11 05:18 metakernel-0.8.0/metakernel/magics/show_magic.py
--rw-r--r--  2.0 unx      833 b- defN 14-Dec-12 09:18 metakernel-0.8.0/metakernel/magics/ls_magic.py
--rw-r--r--  2.0 unx     1307 b- defN 14-Nov-09 11:15 metakernel-0.8.0/metakernel/magics/processing_magic.py
--rw-r--r--  2.0 unx      957 b- defN 14-Oct-11 05:18 metakernel-0.8.0/metakernel/magics/html_magic.py
--rw-r--r--  2.0 unx        0 b- defN 14-Oct-11 05:18 metakernel-0.8.0/metakernel/magics/__init__.py
--rw-r--r--  2.0 unx     1444 b- defN 14-Nov-09 16:02 metakernel-0.8.0/metakernel/magics/install_magic_magic.py
--rw-r--r--  2.0 unx     1814 b- defN 14-Nov-27 10:15 metakernel-0.8.0/metakernel/magics/file_magic.py
--rw-r--r--  2.0 unx     7099 b- defN 14-Nov-09 11:15 metakernel-0.8.0/metakernel/magics/debug_magic.py
--rw-r--r--  2.0 unx     2145 b- defN 14-Nov-09 11:15 metakernel-0.8.0/metakernel/magics/connect_info_magic.py
--rw-r--r--  2.0 unx     1619 b- defN 14-Nov-09 16:02 metakernel-0.8.0/metakernel/magics/download_magic.py
--rw-r--r--  2.0 unx      959 b- defN 14-Oct-11 05:18 metakernel-0.8.0/metakernel/magics/edit_magic.py
--rw-r--r--  2.0 unx     2408 b- defN 15-Jan-25 21:43 metakernel-0.8.0/metakernel/magics/install_magic.py
--rw-r--r--  2.0 unx      729 b- defN 14-Oct-11 05:18 metakernel-0.8.0/metakernel/magics/reload_magics_magic.py
--rw-r--r--  2.0 unx     1074 b- defN 14-Oct-11 05:18 metakernel-0.8.0/metakernel/magics/lsmagic_magic.py
--rw-r--r--  2.0 unx      922 b- defN 14-Oct-11 05:18 metakernel-0.8.0/metakernel/magics/latex_magic.py
--rw-r--r--  2.0 unx      918 b- defN 14-Oct-11 05:18 metakernel-0.8.0/metakernel/magics/time_magic.py
--rw-r--r--  2.0 unx     1108 b- defN 14-Oct-11 05:18 metakernel-0.8.0/metakernel/magics/javascript_magic.py
--rw-r--r--  2.0 unx      842 b- defN 14-Nov-29 19:16 metakernel-0.8.0/metakernel/magics/cd_magic.py
--rw-r--r--  2.0 unx     3050 b- defN 14-Nov-16 21:12 metakernel-0.8.0/metakernel/magics/magic_magic.py
--rw-r--r--  2.0 unx      469 b- defN 14-Dec-12 09:18 metakernel-0.8.0/metakernel/magics/tests/test_ls_magic.py
--rw-r--r--  2.0 unx      911 b- defN 14-Dec-12 09:18 metakernel-0.8.0/metakernel/magics/tests/test_set_get_magic.py
--rw-r--r--  2.0 unx      245 b- defN 14-Nov-08 20:28 metakernel-0.8.0/metakernel/magics/tests/test_magic_magic.py
--rw-r--r--  2.0 unx      984 b- defN 14-Nov-08 20:55 metakernel-0.8.0/metakernel/magics/tests/test_help_magic.py
--rw-r--r--  2.0 unx      630 b- defN 14-Nov-09 11:15 metakernel-0.8.0/metakernel/magics/tests/test_show_magic.py
--rw-r--r--  2.0 unx      722 b- defN 15-Jan-25 21:43 metakernel-0.8.0/metakernel/magics/tests/test_install_magic_magic.py
--rw-r--r--  2.0 unx      335 b- defN 14-Nov-09 11:15 metakernel-0.8.0/metakernel/magics/tests/test_processing_magic.py
--rw-r--r--  2.0 unx      272 b- defN 14-Nov-08 20:24 metakernel-0.8.0/metakernel/magics/tests/test_kernel_magic.py
--rw-r--r--  2.0 unx      212 b- defN 14-Nov-09 16:22 metakernel-0.8.0/metakernel/magics/tests/test_load_magic.py
--rw-r--r--  2.0 unx      581 b- defN 14-Nov-09 11:15 metakernel-0.8.0/metakernel/magics/tests/test_lsmagic_magic.py
--rw-r--r--  2.0 unx      312 b- defN 14-Nov-08 20:27 metakernel-0.8.0/metakernel/magics/tests/test_plot_magic.py
--rw-r--r--  2.0 unx      311 b- defN 14-Nov-09 11:15 metakernel-0.8.0/metakernel/magics/tests/test_html_magic.py
--rw-r--r--  2.0 unx      312 b- defN 14-Nov-09 11:15 metakernel-0.8.0/metakernel/magics/tests/test_time_magic.py
--rw-r--r--  2.0 unx     1013 b- defN 14-Nov-16 08:52 metakernel-0.8.0/metakernel/magics/tests/test_shell_magic.py
--rw-r--r--  2.0 unx      711 b- defN 14-Nov-09 11:15 metakernel-0.8.0/metakernel/magics/tests/test_connect_info_magic.py
--rw-r--r--  2.0 unx        0 b- defN 14-Nov-09 12:52 metakernel-0.8.0/metakernel/magics/tests/__init__.py
--rw-r--r--  2.0 unx      349 b- defN 14-Nov-09 11:15 metakernel-0.8.0/metakernel/magics/tests/test_javascript_magic.py
--rw-r--r--  2.0 unx      917 b- defN 15-Jan-25 21:43 metakernel-0.8.0/metakernel/magics/tests/test_download_magic.py
--rw-r--r--  2.0 unx     1662 b- defN 14-Nov-16 21:18 metakernel-0.8.0/metakernel/magics/tests/test_python_magic.py
--rw-r--r--  2.0 unx      364 b- defN 14-Nov-09 16:27 metakernel-0.8.0/metakernel/magics/tests/test_edit_magic.py
--rw-r--r--  2.0 unx      291 b- defN 14-Nov-09 20:44 metakernel-0.8.0/metakernel/magics/tests/test_restart_magic.py
--rw-r--r--  2.0 unx      333 b- defN 14-Nov-29 19:15 metakernel-0.8.0/metakernel/magics/tests/test_cd_magic.py
--rw-r--r--  2.0 unx     1108 b- defN 14-Nov-27 10:15 metakernel-0.8.0/metakernel/magics/tests/test_file_magic.py
--rw-r--r--  2.0 unx      739 b- defN 14-Nov-08 22:42 metakernel-0.8.0/metakernel/magics/tests/test_spell_magic.py
--rw-r--r--  2.0 unx      187 b- defN 14-Nov-09 18:45 metakernel-0.8.0/metakernel/magics/tests/test_debug_magic.py
--rw-r--r--  2.0 unx      592 b- defN 14-Nov-09 18:45 metakernel-0.8.0/metakernel/magics/tests/test_reload_magics_magic.py
--rw-r--r--  2.0 unx      477 b- defN 14-Nov-09 16:28 metakernel-0.8.0/metakernel/magics/tests/test_latex_magic.py
--rw-r--r--  2.0 unx      763 b- defN 14-Nov-29 19:15 metakernel-0.8.0/metakernel/magics/tests/test_parallel_magic.py
--rw-r--r--  2.0 unx      321 b- defN 14-Nov-09 18:45 metakernel-0.8.0/metakernel/magics/tests/test_run_magic.py
--rw-r--r--  2.0 unx     1733 b- defN 15-Jan-15 19:02 metakernel-0.8.0/metakernel_bash/metakernel_bash.py
--rw-r--r--  2.0 unx     2113 b- defN 15-Jan-29 19:07 metakernel-0.8.0/metakernel_bash/setup.py
--rw-r--r--  2.0 unx       11 b- defN 15-Jan-31 16:12 metakernel-0.8.0/metakernel.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 15-Jan-31 16:12 metakernel-0.8.0/metakernel.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     2632 b- defN 15-Jan-31 16:12 metakernel-0.8.0/metakernel.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     4158 b- defN 15-Jan-31 16:12 metakernel-0.8.0/metakernel.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      543 b- defN 14-Oct-11 05:18 metakernel-0.8.0/docs/index.rst
--rw-r--r--  2.0 unx     9224 b- defN 14-Oct-11 05:18 metakernel-0.8.0/docs/conf.py
--rw-r--r--  2.0 unx       85 b- defN 14-Oct-11 05:18 metakernel-0.8.0/docs/source/info.rst
--rw-r--r--  2.0 unx      202 b- defN 14-Oct-11 05:18 metakernel-0.8.0/docs/source/api.rst
--rw-r--r--  2.0 unx      118 b- defN 14-Oct-11 05:18 metakernel-0.8.0/docs/source/installation.rst
--rw-r--r--  2.0 unx      363 b- defN 14-Sep-03 10:37 metakernel-0.8.0/docs/_build/html/_static/down.png
--rw-r--r--  2.0 unx      372 b- defN 14-Sep-03 10:37 metakernel-0.8.0/docs/_build/html/_static/up-pressed.png
--rw-r--r--  2.0 unx      392 b- defN 14-Sep-03 10:37 metakernel-0.8.0/docs/_build/html/_static/file.png
--rw-r--r--  2.0 unx      199 b- defN 14-Sep-03 10:37 metakernel-0.8.0/docs/_build/html/_static/minus.png
--rw-r--r--  2.0 unx     3578 b- defN 14-Sep-03 10:37 metakernel-0.8.0/docs/_build/html/_static/comment-close.png
--rw-r--r--  2.0 unx      363 b- defN 14-Sep-03 10:37 metakernel-0.8.0/docs/_build/html/_static/up.png
--rw-r--r--  2.0 unx      199 b- defN 14-Sep-03 10:37 metakernel-0.8.0/docs/_build/html/_static/plus.png
--rw-r--r--  2.0 unx      368 b- defN 14-Sep-03 10:37 metakernel-0.8.0/docs/_build/html/_static/down-pressed.png
--rw-r--r--  2.0 unx     3445 b- defN 14-Sep-03 10:37 metakernel-0.8.0/docs/_build/html/_static/comment.png
--rw-r--r--  2.0 unx     3500 b- defN 14-Sep-03 10:37 metakernel-0.8.0/docs/_build/html/_static/comment-bright.png
--rw-r--r--  2.0 unx     8777 b- defN 14-Dec-19 14:56 metakernel-0.8.0/docs/_build/html/_static/bootswatch-2.3.2/img/glyphicons-halflings-white.png
--rw-r--r--  2.0 unx    12799 b- defN 14-Dec-19 14:56 metakernel-0.8.0/docs/_build/html/_static/bootswatch-2.3.2/img/glyphicons-halflings.png
--rw-r--r--  2.0 unx     8777 b- defN 14-Dec-19 14:56 metakernel-0.8.0/docs/_build/html/_static/bootstrap-2.3.2/img/glyphicons-halflings-white.png
--rw-r--r--  2.0 unx    12799 b- defN 14-Dec-19 14:56 metakernel-0.8.0/docs/_build/html/_static/bootstrap-2.3.2/img/glyphicons-halflings.png
--rw-r--r--  2.0 unx     1015 b- defN 15-Jan-15 19:02 metakernel-0.8.0/metakernel_echo/metakernel_echo.py
--rw-r--r--  2.0 unx     2174 b- defN 15-Jan-29 19:07 metakernel-0.8.0/metakernel_echo/setup.py
--rw-r--r--  2.0 unx     2140 b- defN 15-Jan-29 19:07 metakernel-0.8.0/metakernel_python/setup.py
--rw-r--r--  2.0 unx     2132 b- defN 15-Jan-15 19:02 metakernel-0.8.0/metakernel_python/metakernel_python.py
--rw-r--r--  2.0 unx      142 b- defN 14-Nov-22 15:54 metakernel-0.8.0/metakernel_python/kernelspec/kernel.json
-120 files, 362937 bytes uncompressed, 150896 bytes compressed:  58.4%
+Zip file size: 178508 bytes, number of entries: 122
+-rw-r--r--  2.0 unx      240 b- defN 15-Feb-10 21:04 metakernel-0.9.0/CONTRIBUTORS.rst
+-rw-r--r--  2.0 unx      416 b- defN 15-Feb-10 21:04 metakernel-0.9.0/MANIFEST.in
+-rw-r--r--  2.0 unx     1566 b- defN 15-Mar-03 22:25 metakernel-0.9.0/HISTORY.rst
+-rw-r--r--  2.0 unx     1763 b- defN 15-Feb-14 09:06 metakernel-0.9.0/README.rst
+-rw-r--r--  2.0 unx     1709 b- defN 15-Mar-03 22:28 metakernel-0.9.0/Makefile
+-rw-r--r--  2.0 unx      199 b- defN 15-Mar-03 22:28 metakernel-0.9.0/setup.cfg
+-rw-r--r--  2.0 unx      216 b- defN 15-Feb-10 21:04 metakernel-0.9.0/LICENSE.txt
+-rw-r--r--  2.0 unx     2737 b- defN 15-Mar-03 22:28 metakernel-0.9.0/PKG-INFO
+-rw-r--r--  2.0 unx     1540 b- defN 15-Feb-10 21:04 metakernel-0.9.0/setup.py
+-rw-r--r--  2.0 unx      220 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/display.py
+-rw-r--r--  2.0 unx      994 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/config.py
+-rw-r--r--  2.0 unx     7953 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magic.py
+-rw-r--r--  2.0 unx     6806 b- defN 15-Mar-03 22:17 metakernel-0.9.0/metakernel/replwrap.py
+-rw-r--r--  2.0 unx    23052 b- defN 15-Mar-03 22:17 metakernel-0.9.0/metakernel/_metakernel.py
+-rw-r--r--  2.0 unx      325 b- defN 15-Mar-03 22:26 metakernel-0.9.0/metakernel/__init__.py
+-rw-r--r--  2.0 unx    10927 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/parser.py
+-rw-r--r--  2.0 unx    89646 b- defN 15-Mar-03 22:17 metakernel-0.9.0/metakernel/pexpect.py
+-rw-r--r--  2.0 unx     6826 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/process_metakernel.py
+-rw-r--r--  2.0 unx        0 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/utils/__init__.py
+-rw-r--r--  2.0 unx      448 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/utils/kernel.py
+-rw-r--r--  2.0 unx     1492 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/images/logo-32x32.png
+-rw-r--r--  2.0 unx     3823 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/images/logo-64x64.png
+-rwxr-xr-x  2.0 unx    21508 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/tests/test_expect.py
+-rw-r--r--  2.0 unx     2608 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/tests/test_magic.py
+-rwxr-xr-x  2.0 unx     1638 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/tests/_echo_wait.py
+-rwxr-xr-x  2.0 unx      600 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/tests/test_process_metakernel.py
+-rw-r--r--  2.0 unx     3209 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/tests/test_parser.py
+-rw-r--r--  2.0 unx        0 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/tests/__init__.py
+-rw-r--r--  2.0 unx       48 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/tests/_list100.py
+-rw-r--r--  2.0 unx     2833 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/tests/test_replwrap.py
+-rw-r--r--  2.0 unx     2094 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/tests/utils.py
+-rw-r--r--  2.0 unx     7379 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/tests/test_metakernel.py
+-rw-r--r--  2.0 unx      788 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/run_magic.py
+-rw-r--r--  2.0 unx     4666 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/spell_magic.py
+-rw-r--r--  2.0 unx     1274 b- defN 15-Feb-14 09:05 metakernel-0.9.0/metakernel/magics/plot_magic.py
+-rw-r--r--  2.0 unx     9679 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/parallel_magic.py
+-rw-r--r--  2.0 unx      568 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/get_magic.py
+-rw-r--r--  2.0 unx      539 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/restart_magic.py
+-rw-r--r--  2.0 unx     3153 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/shell_magic.py
+-rw-r--r--  2.0 unx     2851 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/kernel_magic.py
+-rw-r--r--  2.0 unx      799 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/load_magic.py
+-rw-r--r--  2.0 unx     4838 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/python_magic.py
+-rw-r--r--  2.0 unx      599 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/set_magic.py
+-rw-r--r--  2.0 unx     4123 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/help_magic.py
+-rw-r--r--  2.0 unx     1405 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/show_magic.py
+-rw-r--r--  2.0 unx      833 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/ls_magic.py
+-rw-r--r--  2.0 unx     1307 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/processing_magic.py
+-rw-r--r--  2.0 unx      957 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/html_magic.py
+-rw-r--r--  2.0 unx        0 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/__init__.py
+-rw-r--r--  2.0 unx     1444 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/install_magic_magic.py
+-rw-r--r--  2.0 unx     1814 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/file_magic.py
+-rw-r--r--  2.0 unx     7099 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/debug_magic.py
+-rw-r--r--  2.0 unx     2145 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/connect_info_magic.py
+-rw-r--r--  2.0 unx     1619 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/download_magic.py
+-rw-r--r--  2.0 unx      959 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/edit_magic.py
+-rw-r--r--  2.0 unx     2408 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/install_magic.py
+-rw-r--r--  2.0 unx      729 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/reload_magics_magic.py
+-rw-r--r--  2.0 unx     1074 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/lsmagic_magic.py
+-rw-r--r--  2.0 unx      922 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/latex_magic.py
+-rw-r--r--  2.0 unx      918 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/time_magic.py
+-rw-r--r--  2.0 unx     1108 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/javascript_magic.py
+-rw-r--r--  2.0 unx      842 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/cd_magic.py
+-rw-r--r--  2.0 unx     3050 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/magic_magic.py
+-rw-r--r--  2.0 unx      469 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_ls_magic.py
+-rw-r--r--  2.0 unx      911 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_set_get_magic.py
+-rw-r--r--  2.0 unx      245 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_magic_magic.py
+-rw-r--r--  2.0 unx      984 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_help_magic.py
+-rw-r--r--  2.0 unx      630 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_show_magic.py
+-rw-r--r--  2.0 unx      722 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_install_magic_magic.py
+-rw-r--r--  2.0 unx      335 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_processing_magic.py
+-rw-r--r--  2.0 unx      272 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_kernel_magic.py
+-rw-r--r--  2.0 unx      212 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_load_magic.py
+-rw-r--r--  2.0 unx      581 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_lsmagic_magic.py
+-rw-r--r--  2.0 unx     1148 b- defN 15-Feb-14 09:05 metakernel-0.9.0/metakernel/magics/tests/test_plot_magic.py
+-rw-r--r--  2.0 unx      311 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_html_magic.py
+-rw-r--r--  2.0 unx      312 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_time_magic.py
+-rw-r--r--  2.0 unx     1013 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_shell_magic.py
+-rw-r--r--  2.0 unx      711 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_connect_info_magic.py
+-rw-r--r--  2.0 unx        0 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/__init__.py
+-rw-r--r--  2.0 unx      349 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_javascript_magic.py
+-rw-r--r--  2.0 unx      917 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_download_magic.py
+-rw-r--r--  2.0 unx     1662 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_python_magic.py
+-rw-r--r--  2.0 unx      364 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_edit_magic.py
+-rw-r--r--  2.0 unx      291 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_restart_magic.py
+-rw-r--r--  2.0 unx      333 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_cd_magic.py
+-rw-r--r--  2.0 unx     1108 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_file_magic.py
+-rw-r--r--  2.0 unx      739 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_spell_magic.py
+-rw-r--r--  2.0 unx      187 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_debug_magic.py
+-rw-r--r--  2.0 unx      592 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_reload_magics_magic.py
+-rw-r--r--  2.0 unx      477 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_latex_magic.py
+-rw-r--r--  2.0 unx      763 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_parallel_magic.py
+-rw-r--r--  2.0 unx      321 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel/magics/tests/test_run_magic.py
+-rw-r--r--  2.0 unx     1733 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel_bash/metakernel_bash.py
+-rw-r--r--  2.0 unx     2113 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel_bash/setup.py
+-rw-r--r--  2.0 unx       11 b- defN 15-Mar-03 22:28 metakernel-0.9.0/metakernel.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 15-Mar-03 22:28 metakernel-0.9.0/metakernel.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     2737 b- defN 15-Mar-03 22:28 metakernel-0.9.0/metakernel.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     4224 b- defN 15-Mar-03 22:28 metakernel-0.9.0/metakernel.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      543 b- defN 15-Feb-10 21:04 metakernel-0.9.0/docs/index.rst
+-rw-r--r--  2.0 unx     9224 b- defN 15-Feb-10 21:04 metakernel-0.9.0/docs/conf.py
+-rw-r--r--  2.0 unx       85 b- defN 15-Feb-10 21:04 metakernel-0.9.0/docs/source/info.rst
+-rw-r--r--  2.0 unx      202 b- defN 15-Feb-10 21:04 metakernel-0.9.0/docs/source/api.rst
+-rw-r--r--  2.0 unx      118 b- defN 15-Feb-10 21:04 metakernel-0.9.0/docs/source/installation.rst
+-rw-r--r--  2.0 unx      363 b- defN 14-Sep-03 10:37 metakernel-0.9.0/docs/_build/html/_static/down.png
+-rw-r--r--  2.0 unx      372 b- defN 14-Sep-03 10:37 metakernel-0.9.0/docs/_build/html/_static/up-pressed.png
+-rw-r--r--  2.0 unx      392 b- defN 14-Sep-03 10:37 metakernel-0.9.0/docs/_build/html/_static/file.png
+-rw-r--r--  2.0 unx      199 b- defN 14-Sep-03 10:37 metakernel-0.9.0/docs/_build/html/_static/minus.png
+-rw-r--r--  2.0 unx     3578 b- defN 14-Sep-03 10:37 metakernel-0.9.0/docs/_build/html/_static/comment-close.png
+-rw-r--r--  2.0 unx      363 b- defN 14-Sep-03 10:37 metakernel-0.9.0/docs/_build/html/_static/up.png
+-rw-r--r--  2.0 unx      199 b- defN 14-Sep-03 10:37 metakernel-0.9.0/docs/_build/html/_static/plus.png
+-rw-r--r--  2.0 unx      368 b- defN 14-Sep-03 10:37 metakernel-0.9.0/docs/_build/html/_static/down-pressed.png
+-rw-r--r--  2.0 unx     3445 b- defN 14-Sep-03 10:37 metakernel-0.9.0/docs/_build/html/_static/comment.png
+-rw-r--r--  2.0 unx     3500 b- defN 14-Sep-03 10:37 metakernel-0.9.0/docs/_build/html/_static/comment-bright.png
+-rw-r--r--  2.0 unx     8777 b- defN 14-Dec-19 14:56 metakernel-0.9.0/docs/_build/html/_static/bootswatch-2.3.2/img/glyphicons-halflings-white.png
+-rw-r--r--  2.0 unx    12799 b- defN 14-Dec-19 14:56 metakernel-0.9.0/docs/_build/html/_static/bootswatch-2.3.2/img/glyphicons-halflings.png
+-rw-r--r--  2.0 unx     8777 b- defN 14-Dec-19 14:56 metakernel-0.9.0/docs/_build/html/_static/bootstrap-2.3.2/img/glyphicons-halflings-white.png
+-rw-r--r--  2.0 unx    12799 b- defN 14-Dec-19 14:56 metakernel-0.9.0/docs/_build/html/_static/bootstrap-2.3.2/img/glyphicons-halflings.png
+-rw-r--r--  2.0 unx     1015 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel_echo/metakernel_echo.py
+-rw-r--r--  2.0 unx     2174 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel_echo/setup.py
+-rw-r--r--  2.0 unx     2140 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel_python/setup.py
+-rw-r--r--  2.0 unx     2132 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel_python/metakernel_python.py
+-rw-r--r--  2.0 unx      142 b- defN 15-Feb-10 21:04 metakernel-0.9.0/metakernel_python/kernelspec/kernel.json
+122 files, 370809 bytes uncompressed, 156842 bytes compressed:  57.7%
```

## zipnote {}

```diff
@@ -1,361 +1,367 @@
-Filename: metakernel-0.8.0/CONTRIBUTORS.rst
+Filename: metakernel-0.9.0/CONTRIBUTORS.rst
 Comment: 
 
-Filename: metakernel-0.8.0/MANIFEST.in
+Filename: metakernel-0.9.0/MANIFEST.in
 Comment: 
 
-Filename: metakernel-0.8.0/HISTORY.rst
+Filename: metakernel-0.9.0/HISTORY.rst
 Comment: 
 
-Filename: metakernel-0.8.0/README.rst
+Filename: metakernel-0.9.0/README.rst
 Comment: 
 
-Filename: metakernel-0.8.0/Makefile
+Filename: metakernel-0.9.0/Makefile
 Comment: 
 
-Filename: metakernel-0.8.0/setup.cfg
+Filename: metakernel-0.9.0/setup.cfg
 Comment: 
 
-Filename: metakernel-0.8.0/LICENSE.txt
+Filename: metakernel-0.9.0/LICENSE.txt
 Comment: 
 
-Filename: metakernel-0.8.0/PKG-INFO
+Filename: metakernel-0.9.0/PKG-INFO
 Comment: 
 
-Filename: metakernel-0.8.0/setup.py
+Filename: metakernel-0.9.0/setup.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/display.py
+Filename: metakernel-0.9.0/metakernel/display.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/config.py
+Filename: metakernel-0.9.0/metakernel/config.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magic.py
+Filename: metakernel-0.9.0/metakernel/magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/replwrap.py
+Filename: metakernel-0.9.0/metakernel/replwrap.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/_metakernel.py
+Filename: metakernel-0.9.0/metakernel/_metakernel.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/__init__.py
+Filename: metakernel-0.9.0/metakernel/__init__.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/parser.py
+Filename: metakernel-0.9.0/metakernel/parser.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/pexpect.py
+Filename: metakernel-0.9.0/metakernel/pexpect.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/process_metakernel.py
+Filename: metakernel-0.9.0/metakernel/process_metakernel.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/utils/__init__.py
+Filename: metakernel-0.9.0/metakernel/utils/__init__.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/utils/kernel.py
+Filename: metakernel-0.9.0/metakernel/utils/kernel.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/tests/test_expect.py
+Filename: metakernel-0.9.0/metakernel/images/logo-32x32.png
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/tests/test_magic.py
+Filename: metakernel-0.9.0/metakernel/images/logo-64x64.png
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/tests/_echo_wait.py
+Filename: metakernel-0.9.0/metakernel/tests/test_expect.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/tests/test_process_metakernel.py
+Filename: metakernel-0.9.0/metakernel/tests/test_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/tests/test_parser.py
+Filename: metakernel-0.9.0/metakernel/tests/_echo_wait.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/tests/__init__.py
+Filename: metakernel-0.9.0/metakernel/tests/test_process_metakernel.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/tests/_list100.py
+Filename: metakernel-0.9.0/metakernel/tests/test_parser.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/tests/test_replwrap.py
+Filename: metakernel-0.9.0/metakernel/tests/__init__.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/tests/utils.py
+Filename: metakernel-0.9.0/metakernel/tests/_list100.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/tests/test_metakernel.py
+Filename: metakernel-0.9.0/metakernel/tests/test_replwrap.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/run_magic.py
+Filename: metakernel-0.9.0/metakernel/tests/utils.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/spell_magic.py
+Filename: metakernel-0.9.0/metakernel/tests/test_metakernel.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/plot_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/run_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/parallel_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/spell_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/get_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/plot_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/restart_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/parallel_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/shell_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/get_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/kernel_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/restart_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/load_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/shell_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/python_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/kernel_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/set_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/load_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/help_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/python_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/show_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/set_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/ls_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/help_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/processing_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/show_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/html_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/ls_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/__init__.py
+Filename: metakernel-0.9.0/metakernel/magics/processing_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/install_magic_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/html_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/file_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/__init__.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/debug_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/install_magic_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/connect_info_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/file_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/download_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/debug_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/edit_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/connect_info_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/install_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/download_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/reload_magics_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/edit_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/lsmagic_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/install_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/latex_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/reload_magics_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/time_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/lsmagic_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/javascript_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/latex_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/cd_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/time_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/magic_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/javascript_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_ls_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/cd_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_set_get_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/magic_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_magic_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_ls_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_help_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_set_get_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_show_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_magic_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_install_magic_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_help_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_processing_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_show_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_kernel_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_install_magic_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_load_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_processing_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_lsmagic_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_kernel_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_plot_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_load_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_html_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_lsmagic_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_time_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_plot_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_shell_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_html_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_connect_info_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_time_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/__init__.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_shell_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_javascript_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_connect_info_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_download_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/__init__.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_python_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_javascript_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_edit_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_download_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_restart_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_python_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_cd_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_edit_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_file_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_restart_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_spell_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_cd_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_debug_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_file_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_reload_magics_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_spell_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_latex_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_debug_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_parallel_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_reload_magics_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel/magics/tests/test_run_magic.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_latex_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel_bash/metakernel_bash.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_parallel_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel_bash/setup.py
+Filename: metakernel-0.9.0/metakernel/magics/tests/test_run_magic.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel.egg-info/top_level.txt
+Filename: metakernel-0.9.0/metakernel_bash/metakernel_bash.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel.egg-info/dependency_links.txt
+Filename: metakernel-0.9.0/metakernel_bash/setup.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel.egg-info/PKG-INFO
+Filename: metakernel-0.9.0/metakernel.egg-info/top_level.txt
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel.egg-info/SOURCES.txt
+Filename: metakernel-0.9.0/metakernel.egg-info/dependency_links.txt
 Comment: 
 
-Filename: metakernel-0.8.0/docs/index.rst
+Filename: metakernel-0.9.0/metakernel.egg-info/PKG-INFO
 Comment: 
 
-Filename: metakernel-0.8.0/docs/conf.py
+Filename: metakernel-0.9.0/metakernel.egg-info/SOURCES.txt
 Comment: 
 
-Filename: metakernel-0.8.0/docs/source/info.rst
+Filename: metakernel-0.9.0/docs/index.rst
 Comment: 
 
-Filename: metakernel-0.8.0/docs/source/api.rst
+Filename: metakernel-0.9.0/docs/conf.py
 Comment: 
 
-Filename: metakernel-0.8.0/docs/source/installation.rst
+Filename: metakernel-0.9.0/docs/source/info.rst
 Comment: 
 
-Filename: metakernel-0.8.0/docs/_build/html/_static/down.png
+Filename: metakernel-0.9.0/docs/source/api.rst
 Comment: 
 
-Filename: metakernel-0.8.0/docs/_build/html/_static/up-pressed.png
+Filename: metakernel-0.9.0/docs/source/installation.rst
 Comment: 
 
-Filename: metakernel-0.8.0/docs/_build/html/_static/file.png
+Filename: metakernel-0.9.0/docs/_build/html/_static/down.png
 Comment: 
 
-Filename: metakernel-0.8.0/docs/_build/html/_static/minus.png
+Filename: metakernel-0.9.0/docs/_build/html/_static/up-pressed.png
 Comment: 
 
-Filename: metakernel-0.8.0/docs/_build/html/_static/comment-close.png
+Filename: metakernel-0.9.0/docs/_build/html/_static/file.png
 Comment: 
 
-Filename: metakernel-0.8.0/docs/_build/html/_static/up.png
+Filename: metakernel-0.9.0/docs/_build/html/_static/minus.png
 Comment: 
 
-Filename: metakernel-0.8.0/docs/_build/html/_static/plus.png
+Filename: metakernel-0.9.0/docs/_build/html/_static/comment-close.png
 Comment: 
 
-Filename: metakernel-0.8.0/docs/_build/html/_static/down-pressed.png
+Filename: metakernel-0.9.0/docs/_build/html/_static/up.png
 Comment: 
 
-Filename: metakernel-0.8.0/docs/_build/html/_static/comment.png
+Filename: metakernel-0.9.0/docs/_build/html/_static/plus.png
 Comment: 
 
-Filename: metakernel-0.8.0/docs/_build/html/_static/comment-bright.png
+Filename: metakernel-0.9.0/docs/_build/html/_static/down-pressed.png
 Comment: 
 
-Filename: metakernel-0.8.0/docs/_build/html/_static/bootswatch-2.3.2/img/glyphicons-halflings-white.png
+Filename: metakernel-0.9.0/docs/_build/html/_static/comment.png
 Comment: 
 
-Filename: metakernel-0.8.0/docs/_build/html/_static/bootswatch-2.3.2/img/glyphicons-halflings.png
+Filename: metakernel-0.9.0/docs/_build/html/_static/comment-bright.png
 Comment: 
 
-Filename: metakernel-0.8.0/docs/_build/html/_static/bootstrap-2.3.2/img/glyphicons-halflings-white.png
+Filename: metakernel-0.9.0/docs/_build/html/_static/bootswatch-2.3.2/img/glyphicons-halflings-white.png
 Comment: 
 
-Filename: metakernel-0.8.0/docs/_build/html/_static/bootstrap-2.3.2/img/glyphicons-halflings.png
+Filename: metakernel-0.9.0/docs/_build/html/_static/bootswatch-2.3.2/img/glyphicons-halflings.png
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel_echo/metakernel_echo.py
+Filename: metakernel-0.9.0/docs/_build/html/_static/bootstrap-2.3.2/img/glyphicons-halflings-white.png
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel_echo/setup.py
+Filename: metakernel-0.9.0/docs/_build/html/_static/bootstrap-2.3.2/img/glyphicons-halflings.png
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel_python/setup.py
+Filename: metakernel-0.9.0/metakernel_echo/metakernel_echo.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel_python/metakernel_python.py
+Filename: metakernel-0.9.0/metakernel_echo/setup.py
 Comment: 
 
-Filename: metakernel-0.8.0/metakernel_python/kernelspec/kernel.json
+Filename: metakernel-0.9.0/metakernel_python/setup.py
+Comment: 
+
+Filename: metakernel-0.9.0/metakernel_python/metakernel_python.py
+Comment: 
+
+Filename: metakernel-0.9.0/metakernel_python/kernelspec/kernel.json
 Comment: 
 
 Zip file comment:
```

## Comparing `metakernel-0.8.0/HISTORY.rst` & `metakernel-0.9.0/HISTORY.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 .. :changelog:
 
 Release History
 ------------------------
 
+0.9.0 (2015-03-03)
+++++++++++++++++++
+- Improved support for ProcessKernel on Windows
+- Improved %plot magic
+- Added metakernel.makSubKernel* helper methods
+
+
 0.8.0 (2015-01-31)
 ++++++++++++++++++
 - Added support for IPython.display.Image for metakernels
 - Improved support for Display formatting
 
 0.7.0 (2015-01-29)
 ++++++++++++++++++
```

## Comparing `metakernel-0.8.0/README.rst` & `metakernel-0.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-A simple Jupyter/IPython kernel template which includes core magic functions.
+A Jupyter/IPython kernel template which includes core magic functions (including help, command and file path completion, parallel and distributed processing, downloads, and much more).
 
 .. image:: https://badge.fury.io/py/metakernel.png/
     :target: http://badge.fury.io/py/metakernel
 
 .. image:: https://pypip.in/d/metakernel/badge.png
         :target: https://crate.io/packages/metakernel/
 
 .. image:: https://coveralls.io/repos/Calysto/metakernel/badge.png?branch=master
   :target: https://coveralls.io/r/Calysto/metakernel
-  
+
 .. image:: https://travis-ci.org/Calysto/metakernel.svg
   :target: https://travis-ci.org/Calysto/metakernel
 
 
 See IPython's docs on `wrapper kernels
 <http://ipython.org/ipython-doc/dev/development/wrapperkernels.html>`_.
```

## Comparing `metakernel-0.8.0/Makefile` & `metakernel-0.9.0/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 cover: clean
 	pip install nose-cov
 	ipcluster2 start -n=3 &
 	nosetests $(TEST_ARGS) --with-cov --cov $(NAME) $(NAME); ipcluster2 stop
 	coverage annotate
 
-release: test gh-pages
+release: gh-pages
 	pip install wheel
 	python setup.py register
 	python setup.py bdist_wheel upload
 	python setup.py sdist --formats=gztar,zip upload
 	git tag v$(VERSION)
 	git push origin --all
```

## Comparing `metakernel-0.8.0/PKG-INFO` & `metakernel-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 1.1
 Name: metakernel
-Version: 0.8.0
+Version: 0.9.0
 Summary: Metakernel for Jupyter
 Home-page: https://github.com/Calysto/metakernel
 Author: Steven Silvester
 Author-email: steven.silvester@ieee.org
 License: UNKNOWN
-Description: A simple Jupyter/IPython kernel template which includes core magic functions.
+Description: A Jupyter/IPython kernel template which includes core magic functions (including help, command and file path completion, parallel and distributed processing, downloads, and much more).
         
         .. image:: https://badge.fury.io/py/metakernel.png/
             :target: http://badge.fury.io/py/metakernel
         
         .. image:: https://pypip.in/d/metakernel/badge.png
                 :target: https://crate.io/packages/metakernel/
         
         .. image:: https://coveralls.io/repos/Calysto/metakernel/badge.png?branch=master
           :target: https://coveralls.io/r/Calysto/metakernel
-          
+        
         .. image:: https://travis-ci.org/Calysto/metakernel.svg
           :target: https://travis-ci.org/Calysto/metakernel
         
         
         See IPython's docs on `wrapper kernels
         <http://ipython.org/ipython-doc/dev/development/wrapperkernels.html>`_.
```

## Comparing `metakernel-0.8.0/setup.py` & `metakernel-0.9.0/setup.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/config.py` & `metakernel-0.9.0/metakernel/config.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magic.py` & `metakernel-0.9.0/metakernel/magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/replwrap.py` & `metakernel-0.9.0/metakernel/replwrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,16 @@
     def __init__(self, cmd_or_spawn, prompt_regex, prompt_change_cmd,
                  new_prompt_regex=PEXPECT_PROMPT,
                  continuation_prompt_regex=PEXPECT_CONTINUATION_PROMPT,
                  extra_init_cmd=None,
                  prompt_emit_cmd=None,
                  echo=False):
         if isinstance(cmd_or_spawn, str):
-            self.child = pexpect.spawnu(cmd_or_spawn, echo=echo)
+            self.child = pexpect.spawnu(cmd_or_spawn, echo=echo,
+                                        errors="ignore")
         else:
             self.child = cmd_or_spawn
 
         if self.child.echo and not echo:
             # Existing spawn instance has echo enabled, disable it
             # to prevent our input from being repeated to output.
             self.child.setecho(False)
@@ -90,14 +91,15 @@
     def set_prompt(self, prompt_regex, prompt_change_cmd):
         self.child.expect(prompt_regex)
         self.sendline(prompt_change_cmd)
 
     def _expect_prompt(self, timeout=-1):
         if self.prompt_emit_cmd:
             self.sendline(self.prompt_emit_cmd)
+
         try:
             return self.child.expect([self.prompt_regex, self.continuation_prompt_regex],
                                      timeout=timeout)
         except KeyboardInterrupt:
             self.child.sendintr()
             if self.prompt_emit_cmd:
                 time.sleep(1.)
@@ -125,22 +127,22 @@
         if command.endswith('\n'):
             cmdlines.append('')
         if not cmdlines:
             raise ValueError("No command was given")
 
         self.sendline(cmdlines[0])
         for line in cmdlines[1:]:
-            self._expect_prompt(timeout=1)
+            self._expect_prompt(timeout=-1)
             self.sendline(line)
 
         # Command was fully submitted, now wait for the next prompt
         if self._expect_prompt(timeout=timeout) == 1:
             # We got the continuation prompt - command was incomplete
             self.child.kill(signal.SIGINT)
-            self._expect_prompt(timeout=1)
+            self._expect_prompt(timeout=-1)
             raise ValueError("Continuation prompt found -"
                              " input was incomplete:\n" + command)
         return self.child.before
 
 
 def python(command="python"):
     """Start a Python shell and return a :class:`REPLWrapper` object."""
```

## Comparing `metakernel-0.8.0/metakernel/_metakernel.py` & `metakernel-0.9.0/metakernel/_metakernel.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 import glob
 import base64
 from .config import get_history_file, get_local_magics_dir
 from .parser import Parser
 import imp
 import inspect
 import logging
+import codecs
 
+PY3 = (sys.version_info[0] >= 3)
 
 def lazy_import_handle_comm_opened(*args, **kwargs):
     Widget.handle_comm_opened(*args, **kwargs)
 
 
 class MetaKernel(Kernel):
 
@@ -79,15 +81,15 @@
         self.max_hist_cache = 1000
         self.hist_cache = []
         self.comm_manager = CommManager(shell=None, parent=self,
                                         kernel=self)
         self.comm_manager.register_target('ipython.widget',
             lazy_import_handle_comm_opened)
 
-        self.plot_settings = dict(backend='inline', format=None, size=None)
+        self.plot_settings = dict(backend='inline')
         self.hist_file = get_history_file(self)
         self.reload_magics()
         # provide a way to get the current instance
         self.set_variable("kernel", self)
         self.parser = Parser(self.identifier_regex, self.func_call_regex,
                              self.magic_prefixes, self.help_suffix)
         self.comm_manager = CommManager(shell=None, parent=self,
@@ -103,14 +105,35 @@
     def subkernel(cls, kernel):
         """
         Handle issues regarding making a kernel a subkernel to this
         one. Used in %parallel and %kernel.
         """
         pass
 
+    def makeSubkernelTo(self, main_kernel, display_function):
+        """
+        Handle issues regarding making this kernel be a subkernel to 
+        another. Used in making metakernels be magics for IPython.
+        """
+        self.session = main_kernel.session
+        self.Display = display_function
+
+    def makeSubkernelToIPython(self):
+        """
+        Run this method in an IPython kernel to set
+        this kernel's input/output settings.
+        """
+        from IPython import get_ipython
+        from IPython.display import display
+        ip = get_ipython()
+        if ip: # we are running under an IPython kernel
+            self.makeSubkernelTo(ip.parent, display)
+        else:
+            raise Exception("Need to run under an IPython kernel")
+
     #####################################
     # Methods which provide kernel - specific behavior
 
     def set_variable(self, name, value):
         """
         Set a variable to a Python-typed value.
         """
@@ -521,15 +544,18 @@
         message = ""
         for item in args:
             if isinstance(item, Widget):
                 self.Display(item)
             else:
                 if message:
                     message += " "
-                message += str(item)
+                if PY3:
+                    message += str(item)
+                else:
+                    message += codecs.encode(item, "utf-8")
         message += end
         stream_content = {
             'name': 'stdout', 'text': message, 'metadata': dict()}
         self.log.debug('Print: %s' % message)
         self.send_response(self.iopub_socket, 'stream', stream_content)
 
     def Write(self, message):
@@ -542,22 +568,14 @@
         end = kwargs["end"] if ("end" in kwargs) else "\n"
         message = " ".join([str(a) for a in args]) + end
         self.log.debug('Error: %s' % message)
         stream_content = {
             'name': 'stderr', 'text': message, 'metadata': dict()}
         self.send_response(self.iopub_socket, 'stream', stream_content)
 
-    def update_plot_settings(self, backend, size, format):
-        """Update the default plot settings for the kernel."""
-        self.plot_settings['backend'] = backend
-        size = size or self.plot_settings['size']
-        self.plot_settings['size'] = size
-        format = format or self.plot_settings['format']
-        self.plot_settings['format'] = format
-
     def get_magic(self, text):
         # if first line matches a magic,
         # call magic.call_magic() and return magic object
         info = self.parse_code(text)
         magic = self.line_magics['magic']
         return magic.get_magic(info)
```

## Comparing `metakernel-0.8.0/metakernel/parser.py` & `metakernel-0.9.0/metakernel/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -302,16 +302,21 @@
     """Perform completion of filesystem path.
     http://stackoverflow.com/questions/5637124/tab-completion-in-pythons-raw-input
     """
     if not path or path == '.':
         return _listdir('.')
     dirname, rest = os.path.split(path)
     tmp = dirname if dirname else '.'
-    res = [os.path.join(dirname, p) for p in _listdir(tmp)
-           if p.startswith(rest)]
+    res = []
+    for p in _listdir(tmp):
+        try:
+            if p.startswith(rest):
+                res.append(os.path.join(dirname, p))
+        except UnicodeDecodeError:
+            pass # directory name does not allow join in Python 2.7
     # more than one match, or single match which does not exist (typo)
     if len(res) > 1 or not os.path.exists(path):
         return res
     # resolved to a single directory, so return list of files below it
     if os.path.isdir(path):
         return [os.path.join(path, p) for p in _listdir(path)]
     # exact file match terminates this completion
```

## Comparing `metakernel-0.8.0/metakernel/pexpect.py` & `metakernel-0.9.0/metakernel/pexpect.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,18 @@
     import tty
     import resource
     import fcntl
 except ImportError:
     pty = None
     import threading
     import subprocess
-    import Queue
+    try:
+        import Queue
+    except ImportError:
+        import queue as Queue
     import ctypes
 
 import os
 import sys
 import time
 import re
 import struct
@@ -1018,15 +1021,15 @@
             except OSError as e:
                 self._log(e, 'read')
 
             if not buf:
                 self.flag_eof = True
                 return
 
-            self._read_queue.put(buf)
+            self._read_queue.put(buf.decode('utf-8'))
             time.sleep(0.001)
 
     def _winread(self, size, timeout):
         t0 = time.time()
         buf = ''
         while (time.time() - t0) < timeout and len(buf) < size:
             try:
@@ -1923,15 +1926,18 @@
         return s
 
     @staticmethod
     def _coerce_send_string(s):
         return s
 
     def _coerce_read_string(self, s):
-        return self._decoder.decode(s, final=False)
+        try:
+            return self._decoder.decode(s, final=False)
+        except TypeError:
+            return s
 
     def _send(self, s):
         return super(spawnu, self)._send(s.encode(self.encoding, self.errors))
 
 
 class searcher_string(object):
```

## Comparing `metakernel-0.8.0/metakernel/process_metakernel.py` & `metakernel-0.9.0/metakernel/process_metakernel.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/tests/test_expect.py` & `metakernel-0.9.0/metakernel/tests/test_expect.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/tests/test_magic.py` & `metakernel-0.9.0/metakernel/tests/test_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/tests/_echo_wait.py` & `metakernel-0.9.0/metakernel/tests/_echo_wait.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/tests/test_process_metakernel.py` & `metakernel-0.9.0/metakernel/tests/test_process_metakernel.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/tests/test_parser.py` & `metakernel-0.9.0/metakernel/tests/test_parser.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/tests/test_replwrap.py` & `metakernel-0.9.0/metakernel/tests/test_replwrap.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/tests/utils.py` & `metakernel-0.9.0/metakernel/tests/utils.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/tests/test_metakernel.py` & `metakernel-0.9.0/metakernel/tests/test_metakernel.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/run_magic.py` & `metakernel-0.9.0/metakernel/magics/run_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/spell_magic.py` & `metakernel-0.9.0/metakernel/magics/spell_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/plot_magic.py` & `metakernel-0.9.0/metakernel/magics/plot_magic.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,25 +10,37 @@
         '-s', '--size', action='store',
         help='Pixel size of plots, "width,height"'
     )
     @option(
         '-f', '--format', action='store', default='png',
         help='Plot format (png, svg or jpg).'
     )
-    def line_plot(self, backend, size=None, format=None):
+    @option(
+        '-b', '--backend', action='store', default='inline',
+        help='Backend selection'
+    )
+    @option(
+        '-r', '--resolution', action='store', default=96,
+        help='Resolution in pixels per inch'
+    )
+    def line_plot(self, *args, **kwargs):
         """
         %plot [options] backend - configure plotting for the session.
 
         This line magic will configure the plot settings for this
         language.
 
         Examples:
-            %plot --format=png matplotlib
-            %plot -s 640,480 matplotlib
+            %plot qt --format=png
+            %plot inline -s 640,480
 
-        Note: not all languages may support the %plot magic.
+        Note: not all languages may support the %plot magic, and not all
+        options may be supported.
         """
-        self.kernel.update_plot_settings(backend.lower(), size, format)
+        if args:
+            kwargs['backend'] = args[0]
+        self.kernel.plot_settings.update(**kwargs)
         self.kernel.handle_plot_settings()
 
+
 def register_magics(kernel):
     kernel.register_magics(PlotMagic)
```

## Comparing `metakernel-0.8.0/metakernel/magics/parallel_magic.py` & `metakernel-0.9.0/metakernel/magics/parallel_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/get_magic.py` & `metakernel-0.9.0/metakernel/magics/get_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/restart_magic.py` & `metakernel-0.9.0/metakernel/magics/restart_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/shell_magic.py` & `metakernel-0.9.0/metakernel/magics/shell_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/kernel_magic.py` & `metakernel-0.9.0/metakernel/magics/kernel_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/load_magic.py` & `metakernel-0.9.0/metakernel/magics/load_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/python_magic.py` & `metakernel-0.9.0/metakernel/magics/python_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/set_magic.py` & `metakernel-0.9.0/metakernel/magics/set_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/help_magic.py` & `metakernel-0.9.0/metakernel/magics/help_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/show_magic.py` & `metakernel-0.9.0/metakernel/magics/show_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/ls_magic.py` & `metakernel-0.9.0/metakernel/magics/ls_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/processing_magic.py` & `metakernel-0.9.0/metakernel/magics/processing_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/html_magic.py` & `metakernel-0.9.0/metakernel/magics/html_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/install_magic_magic.py` & `metakernel-0.9.0/metakernel/magics/install_magic_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/file_magic.py` & `metakernel-0.9.0/metakernel/magics/file_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/debug_magic.py` & `metakernel-0.9.0/metakernel/magics/debug_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/connect_info_magic.py` & `metakernel-0.9.0/metakernel/magics/connect_info_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/download_magic.py` & `metakernel-0.9.0/metakernel/magics/download_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/edit_magic.py` & `metakernel-0.9.0/metakernel/magics/edit_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/install_magic.py` & `metakernel-0.9.0/metakernel/magics/install_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/reload_magics_magic.py` & `metakernel-0.9.0/metakernel/magics/reload_magics_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/lsmagic_magic.py` & `metakernel-0.9.0/metakernel/magics/lsmagic_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/latex_magic.py` & `metakernel-0.9.0/metakernel/magics/latex_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/time_magic.py` & `metakernel-0.9.0/metakernel/magics/time_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/javascript_magic.py` & `metakernel-0.9.0/metakernel/magics/javascript_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/cd_magic.py` & `metakernel-0.9.0/metakernel/magics/cd_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/magic_magic.py` & `metakernel-0.9.0/metakernel/magics/magic_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/tests/test_set_get_magic.py` & `metakernel-0.9.0/metakernel/magics/tests/test_set_get_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/tests/test_help_magic.py` & `metakernel-0.9.0/metakernel/magics/tests/test_help_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/tests/test_show_magic.py` & `metakernel-0.9.0/metakernel/magics/tests/test_show_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/tests/test_install_magic_magic.py` & `metakernel-0.9.0/metakernel/magics/tests/test_install_magic_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/tests/test_lsmagic_magic.py` & `metakernel-0.9.0/metakernel/magics/tests/test_lsmagic_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/tests/test_shell_magic.py` & `metakernel-0.9.0/metakernel/magics/tests/test_shell_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/tests/test_connect_info_magic.py` & `metakernel-0.9.0/metakernel/magics/tests/test_connect_info_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/tests/test_download_magic.py` & `metakernel-0.9.0/metakernel/magics/tests/test_download_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/tests/test_python_magic.py` & `metakernel-0.9.0/metakernel/magics/tests/test_python_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/tests/test_file_magic.py` & `metakernel-0.9.0/metakernel/magics/tests/test_file_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/tests/test_spell_magic.py` & `metakernel-0.9.0/metakernel/magics/tests/test_spell_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/tests/test_reload_magics_magic.py` & `metakernel-0.9.0/metakernel/magics/tests/test_reload_magics_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel/magics/tests/test_parallel_magic.py` & `metakernel-0.9.0/metakernel/magics/tests/test_parallel_magic.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel_bash/metakernel_bash.py` & `metakernel-0.9.0/metakernel_bash/metakernel_bash.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel_bash/setup.py` & `metakernel-0.9.0/metakernel_bash/setup.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel.egg-info/PKG-INFO` & `metakernel-0.9.0/metakernel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 1.1
 Name: metakernel
-Version: 0.8.0
+Version: 0.9.0
 Summary: Metakernel for Jupyter
 Home-page: https://github.com/Calysto/metakernel
 Author: Steven Silvester
 Author-email: steven.silvester@ieee.org
 License: UNKNOWN
-Description: A simple Jupyter/IPython kernel template which includes core magic functions.
+Description: A Jupyter/IPython kernel template which includes core magic functions (including help, command and file path completion, parallel and distributed processing, downloads, and much more).
         
         .. image:: https://badge.fury.io/py/metakernel.png/
             :target: http://badge.fury.io/py/metakernel
         
         .. image:: https://pypip.in/d/metakernel/badge.png
                 :target: https://crate.io/packages/metakernel/
         
         .. image:: https://coveralls.io/repos/Calysto/metakernel/badge.png?branch=master
           :target: https://coveralls.io/r/Calysto/metakernel
-          
+        
         .. image:: https://travis-ci.org/Calysto/metakernel.svg
           :target: https://travis-ci.org/Calysto/metakernel
         
         
         See IPython's docs on `wrapper kernels
         <http://ipython.org/ipython-doc/dev/development/wrapperkernels.html>`_.
```

## Comparing `metakernel-0.8.0/metakernel.egg-info/SOURCES.txt` & `metakernel-0.9.0/metakernel.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 metakernel/pexpect.py
 metakernel/process_metakernel.py
 metakernel/replwrap.py
 metakernel.egg-info/PKG-INFO
 metakernel.egg-info/SOURCES.txt
 metakernel.egg-info/dependency_links.txt
 metakernel.egg-info/top_level.txt
+metakernel/images/logo-32x32.png
+metakernel/images/logo-64x64.png
 metakernel/magics/__init__.py
 metakernel/magics/cd_magic.py
 metakernel/magics/connect_info_magic.py
 metakernel/magics/debug_magic.py
 metakernel/magics/download_magic.py
 metakernel/magics/edit_magic.py
 metakernel/magics/file_magic.py
```

## Comparing `metakernel-0.8.0/docs/index.rst` & `metakernel-0.9.0/docs/index.rst`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/docs/conf.py` & `metakernel-0.9.0/docs/conf.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/docs/_build/html/_static/comment-close.png` & `metakernel-0.9.0/docs/_build/html/_static/comment-close.png`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/docs/_build/html/_static/comment.png` & `metakernel-0.9.0/docs/_build/html/_static/comment.png`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/docs/_build/html/_static/comment-bright.png` & `metakernel-0.9.0/docs/_build/html/_static/comment-bright.png`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/docs/_build/html/_static/bootswatch-2.3.2/img/glyphicons-halflings-white.png` & `metakernel-0.9.0/docs/_build/html/_static/bootswatch-2.3.2/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/docs/_build/html/_static/bootswatch-2.3.2/img/glyphicons-halflings.png` & `metakernel-0.9.0/docs/_build/html/_static/bootswatch-2.3.2/img/glyphicons-halflings.png`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/docs/_build/html/_static/bootstrap-2.3.2/img/glyphicons-halflings-white.png` & `metakernel-0.9.0/docs/_build/html/_static/bootstrap-2.3.2/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/docs/_build/html/_static/bootstrap-2.3.2/img/glyphicons-halflings.png` & `metakernel-0.9.0/docs/_build/html/_static/bootstrap-2.3.2/img/glyphicons-halflings.png`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel_echo/metakernel_echo.py` & `metakernel-0.9.0/metakernel_echo/metakernel_echo.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel_echo/setup.py` & `metakernel-0.9.0/metakernel_echo/setup.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel_python/setup.py` & `metakernel-0.9.0/metakernel_python/setup.py`

 * *Files identical despite different names*

## Comparing `metakernel-0.8.0/metakernel_python/metakernel_python.py` & `metakernel-0.9.0/metakernel_python/metakernel_python.py`

 * *Files identical despite different names*

