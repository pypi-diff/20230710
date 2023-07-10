# Comparing `tmp/emperor-1.0.3.tar.gz` & `tmp/emperor-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emperor-1.0.3.tar", last modified: Thu Apr 15 06:21:44 2021, max compression
+gzip compressed data, was "emperor-1.0.4.tar", last modified: Mon Jul 10 15:34:39 2023, max compression
```

## Comparing `emperor-1.0.3.tar` & `emperor-1.0.4.tar`

### file list

```diff
@@ -1,245 +1,245 @@
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.208998 emperor-1.0.3/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    12710 2021-04-15 06:21:30.000000 emperor-1.0.3/ChangeLog.md
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1022 2021-04-15 06:21:30.000000 emperor-1.0.3/INSTALL.md
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    18695 2021-04-15 06:21:30.000000 emperor-1.0.3/LICENSE.md
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      222 2021-04-15 06:21:30.000000 emperor-1.0.3/MANIFEST.in
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2904 2021-04-15 06:21:44.208570 emperor-1.0.3/PKG-INFO
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1652 2021-04-15 06:21:30.000000 emperor-1.0.3/README.md
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.114757 emperor-1.0.3/doc/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     6932 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/Makefile
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2158 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/README.md
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.103566 emperor-1.0.3/doc/bootstrap/
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.115767 emperor-1.0.3/doc/bootstrap/css/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    23409 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/bootstrap/css/bootstrap-theme.min.css
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)   121260 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.118723 emperor-1.0.3/doc/bootstrap/fonts/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    20127 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)   108738 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    45404 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    23424 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    18028 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.120670 emperor-1.0.3/doc/bootstrap/js/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    36868 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    85659 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/bootstrap/js/jquery-2.2.3.min.js
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.121313 emperor-1.0.3/doc/files/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)   542041 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/files/files.zip
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.124049 emperor-1.0.3/doc/img/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    12582 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/img/emperor_heading.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     5558 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/img/favicon.ico
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    78421 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/img/sample_1.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     6026 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/index.html
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     7814 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/installation_index.html
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      445 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/jsdoc-config.json
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.127612 emperor-1.0.3/doc/source/
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.128395 emperor-1.0.3/doc/source/_static/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2655 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/source/_static/copybutton.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      596 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/source/_static/style.css
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.128776 emperor-1.0.3/doc/source/_templates/
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.129982 emperor-1.0.3/doc/source/_templates/autosummary/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      109 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/source/_templates/autosummary/attribute.rst
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      727 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/source/_templates/autosummary/class.rst
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      106 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/source/_templates/autosummary/method.rst
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      852 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/source/_templates/layout.html
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     8616 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/source/conf.py
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      184 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/source/description.rst
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     5307 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/source/examples.rst
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2462 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/source/formats.rst
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1449 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/source/index.rst
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     4862 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/source/js_integration.rst
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.130798 emperor-1.0.3/doc/source/tutorials/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     8151 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/source/tutorials/animations.rst
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    82332 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/source/tutorials/trajectories.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    16050 2021-04-15 06:21:30.000000 emperor-1.0.3/doc/tutorial_index.html
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.133562 emperor-1.0.3/emperor/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      671 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/__init__.py
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    18736 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/_format_strings.py
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     3380 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/_pandas.py
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    55812 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/core.py
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2507 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/format.py
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.136837 emperor-1.0.3/emperor/qiime_backports/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      369 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/qiime_backports/__init__.py
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2714 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/qiime_backports/make_3d_plots.py
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     5749 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/qiime_backports/util.py
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.137242 emperor-1.0.3/emperor/support_files/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      928 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/README.md
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.137612 emperor-1.0.3/emperor/support_files/css/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2069 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/css/emperor.css
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.139675 emperor-1.0.3/emperor/support_files/img/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     8747 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/img/emperor.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     5558 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/img/favicon.ico
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2919 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/img/pause.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2946 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/img/play.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2965 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/img/reset.png
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.149830 emperor-1.0.3/emperor/support_files/js/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     6381 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/abc-view-controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    12874 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/animate.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    27264 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/animations-controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    24495 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/axes-controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     4982 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/color-editor.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    23333 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/color-view-controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    36949 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    17159 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/draw.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    17070 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/model.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     3698 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/multi-model.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2905 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/opacity-view-controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     4753 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/scale-editor.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     3159 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/scale-view-controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    44934 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/sceneplotview3d.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     4587 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/shape-controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2827 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/shape-editor.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     3055 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/shapes.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    16970 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/trajectory.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     6734 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/ui-state.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     4606 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/util.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    32253 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/view-controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    43894 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/view.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     3676 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/js/visibility-controller.js
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.156334 emperor-1.0.3/emperor/support_files/templates/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      220 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/templates/base-dependencies.html
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      394 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/templates/html-container-template.html
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      219 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/templates/jupyter-template.html
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     5504 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/templates/logic-template.html
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      561 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/templates/standalone-template.html
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      758 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/templates/style-template.html
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.107169 emperor-1.0.3/emperor/support_files/vendor/
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.159150 emperor-1.0.3/emperor/support_files/vendor/css/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      538 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/chosen-sprite.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      738 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/chosen-sprite@2x.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    11115 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/chosen.min.css
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.160675 emperor-1.0.3/emperor/support_files/vendor/css/font/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     5056 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/font/context-menu-icons.eot
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     4848 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/font/context-menu-icons.ttf
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     3188 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/font/context-menu-icons.woff
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2604 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/font/context-menu-icons.woff2
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.165405 emperor-1.0.3/emperor/support_files/vendor/css/images/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      335 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      207 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      262 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      262 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      332 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      280 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      328 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/images/ui-bg_highlight-soft_75_ffe45c_1x100.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     6922 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/images/ui-icons_222222_256x240.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     4549 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     6992 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/images/ui-icons_454545_256x240.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     6999 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/images/ui-icons_888888_256x240.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     4549 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    29829 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/jquery-ui.min.css
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     4150 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/jquery.contextMenu.min.css
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2146 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/slick.grid.min.css
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    11281 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/css/spectrum.min.css
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.175696 emperor-1.0.3/emperor/support_files/vendor/js/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     3164 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/Blob.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     3257 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/FileSaver.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1379 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/canvas-toBlob.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    28001 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/chosen.jquery.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    41616 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/chroma.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)   151725 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/d3.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    84345 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/jquery-2.1.4.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)   240422 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/jquery-ui.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    25850 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/jquery.contextMenu.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     5374 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/jquery.event.drag-2.2.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     6398 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/jquery.ui.position.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    15825 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/require-2.1.22.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2967 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/slick.core.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    21767 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/slick.dataview.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     8665 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/slick.editors.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      918 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/slick.formatters.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    57026 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/slick.grid.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    28250 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/spectrum.min.js
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.178164 emperor-1.0.3/emperor/support_files/vendor/js/three.js-plugins/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    26045 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/three.js-plugins/CanvasRenderer.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    24519 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/three.js-plugins/OrbitControls.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    25361 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/three.js-plugins/Projector.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    13336 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/three.js-plugins/SVGRenderer.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     6507 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/three.js-plugins/SelectionBox.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2523 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/three.js-plugins/SelectionHelper.js
--rwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)   618895 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/three.min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    16449 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/support_files/vendor/js/underscore-min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    14467 2021-04-15 06:21:30.000000 emperor-1.0.3/emperor/util.py
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.135690 emperor-1.0.3/emperor.egg-info/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2904 2021-04-15 06:21:44.000000 emperor-1.0.3/emperor.egg-info/PKG-INFO
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     9410 2021-04-15 06:21:44.000000 emperor-1.0.3/emperor.egg-info/SOURCES.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)        1 2021-04-15 06:21:44.000000 emperor-1.0.3/emperor.egg-info/dependency_links.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      284 2021-04-15 06:21:44.000000 emperor-1.0.3/emperor.egg-info/requires.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)       14 2021-04-15 06:21:44.000000 emperor-1.0.3/emperor.egg-info/top_level.txt
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.184085 emperor-1.0.3/images/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    56076 2021-04-15 06:21:30.000000 emperor-1.0.3/images/emperor-animation.gif
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)   843687 2021-04-15 06:21:30.000000 emperor-1.0.3/images/emperor-animation.psd
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    57353 2021-04-15 06:21:30.000000 emperor-1.0.3/images/emperor-frame1.ai
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    22814 2021-04-15 06:21:30.000000 emperor-1.0.3/images/emperor-frame1.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    61587 2021-04-15 06:21:30.000000 emperor-1.0.3/images/emperor-frame2.ai
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    20985 2021-04-15 06:21:30.000000 emperor-1.0.3/images/emperor-frame2.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    61996 2021-04-15 06:21:30.000000 emperor-1.0.3/images/emperor-frame3.ai
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    21045 2021-04-15 06:21:30.000000 emperor-1.0.3/images/emperor-frame3.png
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)   199499 2021-04-15 06:21:30.000000 emperor-1.0.3/images/emperor-logos.ai
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)       38 2021-04-15 06:21:44.209122 emperor-1.0.3/setup.cfg
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     2869 2021-04-15 06:21:30.000000 emperor-1.0.3/setup.py
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.188268 emperor-1.0.3/tests/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      349 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/__init__.py
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    46016 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/_test_core_strings.py
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    79784 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/_test_format_strings.py
--rwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)     4406 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/all_tests.py
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.196340 emperor-1.0.3/tests/javascript_tests/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     9403 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/index.html
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.197135 emperor-1.0.3/tests/javascript_tests/qunit/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     3719 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/qunit/qunit-min.css
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    26633 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/qunit/qunit-min.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    12349 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/runner.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    15422 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_animate.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    15215 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_animations_controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    12832 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_axes_controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    38327 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_color_view_controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    30010 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_decomposition_model.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    35857 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_decomposition_view.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     8999 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_draw.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     9092 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_opacity_view_controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     3744 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_plottable.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    10004 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_scalar_view_controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    10593 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_scale_view_controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    33555 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_sceneplotview3d.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     8081 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_shape_controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    23305 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_trajectory.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     7102 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_util.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    22664 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_view_controller.js
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     9519 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/javascript_tests/test_visibility_controller.js
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.108551 emperor-1.0.3/tests/scripts_test_data/
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.199957 emperor-1.0.3/tests/scripts_test_data/make_emperor/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      982 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/Fasting_Map.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1067 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/Fasting_Map_modified.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)      582 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/biplot.txt
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.200713 emperor-1.0.3/tests/scripts_test_data/make_emperor/compare/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1725 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/compare/pcoa_unweighted_unifrac_rarefaction_110_0.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1745 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/compare/pcoa_unweighted_unifrac_rarefaction_110_1.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1530 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/euclidian_pc.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1105 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/makefolders.sh
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1149 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/otu_table_L3.txt
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.204650 emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1725 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_0.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1745 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_1.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1734 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_2.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1734 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_3.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1743 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_4.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1736 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_5.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1741 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_6.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1735 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_7.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1726 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_8.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1736 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_9.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     1735 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    75254 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/test_core.py
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.205905 emperor-1.0.3/tests/test_data/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/test_data/.some-hidden-file
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.207188 emperor-1.0.3/tests/test_data/dir-with-only-hidden-files/
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/test_data/dir-with-only-hidden-files/.1.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/test_data/dir-with-only-hidden-files/.2.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/test_data/dir-with-only-hidden-files/.3.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/test_data/dir-with-only-hidden-files/.4.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/test_data/procrustes_results.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/test_data/unweighted_unifrac_pc_transformed_reference.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/test_data/weighted_unifrac_pc_transformed_q1.txt
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     4129 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/test_format.py
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)     4452 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/test_pandas.py
-drwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)        0 2021-04-15 06:21:44.207967 emperor-1.0.3/tests/test_qiime_backports/
--rwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)     4777 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/test_qiime_backports/test_make_3d_plots.py
--rwxr-xr-x   0 yoshikivazquezbaeza   (503) staff       (20)     7690 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/test_qiime_backports/test_util.py
--rw-r--r--   0 yoshikivazquezbaeza   (503) staff       (20)    26277 2021-04-15 06:21:30.000000 emperor-1.0.3/tests/test_util.py
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.837499 emperor-1.0.4/
+-rw-r--r--   0 yoshiki    (501) staff       (20)    13318 2023-07-10 15:34:11.000000 emperor-1.0.4/ChangeLog.md
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1022 2023-07-10 15:31:50.000000 emperor-1.0.4/INSTALL.md
+-rw-r--r--   0 yoshiki    (501) staff       (20)    18695 2023-07-10 15:31:50.000000 emperor-1.0.4/LICENSE.md
+-rw-r--r--   0 yoshiki    (501) staff       (20)      222 2023-07-10 15:31:50.000000 emperor-1.0.4/MANIFEST.in
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2738 2023-07-10 15:34:39.837134 emperor-1.0.4/PKG-INFO
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1652 2023-07-10 15:31:50.000000 emperor-1.0.4/README.md
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.738407 emperor-1.0.4/doc/
+-rw-r--r--   0 yoshiki    (501) staff       (20)     6932 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/Makefile
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2158 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/README.md
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.729482 emperor-1.0.4/doc/bootstrap/
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.739083 emperor-1.0.4/doc/bootstrap/css/
+-rw-r--r--   0 yoshiki    (501) staff       (20)    23409 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/bootstrap/css/bootstrap-theme.min.css
+-rw-r--r--   0 yoshiki    (501) staff       (20)   121260 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.741144 emperor-1.0.4/doc/bootstrap/fonts/
+-rw-r--r--   0 yoshiki    (501) staff       (20)    20127 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 yoshiki    (501) staff       (20)   108738 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 yoshiki    (501) staff       (20)    45404 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 yoshiki    (501) staff       (20)    23424 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 yoshiki    (501) staff       (20)    18028 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.741899 emperor-1.0.4/doc/bootstrap/js/
+-rw-r--r--   0 yoshiki    (501) staff       (20)    36868 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    85659 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/bootstrap/js/jquery-2.2.3.min.js
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.742334 emperor-1.0.4/doc/files/
+-rw-r--r--   0 yoshiki    (501) staff       (20)   542041 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/files/files.zip
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.744049 emperor-1.0.4/doc/img/
+-rw-r--r--   0 yoshiki    (501) staff       (20)    12582 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/img/emperor_heading.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)     5558 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/img/favicon.ico
+-rw-r--r--   0 yoshiki    (501) staff       (20)    78421 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/img/sample_1.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)     6026 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/index.html
+-rw-r--r--   0 yoshiki    (501) staff       (20)     7814 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/installation_index.html
+-rw-r--r--   0 yoshiki    (501) staff       (20)      445 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/jsdoc-config.json
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.746854 emperor-1.0.4/doc/source/
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.747800 emperor-1.0.4/doc/source/_static/
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2655 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/source/_static/copybutton.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)      596 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/source/_static/style.css
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.748342 emperor-1.0.4/doc/source/_templates/
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.750010 emperor-1.0.4/doc/source/_templates/autosummary/
+-rw-r--r--   0 yoshiki    (501) staff       (20)      109 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/source/_templates/autosummary/attribute.rst
+-rw-r--r--   0 yoshiki    (501) staff       (20)      727 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/source/_templates/autosummary/class.rst
+-rw-r--r--   0 yoshiki    (501) staff       (20)      106 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/source/_templates/autosummary/method.rst
+-rw-r--r--   0 yoshiki    (501) staff       (20)      852 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/source/_templates/layout.html
+-rw-r--r--   0 yoshiki    (501) staff       (20)     8616 2023-07-10 15:34:11.000000 emperor-1.0.4/doc/source/conf.py
+-rw-r--r--   0 yoshiki    (501) staff       (20)      184 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/source/description.rst
+-rw-r--r--   0 yoshiki    (501) staff       (20)     5307 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/source/examples.rst
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2462 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/source/formats.rst
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1449 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/source/index.rst
+-rw-r--r--   0 yoshiki    (501) staff       (20)     4862 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/source/js_integration.rst
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.751100 emperor-1.0.4/doc/source/tutorials/
+-rw-r--r--   0 yoshiki    (501) staff       (20)     8151 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/source/tutorials/animations.rst
+-rw-r--r--   0 yoshiki    (501) staff       (20)    82332 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/source/tutorials/trajectories.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)    16050 2023-07-10 15:31:50.000000 emperor-1.0.4/doc/tutorial_index.html
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.754318 emperor-1.0.4/emperor/
+-rw-r--r--   0 yoshiki    (501) staff       (20)      671 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/__init__.py
+-rw-r--r--   0 yoshiki    (501) staff       (20)    18736 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/_format_strings.py
+-rw-r--r--   0 yoshiki    (501) staff       (20)     3380 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/_pandas.py
+-rw-r--r--   0 yoshiki    (501) staff       (20)    55809 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/core.py
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2507 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/format.py
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.758265 emperor-1.0.4/emperor/qiime_backports/
+-rw-r--r--   0 yoshiki    (501) staff       (20)      369 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/qiime_backports/__init__.py
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2714 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/qiime_backports/make_3d_plots.py
+-rw-r--r--   0 yoshiki    (501) staff       (20)     5749 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/qiime_backports/util.py
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.758785 emperor-1.0.4/emperor/support_files/
+-rw-r--r--   0 yoshiki    (501) staff       (20)      928 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/README.md
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.759314 emperor-1.0.4/emperor/support_files/css/
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2069 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/css/emperor.css
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.761608 emperor-1.0.4/emperor/support_files/img/
+-rw-r--r--   0 yoshiki    (501) staff       (20)     8747 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/img/emperor.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)     5558 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/img/favicon.ico
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2919 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/img/pause.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2946 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/img/play.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2965 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/img/reset.png
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.772767 emperor-1.0.4/emperor/support_files/js/
+-rw-r--r--   0 yoshiki    (501) staff       (20)     6381 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/abc-view-controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    12874 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/animate.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    27264 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/animations-controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    24495 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/axes-controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     4982 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/color-editor.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    23333 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/color-view-controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    36949 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    17159 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/draw.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    17070 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/model.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     3698 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/multi-model.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2905 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/opacity-view-controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     4753 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/scale-editor.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     3159 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/scale-view-controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    44934 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/sceneplotview3d.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     4587 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/shape-controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2827 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/shape-editor.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     3055 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/shapes.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    16970 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/trajectory.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     6734 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/ui-state.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     4606 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/util.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    32253 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/view-controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    43894 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/view.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     4985 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/js/visibility-controller.js
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.775286 emperor-1.0.4/emperor/support_files/templates/
+-rw-r--r--   0 yoshiki    (501) staff       (20)      220 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/templates/base-dependencies.html
+-rw-r--r--   0 yoshiki    (501) staff       (20)      394 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/templates/html-container-template.html
+-rw-r--r--   0 yoshiki    (501) staff       (20)      219 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/templates/jupyter-template.html
+-rw-r--r--   0 yoshiki    (501) staff       (20)     5504 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/templates/logic-template.html
+-rw-r--r--   0 yoshiki    (501) staff       (20)      561 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/templates/standalone-template.html
+-rw-r--r--   0 yoshiki    (501) staff       (20)      796 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/templates/style-template.html
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.732567 emperor-1.0.4/emperor/support_files/vendor/
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.779197 emperor-1.0.4/emperor/support_files/vendor/css/
+-rw-r--r--   0 yoshiki    (501) staff       (20)      538 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/chosen-sprite.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)      738 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/chosen-sprite@2x.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)    11115 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/chosen.min.css
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.781245 emperor-1.0.4/emperor/support_files/vendor/css/font/
+-rw-r--r--   0 yoshiki    (501) staff       (20)     5056 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/font/context-menu-icons.eot
+-rw-r--r--   0 yoshiki    (501) staff       (20)     4848 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/font/context-menu-icons.ttf
+-rw-r--r--   0 yoshiki    (501) staff       (20)     3188 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/font/context-menu-icons.woff
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2604 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/font/context-menu-icons.woff2
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.786677 emperor-1.0.4/emperor/support_files/vendor/css/images/
+-rw-r--r--   0 yoshiki    (501) staff       (20)      335 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)      207 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)      262 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)      262 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)      332 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)      280 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)      328 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/images/ui-bg_highlight-soft_75_ffe45c_1x100.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)     6922 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)     4549 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)     6992 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)     6999 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)     4549 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)    29829 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/jquery-ui.min.css
+-rw-r--r--   0 yoshiki    (501) staff       (20)     4150 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/jquery.contextMenu.min.css
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2146 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/slick.grid.min.css
+-rw-r--r--   0 yoshiki    (501) staff       (20)    11281 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/css/spectrum.min.css
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.798884 emperor-1.0.4/emperor/support_files/vendor/js/
+-rw-r--r--   0 yoshiki    (501) staff       (20)     3164 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/Blob.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     3257 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/FileSaver.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1379 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/canvas-toBlob.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    28001 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/chosen.jquery.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    41616 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/chroma.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)   151725 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/d3.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    84345 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/jquery-2.1.4.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)   240422 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/jquery-ui.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    25850 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/jquery.contextMenu.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     5374 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/jquery.event.drag-2.2.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     6398 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/jquery.ui.position.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    15825 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/require-2.1.22.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2967 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/slick.core.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    21767 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/slick.dataview.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     8665 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/slick.editors.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)      918 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/slick.formatters.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    57026 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/slick.grid.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    28250 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/spectrum.min.js
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.802065 emperor-1.0.4/emperor/support_files/vendor/js/three.js-plugins/
+-rw-r--r--   0 yoshiki    (501) staff       (20)    26045 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/three.js-plugins/CanvasRenderer.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    24519 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/three.js-plugins/OrbitControls.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    25361 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/three.js-plugins/Projector.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    13336 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/three.js-plugins/SVGRenderer.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     6507 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/three.js-plugins/SelectionBox.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2523 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/three.js-plugins/SelectionHelper.js
+-rwxr-xr-x   0 yoshiki    (501) staff       (20)   618895 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/three.min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    16449 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/support_files/vendor/js/underscore-min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    14882 2023-07-10 15:31:50.000000 emperor-1.0.4/emperor/util.py
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.756856 emperor-1.0.4/emperor.egg-info/
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2738 2023-07-10 15:34:39.000000 emperor-1.0.4/emperor.egg-info/PKG-INFO
+-rw-r--r--   0 yoshiki    (501) staff       (20)     9410 2023-07-10 15:34:39.000000 emperor-1.0.4/emperor.egg-info/SOURCES.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)        1 2023-07-10 15:34:39.000000 emperor-1.0.4/emperor.egg-info/dependency_links.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)      322 2023-07-10 15:34:39.000000 emperor-1.0.4/emperor.egg-info/requires.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)       14 2023-07-10 15:34:39.000000 emperor-1.0.4/emperor.egg-info/top_level.txt
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.808337 emperor-1.0.4/images/
+-rw-r--r--   0 yoshiki    (501) staff       (20)    56076 2023-07-10 15:31:50.000000 emperor-1.0.4/images/emperor-animation.gif
+-rw-r--r--   0 yoshiki    (501) staff       (20)   843687 2023-07-10 15:31:50.000000 emperor-1.0.4/images/emperor-animation.psd
+-rw-r--r--   0 yoshiki    (501) staff       (20)    57353 2023-07-10 15:31:50.000000 emperor-1.0.4/images/emperor-frame1.ai
+-rw-r--r--   0 yoshiki    (501) staff       (20)    22814 2023-07-10 15:31:50.000000 emperor-1.0.4/images/emperor-frame1.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)    61587 2023-07-10 15:31:50.000000 emperor-1.0.4/images/emperor-frame2.ai
+-rw-r--r--   0 yoshiki    (501) staff       (20)    20985 2023-07-10 15:31:50.000000 emperor-1.0.4/images/emperor-frame2.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)    61996 2023-07-10 15:31:50.000000 emperor-1.0.4/images/emperor-frame3.ai
+-rw-r--r--   0 yoshiki    (501) staff       (20)    21045 2023-07-10 15:31:50.000000 emperor-1.0.4/images/emperor-frame3.png
+-rw-r--r--   0 yoshiki    (501) staff       (20)   199499 2023-07-10 15:31:50.000000 emperor-1.0.4/images/emperor-logos.ai
+-rw-r--r--   0 yoshiki    (501) staff       (20)       38 2023-07-10 15:34:39.837624 emperor-1.0.4/setup.cfg
+-rw-r--r--   0 yoshiki    (501) staff       (20)     2902 2023-07-10 15:34:11.000000 emperor-1.0.4/setup.py
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.813027 emperor-1.0.4/tests/
+-rw-r--r--   0 yoshiki    (501) staff       (20)      349 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/__init__.py
+-rw-r--r--   0 yoshiki    (501) staff       (20)    46193 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/_test_core_strings.py
+-rw-r--r--   0 yoshiki    (501) staff       (20)    79784 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/_test_format_strings.py
+-rwxr-xr-x   0 yoshiki    (501) staff       (20)     4406 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/all_tests.py
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.822405 emperor-1.0.4/tests/javascript_tests/
+-rw-r--r--   0 yoshiki    (501) staff       (20)     9403 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/index.html
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.823299 emperor-1.0.4/tests/javascript_tests/qunit/
+-rw-r--r--   0 yoshiki    (501) staff       (20)     3719 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/qunit/qunit-min.css
+-rw-r--r--   0 yoshiki    (501) staff       (20)    26633 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/qunit/qunit-min.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    12349 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/runner.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    15422 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_animate.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    15215 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_animations_controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    12832 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_axes_controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    38327 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_color_view_controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    30010 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_decomposition_model.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    35857 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_decomposition_view.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     8999 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_draw.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     9092 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_opacity_view_controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     3744 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_plottable.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    10004 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_scalar_view_controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    10593 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_scale_view_controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    33555 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_sceneplotview3d.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     8081 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_shape_controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    23305 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_trajectory.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)     7102 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_util.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    22664 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_view_controller.js
+-rw-r--r--   0 yoshiki    (501) staff       (20)    10992 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/javascript_tests/test_visibility_controller.js
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.733745 emperor-1.0.4/tests/scripts_test_data/
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.826598 emperor-1.0.4/tests/scripts_test_data/make_emperor/
+-rw-r--r--   0 yoshiki    (501) staff       (20)      982 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/Fasting_Map.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1067 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/Fasting_Map_modified.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)      582 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/biplot.txt
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.827616 emperor-1.0.4/tests/scripts_test_data/make_emperor/compare/
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1725 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/compare/pcoa_unweighted_unifrac_rarefaction_110_0.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1745 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/compare/pcoa_unweighted_unifrac_rarefaction_110_1.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1530 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/euclidian_pc.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1105 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/makefolders.sh
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1149 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/otu_table_L3.txt
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.832631 emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1725 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_0.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1745 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_1.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1734 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_2.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1734 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_3.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1743 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_4.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1736 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_5.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1741 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_6.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1735 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_7.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1726 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_8.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1736 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_9.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)     1735 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)    75254 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/test_core.py
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.834243 emperor-1.0.4/tests/test_data/
+-rw-r--r--   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/test_data/.some-hidden-file
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.835669 emperor-1.0.4/tests/test_data/dir-with-only-hidden-files/
+-rw-r--r--   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/test_data/dir-with-only-hidden-files/.1.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/test_data/dir-with-only-hidden-files/.2.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/test_data/dir-with-only-hidden-files/.3.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/test_data/dir-with-only-hidden-files/.4.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/test_data/procrustes_results.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/test_data/unweighted_unifrac_pc_transformed_reference.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/test_data/weighted_unifrac_pc_transformed_q1.txt
+-rw-r--r--   0 yoshiki    (501) staff       (20)     4129 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/test_format.py
+-rw-r--r--   0 yoshiki    (501) staff       (20)     4452 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/test_pandas.py
+drwxr-xr-x   0 yoshiki    (501) staff       (20)        0 2023-07-10 15:34:39.836534 emperor-1.0.4/tests/test_qiime_backports/
+-rwxr-xr-x   0 yoshiki    (501) staff       (20)     4777 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/test_qiime_backports/test_make_3d_plots.py
+-rwxr-xr-x   0 yoshiki    (501) staff       (20)     7690 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/test_qiime_backports/test_util.py
+-rw-r--r--   0 yoshiki    (501) staff       (20)    26287 2023-07-10 15:31:50.000000 emperor-1.0.4/tests/test_util.py
```

### Comparing `emperor-1.0.3/ChangeLog.md` & `emperor-1.0.4/ChangeLog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,31 @@
 Emperor ChangeLog
 =================
 
