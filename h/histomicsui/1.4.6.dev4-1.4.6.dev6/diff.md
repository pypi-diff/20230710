# Comparing `tmp/histomicsui-1.4.6.dev4.tar.gz` & `tmp/histomicsui-1.4.6.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histomicsui-1.4.6.dev4.tar", last modified: Mon Jul 10 13:51:12 2023, max compression
+gzip compressed data, was "histomicsui-1.4.6.dev6.tar", last modified: Mon Jul 10 14:16:28 2023, max compression
```

## Comparing `histomicsui-1.4.6.dev4.tar` & `histomicsui-1.4.6.dev6.tar`

### file list

```diff
@@ -1,211 +1,211 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.629715 histomicsui-1.4.6.dev4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.601714 histomicsui-1.4.6.dev4/.circleci/
--rw-r--r--   0 root         (0) root         (0)     3884 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)      303 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/.editorconfig
--rw-r--r--   0 root         (0) root         (0)      532 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/.git-blame-ignore-revs
--rw-r--r--   0 root         (0) root         (0)      556 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/.gitignore
--rw-r--r--   0 root         (0) root         (0)      690 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/.travis.yml
--rw-r--r--   0 root         (0) root         (0)    10173 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      150 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      585 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/NOTICE
--rw-r--r--   0 root         (0) root         (0)     7025 2023-07-10 13:51:12.629715 histomicsui-1.4.6.dev4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6076 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/README.rst
--rw-r--r--   0 root         (0) root         (0)      460 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/codecov.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.601714 histomicsui-1.4.6.dev4/docs/
--rw-r--r--   0 root         (0) root         (0)     2399 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/docs/config_options.rst
--rw-r--r--   0 root         (0) root         (0)     6407 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/docs/controls.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.605714 histomicsui-1.4.6.dev4/docs/images/
--rwxr-xr-x   0 root         (0) root         (0)   133796 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/docs/images/difference.gif
--rwxr-xr-x   0 root         (0) root         (0)   133603 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/docs/images/intersect.gif
--rwxr-xr-x   0 root         (0) root         (0)   154141 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/docs/images/union.gif
--rwxr-xr-x   0 root         (0) root         (0)   168255 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/docs/images/xor.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.605714 histomicsui-1.4.6.dev4/histomicsui/
--rw-r--r--   0 root         (0) root         (0)    17663 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/__init__.py
--rw-r--r--   0 root         (0) root         (0)      917 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/constants.py
--rw-r--r--   0 root         (0) root         (0)    10489 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.605714 histomicsui-1.4.6.dev4/histomicsui/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/models/aperio.py
--rw-r--r--   0 root         (0) root         (0)     1832 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/models/case.py
--rw-r--r--   0 root         (0) root         (0)     1057 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/models/cohort.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/models/image.py
--rw-r--r--   0 root         (0) root         (0)     8504 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/models/meta.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/models/pathology.py
--rw-r--r--   0 root         (0) root         (0)     1549 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/models/slide.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.609714 histomicsui-1.4.6.dev4/histomicsui/rest/
--rw-r--r--   0 root         (0) root         (0)      512 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3728 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/rest/aperio.py
--rw-r--r--   0 root         (0) root         (0)     9313 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/rest/hui_resource.py
--rw-r--r--   0 root         (0) root         (0)     4584 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/rest/image_browse_resource.py
--rw-r--r--   0 root         (0) root         (0)    15298 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/rest/system.py
--rw-r--r--   0 root         (0) root         (0)    28968 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/rest/tcga.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.609714 histomicsui-1.4.6.dev4/histomicsui/web_client/
--rw-r--r--   0 root         (0) root         (0)     2450 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/app.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.609714 histomicsui-1.4.6.dev4/histomicsui/web_client/collections/
--rw-r--r--   0 root         (0) root         (0)      308 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/collections/StyleCollection.js
--rw-r--r--   0 root         (0) root         (0)      405 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/collections/UserCollection.js
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/collections/index.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.609714 histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/
--rw-r--r--   0 root         (0) root         (0)     1326 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/confirmDialog.js
--rw-r--r--   0 root         (0) root         (0)     3936 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/editElement.js
--rw-r--r--   0 root         (0) root         (0)     6663 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/editRegionOfInterest.js
--rw-r--r--   0 root         (0) root         (0)    11216 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/editStyleGroups.js
--rw-r--r--   0 root         (0) root         (0)      478 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/index.js
--rw-r--r--   0 root         (0) root         (0)     1153 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/metadataPlot.js
--rw-r--r--   0 root         (0) root         (0)     4936 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/openAnnotatedImage.js
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/openImage.js
--rw-r--r--   0 root         (0) root         (0)    22740 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/saveAnnotation.js
--rw-r--r--   0 root         (0) root         (0)       78 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/events.js
--rw-r--r--   0 root         (0) root         (0)      391 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/index.js
--rw-r--r--   0 root         (0) root         (0)      787 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/main.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.613714 histomicsui-1.4.6.dev4/histomicsui/web_client/models/
--rw-r--r--   0 root         (0) root         (0)      221 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/models/StyleModel.js
--rw-r--r--   0 root         (0) root         (0)       67 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/models/index.js
--rw-r--r--   0 root         (0) root         (0)     3689 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.613714 histomicsui-1.4.6.dev4/histomicsui/web_client/panels/
--rw-r--r--   0 root         (0) root         (0)    23881 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/panels/AnnotationSelector.js
--rw-r--r--   0 root         (0) root         (0)    43398 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/panels/DrawWidget.js
--rw-r--r--   0 root         (0) root         (0)     1943 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/panels/FrameSelectorWidget.js
--rw-r--r--   0 root         (0) root         (0)    14204 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/panels/MetadataPlot.js
--rw-r--r--   0 root         (0) root         (0)     5170 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/panels/MetadataWidget.js
--rw-r--r--   0 root         (0) root         (0)     8115 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/panels/OverviewWidget.js
--rw-r--r--   0 root         (0) root         (0)     1121 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/panels/RegionSelector.js
--rw-r--r--   0 root         (0) root         (0)     9946 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/panels/ZoomWidget.js
--rw-r--r--   0 root         (0) root         (0)      146 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/panels/index.js
--rw-r--r--   0 root         (0) root         (0)     1485 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/router.js
--rw-r--r--   0 root         (0) root         (0)      292 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/routes.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.613714 histomicsui-1.4.6.dev4/histomicsui/web_client/static/
--rwxr-xr-x   0 root         (0) root         (0)     5072 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/static/favicon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.597714 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.613714 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/body/
--rw-r--r--   0 root         (0) root         (0)      504 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/body/configView.styl
--rw-r--r--   0 root         (0) root         (0)     1258 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/body/image.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.613714 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/dialogs/
--rw-r--r--   0 root         (0) root         (0)      195 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/dialogs/editStyleGroups.styl
--rw-r--r--   0 root         (0) root         (0)      237 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/dialogs/openAnnotatedImage.styl
--rw-r--r--   0 root         (0) root         (0)      775 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.613714 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/layout/
--rw-r--r--   0 root         (0) root         (0)      986 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/layout/header.styl
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/layout/headerAnalyses.styl
--rw-r--r--   0 root         (0) root         (0)      151 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/layout/headerImage.styl
--rw-r--r--   0 root         (0) root         (0)     1387 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/layout/layout.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.617715 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/panels/
--rw-r--r--   0 root         (0) root         (0)     1671 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/panels/annotationSelector.styl
--rw-r--r--   0 root         (0) root         (0)     2651 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/panels/drawWidget.styl
--rw-r--r--   0 root         (0) root         (0)     1568 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/panels/frameSelectorWidget.styl
--rw-r--r--   0 root         (0) root         (0)      430 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/panels/metadataPlot.styl
--rw-r--r--   0 root         (0) root         (0)      929 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/panels/metadataWidget.styl
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/panels/overviewWidget.styl
--rw-r--r--   0 root         (0) root         (0)       67 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/panels/regionSelector.styl
--rw-r--r--   0 root         (0) root         (0)      878 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/panels/zoomWidget.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.617715 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/popover/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/popover/annotationContextMenu.styl
--rw-r--r--   0 root         (0) root         (0)     1513 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/popover/annotationPopover.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.617715 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/views/
--rw-r--r--   0 root         (0) root         (0)      222 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/views/itemList.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.597714 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.617715 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/body/
--rw-r--r--   0 root         (0) root         (0)     5608 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/body/configView.pug
--rw-r--r--   0 root         (0) root         (0)      783 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/body/image.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.617715 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/
--rw-r--r--   0 root         (0) root         (0)      501 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/annotatedImageList.pug
--rw-r--r--   0 root         (0) root         (0)      428 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/confirmDialog.pug
--rw-r--r--   0 root         (0) root         (0)     2079 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/editElement.pug
--rw-r--r--   0 root         (0) root         (0)     1730 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug
--rw-r--r--   0 root         (0) root         (0)     3201 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/editStyleGroups.pug
--rw-r--r--   0 root         (0) root         (0)     1541 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/metadataPlot.pug
--rw-r--r--   0 root         (0) root         (0)      838 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/openImage.pug
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/saveAnnotation.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.617715 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/layout/
--rw-r--r--   0 root         (0) root         (0)      925 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/layout/header.pug
--rw-r--r--   0 root         (0) root         (0)      865 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/layout/headerAnalyses.pug
--rw-r--r--   0 root         (0) root         (0)     1467 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/layout/headerImage.pug
--rw-r--r--   0 root         (0) root         (0)      641 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/layout/headerUser.pug
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/layout/layout.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.621715 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/panels/
--rw-r--r--   0 root         (0) root         (0)     3961 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/panels/annotationSelector.pug
--rw-r--r--   0 root         (0) root         (0)     5685 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/panels/drawWidget.pug
--rw-r--r--   0 root         (0) root         (0)     2166 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/panels/drawWidgetElement.pug
--rw-r--r--   0 root         (0) root         (0)      116 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/panels/frameSelectorWidget.pug
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/panels/metadataPlot.pug
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/panels/metadataWidgetPanel.pug
--rw-r--r--   0 root         (0) root         (0)      102 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/panels/overviewWidget.pug
--rw-r--r--   0 root         (0) root         (0)      398 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/panels/panel.pug
--rw-r--r--   0 root         (0) root         (0)      345 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/panels/regionSelector.pug
--rw-r--r--   0 root         (0) root         (0)     1281 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/panels/zoomWidget.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.621715 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/popover/
--rw-r--r--   0 root         (0) root         (0)      576 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/popover/annotationContextMenu.pug
--rw-r--r--   0 root         (0) root         (0)     1404 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/popover/annotationPopover.pug
--rw-r--r--   0 root         (0) root         (0)      204 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/templates/popover/pixelmapContextMenu.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.621715 histomicsui-1.4.6.dev4/histomicsui/web_client/views/
--rw-r--r--   0 root         (0) root         (0)      525 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/HierarchyWidget.js
--rw-r--r--   0 root         (0) root         (0)     2263 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/View.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.621715 histomicsui-1.4.6.dev4/histomicsui/web_client/views/body/
--rw-r--r--   0 root         (0) root         (0)     7205 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/body/ConfigView.js
--rw-r--r--   0 root         (0) root         (0)    68637 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/body/ImageView.js
--rw-r--r--   0 root         (0) root         (0)      119 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/body/index.js
--rw-r--r--   0 root         (0) root         (0)      190 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/index.js
--rw-r--r--   0 root         (0) root         (0)     3436 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/itemList.js
--rw-r--r--   0 root         (0) root         (0)     2375 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/itemPage.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.621715 histomicsui-1.4.6.dev4/histomicsui/web_client/views/layout/
--rw-r--r--   0 root         (0) root         (0)     1658 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/layout/HeaderAnalysesView.js
--rw-r--r--   0 root         (0) root         (0)     2861 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/layout/HeaderImageView.js
--rw-r--r--   0 root         (0) root         (0)      421 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/layout/HeaderUserView.js
--rw-r--r--   0 root         (0) root         (0)     1621 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/layout/HeaderView.js
--rw-r--r--   0 root         (0) root         (0)      134 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/layout/index.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.625715 histomicsui-1.4.6.dev4/histomicsui/web_client/views/popover/
--rw-r--r--   0 root         (0) root         (0)     4506 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/popover/AnnotationContextMenu.js
--rw-r--r--   0 root         (0) root         (0)    10799 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/popover/AnnotationPopover.js
--rw-r--r--   0 root         (0) root         (0)     1231 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/popover/PixelmapContextMenu.js
--rw-r--r--   0 root         (0) root         (0)      176 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/popover/index.js
--rw-r--r--   0 root         (0) root         (0)     2847 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/views/utils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.597714 histomicsui-1.4.6.dev4/histomicsui/web_client/vue/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.625715 histomicsui-1.4.6.dev4/histomicsui/web_client/vue/components/
--rw-r--r--   0 root         (0) root         (0)     2650 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/vue/components/ColorPickerInput.vue
--rw-r--r--   0 root         (0) root         (0)    12531 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue
--rw-r--r--   0 root         (0) root         (0)      745 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue
--rw-r--r--   0 root         (0) root         (0)      906 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/web_client/webpack.helper.js
--rw-r--r--   0 root         (0) root         (0)     1538 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/histomicsui/webroot.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.605714 histomicsui-1.4.6.dev4/histomicsui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7025 2023-07-10 13:51:12.000000 histomicsui-1.4.6.dev4/histomicsui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7365 2023-07-10 13:51:12.000000 histomicsui-1.4.6.dev4/histomicsui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 13:51:12.000000 histomicsui-1.4.6.dev4/histomicsui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-10 13:51:12.000000 histomicsui-1.4.6.dev4/histomicsui.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 13:50:20.000000 histomicsui-1.4.6.dev4/histomicsui.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      182 2023-07-10 13:51:12.000000 histomicsui-1.4.6.dev4/histomicsui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 13:51:12.000000 histomicsui-1.4.6.dev4/histomicsui.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      314 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-07-10 13:51:12.629715 histomicsui-1.4.6.dev4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2339 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.625715 histomicsui-1.4.6.dev4/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1110 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/datastore.py
--rw-r--r--   0 root         (0) root         (0)     2202 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/girder_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.625715 histomicsui-1.4.6.dev4/tests/test_files/
--rw-r--r--   0 root         (0) root         (0)     1286 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/test_files/.histomicsui_config.yaml
--rw-r--r--   0 root         (0) root         (0)      424 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/test_files/sample.anot
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/test_files/sample.meta
--rw-r--r--   0 root         (0) root         (0)      493 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/test_files/sample_girder_id.anot
--rw-r--r--   0 root         (0) root         (0)     8928 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/test_files/test_analysis_detection.xml
--rw-r--r--   0 root         (0) root         (0)    12017 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/test_files/test_analysis_features.xml
--rw-r--r--   0 root         (0) root         (0)     5257 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/test_handlers.py
--rw-r--r--   0 root         (0) root         (0)    19443 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/test_hui_rest.py
--rw-r--r--   0 root         (0) root         (0)     4365 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/test_image_browse_endpoints.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/test_load.py
--rw-r--r--   0 root         (0) root         (0)    32496 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/test_tcga.py
--rw-r--r--   0 root         (0) root         (0)     5993 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/test_web_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:51:12.629715 histomicsui-1.4.6.dev4/tests/web_client_specs/
--rw-r--r--   0 root         (0) root         (0)      238 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/web_client_specs/.eslintrc
--rw-r--r--   0 root         (0) root         (0)     6643 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/web_client_specs/analysisSpec.js
--rw-r--r--   0 root         (0) root         (0)    81737 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/web_client_specs/annotationSpec.js
--rw-r--r--   0 root         (0) root         (0)     1985 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/web_client_specs/girderUISpec.js
--rw-r--r--   0 root         (0) root         (0)     4036 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/web_client_specs/huiSpec.js
--rw-r--r--   0 root         (0) root         (0)     4391 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/web_client_specs/huiTest.js
--rw-r--r--   0 root         (0) root         (0)     4393 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/web_client_specs/itemSpec.js
--rw-r--r--   0 root         (0) root         (0)     4436 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/web_client_specs/metadataPanelSpec.js
--rw-r--r--   0 root         (0) root         (0)     6855 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/web_client_specs/metadataPlotSpec.js
--rw-r--r--   0 root         (0) root         (0)     6131 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/web_client_specs/overviewPanelSpec.js
--rw-r--r--   0 root         (0) root         (0)     2996 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/web_client_specs/panelLayoutSpec.js
--rw-r--r--   0 root         (0) root         (0)    13991 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tests/web_client_specs/pixelmapCategorySpec.js
--rw-r--r--   0 root         (0) root         (0)     2944 2023-07-10 13:50:05.000000 histomicsui-1.4.6.dev4/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.694293 histomicsui-1.4.6.dev6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.666293 histomicsui-1.4.6.dev6/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     3884 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)      303 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/.editorconfig
+-rw-r--r--   0 root         (0) root         (0)      532 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/.git-blame-ignore-revs
+-rw-r--r--   0 root         (0) root         (0)      556 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/.travis.yml
+-rw-r--r--   0 root         (0) root         (0)    10173 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      585 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     7025 2023-07-10 14:16:28.694293 histomicsui-1.4.6.dev6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6076 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/README.rst
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/codecov.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.666293 histomicsui-1.4.6.dev6/docs/
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/docs/config_options.rst
+-rw-r--r--   0 root         (0) root         (0)     6407 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/docs/controls.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.670293 histomicsui-1.4.6.dev6/docs/images/
+-rwxr-xr-x   0 root         (0) root         (0)   133796 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/docs/images/difference.gif
+-rwxr-xr-x   0 root         (0) root         (0)   133603 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/docs/images/intersect.gif
+-rwxr-xr-x   0 root         (0) root         (0)   154141 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/docs/images/union.gif
+-rwxr-xr-x   0 root         (0) root         (0)   168255 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/docs/images/xor.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.670293 histomicsui-1.4.6.dev6/histomicsui/
+-rw-r--r--   0 root         (0) root         (0)    17663 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      917 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/constants.py
+-rw-r--r--   0 root         (0) root         (0)    10489 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.674293 histomicsui-1.4.6.dev6/histomicsui/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/models/aperio.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/models/case.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/models/cohort.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/models/image.py
+-rw-r--r--   0 root         (0) root         (0)     8504 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/models/meta.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/models/pathology.py
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/models/slide.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.674293 histomicsui-1.4.6.dev6/histomicsui/rest/
+-rw-r--r--   0 root         (0) root         (0)      512 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3728 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/rest/aperio.py
+-rw-r--r--   0 root         (0) root         (0)     9313 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/rest/hui_resource.py
+-rw-r--r--   0 root         (0) root         (0)     4584 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/rest/image_browse_resource.py
+-rw-r--r--   0 root         (0) root         (0)    15298 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/rest/system.py
+-rw-r--r--   0 root         (0) root         (0)    28968 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/rest/tcga.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.674293 histomicsui-1.4.6.dev6/histomicsui/web_client/
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/app.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.674293 histomicsui-1.4.6.dev6/histomicsui/web_client/collections/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/collections/StyleCollection.js
+-rw-r--r--   0 root         (0) root         (0)      405 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/collections/UserCollection.js
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/collections/index.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.678293 histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/
+-rw-r--r--   0 root         (0) root         (0)     1326 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/confirmDialog.js
+-rw-r--r--   0 root         (0) root         (0)     3936 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/editElement.js
+-rw-r--r--   0 root         (0) root         (0)     6663 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/editRegionOfInterest.js
+-rw-r--r--   0 root         (0) root         (0)    11216 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/editStyleGroups.js
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/index.js
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/metadataPlot.js
+-rw-r--r--   0 root         (0) root         (0)     4936 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/openAnnotatedImage.js
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/openImage.js
+-rw-r--r--   0 root         (0) root         (0)    22740 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/saveAnnotation.js
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/events.js
+-rw-r--r--   0 root         (0) root         (0)      391 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/index.js
+-rw-r--r--   0 root         (0) root         (0)      787 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/main.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.678293 histomicsui-1.4.6.dev6/histomicsui/web_client/models/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/models/StyleModel.js
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/models/index.js
+-rw-r--r--   0 root         (0) root         (0)     3689 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.678293 histomicsui-1.4.6.dev6/histomicsui/web_client/panels/
+-rw-r--r--   0 root         (0) root         (0)    23881 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/panels/AnnotationSelector.js
+-rw-r--r--   0 root         (0) root         (0)    43398 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/panels/DrawWidget.js
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/panels/FrameSelectorWidget.js
+-rw-r--r--   0 root         (0) root         (0)    14204 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/panels/MetadataPlot.js
+-rw-r--r--   0 root         (0) root         (0)     5170 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/panels/MetadataWidget.js
+-rw-r--r--   0 root         (0) root         (0)     8115 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/panels/OverviewWidget.js
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/panels/RegionSelector.js
+-rw-r--r--   0 root         (0) root         (0)     9946 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/panels/ZoomWidget.js
+-rw-r--r--   0 root         (0) root         (0)      146 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/panels/index.js
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/router.js
+-rw-r--r--   0 root         (0) root         (0)      292 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/routes.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.678293 histomicsui-1.4.6.dev6/histomicsui/web_client/static/
+-rwxr-xr-x   0 root         (0) root         (0)     5072 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/static/favicon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.662293 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.678293 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/body/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/body/configView.styl
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/body/image.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.678293 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/dialogs/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/dialogs/editStyleGroups.styl
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/dialogs/openAnnotatedImage.styl
+-rw-r--r--   0 root         (0) root         (0)      775 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.678293 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/layout/
+-rw-r--r--   0 root         (0) root         (0)      986 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/layout/header.styl
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/layout/headerAnalyses.styl
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/layout/headerImage.styl
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/layout/layout.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.682293 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/panels/
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/panels/annotationSelector.styl
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/panels/drawWidget.styl
+-rw-r--r--   0 root         (0) root         (0)     1568 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/panels/frameSelectorWidget.styl
+-rw-r--r--   0 root         (0) root         (0)      430 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/panels/metadataPlot.styl
+-rw-r--r--   0 root         (0) root         (0)      929 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/panels/metadataWidget.styl
+-rw-r--r--   0 root         (0) root         (0)       81 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/panels/overviewWidget.styl
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/panels/regionSelector.styl
+-rw-r--r--   0 root         (0) root         (0)      878 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/panels/zoomWidget.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.682293 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/popover/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/popover/annotationContextMenu.styl
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/popover/annotationPopover.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.682293 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/views/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/views/itemList.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.662293 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.682293 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/body/
+-rw-r--r--   0 root         (0) root         (0)     5608 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/body/configView.pug
+-rw-r--r--   0 root         (0) root         (0)      783 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/body/image.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.682293 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/annotatedImageList.pug
+-rw-r--r--   0 root         (0) root         (0)      428 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/confirmDialog.pug
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/editElement.pug
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/editStyleGroups.pug
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/metadataPlot.pug
+-rw-r--r--   0 root         (0) root         (0)      838 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/openImage.pug
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/saveAnnotation.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.682293 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/layout/
+-rw-r--r--   0 root         (0) root         (0)      925 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/layout/header.pug
+-rw-r--r--   0 root         (0) root         (0)      865 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/layout/headerAnalyses.pug
+-rw-r--r--   0 root         (0) root         (0)     1467 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/layout/headerImage.pug
+-rw-r--r--   0 root         (0) root         (0)      641 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/layout/headerUser.pug
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/layout/layout.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.686293 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/panels/
+-rw-r--r--   0 root         (0) root         (0)     3961 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/panels/annotationSelector.pug
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/panels/drawWidget.pug
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/panels/drawWidgetElement.pug
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/panels/frameSelectorWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/panels/metadataPlot.pug
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/panels/metadataWidgetPanel.pug
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/panels/overviewWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      398 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/panels/panel.pug
+-rw-r--r--   0 root         (0) root         (0)      345 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/panels/regionSelector.pug
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/panels/zoomWidget.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.686293 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/popover/
+-rw-r--r--   0 root         (0) root         (0)      576 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/popover/annotationContextMenu.pug
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/popover/annotationPopover.pug
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/templates/popover/pixelmapContextMenu.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.686293 histomicsui-1.4.6.dev6/histomicsui/web_client/views/
+-rw-r--r--   0 root         (0) root         (0)      525 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/HierarchyWidget.js
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/View.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.686293 histomicsui-1.4.6.dev6/histomicsui/web_client/views/body/
+-rw-r--r--   0 root         (0) root         (0)     7205 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/body/ConfigView.js
+-rw-r--r--   0 root         (0) root         (0)    68637 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/body/ImageView.js
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/body/index.js
+-rw-r--r--   0 root         (0) root         (0)      190 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/index.js
+-rw-r--r--   0 root         (0) root         (0)     3436 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/itemList.js
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/itemPage.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.686293 histomicsui-1.4.6.dev6/histomicsui/web_client/views/layout/
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/layout/HeaderAnalysesView.js
+-rw-r--r--   0 root         (0) root         (0)     2861 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/layout/HeaderImageView.js
+-rw-r--r--   0 root         (0) root         (0)      421 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/layout/HeaderUserView.js
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/layout/HeaderView.js
+-rw-r--r--   0 root         (0) root         (0)      134 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/layout/index.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.690293 histomicsui-1.4.6.dev6/histomicsui/web_client/views/popover/
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/popover/AnnotationContextMenu.js
+-rw-r--r--   0 root         (0) root         (0)    10799 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/popover/AnnotationPopover.js
+-rw-r--r--   0 root         (0) root         (0)     1231 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/popover/PixelmapContextMenu.js
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/popover/index.js
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/views/utils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.662293 histomicsui-1.4.6.dev6/histomicsui/web_client/vue/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.690293 histomicsui-1.4.6.dev6/histomicsui/web_client/vue/components/
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/vue/components/ColorPickerInput.vue
+-rw-r--r--   0 root         (0) root         (0)    12531 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue
+-rw-r--r--   0 root         (0) root         (0)      745 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue
+-rw-r--r--   0 root         (0) root         (0)      906 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/web_client/webpack.helper.js
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/histomicsui/webroot.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.670293 histomicsui-1.4.6.dev6/histomicsui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7025 2023-07-10 14:16:28.000000 histomicsui-1.4.6.dev6/histomicsui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7365 2023-07-10 14:16:28.000000 histomicsui-1.4.6.dev6/histomicsui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 14:16:28.000000 histomicsui-1.4.6.dev6/histomicsui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-10 14:16:28.000000 histomicsui-1.4.6.dev6/histomicsui.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 14:15:35.000000 histomicsui-1.4.6.dev6/histomicsui.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      182 2023-07-10 14:16:28.000000 histomicsui-1.4.6.dev6/histomicsui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 14:16:28.000000 histomicsui-1.4.6.dev6/histomicsui.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      314 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-10 14:16:28.694293 histomicsui-1.4.6.dev6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.690293 histomicsui-1.4.6.dev6/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/datastore.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/girder_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.690293 histomicsui-1.4.6.dev6/tests/test_files/
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/test_files/.histomicsui_config.yaml
+-rw-r--r--   0 root         (0) root         (0)      424 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/test_files/sample.anot
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/test_files/sample.meta
+-rw-r--r--   0 root         (0) root         (0)      493 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/test_files/sample_girder_id.anot
+-rw-r--r--   0 root         (0) root         (0)     8928 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/test_files/test_analysis_detection.xml
+-rw-r--r--   0 root         (0) root         (0)    12017 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/test_files/test_analysis_features.xml
+-rw-r--r--   0 root         (0) root         (0)     5257 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/test_handlers.py
+-rw-r--r--   0 root         (0) root         (0)    19443 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/test_hui_rest.py
+-rw-r--r--   0 root         (0) root         (0)     4365 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/test_image_browse_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/test_load.py
+-rw-r--r--   0 root         (0) root         (0)    32845 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/test_tcga.py
+-rw-r--r--   0 root         (0) root         (0)     5993 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/test_web_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:28.694293 histomicsui-1.4.6.dev6/tests/web_client_specs/
+-rw-r--r--   0 root         (0) root         (0)      238 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/web_client_specs/.eslintrc
+-rw-r--r--   0 root         (0) root         (0)     6643 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/web_client_specs/analysisSpec.js
+-rw-r--r--   0 root         (0) root         (0)    81781 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/web_client_specs/annotationSpec.js
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/web_client_specs/girderUISpec.js
+-rw-r--r--   0 root         (0) root         (0)     4036 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/web_client_specs/huiSpec.js
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/web_client_specs/huiTest.js
+-rw-r--r--   0 root         (0) root         (0)     4393 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/web_client_specs/itemSpec.js
+-rw-r--r--   0 root         (0) root         (0)     4436 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/web_client_specs/metadataPanelSpec.js
+-rw-r--r--   0 root         (0) root         (0)     6855 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/web_client_specs/metadataPlotSpec.js
+-rw-r--r--   0 root         (0) root         (0)     6131 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/web_client_specs/overviewPanelSpec.js
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/web_client_specs/panelLayoutSpec.js
+-rw-r--r--   0 root         (0) root         (0)    13991 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tests/web_client_specs/pixelmapCategorySpec.js
+-rw-r--r--   0 root         (0) root         (0)     3016 2023-07-10 14:15:19.000000 histomicsui-1.4.6.dev6/tox.ini
```

### Comparing `histomicsui-1.4.6.dev4/.circleci/config.yml` & `histomicsui-1.4.6.dev6/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/.git-blame-ignore-revs` & `histomicsui-1.4.6.dev6/.git-blame-ignore-revs`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/.gitignore` & `histomicsui-1.4.6.dev6/.gitignore`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/.travis.yml` & `histomicsui-1.4.6.dev6/.travis.yml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/LICENSE` & `histomicsui-1.4.6.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/NOTICE` & `histomicsui-1.4.6.dev6/NOTICE`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/PKG-INFO` & `histomicsui-1.4.6.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histomicsui
-Version: 1.4.6.dev4
+Version: 1.4.6.dev6
 Summary: Organize, visualize, and analyze histology images.
 Home-page: https://github.com/DigitalSlideArchive/histomicsui
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,histomicsui
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `histomicsui-1.4.6.dev4/README.rst` & `histomicsui-1.4.6.dev6/README.rst`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/docs/config_options.rst` & `histomicsui-1.4.6.dev6/docs/config_options.rst`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/docs/controls.rst` & `histomicsui-1.4.6.dev6/docs/controls.rst`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/docs/images/difference.gif` & `histomicsui-1.4.6.dev6/docs/images/difference.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/docs/images/intersect.gif` & `histomicsui-1.4.6.dev6/docs/images/intersect.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/docs/images/union.gif` & `histomicsui-1.4.6.dev6/docs/images/union.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/docs/images/xor.gif` & `histomicsui-1.4.6.dev6/docs/images/xor.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/__init__.py` & `histomicsui-1.4.6.dev6/histomicsui/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/constants.py` & `histomicsui-1.4.6.dev6/histomicsui/constants.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/handlers.py` & `histomicsui-1.4.6.dev6/histomicsui/handlers.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/models/aperio.py` & `histomicsui-1.4.6.dev6/histomicsui/models/aperio.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/models/case.py` & `histomicsui-1.4.6.dev6/histomicsui/models/case.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/models/cohort.py` & `histomicsui-1.4.6.dev6/histomicsui/models/cohort.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/models/image.py` & `histomicsui-1.4.6.dev6/histomicsui/models/image.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/models/meta.py` & `histomicsui-1.4.6.dev6/histomicsui/models/meta.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/models/pathology.py` & `histomicsui-1.4.6.dev6/histomicsui/models/pathology.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/models/slide.py` & `histomicsui-1.4.6.dev6/histomicsui/models/slide.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/rest/__init__.py` & `histomicsui-1.4.6.dev6/histomicsui/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/rest/aperio.py` & `histomicsui-1.4.6.dev6/histomicsui/rest/aperio.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/rest/hui_resource.py` & `histomicsui-1.4.6.dev6/histomicsui/rest/hui_resource.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/rest/image_browse_resource.py` & `histomicsui-1.4.6.dev6/histomicsui/rest/image_browse_resource.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/rest/system.py` & `histomicsui-1.4.6.dev6/histomicsui/rest/system.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/rest/tcga.py` & `histomicsui-1.4.6.dev6/histomicsui/rest/tcga.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/app.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/app.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/confirmDialog.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/confirmDialog.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/editElement.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/editElement.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/editRegionOfInterest.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/editRegionOfInterest.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/editStyleGroups.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/editStyleGroups.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/metadataPlot.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/metadataPlot.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/openAnnotatedImage.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/openAnnotatedImage.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/openImage.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/openImage.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/dialogs/saveAnnotation.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/dialogs/saveAnnotation.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/main.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/main.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/package.json` & `histomicsui-1.4.6.dev6/histomicsui/web_client/package.json`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/panels/AnnotationSelector.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/panels/AnnotationSelector.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/panels/DrawWidget.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/panels/DrawWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/panels/FrameSelectorWidget.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/panels/FrameSelectorWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/panels/MetadataPlot.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/panels/MetadataPlot.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/panels/MetadataWidget.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/panels/MetadataWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/panels/OverviewWidget.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/panels/OverviewWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/panels/RegionSelector.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/panels/RegionSelector.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/panels/ZoomWidget.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/panels/ZoomWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/router.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/router.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/static/favicon.png` & `histomicsui-1.4.6.dev6/histomicsui/web_client/static/favicon.png`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/body/image.styl` & `histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/body/image.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl` & `histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/layout/header.styl` & `histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/layout/header.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/layout/layout.styl` & `histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/layout/layout.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/panels/annotationSelector.styl` & `histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/panels/annotationSelector.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/panels/drawWidget.styl` & `histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/panels/drawWidget.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/panels/frameSelectorWidget.styl` & `histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/panels/frameSelectorWidget.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/panels/metadataWidget.styl` & `histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/panels/metadataWidget.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/panels/zoomWidget.styl` & `histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/panels/zoomWidget.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/stylesheets/popover/annotationPopover.styl` & `histomicsui-1.4.6.dev6/histomicsui/web_client/stylesheets/popover/annotationPopover.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/body/configView.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/body/configView.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/body/image.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/body/image.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/editElement.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/editElement.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/editStyleGroups.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/editStyleGroups.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/metadataPlot.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/metadataPlot.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/dialogs/saveAnnotation.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/dialogs/saveAnnotation.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/layout/header.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/layout/header.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/layout/headerAnalyses.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/layout/headerAnalyses.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/layout/headerImage.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/layout/headerImage.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/layout/headerUser.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/layout/headerUser.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/panels/annotationSelector.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/panels/annotationSelector.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/panels/drawWidget.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/panels/drawWidget.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/panels/drawWidgetElement.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/panels/drawWidgetElement.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/panels/zoomWidget.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/panels/zoomWidget.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/popover/annotationContextMenu.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/popover/annotationContextMenu.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/templates/popover/annotationPopover.pug` & `histomicsui-1.4.6.dev6/histomicsui/web_client/templates/popover/annotationPopover.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/views/HierarchyWidget.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/views/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/views/View.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/views/View.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/views/body/ConfigView.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/views/body/ConfigView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/views/body/ImageView.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/views/body/ImageView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/views/itemList.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/views/itemList.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/views/itemPage.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/views/itemPage.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/views/layout/HeaderAnalysesView.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/views/layout/HeaderAnalysesView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/views/layout/HeaderImageView.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/views/layout/HeaderImageView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/views/layout/HeaderView.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/views/layout/HeaderView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/views/popover/AnnotationContextMenu.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/views/popover/AnnotationContextMenu.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/views/popover/AnnotationPopover.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/views/popover/AnnotationPopover.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/views/popover/PixelmapContextMenu.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/views/popover/PixelmapContextMenu.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/views/utils.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/views/utils.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/vue/components/ColorPickerInput.vue` & `histomicsui-1.4.6.dev6/histomicsui/web_client/vue/components/ColorPickerInput.vue`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue` & `histomicsui-1.4.6.dev6/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue` & `histomicsui-1.4.6.dev6/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/web_client/webpack.helper.js` & `histomicsui-1.4.6.dev6/histomicsui/web_client/webpack.helper.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui/webroot.mako` & `histomicsui-1.4.6.dev6/histomicsui/webroot.mako`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/histomicsui.egg-info/PKG-INFO` & `histomicsui-1.4.6.dev6/histomicsui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histomicsui
-Version: 1.4.6.dev4
+Version: 1.4.6.dev6
 Summary: Organize, visualize, and analyze histology images.
 Home-page: https://github.com/DigitalSlideArchive/histomicsui
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,histomicsui
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `histomicsui-1.4.6.dev4/histomicsui.egg-info/SOURCES.txt` & `histomicsui-1.4.6.dev6/histomicsui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/setup.py` & `histomicsui-1.4.6.dev6/setup.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/datastore.py` & `histomicsui-1.4.6.dev6/tests/datastore.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/girder_utilities.py` & `histomicsui-1.4.6.dev6/tests/girder_utilities.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/test_files/.histomicsui_config.yaml` & `histomicsui-1.4.6.dev6/tests/test_files/.histomicsui_config.yaml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/test_files/test_analysis_detection.xml` & `histomicsui-1.4.6.dev6/tests/test_files/test_analysis_detection.xml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/test_files/test_analysis_features.xml` & `histomicsui-1.4.6.dev6/tests/test_files/test_analysis_features.xml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/test_handlers.py` & `histomicsui-1.4.6.dev6/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/test_hui_rest.py` & `histomicsui-1.4.6.dev6/tests/test_hui_rest.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/test_image_browse_endpoints.py` & `histomicsui-1.4.6.dev6/tests/test_image_browse_endpoints.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/test_tcga.py` & `histomicsui-1.4.6.dev6/tests/test_tcga.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import time
 
+import filelock
 import pytest
 from girder.exceptions import ValidationException
 from girder.models.collection import Collection
 from girder.models.file import File
 from girder.models.folder import Folder
 from girder.models.item import Item
 from girder.models.setting import Setting
@@ -15,14 +16,21 @@
 from histomicsui.models.image import Image
 from histomicsui.models.meta import pruneNoneValues, updateDict
 from histomicsui.models.slide import Slide
 
 from . import girder_utilities as utilities
 
 
+@pytest.fixture
+def singular(tmp_path_factory):
+    root_tmp_dir = tmp_path_factory.getbasetemp().parent
+    with filelock.FileLock(root_tmp_dir / '.test_tcga.lock'):
+        yield
+
+
 def createFileItem(name, creator, parent):
     doc = Item().createItem(
         name, creator, parent
     )
     file = File().createFile(
         creator, doc, doc['name'],
         0, {'_id': ''}
@@ -170,28 +178,28 @@
         doc = {}
         Cohort().updateTCGAMeta(doc, {'name': 'value', 'other': 'old'})
         assert Cohort().getTCGAMeta(doc) == {'name': 'value', 'other': 'old'}
 
         Cohort().updateTCGAMeta(doc, {'name': None, 'other': 'new'})
         assert Cohort().getTCGAMeta(doc) == {'other': 'new'}
 
-    def testLoadDocument(self, server, admin, user):
+    def testLoadDocument(self, server, admin, user, singular):
         makeResources(self, admin, user)
         with pytest.raises(ValidationException):
             Cohort().loadDocument('')
 
         assert Cohort().loadDocument(user['_id'], user=admin)['_id'] == user['_id']
 
         assert Cohort().loadDocument(
             self.tcgaCollection['_id'], user=admin)['_id'] == self.tcgaCollection['_id']
 
         assert Cohort().loadDocument(
             self.publicFolder['_id'], user=admin)['_id'] == self.publicFolder['_id']
 
-    def testCohortModel(self, server, admin, user):
+    def testCohortModel(self, server, admin, user, singular):
         makeResources(self, admin, user)
         doc = Folder().createFolder(
             self.tcgaCollection, 'ucec', parentType='collection',
             public=True, creator=admin
         )
         Cohort().importDocument(doc, user=admin)
         assert Cohort().getTCGAType(doc) == 'cohort'
@@ -202,15 +210,15 @@
         Cohort().removeTCGA(doc)
         assert Cohort().findOne({}) is None
 
         Folder().createFolder(doc, 'subfolder', public=True, creator=admin)
         Cohort().importDocument(doc, user=admin, recurse=True)
         assert Cohort().findOne({}).get('_id') == doc['_id']
 
-    def testCaseModel(self, server, admin, user):
+    def testCaseModel(self, server, admin, user, singular):
         makeResources(self, admin, user)
         cohort = Folder().createFolder(
             self.tcgaCollection, 'ucec', parentType='collection',
             public=True, creator=admin
         )
         invaliddoc = Folder().createFolder(
             cohort, 'invalid name', parentType='folder',
@@ -232,15 +240,15 @@
 
         Cohort().importDocument(cohort, user=admin, recurse=True)
         assert Case().findOne({'_id': doc['_id']}).get('_id') == doc['_id']
 
         with pytest.raises(ValidationException):
             Case().importDocument(invaliddoc, user=admin)
 
-    def testSlideModel(self, server, admin, user):
+    def testSlideModel(self, server, admin, user, singular):
         makeResources(self, admin, user)
 
         cohort = Folder().createFolder(
             self.tcgaCollection, 'ucec', parentType='collection',
             public=True, creator=admin
         )
         case = Folder().createFolder(
@@ -257,15 +265,15 @@
 
         with pytest.raises(ValidationException):
             Slide().importDocument(doc, user=admin)
 
         Cohort().importDocument(cohort, user=admin, recurse=True)
         assert Slide().findOne({'_id': doc['_id']}).get('_id') == doc['_id']
 
-    def testImageModel(self, server, admin, user):
+    def testImageModel(self, server, admin, user, singular):
         makeResources(self, admin, user)
 
         cohort = Folder().createFolder(
             self.tcgaCollection, 'ucec', parentType='collection',
             public=True, creator=admin
         )
         case = Folder().createFolder(
@@ -324,15 +332,15 @@
             user=admin
         )
         assert utilities.respStatus(resp) == 200
 
         job = resp.json
 
         # loop until it is done
-        for _idx in range(100):
+        for _idx in range(200):
             time.sleep(0.1)
 
             resp = server.request(
                 path='/job/' + job['_id'],
                 user=admin
             )
             assert utilities.respStatus(resp) == 200
@@ -341,15 +349,15 @@
             if status == JobStatus.SUCCESS:
                 return
             elif status in (JobStatus.ERROR, JobStatus.CANCELED):
                 raise Exception('TCGA import failed')
 
         raise Exception('TCGA import did not finish in time')
 
-    def testTCGACollection(self, server, admin, user):
+    def testTCGACollection(self, server, admin, user, singular):
         makeResources(self, admin, user)
         resp = server.request(
             path='/tcga'
         )
         assert utilities.respStatus(resp) == 200
         assert resp.json['_id'] == str(self.tcgaCollection['_id'])
 
@@ -389,21 +397,21 @@
 
         resp = server.request(
             path='/tcga'
         )
         assert utilities.respStatus(resp) == 200
         assert resp.json['_id'] == str(self.tcgaCollection['_id'])
 
-    def testRecursiveImport(self, server, admin, user):
+    def testRecursiveImport(self, server, admin, user, singular):
         makeResources(self, admin, user)
         self.runRecursiveImport(server, admin)
         images = list(Image().find({}))
         assert len(images) == 3
 
-    def testCohortEndpoints(self, server, admin, user):
+    def testCohortEndpoints(self, server, admin, user, singular):
         makeResources(self, admin, user)
         resp = server.request(
             path='/tcga/cohort'
         )
         assert utilities.respStatus(resp) == 200
         assert resp.json['data'] == []
 
@@ -458,15 +466,15 @@
         resp = server.request(
             path='/tcga/cohort/' + str(self.cohort['_id']) + '/images'
         )
         assert utilities.respStatus(resp) == 200
         assert len(resp.json['data']) == 3
         assert resp.json['data'][0]['tcga']['type'] == 'image'
 
-    def testCaseEndpoints(self, server, admin, user):
+    def testCaseEndpoints(self, server, admin, user, singular):
         makeResources(self, admin, user)
         self.runRecursiveImport(server, admin)
 
         resp = server.request(
             path='/tcga/case',
             params={'cohort': str(self.cohort['_id'])}
         )
@@ -523,15 +531,15 @@
         assert resp.json['_id'] == str(self.case2['_id'])
 
         resp = server.request(
             path='/tcga/case/label/' + 'notalabel'
         )
         assert utilities.respStatus(resp) == 400
 
-    def testCaseMetadata(self, server, admin, user):
+    def testCaseMetadata(self, server, admin, user, singular):
         makeResources(self, admin, user)
         id1 = str(self.case1['_id'])
         id2 = str(self.case2['_id'])
         self.runRecursiveImport(server, admin)
 
         resp = server.request(
             path='/tcga/case/' + id1 + '/metadata/tables'
@@ -660,15 +668,15 @@
 
         resp = server.request(
             path='/tcga/case/' + id2 + '/metadata/tables'
         )
         assert utilities.respStatus(resp) == 200
         assert resp.json == []
 
-    def testSlideEndpoints(self, server, admin, user):
+    def testSlideEndpoints(self, server, admin, user, singular):
         makeResources(self, admin, user)
         case1 = str(self.case1['_id'])
         slide1 = str(self.slide1['_id'])
         self.runRecursiveImport(server, admin)
 
         resp = server.request(
             path='/tcga/slide',
@@ -719,15 +727,15 @@
         assert utilities.respStatus(resp) == 200
 
         resp = server.request(
             path='/tcga/slide/' + slide1
         )
         assert utilities.respStatus(resp) == 200
 
-    def testImageEndpoints(self, server, admin, user):
+    def testImageEndpoints(self, server, admin, user, singular):
         makeResources(self, admin, user)
         slide1 = str(self.slide1['_id'])
         image1 = str(self.image1['_id'])
         self.runRecursiveImport(server, admin)
 
         resp = server.request(
             path='/tcga/image',
@@ -786,15 +794,15 @@
         assert utilities.respStatus(resp) == 200
 
         resp = server.request(
             path='/tcga/image/' + image1
         )
         assert utilities.respStatus(resp) == 200
 
-    def testPathologyEndpoints(self, server, admin, user):
+    def testPathologyEndpoints(self, server, admin, user, singular):
         makeResources(self, admin, user)
         case1 = str(self.case1['_id'])
         pathology1 = str(self.pathology1['_id'])
         self.runRecursiveImport(server, admin)
 
         resp = server.request(
             path='/tcga/pathology',
@@ -877,15 +885,15 @@
         assert utilities.respStatus(resp) == 200
 
         resp = server.request(
             path='/tcga/pathology/' + str(self.pathology2['_id'])
         )
         assert utilities.respStatus(resp) == 200
 
-    def testAperioEndpoints(self, server, admin, user):
+    def testAperioEndpoints(self, server, admin, user, singular):
         makeResources(self, admin, user)
         aperio1 = str(self.aperio1['_id'])
         aperio2 = str(self.aperio2['_id'])
         image = str(self.image2['_id'])
         self.runRecursiveImport(server, admin)
 
         # test access control
@@ -967,15 +975,15 @@
         resp = server.request(
             path='/item/' + image + '/aperio',
             params={'tag': 'bar'}
         )
         assert utilities.respStatus(resp) == 200
         assert len(resp.json) == 0
 
-    def testPagingParams(self, server, admin, user):
+    def testPagingParams(self, server, admin, user, singular):
         makeResources(self, admin, user)
         cohort1 = str(self.cohort['_id'])
         self.runRecursiveImport(server, admin)
 
         resp = server.request(
             path='/tcga/case',
             params={'cohort': cohort1, 'limit': 2, 'offset': 0}
```

### Comparing `histomicsui-1.4.6.dev4/tests/test_web_client.py` & `histomicsui-1.4.6.dev6/tests/test_web_client.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/web_client_specs/analysisSpec.js` & `histomicsui-1.4.6.dev6/tests/web_client_specs/analysisSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/web_client_specs/annotationSpec.js` & `histomicsui-1.4.6.dev6/tests/web_client_specs/annotationSpec.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1749,14 +1749,15 @@
                     $('#h-element-line-width').val('10');
                     $('#h-element-label').val('newlabel');
                     $('#h-reset-defaults').click();
                 });
                 waitsFor(function() {
                     return $('#h-element-label').val() === '';
                 }, 'label to reset');
+                girderTest.waitForDialog();
                 runs(function() {
                     expect($('#h-element-line-width').val()).toBe('2');
                 });
             });
             it('cancel changes', function() {
                 runs(function() {
                     $('.h-cancel').click();
```

### Comparing `histomicsui-1.4.6.dev4/tests/web_client_specs/girderUISpec.js` & `histomicsui-1.4.6.dev6/tests/web_client_specs/girderUISpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/web_client_specs/huiSpec.js` & `histomicsui-1.4.6.dev6/tests/web_client_specs/huiSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/web_client_specs/huiTest.js` & `histomicsui-1.4.6.dev6/tests/web_client_specs/huiTest.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/web_client_specs/itemSpec.js` & `histomicsui-1.4.6.dev6/tests/web_client_specs/itemSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/web_client_specs/metadataPanelSpec.js` & `histomicsui-1.4.6.dev6/tests/web_client_specs/metadataPanelSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/web_client_specs/metadataPlotSpec.js` & `histomicsui-1.4.6.dev6/tests/web_client_specs/metadataPlotSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/web_client_specs/overviewPanelSpec.js` & `histomicsui-1.4.6.dev6/tests/web_client_specs/overviewPanelSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/web_client_specs/panelLayoutSpec.js` & `histomicsui-1.4.6.dev6/tests/web_client_specs/panelLayoutSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tests/web_client_specs/pixelmapCategorySpec.js` & `histomicsui-1.4.6.dev6/tests/web_client_specs/pixelmapCategorySpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.6.dev4/tox.ini` & `histomicsui-1.4.6.dev6/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tox]
 envlist =
-  py{36,37,38,39,310}
+  py{36,37,38,39,310,311}
   flake8
   lintclient
 
 [testenv]
 deps =
   coverage
+  filelock
   mock
   pooch
   pytest
   pytest-cov
   pytest-girder>=3.0.5
   pytest-xdist
   setuptools_scm
@@ -127,17 +128,19 @@
 [testenv:format]
 description = Autoformat import order and pep8
 skipsdist = true
 skip_install = true
 deps =
   autopep8
   isort
+  unify
 commands =
   isort {posargs:.}
   autopep8 -ria histomicsui tests
+  unify --in-place --recursive histomicsui tests
 
 [pytest]
 addopts = --verbose --strict-markers --showlocals --cov-report="term" --cov-report="xml" --cov
 testpaths = tests
 
 [coverage:paths]
 source =
```