-# Emperor 1.0.3
----------------
+# Emperor 1.0.4 (10 Jul 2023)
+-----------------------------
+
+### Bug Fixes
+
+* Update remote URL to no longer use rawgit.
+  ([#751](https://github.com/biocore/emperor/issues/751)).
+
+### New Features
+
+* Add `Toggle Visible` button to `Visibility` tab.
+
+### Miscellaneous
+
+* Pin Sphinx version to be less than 4.0.
+* Jupyter templates no longer require jQuery to add the CSS headers.
+* Limit jinja2 version for doc dependencies in setup.py. Allowed versions are: `>=2.9` and `<3.1`.
+* Fix broken test suite with Pandas >=1.5 ([#810](https://github.com/biocore/emperor/issues/810)).
+
+# Emperor 1.0.3 (14 Apr 2021)
+-----------------------------
 
 ### Bug Fixes
 
 * Fix a bug causing slight inaccuracies in how color gradients were drawn
   ([#788](https://github.com/biocore/emperor/issues/788)).
 
 ### New Features
```

### Comparing `emperor-1.0.3/INSTALL.md` & `emperor-1.0.4/INSTALL.md`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/LICENSE.md` & `emperor-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/PKG-INFO` & `emperor-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,17 @@
 Metadata-Version: 2.1
 Name: emperor
-Version: 1.0.3
+Version: 1.0.4
 Summary: Emperor
 Home-page: http://github.com/biocore/emperor
 Author: Antonio Gonzalez Pena, Meg Pirrung & Yoshiki Vazquez Baeza
 Author-email: yoshiki89@gmail.com
 Maintainer: Emperor development team
 Maintainer-email: yoshiki89@gmail.com
 License: BSD-3-Clause
-Description: Emperor
-        =======
-        
-        [![Join the chat at https://gitter.im/biocore/emperor](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/biocore/emperor?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![](https://github.com/biocore/emperor/workflows/Emperor%20CI/badge.svg)](https://github.com/biocore/emperor/actions) [![Coverage Status](https://coveralls.io/repos/biocore/emperor/badge.svg)](https://coveralls.io/r/biocore/emperor)
-        
-        Emperor is a next-generation tool for the analysis and visualization of large microbial ecology datasets. Amongst its many features, Emperor provides a modern user interface that can be rapidly adjusted to your data analysis workflow.
-        
-        To start using Emperor, please refer to the [installation notes](INSTALL.md).
-        
-        Before contributing code to Emperor, please familiarize yourself with the [contributing guidelines](CONTRIBUTING.md).
-        
-        ## Usage
-        
-        You can start using Emperor through [QIIME 2](https://qiime2.org)'s [interfaces](https://docs.qiime2.org/2021.2/interfaces/) (the command line or the graphical user interface), or alternatively using the Python interface (compatible with the Jupyter notebook, see [this example](http://nbviewer.jupyter.org/github/biocore/emperor/blob/new-api/examples/keyboard.ipynb)). For more details, refer to our [online documentation](http://emperor.microbio.me).
-        
-        ## Publications
-        
-        - [EMPeror: a tool for visualizing high-throughput microbial community data](https://www.ncbi.nlm.nih.gov/pubmed/24280061). GigaScience, 2013.
-        
-        - [Bringing the Dynamic Microbiome to Life with Animations](https://www.ncbi.nlm.nih.gov/pubmed/28081445). Cell Host & Microbe, 2016.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -42,7 +20,29 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: all
+License-File: LICENSE.md
+
+Emperor
+=======
+
+[![Join the chat at https://gitter.im/biocore/emperor](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/biocore/emperor?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![](https://github.com/biocore/emperor/workflows/Emperor%20CI/badge.svg)](https://github.com/biocore/emperor/actions) [![Coverage Status](https://coveralls.io/repos/biocore/emperor/badge.svg)](https://coveralls.io/r/biocore/emperor)
+
+Emperor is a next-generation tool for the analysis and visualization of large microbial ecology datasets. Amongst its many features, Emperor provides a modern user interface that can be rapidly adjusted to your data analysis workflow.
+
+To start using Emperor, please refer to the [installation notes](INSTALL.md).
+
+Before contributing code to Emperor, please familiarize yourself with the [contributing guidelines](CONTRIBUTING.md).
+
+## Usage
+
+You can start using Emperor through [QIIME 2](https://qiime2.org)'s [interfaces](https://docs.qiime2.org/2021.2/interfaces/) (the command line or the graphical user interface), or alternatively using the Python interface (compatible with the Jupyter notebook, see [this example](http://nbviewer.jupyter.org/github/biocore/emperor/blob/new-api/examples/keyboard.ipynb)). For more details, refer to our [online documentation](http://emperor.microbio.me).
+
+## Publications
+
+- [EMPeror: a tool for visualizing high-throughput microbial community data](https://www.ncbi.nlm.nih.gov/pubmed/24280061). GigaScience, 2013.
+
+- [Bringing the Dynamic Microbiome to Life with Animations](https://www.ncbi.nlm.nih.gov/pubmed/28081445). Cell Host & Microbe, 2016.
```

### Comparing `emperor-1.0.3/README.md` & `emperor-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/Makefile` & `emperor-1.0.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/README.md` & `emperor-1.0.4/doc/README.md`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/bootstrap/css/bootstrap-theme.min.css` & `emperor-1.0.4/doc/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/bootstrap/css/bootstrap.min.css` & `emperor-1.0.4/doc/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/bootstrap/fonts/glyphicons-halflings-regular.eot` & `emperor-1.0.4/doc/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/bootstrap/fonts/glyphicons-halflings-regular.svg` & `emperor-1.0.4/doc/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `emperor-1.0.4/doc/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/bootstrap/fonts/glyphicons-halflings-regular.woff` & `emperor-1.0.4/doc/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `emperor-1.0.4/doc/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/bootstrap/js/bootstrap.min.js` & `emperor-1.0.4/doc/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/bootstrap/js/jquery-2.2.3.min.js` & `emperor-1.0.4/doc/bootstrap/js/jquery-2.2.3.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/files/files.zip` & `emperor-1.0.4/doc/files/files.zip`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/img/emperor_heading.png` & `emperor-1.0.4/doc/img/emperor_heading.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/img/favicon.ico` & `emperor-1.0.4/doc/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/img/sample_1.png` & `emperor-1.0.4/doc/img/sample_1.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/index.html` & `emperor-1.0.4/doc/index.html`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/installation_index.html` & `emperor-1.0.4/doc/installation_index.html`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/source/_static/copybutton.js` & `emperor-1.0.4/doc/source/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/source/_static/style.css` & `emperor-1.0.4/doc/source/_static/style.css`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/source/_templates/autosummary/class.rst` & `emperor-1.0.4/doc/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/source/_templates/layout.html` & `emperor-1.0.4/doc/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/source/conf.py` & `emperor-1.0.4/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,18 +54,18 @@
 copyright = u'2014, Emperor Development Team'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '1.0.3'
+version = '1.0.4'
 
 # The full version, including alpha/beta/rc tags.
-release = '1.0.3'
+release = '1.0.4'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `emperor-1.0.3/doc/source/examples.rst` & `emperor-1.0.4/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/source/formats.rst` & `emperor-1.0.4/doc/source/formats.rst`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/source/index.rst` & `emperor-1.0.4/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/source/js_integration.rst` & `emperor-1.0.4/doc/source/js_integration.rst`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/source/tutorials/animations.rst` & `emperor-1.0.4/doc/source/tutorials/animations.rst`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/source/tutorials/trajectories.png` & `emperor-1.0.4/doc/source/tutorials/trajectories.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/doc/tutorial_index.html` & `emperor-1.0.4/doc/tutorial_index.html`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/__init__.py` & `emperor-1.0.4/emperor/__init__.py`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/_format_strings.py` & `emperor-1.0.4/emperor/_format_strings.py`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/_pandas.py` & `emperor-1.0.4/emperor/_pandas.py`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/core.py` & `emperor-1.0.4/emperor/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 from emperor import __version__ as emperor_version
 from emperor.util import (get_emperor_support_files_dir,
                           preprocess_coords_file, resolve_stable_url,
                           validate_and_process_custom_axes, EmperorWarning)
 
 # we are going to use this remote location to load external resources
-REMOTE_URL = ('https://cdn.rawgit.com/biocore/emperor/%s/emperor'
-              '/support_files')
+REMOTE_URL = ('https://cdn.jsdelivr.net/gh/biocore/emperor@%s/emperor/'
+              'support_files')
 LOCAL_URL = "/nbextensions/emperor/support_files"
 
 BASE_DEPENDENCIES_PATH = 'base-dependencies.html'
 STYLE_PATH = 'style-template.html'
 LOGIC_PATH = 'logic-template.html'
 HTML_CONTAINER_PATH = 'html-container-template.html'
 
@@ -302,17 +302,17 @@
 
         if difference == ordination_elements:
             raise ValueError('None of the %s identifiers match between the'
                              ' metadata and the coordinates. Verify that you '
                              'are using metadata and coordinates corresponding'
                              ' to the same dataset.' % kind)
 
+        # sort the elements so we have a deterministic output
+        difference = sorted([str(i) for i in difference])
         if difference and not ignore_missing_samples:
-            # sort the elements so we have a deterministic output
-            difference = sorted([str(i) for i in difference])
 
             # if there's more than 5 missing elements, truncate the list
             if len(difference) > 5:
                 elements = ', '.join(difference[:5])
                 suffix = ("Showing only the first 5 %ss out of %d: %s ..." %
                           (kind, len(difference), elements))
             else:
```

### Comparing `emperor-1.0.3/emperor/format.py` & `emperor-1.0.4/emperor/format.py`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/qiime_backports/make_3d_plots.py` & `emperor-1.0.4/emperor/qiime_backports/make_3d_plots.py`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/qiime_backports/util.py` & `emperor-1.0.4/emperor/qiime_backports/util.py`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/README.md` & `emperor-1.0.4/emperor/support_files/README.md`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/css/emperor.css` & `emperor-1.0.4/emperor/support_files/css/emperor.css`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/img/emperor.png` & `emperor-1.0.4/emperor/support_files/img/emperor.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/img/favicon.ico` & `emperor-1.0.4/emperor/support_files/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/img/pause.png` & `emperor-1.0.4/emperor/support_files/img/pause.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/img/play.png` & `emperor-1.0.4/emperor/support_files/img/play.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/img/reset.png` & `emperor-1.0.4/emperor/support_files/img/reset.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/abc-view-controller.js` & `emperor-1.0.4/emperor/support_files/js/abc-view-controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/animate.js` & `emperor-1.0.4/emperor/support_files/js/animate.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/animations-controller.js` & `emperor-1.0.4/emperor/support_files/js/animations-controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/axes-controller.js` & `emperor-1.0.4/emperor/support_files/js/axes-controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/color-editor.js` & `emperor-1.0.4/emperor/support_files/js/color-editor.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/color-view-controller.js` & `emperor-1.0.4/emperor/support_files/js/color-view-controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/controller.js` & `emperor-1.0.4/emperor/support_files/js/controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/draw.js` & `emperor-1.0.4/emperor/support_files/js/draw.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/model.js` & `emperor-1.0.4/emperor/support_files/js/model.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/multi-model.js` & `emperor-1.0.4/emperor/support_files/js/multi-model.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/opacity-view-controller.js` & `emperor-1.0.4/emperor/support_files/js/opacity-view-controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/scale-editor.js` & `emperor-1.0.4/emperor/support_files/js/scale-editor.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/scale-view-controller.js` & `emperor-1.0.4/emperor/support_files/js/scale-view-controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/sceneplotview3d.js` & `emperor-1.0.4/emperor/support_files/js/sceneplotview3d.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/shape-controller.js` & `emperor-1.0.4/emperor/support_files/js/shape-controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/shape-editor.js` & `emperor-1.0.4/emperor/support_files/js/shape-editor.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/shapes.js` & `emperor-1.0.4/emperor/support_files/js/shapes.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/trajectory.js` & `emperor-1.0.4/emperor/support_files/js/trajectory.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/ui-state.js` & `emperor-1.0.4/emperor/support_files/js/ui-state.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/util.js` & `emperor-1.0.4/emperor/support_files/js/util.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/view-controller.js` & `emperor-1.0.4/emperor/support_files/js/view-controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/view.js` & `emperor-1.0.4/emperor/support_files/js/view.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/js/visibility-controller.js` & `emperor-1.0.4/emperor/support_files/js/visibility-controller.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -72,14 +72,29 @@
                 formatter: Slick.Formatters.Checkmark,
                 editor: Slick.Editors.Checkbox
             }
         };
 
         EmperorAttributeABC.call(this, uiState, container, title, helpmenu,
             decompViewDict, options);
+
+        this.$applyAll = $("<input type='button' value='Toggle Visible'>").css({
+            'margin': '0 auto',
+            'display': 'block'
+        });
+        this.$header.append(this.$applyAll);
+
+        $(function() {
+            scope.$applyAll.hide();
+            scope.$applyAll.on('click', function() {
+                scope.toggleVisibility();
+            });
+        });
+
+
         return this;
     }
     VisibilityController.prototype = Object.create(EmperorAttributeABC.prototype);
     VisibilityController.prototype.constructor = EmperorAttributeABC;
 
     /**
      *
@@ -106,9 +121,46 @@
      * @param {Object[]} group Array of objects that should be changed in scope
      */
     VisibilityController.prototype.setPlottableAttributes =
         function(scope, visible, group) {
             scope.setVisibility(visible, group);
         };
 
+    /**
+     * Sets whether or not elements in the tab can be modified.
+     *
+     * @param {Boolean} trulse option to enable elements.
+     */
+    VisibilityController.prototype.setEnabled = function(trulse) {
+        EmperorAttributeABC.prototype.setEnabled.call(this, trulse);
+
+        // prevent errors when this method is called before the element exists
+        if (this.$applyAll) {
+            if (trulse) {
+                this.$applyAll.show();
+            } else {
+                this.$applyAll.hide();
+            }
+        }
+    };
+
+    /**
+     * Toggle visible objects
+     */
+    VisibilityController.prototype.toggleVisibility = function() {
+        var view = this.getView();
+
+        var groups = this.getSlickGridDataset();
+        _.each(groups, function(group) {
+
+            // toggle the value in the data container and update the view
+            group.value = Boolean(true ^ group.value);
+            view.setVisibility(group.value, group.plottables);
+        });
+
+        // lastly, update the grid table
+        this.setSlickGridDataset(groups);
+    };
+
+
     return VisibilityController;
 });
```

### Comparing `emperor-1.0.3/emperor/support_files/templates/logic-template.html` & `emperor-1.0.4/emperor/support_files/templates/logic-template.html`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/templates/standalone-template.html` & `emperor-1.0.4/emperor/support_files/templates/standalone-template.html`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/templates/style-template.html` & `emperor-1.0.4/emperor/support_files/templates/style-template.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 <script type="text/javascript">
-{% raw %}
-if ($("#emperor-css").length == 0){{
-    $("head").append([
-{% endraw %}
+if (document.querySelector("#emperor-css") === null){
+    document.querySelector("head").insertAdjacentHTML("beforeend",[
         '<link id="emperor-css" rel="stylesheet" type="text/css" href="{{ base_url }}/css/emperor.css">',
         '<link rel="stylesheet" type="text/css" href="{{ base_url }}/vendor/css/jquery-ui.min.css">',
         '<link rel="stylesheet" type="text/css" href="{{ base_url }}/vendor/css/slick.grid.min.css">',
         '<link rel="stylesheet" type="text/css" href="{{ base_url }}/vendor/css/spectrum.min.css">',
         '<link rel="stylesheet" type="text/css" href="{{ base_url }}/vendor/css/chosen.min.css">',
         '<link rel="stylesheet" type="text/css" href="{{ base_url }}/vendor/css/jquery.contextMenu.min.css">'
     ]);
-}}
+}
 </script>
```

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/chosen-sprite.png` & `emperor-1.0.4/emperor/support_files/vendor/css/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/chosen-sprite@2x.png` & `emperor-1.0.4/emperor/support_files/vendor/css/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/chosen.min.css` & `emperor-1.0.4/emperor/support_files/vendor/css/chosen.min.css`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/font/context-menu-icons.eot` & `emperor-1.0.4/emperor/support_files/vendor/css/font/context-menu-icons.eot`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/font/context-menu-icons.ttf` & `emperor-1.0.4/emperor/support_files/vendor/css/font/context-menu-icons.ttf`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/font/context-menu-icons.woff` & `emperor-1.0.4/emperor/support_files/vendor/css/font/context-menu-icons.woff`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/font/context-menu-icons.woff2` & `emperor-1.0.4/emperor/support_files/vendor/css/font/context-menu-icons.woff2`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/images/ui-icons_222222_256x240.png` & `emperor-1.0.4/emperor/support_files/vendor/css/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/images/ui-icons_2e83ff_256x240.png` & `emperor-1.0.4/emperor/support_files/vendor/css/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/images/ui-icons_454545_256x240.png` & `emperor-1.0.4/emperor/support_files/vendor/css/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/images/ui-icons_888888_256x240.png` & `emperor-1.0.4/emperor/support_files/vendor/css/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/images/ui-icons_cd0a0a_256x240.png` & `emperor-1.0.4/emperor/support_files/vendor/css/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/jquery-ui.min.css` & `emperor-1.0.4/emperor/support_files/vendor/css/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/jquery.contextMenu.min.css` & `emperor-1.0.4/emperor/support_files/vendor/css/jquery.contextMenu.min.css`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/slick.grid.min.css` & `emperor-1.0.4/emperor/support_files/vendor/css/slick.grid.min.css`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/css/spectrum.min.css` & `emperor-1.0.4/emperor/support_files/vendor/css/spectrum.min.css`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/Blob.js` & `emperor-1.0.4/emperor/support_files/vendor/js/Blob.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/FileSaver.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/FileSaver.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/canvas-toBlob.js` & `emperor-1.0.4/emperor/support_files/vendor/js/canvas-toBlob.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/chosen.jquery.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/chroma.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/chroma.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/d3.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/jquery-2.1.4.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/jquery-2.1.4.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/jquery-ui.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/jquery.contextMenu.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/jquery.contextMenu.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/jquery.event.drag-2.2.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/jquery.event.drag-2.2.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/jquery.ui.position.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/jquery.ui.position.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/require-2.1.22.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/require-2.1.22.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/slick.core.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/slick.core.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/slick.dataview.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/slick.dataview.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/slick.editors.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/slick.editors.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/slick.formatters.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/slick.formatters.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/slick.grid.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/slick.grid.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/spectrum.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/spectrum.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/three.js-plugins/CanvasRenderer.js` & `emperor-1.0.4/emperor/support_files/vendor/js/three.js-plugins/CanvasRenderer.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/three.js-plugins/OrbitControls.js` & `emperor-1.0.4/emperor/support_files/vendor/js/three.js-plugins/OrbitControls.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/three.js-plugins/Projector.js` & `emperor-1.0.4/emperor/support_files/vendor/js/three.js-plugins/Projector.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/three.js-plugins/SVGRenderer.js` & `emperor-1.0.4/emperor/support_files/vendor/js/three.js-plugins/SVGRenderer.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/three.js-plugins/SelectionBox.js` & `emperor-1.0.4/emperor/support_files/vendor/js/three.js-plugins/SelectionBox.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/three.js-plugins/SelectionHelper.js` & `emperor-1.0.4/emperor/support_files/vendor/js/three.js-plugins/SelectionHelper.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/three.min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/three.min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/support_files/vendor/js/underscore-min.js` & `emperor-1.0.4/emperor/support_files/vendor/js/underscore-min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/emperor/util.py` & `emperor-1.0.4/emperor/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -359,20 +359,28 @@
         A URL that points to the emperor's resources.
 
     Notes
     -----
     An EmperorWarning is shown when development URLs are used.
     """
     if 'dev' in version:
-        warnings.warn("Plots generated with `remote=True` using a development "
-                      "version of Emperor, may fail to load in the future "
-                      "(only the logo may be displayed instead of the plot). "
-                      "To avoid this, use a release version of Emperor.",
+        warnings.warn("Plots generated with `remote=True` using a development"
+                      " version of Emperor may fail to load (only the logo "
+                      "may be displayed instead of the plot). Using this flag"
+                      " might also load outdated JS or CSS files. If you are "
+                      "doing development, we recommend running nbinstall and "
+                      "sourcing JS and CSS files locally. Otherwise use "
+                      "`remote=True` only with a release version of Emperor.",
                       EmperorWarning)
 
-        # this will need to be fixed when new-api is merged to master
-        return base_url % 'new-api'
-    else:
-        # version names are changed for git tags from betaxx to -beta.xx
-        if 'b' in version:
-            version = version.replace('b', '-beta.')
-        return base_url % version
+        version = version.rstrip('.dev0')
+
+    if 'b' in version:
+        # Version numbers appear in slightly different formats in different
+        # places. Setuptools converts 1.0.0beta19 into 1.0.0b19. This is then
+        # converted to 1.0.0-beta.19 for the git tag.
+        #
+        # The replacement below makes the setuptools version string match what
+        # the git tag will look like.
+        version = version.replace('b', '-beta.')
+
+    return base_url % version
```

### Comparing `emperor-1.0.3/emperor.egg-info/PKG-INFO` & `emperor-1.0.4/emperor.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,17 @@
 Metadata-Version: 2.1
 Name: emperor
-Version: 1.0.3
+Version: 1.0.4
 Summary: Emperor
 Home-page: http://github.com/biocore/emperor
 Author: Antonio Gonzalez Pena, Meg Pirrung & Yoshiki Vazquez Baeza
 Author-email: yoshiki89@gmail.com
 Maintainer: Emperor development team
 Maintainer-email: yoshiki89@gmail.com
 License: BSD-3-Clause
-Description: Emperor
-        =======
-        
-        [![Join the chat at https://gitter.im/biocore/emperor](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/biocore/emperor?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![](https://github.com/biocore/emperor/workflows/Emperor%20CI/badge.svg)](https://github.com/biocore/emperor/actions) [![Coverage Status](https://coveralls.io/repos/biocore/emperor/badge.svg)](https://coveralls.io/r/biocore/emperor)
-        
-        Emperor is a next-generation tool for the analysis and visualization of large microbial ecology datasets. Amongst its many features, Emperor provides a modern user interface that can be rapidly adjusted to your data analysis workflow.
-        
-        To start using Emperor, please refer to the [installation notes](INSTALL.md).
-        
-        Before contributing code to Emperor, please familiarize yourself with the [contributing guidelines](CONTRIBUTING.md).
-        
-        ## Usage
-        
-        You can start using Emperor through [QIIME 2](https://qiime2.org)'s [interfaces](https://docs.qiime2.org/2021.2/interfaces/) (the command line or the graphical user interface), or alternatively using the Python interface (compatible with the Jupyter notebook, see [this example](http://nbviewer.jupyter.org/github/biocore/emperor/blob/new-api/examples/keyboard.ipynb)). For more details, refer to our [online documentation](http://emperor.microbio.me).
-        
-        ## Publications
-        
-        - [EMPeror: a tool for visualizing high-throughput microbial community data](https://www.ncbi.nlm.nih.gov/pubmed/24280061). GigaScience, 2013.
-        
-        - [Bringing the Dynamic Microbiome to Life with Animations](https://www.ncbi.nlm.nih.gov/pubmed/28081445). Cell Host & Microbe, 2016.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -42,7 +20,29 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: all
+License-File: LICENSE.md
+
+Emperor
+=======
+
+[![Join the chat at https://gitter.im/biocore/emperor](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/biocore/emperor?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![](https://github.com/biocore/emperor/workflows/Emperor%20CI/badge.svg)](https://github.com/biocore/emperor/actions) [![Coverage Status](https://coveralls.io/repos/biocore/emperor/badge.svg)](https://coveralls.io/r/biocore/emperor)
+
+Emperor is a next-generation tool for the analysis and visualization of large microbial ecology datasets. Amongst its many features, Emperor provides a modern user interface that can be rapidly adjusted to your data analysis workflow.
+
+To start using Emperor, please refer to the [installation notes](INSTALL.md).
+
+Before contributing code to Emperor, please familiarize yourself with the [contributing guidelines](CONTRIBUTING.md).
+
+## Usage
+
+You can start using Emperor through [QIIME 2](https://qiime2.org)'s [interfaces](https://docs.qiime2.org/2021.2/interfaces/) (the command line or the graphical user interface), or alternatively using the Python interface (compatible with the Jupyter notebook, see [this example](http://nbviewer.jupyter.org/github/biocore/emperor/blob/new-api/examples/keyboard.ipynb)). For more details, refer to our [online documentation](http://emperor.microbio.me).
+
+## Publications
+
+- [EMPeror: a tool for visualizing high-throughput microbial community data](https://www.ncbi.nlm.nih.gov/pubmed/24280061). GigaScience, 2013.
+
+- [Bringing the Dynamic Microbiome to Life with Animations](https://www.ncbi.nlm.nih.gov/pubmed/28081445). Cell Host & Microbe, 2016.
```

### Comparing `emperor-1.0.3/emperor.egg-info/SOURCES.txt` & `emperor-1.0.4/emperor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/images/emperor-animation.gif` & `emperor-1.0.4/images/emperor-animation.gif`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/images/emperor-animation.psd` & `emperor-1.0.4/images/emperor-animation.psd`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/images/emperor-frame1.ai` & `emperor-1.0.4/images/emperor-frame1.ai`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/images/emperor-frame1.png` & `emperor-1.0.4/images/emperor-frame1.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/images/emperor-frame2.ai` & `emperor-1.0.4/images/emperor-frame2.ai`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/images/emperor-frame2.png` & `emperor-1.0.4/images/emperor-frame2.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/images/emperor-frame3.ai` & `emperor-1.0.4/images/emperor-frame3.ai`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/images/emperor-frame3.png` & `emperor-1.0.4/images/emperor-frame3.png`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/images/emperor-logos.ai` & `emperor-1.0.4/images/emperor-logos.ai`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/setup.py` & `emperor-1.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file LICENSE.md, distributed with this software.
 # ----------------------------------------------------------------------------
 
 from setuptools import setup, find_packages
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 __maintainer__ = "Emperor development team"
 __email__ = "yoshiki89@gmail.com"
 
 # based on the text found in github.com/qiime/pynast
 classes = """
     Development Status :: 5 - Production/Stable
     License :: OSI Approved :: BSD License
@@ -32,15 +32,16 @@
 classifiers = [s.strip() for s in classes.split('\n') if s]
 
 with open('README.md') as f:
     long_description = f.read()
 
 base = ["numpy >= 1.7", "scipy >= 0.17.0", "click", "pandas",
         "scikit-bio >= 0.4.1", "jinja2 >= 2.9", "future"]
-doc = ["Sphinx", "sphinx-bootstrap-theme", "numpydoc"]
+doc = ["Sphinx<4", "jinja2 >= 2.9, < 3.1", "sphinx-bootstrap-theme",
+       "numpydoc"]
 test = ["pep8", "flake8", "nose"]
 all_deps = base + doc + test
 
 setup(
     name='emperor',
     version=__version__,
     description='Emperor',
```

### Comparing `emperor-1.0.3/tests/_test_core_strings.py` & `emperor-1.0.4/tests/_test_core_strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,26 +51,24 @@
 Biplot	0	0
 
 Site constraints	0	0
 """
 
 HTML_STRING = u"""
 <script type="text/javascript">
-
-if ($("#emperor-css").length == 0){{
-    $("head").append([
-
+if (document.querySelector("#emperor-css") === null){
+    document.querySelector("head").insertAdjacentHTML("beforeend",[
         '<link id="emperor-css" rel="stylesheet" type="text/css" href="https://cdn.rawgit.com/biocore/emperor/new-api/emperor/support_files/css/emperor.css">',
         '<link rel="stylesheet" type="text/css" href="https://cdn.rawgit.com/biocore/emperor/new-api/emperor/support_files/vendor/css/jquery-ui.min.css">',
         '<link rel="stylesheet" type="text/css" href="https://cdn.rawgit.com/biocore/emperor/new-api/emperor/support_files/vendor/css/slick.grid.min.css">',
         '<link rel="stylesheet" type="text/css" href="https://cdn.rawgit.com/biocore/emperor/new-api/emperor/support_files/vendor/css/spectrum.min.css">',
         '<link rel="stylesheet" type="text/css" href="https://cdn.rawgit.com/biocore/emperor/new-api/emperor/support_files/vendor/css/chosen.min.css">',
         '<link rel="stylesheet" type="text/css" href="https://cdn.rawgit.com/biocore/emperor/new-api/emperor/support_files/vendor/css/jquery.contextMenu.min.css">'
     ]);
-}}
+}
 </script>
 
 <div id='emperor-notebook-0x9cb72f54' style="position: relative; width:100%; height:500px;">
   <div class='loading' style="position: absolute;top: 50%;left: 50%;margin-left: -229px; margin-top: -59px; z-index: 10000;height:118px;width:458px;padding:0px"><img src='https://cdn.rawgit.com/biocore/emperor/new-api/emperor/support_files/img/emperor.png' alt='Emperor resources missing. Expected them to be found in https://cdn.rawgit.com/biocore/emperor/new-api/emperor/support_files'></div>
 </div>
 </div>
 <script type="text/javascript">
@@ -237,26 +235,24 @@
     <title>Emperor</title>
     <!-- core dependencies that are otherwise included via the jupyter notebook -->
 <script src="./some-local-path//vendor/js/require-2.1.22.min.js"></script>
 <script src="./some-local-path//vendor/js/jquery-2.1.4.min.js"></script>
     <meta charset="utf-8">
 
     <script type="text/javascript">
-
-if ($("#emperor-css").length == 0){{
-    $("head").append([
-
+if (document.querySelector("#emperor-css") === null){
+    document.querySelector("head").insertAdjacentHTML("beforeend",[
         '<link id="emperor-css" rel="stylesheet" type="text/css" href="./some-local-path//css/emperor.css">',
         '<link rel="stylesheet" type="text/css" href="./some-local-path//vendor/css/jquery-ui.min.css">',
         '<link rel="stylesheet" type="text/css" href="./some-local-path//vendor/css/slick.grid.min.css">',
         '<link rel="stylesheet" type="text/css" href="./some-local-path//vendor/css/spectrum.min.css">',
         '<link rel="stylesheet" type="text/css" href="./some-local-path//vendor/css/chosen.min.css">',
         '<link rel="stylesheet" type="text/css" href="./some-local-path//vendor/css/jquery.contextMenu.min.css">'
     ]);
-}}
+}
 </script>
 
 
     <style>
       #emperor-notebook-0x9cb72f54 {
         height:100vh !important;
         padding: 0px !important;
@@ -431,26 +427,24 @@
 
 }); // END REQUIRE.JS block
     </script>
   </body>
 </html>"""
 
 STYLE_STRING = """<script type="text/javascript">
-
-if ($("#emperor-css").length == 0){{
-    $("head").append([
-
+if (document.querySelector("#emperor-css") === null){
+    document.querySelector("head").insertAdjacentHTML("beforeend",[
         '<link id="emperor-css" rel="stylesheet" type="text/css" href="/nbextensions/emperor/support_files/css/emperor.css">',
         '<link rel="stylesheet" type="text/css" href="/nbextensions/emperor/support_files/vendor/css/jquery-ui.min.css">',
         '<link rel="stylesheet" type="text/css" href="/nbextensions/emperor/support_files/vendor/css/slick.grid.min.css">',
         '<link rel="stylesheet" type="text/css" href="/nbextensions/emperor/support_files/vendor/css/spectrum.min.css">',
         '<link rel="stylesheet" type="text/css" href="/nbextensions/emperor/support_files/vendor/css/chosen.min.css">',
         '<link rel="stylesheet" type="text/css" href="/nbextensions/emperor/support_files/vendor/css/jquery.contextMenu.min.css">'
     ]);
-}}
+}
 </script>
 """
 
 DIV_STRING = """<div id='emperor-notebook-0x9cb72f54' style="position: relative; width:100%; height:500px;">
   <div class='loading' style="position: absolute;top: 50%;left: 50%;margin-left: -229px; margin-top: -59px; z-index: 10000;height:118px;width:458px;padding:0px"><img src='/nbextensions/emperor/support_files/img/emperor.png' alt='Emperor resources missing. Expected them to be found in /nbextensions/emperor/support_files'></div>
 </div>
 </div>"""
```

### Comparing `emperor-1.0.3/tests/_test_format_strings.py` & `emperor-1.0.4/tests/_test_format_strings.py`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/all_tests.py` & `emperor-1.0.4/tests/all_tests.py`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/index.html` & `emperor-1.0.4/tests/javascript_tests/index.html`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/qunit/qunit-min.css` & `emperor-1.0.4/tests/javascript_tests/qunit/qunit-min.css`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/qunit/qunit-min.js` & `emperor-1.0.4/tests/javascript_tests/qunit/qunit-min.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/runner.js` & `emperor-1.0.4/tests/javascript_tests/runner.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_animate.js` & `emperor-1.0.4/tests/javascript_tests/test_animate.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_animations_controller.js` & `emperor-1.0.4/tests/javascript_tests/test_animations_controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_axes_controller.js` & `emperor-1.0.4/tests/javascript_tests/test_axes_controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_color_view_controller.js` & `emperor-1.0.4/tests/javascript_tests/test_color_view_controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_decomposition_model.js` & `emperor-1.0.4/tests/javascript_tests/test_decomposition_model.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_decomposition_view.js` & `emperor-1.0.4/tests/javascript_tests/test_decomposition_view.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_draw.js` & `emperor-1.0.4/tests/javascript_tests/test_draw.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_opacity_view_controller.js` & `emperor-1.0.4/tests/javascript_tests/test_opacity_view_controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_plottable.js` & `emperor-1.0.4/tests/javascript_tests/test_plottable.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_scalar_view_controller.js` & `emperor-1.0.4/tests/javascript_tests/test_scalar_view_controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_scale_view_controller.js` & `emperor-1.0.4/tests/javascript_tests/test_scale_view_controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_sceneplotview3d.js` & `emperor-1.0.4/tests/javascript_tests/test_sceneplotview3d.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_shape_controller.js` & `emperor-1.0.4/tests/javascript_tests/test_shape_controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_trajectory.js` & `emperor-1.0.4/tests/javascript_tests/test_trajectory.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_util.js` & `emperor-1.0.4/tests/javascript_tests/test_util.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_view_controller.js` & `emperor-1.0.4/tests/javascript_tests/test_view_controller.js`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/javascript_tests/test_visibility_controller.js` & `emperor-1.0.4/tests/javascript_tests/test_visibility_controller.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -144,14 +144,47 @@
             var testColumn = controller.bodyGrid.getColumns()[0];
             equal(testColumn.field, 'value');
 
             // verify the visibility value is set properly
             equal(controller.getMetadataField(), null);
         });
 
+        test('Testing toggleVisibility', function(assert) {
+            var container = $('<div id="does-not-exist" style="height:11px; ' +
+                'width:12px"></div>');
+            var controller = new VisibilityController(new UIState(), container,
+                this.sharedDecompositionViewDict);
+            controller.setMetadataField('Treatment');
+
+            // trun everything off
+            controller.toggleVisibility();
+            equal(controller.decompViewDict.scatter.markers[0].visible, false);
+            equal(controller.decompViewDict.scatter.markers[1].visible, false);
+
+            var groupVisibility = controller.getSlickGridDataset();
+            equal(groupVisibility[0].value, false);
+            equal(groupVisibility[1].value, false);
+
+            // set the first group to false the second group to true
+            groupVisibility = controller.getSlickGridDataset();
+            groupVisibility[0].value = false;
+            groupVisibility[1].value = true;
+            controller.getView().setVisibility(false, groupVisibility[0].plottables);
+            controller.getView().setVisibility(true, groupVisibility[1].plottables);
+            controller.setSlickGridDataset(groupVisibility);
+
+            controller.toggleVisibility();
+            equal(controller.decompViewDict.scatter.markers[0].visible, true);
+            equal(controller.decompViewDict.scatter.markers[1].visible, false);
+
+            groupVisibility = controller.getSlickGridDataset();
+            equal(groupVisibility[0].value, true);
+            equal(groupVisibility[1].value, false);
+        });
+
         test('Testing setPlottableAttributes helper function', function(assert) {
             // testing with one plottable
             var idx = 0;
             plottables = [{
                 idx: idx
             }];
             equal(this.dv.markers[idx].visible, true);
```

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/Fasting_Map.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/Fasting_Map.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/Fasting_Map_modified.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/Fasting_Map_modified.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/biplot.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/biplot.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/compare/pcoa_unweighted_unifrac_rarefaction_110_0.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/compare/pcoa_unweighted_unifrac_rarefaction_110_0.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/compare/pcoa_unweighted_unifrac_rarefaction_110_1.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/compare/pcoa_unweighted_unifrac_rarefaction_110_1.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/euclidian_pc.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/euclidian_pc.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/makefolders.sh` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/makefolders.sh`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/otu_table_L3.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/otu_table_L3.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_0.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_0.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_1.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_1.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_2.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_2.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_3.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_3.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_4.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_4.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_5.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_5.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_6.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_6.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_7.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_7.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_8.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_8.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_9.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc/pcoa_unweighted_unifrac_rarefaction_110_9.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc.txt` & `emperor-1.0.4/tests/scripts_test_data/make_emperor/unweighted_unifrac_pc.txt`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/test_core.py` & `emperor-1.0.4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/test_format.py` & `emperor-1.0.4/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/test_pandas.py` & `emperor-1.0.4/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/test_qiime_backports/test_make_3d_plots.py` & `emperor-1.0.4/tests/test_qiime_backports/test_make_3d_plots.py`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/test_qiime_backports/test_util.py` & `emperor-1.0.4/tests/test_qiime_backports/test_util.py`

 * *Files identical despite different names*

### Comparing `emperor-1.0.3/tests/test_util.py` & `emperor-1.0.4/tests/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,39 +314,39 @@
             validate_and_process_custom_axes(mf, ['louie'])
 
         with self.assertRaises(ValueError):
             validate_and_process_custom_axes(mf, ['louie', 'dewey'])
 
     def test_resolve_stable_url_release(self):
         # we test that no warnings are raised
-        url = 'https://github.com/biocore/emperor/%s/emperor/support_files'
+        url = 'https://github.com/biocore/emperor@%s/emperor/support_files'
         with warnings.catch_warnings(record=True) as w:
             obs = resolve_stable_url('1.0.0b7', url)
             self.assertTrue(len(w) == 0)
             self.assertEqual(obs, url % '1.0.0-beta.7')
 
     def test_resolve_stable_url_release_check_warning(self):
-        url = 'https://github.com/biocore/emperor/%s/emperor/support_files'
+        url = 'https://github.com/biocore/emperor@%s/emperor/support_files'
         with warnings.catch_warnings(record=True) as w:
             warnings.simplefilter('always')
-            obs = resolve_stable_url('1.0.0b7-dev', url)
+            obs = resolve_stable_url('1.0.0b7.dev', url)
 
             self.assertTrue(len(w) == 1)
             self.assertTrue(issubclass(w[-1].category, EmperorWarning))
-            self.assertEqual(obs, url % 'new-api')
+            self.assertEqual(obs, url % '1.0.0-beta.7')
 
     def test_resolve_stable_url_release_number_check_warning(self):
-        url = 'https://github.com/biocore/emperor/%s/emperor/support_files'
+        url = 'https://github.com/biocore/emperor@%s/emperor/support_files'
         with warnings.catch_warnings(record=True) as w:
             warnings.simplefilter('always')
-            obs = resolve_stable_url('1.0.0b7-dev0', url)
+            obs = resolve_stable_url('1.0.0b7.dev0', url)
 
             self.assertTrue(len(w) == 1)
             self.assertTrue(issubclass(w[-1].category, EmperorWarning))
-            self.assertEqual(obs, url % 'new-api')
+            self.assertEqual(obs, url % '1.0.0-beta.7')
 
 
 MAPPING_FILE_DATA = [
     ['PC.354', 'AGCACGAGCCTA', 'YATGCTGCCTCCCGTAGGAGT', 'Control', '20061218',
      'Control_mouse_I.D._354'],
     ['PC.355', 'AACTCGTCGATG', 'YATGCTGCCTCCCGTAGGAGT', 'Control', '20061218',
      'Control_mouse_I.D._355'],
```

