# Comparing `tmp/analogic-framework-4.1.1.tar.gz` & `tmp/analogic-framework-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analogic-framework-4.1.1.tar", last modified: Sat Apr 15 08:59:29 2023, max compression
+gzip compressed data, was "analogic-framework-4.1.2.tar", last modified: Mon Jul 10 13:49:42 2023, max compression
```

## Comparing `analogic-framework-4.1.1.tar` & `analogic-framework-4.1.2.tar`

### file list

```diff
@@ -1,255 +1,261 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.435998 analogic-framework-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-15 08:59:29.435998 analogic-framework-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.399997 analogic-framework-4.1.1/analogic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/analogic.py
--rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/analogic_tm1_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/authentication_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/cam.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/camsecure.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/core_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/logging.json
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/loginbasic.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/logincam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/nologin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/pivot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/setting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.391997 analogic-framework-4.1.1/analogic/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.391997 analogic-framework-4.1.1/analogic/static/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.399997 analogic-framework-4.1.1/analogic/static/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)    48488 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   108539 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/css/bootstrap-grid.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.399997 analogic-framework-4.1.1/analogic/static/assets/css/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/css/lib/Chart-2.9.3.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/css/lib/nouislider.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    65538 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.399997 analogic-framework-4.1.1/analogic/static/assets/css/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/css/widgets/loader.css
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/css/widgets/simulation-panel-slider.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.399997 analogic-framework-4.1.1/analogic/static/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/images/loading.gif
--rw-r--r--   0 runner    (1001) docker     (123)   120349 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/images/loading2.gif
--rw-r--r--   0 runner    (1001) docker     (123)    55508 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/images/loading2_transparent.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/images/triangle.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.391997 analogic-framework-4.1.1/analogic/static/assets/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.403997 analogic-framework-4.1.1/analogic/static/assets/js/framework/
--rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/api.js
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/authentication.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.403997 analogic-framework-4.1.1/analogic/static/assets/js/framework/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/extensions/authentication-provider.js
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/extensions/write-executor.js
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/listener.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.403997 analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/array.js
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/base.js
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/default.js
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/factory.js
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/skip.js
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/state.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.407997 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/base.js
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/factory.js
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/list.js
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/matrix.js
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/object.js
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/script.js
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/skip.js
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/pivot.js
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/query-builder.js
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/redirect.js
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/render.js
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/rest-request.js
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/server.js
--rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.407997 analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/base.js
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/download.js
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/factory.js
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/function.js
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/grid-table.js
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/skip.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.407997 analogic-framework-4.1.1/analogic/static/assets/js/lib/
--rw-r--r--   0 runner    (1001) docker     (123)   172689 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/Chart-2.9.3.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    44136 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/Sortable.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    21295 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.407997 analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/
--rw-r--r--   0 runner    (1001) docker     (123)    89411 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery.actual.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery.cookie.js
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery.doubletap.js
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/tableSort.js
--rw-r--r--   0 runner    (1001) docker     (123)    26460 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/lib/nouislider.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.415997 analogic-framework-4.1.1/analogic/static/assets/js/widgets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.415997 analogic-framework-4.1.1/analogic/static/assets/js/widgets/base/
--rw-r--r--   0 runner    (1001) docker     (123)    23255 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/base/widget.js
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/button.js
--rw-r--r--   0 runner    (1001) docker     (123)    27607 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/combo-chart.js
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/container.js
--rw-r--r--   0 runner    (1001) docker     (123)    16545 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/datepicker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.419997 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/BubbleChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/ButtonWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/ComboChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/ContainerWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/DatePickerWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/DropBoxWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/GaugeWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/GridCellWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/GridRowWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/GridWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/HistogramComboChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/HorizontalTableWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/ImageWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/LineAreaChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/PanelWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/PieChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/PopupWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/ScrollTableWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SegmentedBarWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SegmentedControlItemWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SegmentedControlWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SideBarWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SimulationPanelSliderWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SimulationPanelWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SliderWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/SwipeWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/TextAreaWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/TextBoxWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/TextWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/ToggleWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/TornadoChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/VerticalLineBoxWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/WaterFallWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/dropbox.js
--rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/gauge.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.423997 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid/grid-cell.js
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid/grid-row.js
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid/grid.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.423997 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js
--rw-r--r--   0 runner    (1001) docker     (123)    18935 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table.js
--rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/histogram-combo-chart.js
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontal-bar-chart.js
--rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontal-table.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.423997 analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontaltable/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/image.js
--rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/line-area-chart.js
--rw-r--r--   0 runner    (1001) docker     (123)    26611 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/line-scatter-combo.js
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/loader.js
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/page.js
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/panel.js
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/pie-chart.js
--rw-r--r--   0 runner    (1001) docker     (123)    81004 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/pivot-table.js
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/popup.js
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/radar-chart.js
--rw-r--r--   0 runner    (1001) docker     (123)    36449 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/scroll-table.js
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/segmented-bar.js
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/segmented-control-item.js
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/segmented-control.js
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/shadow.js
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/simulation-panel-slider.js
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/simulation-panel.js
--rw-r--r--   0 runner    (1001) docker     (123)    19961 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/slider.js
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/swipe.js
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/system-popup.js
--rw-r--r--   0 runner    (1001) docker     (123)    20395 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/text.js
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/textarea.js
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/textbox.js
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/toggle.js
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/tornado-chart.js
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/vertical-line-box.js
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/js/widgets/water-fall.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.395997 analogic-framework-4.1.1/analogic/static/assets/skin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.427997 analogic-framework-4.1.1/analogic/static/assets/skin/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-button.css
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-combo-chart.css
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-container.css
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-datepicker.css
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-dropbox.css
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-gauge.css
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-general.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-grid-cell.css
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-grid-row.css
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-grid-table-cell.css
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-grid-table.css
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-grid.css
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-horizontal-table.css
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-horizontalbarchart.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-image.css
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-legend.css
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-line-area-chart.css
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-line-scatter-combo.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-page.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-panel.css
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-pie-chart.css
--rw-r--r--   0 runner    (1001) docker     (123)    20239 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-pivot-table.css
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-popup.css
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-radar-chart.css
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-scrolltable.css
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-segmented.css
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-segmentedbar.css
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-slider-touch.css
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-slider.css
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-text.css
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-textarea.css
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-textbox.css
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-toggle.css
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-tornado.css
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-vertical-line-box.css
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-waterfall.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.431998 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    75822 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.eot
--rw-r--r--   0 runner    (1001) docker     (123)   253851 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.svg
--rw-r--r--   0 runner    (1001) docker     (123)    75604 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    32032 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    23076 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    75582 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.eot
--rw-r--r--   0 runner    (1001) docker     (123)   256592 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.svg
--rw-r--r--   0 runner    (1001) docker     (123)    75356 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    32152 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff
--rw-r--r--   0 runner    (1001) docker     (123)    23124 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108091 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.svg
--rw-r--r--   0 runner    (1001) docker     (123)    26028 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.woff
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.435998 analogic-framework-4.1.1/analogic/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/authenticated.html
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/config.html
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/css.html
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/javascripts.html
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/redirect.html
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/sso_error.html
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/templates/unauthorized.html
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/version.config
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/analogic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:59:29.435998 analogic-framework-4.1.1/analogic_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-15 08:59:29.000000 analogic-framework-4.1.1/analogic_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11099 2023-04-15 08:59:29.000000 analogic-framework-4.1.1/analogic_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:59:29.000000 analogic-framework-4.1.1/analogic_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-15 08:59:29.000000 analogic-framework-4.1.1/analogic_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 08:59:29.000000 analogic-framework-4.1.1/analogic_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 08:59:29.435998 analogic-framework-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-15 08:59:11.000000 analogic-framework-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.271141 analogic-framework-4.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-10 13:49:42.271141 analogic-framework-4.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.243141 analogic-framework-4.1.2/analogic/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/analogic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27489 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/analogic_tm1_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/authentication_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/cam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/camsecure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/core_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/logging.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/loginbasic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/logincam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/nologin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/pivot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/setting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.235141 analogic-framework-4.1.2/analogic/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.239141 analogic-framework-4.1.2/analogic/static/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.243141 analogic-framework-4.1.2/analogic/static/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    48488 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   108539 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/css/bootstrap-grid.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.243141 analogic-framework-4.1.2/analogic/static/assets/css/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/css/lib/Chart-2.9.3.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/css/lib/nouislider.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    65538 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.243141 analogic-framework-4.1.2/analogic/static/assets/css/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/css/widgets/loader.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/css/widgets/simulation-panel-slider.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.243141 analogic-framework-4.1.2/analogic/static/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/images/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   120349 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/images/loading2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    55508 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/images/loading2_transparent.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/images/triangle.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.239141 analogic-framework-4.1.2/analogic/static/assets/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.243141 analogic-framework-4.1.2/analogic/static/assets/js/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)    20675 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/authentication.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.247141 analogic-framework-4.1.2/analogic/static/assets/js/framework/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/extensions/authentication-provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/extensions/write-executor.js
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/listener.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.247141 analogic-framework-4.1.2/analogic/static/assets/js/framework/load-executor/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/load-executor/array.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/load-executor/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/load-executor/default.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/load-executor/factory.js
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/load-executor/skip.js
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/load-executor/state.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.247141 analogic-framework-4.1.2/analogic/static/assets/js/framework/parsing-control/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/parsing-control/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/parsing-control/factory.js
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/parsing-control/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/parsing-control/matrix.js
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/parsing-control/object.js
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/parsing-control/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/parsing-control/skip.js
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/pivot.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/query-builder.js
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/redirect.js
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/render.js
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/rest-request.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/server.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22895 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.247141 analogic-framework-4.1.2/analogic/static/assets/js/framework/write-executor/
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/write-executor/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/write-executor/download.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/write-executor/factory.js
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/write-executor/function.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/write-executor/grid-table.js
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/framework/write-executor/skip.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.247141 analogic-framework-4.1.2/analogic/static/assets/js/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   172689 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/lib/Chart-2.9.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44136 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/lib/Sortable.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21295 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.251141 analogic-framework-4.1.2/analogic/static/assets/js/lib/chartjs4/
+-rw-r--r--   0 runner    (1001) docker     (123)   204509 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/lib/chartjs4/chart.umd.js
+-rw-r--r--   0 runner    (1001) docker     (123)   950937 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/lib/chartjs4/chart.umd.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/lib/chartjs4/chartjs-plugin-datalabels.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/lib/chartjs4/init.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.251141 analogic-framework-4.1.2/analogic/static/assets/js/lib/jquery/
+-rw-r--r--   0 runner    (1001) docker     (123)    89411 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/lib/jquery/jquery.actual.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/lib/jquery/jquery.cookie.js
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/lib/jquery/jquery.doubletap.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/lib/jquery/tableSort.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26460 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/lib/nouislider.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.255141 analogic-framework-4.1.2/analogic/static/assets/js/widgets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.255141 analogic-framework-4.1.2/analogic/static/assets/js/widgets/base/
+-rw-r--r--   0 runner    (1001) docker     (123)    23425 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/base/widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/button.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27762 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/combo-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/container.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18887 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/datepicker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.259141 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/BubbleChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/ButtonWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/ComboChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/ContainerWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/DatePickerWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/DropBoxWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/GaugeWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/GridCellWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/GridRowWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/GridWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/HistogramComboChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/HorizontalTableWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/ImageWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/LineAreaChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/PanelWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/PieChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/PopupWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/ScrollTableWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/SegmentedBarWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/SegmentedControlItemWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/SegmentedControlWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/SideBarWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/SimulationPanelSliderWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/SimulationPanelWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/SliderWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/SwipeWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/TextAreaWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/TextBoxWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/TextWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/ToggleWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/TornadoChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/VerticalLineBoxWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/WaterFallWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/dropbox.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/gauge.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.259141 analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid/grid-cell.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid/grid-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid/grid.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.263141 analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid-table/
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18941 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid-table/grid-table.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/histogram-combo-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/horizontal-bar-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/horizontal-table.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.263141 analogic-framework-4.1.2/analogic/static/assets/js/widgets/horizontaltable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/image.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18693 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/line-area-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26611 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/line-scatter-combo.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/loader.js
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/page.js
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/pie-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)    81168 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/pivot-table.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/popup.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/radar-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36449 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/scroll-table.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/segmented-bar.js
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/segmented-control-item.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/segmented-control.js
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/shadow.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/simulation-panel-slider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/simulation-panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19961 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/slider.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33957 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/stacked-column-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/swipe.js
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/system-popup.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20395 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/text.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/textarea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/textbox.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/toggle.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/tornado-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/vertical-line-box.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13525 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/js/widgets/water-fall.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.239141 analogic-framework-4.1.2/analogic/static/assets/skin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.267141 analogic-framework-4.1.2/analogic/static/assets/skin/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-button.css
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-combo-chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-container.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-datepicker.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-dropbox.css
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-gauge.css
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-general.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-grid-cell.css
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-grid-row.css
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-grid-table-cell.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-grid-table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-horizontal-table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-horizontalbarchart.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-image.css
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-legend.css
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-line-area-chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-line-scatter-combo.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-page.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-panel.css
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-pie-chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20239 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-pivot-table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-popup.css
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-radar-chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-scrolltable.css
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-segmented.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-segmentedbar.css
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-slider-touch.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-slider.css
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-text.css
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-textarea.css
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-textbox.css
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-toggle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-tornado.css
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-vertical-line-box.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-waterfall.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.271141 analogic-framework-4.1.2/analogic/static/assets/skin/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    75822 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Bold.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   253851 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Bold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    75604 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32032 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    23076 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    75582 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Medium.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   256592 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Medium.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    75356 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32152 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    23124 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/fonts/pivot.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108091 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/fonts/pivot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26028 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/fonts/pivot.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/static/assets/skin/fonts/pivot.woff
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.271141 analogic-framework-4.1.2/analogic/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/templates/authenticated.html
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/templates/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/templates/css.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/templates/javascripts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/templates/redirect.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/templates/sso_error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/templates/unauthorized.html
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/version.config
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/analogic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:49:42.271141 analogic-framework-4.1.2/analogic_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-10 13:49:42.000000 analogic-framework-4.1.2/analogic_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-07-10 13:49:42.000000 analogic-framework-4.1.2/analogic_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:49:42.000000 analogic-framework-4.1.2/analogic_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-10 13:49:42.000000 analogic-framework-4.1.2/analogic_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 13:49:42.000000 analogic-framework-4.1.2/analogic_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 13:49:42.271141 analogic-framework-4.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-10 13:49:24.000000 analogic-framework-4.1.2/setup.py
```

### Comparing `analogic-framework-4.1.1/LICENSE` & `analogic-framework-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/README.md` & `analogic-framework-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/__init__.py` & `analogic-framework-4.1.2/analogic/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,7 +18,8 @@
 from .nologin import NoLogin
 from .camsecure import CamSecure
 from . import core_endpoints
 from .task import scheduler
 from .exceptions import AnalogicException
 from .exceptions import AnalogicProxyException
 from .exceptions import AnalogicTM1ServiceException
+from .exceptions import AnalogicAccessDeniedException
```

### Comparing `analogic-framework-4.1.1/analogic/analogic.py` & `analogic-framework-4.1.2/analogic/analogic.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 import json
 import sys
 from importlib import resources
 from analogic.core_endpoints import core_endpoints
 from analogic.authentication_provider import AuthenticationProvider
 from analogic.condition import Condition
 import inspect
-from flask_caching import Cache
 from analogic.setting import SettingManager
 from datetime import timedelta
 import importlib
-from analogic.version import version
 from analogic.task import scheduler
 import atexit
 
 APPLICATIONS_DIR = 'apps'
 APPLICATIONS_DIR_EXTRA = os.environ.get('APPLICATIONS_DIR_EXTRA', '')
 EXTENSIONS_DIR = 'extensions'
 EXTENSIONS_DIR_EXTRA = os.environ.get('EXTENSIONS_DIR_EXTRA', '')
@@ -76,15 +74,15 @@
             self.register_analogic_url_rules(instance)
 
             self.analogic_applications[blueprint.name] = self.create_authentication_provider(blueprint.name,
                                                                                          application_dir)
 
             super().register_blueprint(blueprint, **options)
         except Exception as e:
-            logging.getLogger(__name__).error('Error registering application' + blueprint.name + ': ' + str(e))
+            logging.getLogger(__name__).error('Error registering application ' + blueprint.name + ': ' + str(e))
 
     def create_authentication_provider(self, analogic_application, analogic_application_path):
         with self.app_context():
             setting = SettingManager(analogic_application_path, analogic_application)
             config = setting.config
 
             class_name = config['authenticationMode']
@@ -142,15 +140,15 @@
     def evaluate_condition(self, config):
         class_name = config.get('authenticationModeCondition')
         module_name = self.get_condition_module_name(class_name)
 
         if module_name in sys.modules:
             module = sys.modules[module_name]
         else:
-            module = importlib.import_module(module_name)  # Todo ModuleNotFoundError
+            module = importlib.import_module(module_name)
 
         condition_class = getattr(module, class_name)
         condition = condition_class()
         return condition.get_authentication_provider_name(config)
 
     def on_exit(self):
         print('on_exit')
@@ -275,15 +273,15 @@
 
 
 def _load_modules(app, modules_dir, check_prefix, register_func):
     for module_dir_name in os.listdir(modules_dir):
 
         module_dir = os.path.join(modules_dir, module_dir_name)
 
-        if os.path.isdir(module_dir) and module_dir_name != '.git' and (
+        if os.path.isdir(module_dir) and module_dir_name != '.git' and module_dir_name != 'tests' and (
                 check_prefix is False or (
                 module_dir_name.startswith(ALLOWED_EXTENSION_PREFIX) and not module_dir_name.endswith('dist-info'))):
 
             # workaround to handle repeating names in module path
             if module_dir_name == modules_dir.rsplit('/', 1)[-1]:
                 module_dir_name = module_dir_name + '.' + module_dir_name
 
@@ -304,14 +302,16 @@
         for name, obj in inspect.getmembers(sys.modules[module]):
             if isinstance(obj, Blueprint):
                 app.register_application(application_dir=application_dir, blueprint=obj)
 
 
 def _fast_scan_dir(directory, ext):
     sub_folders, files = [], {}
+    if '.git' in directory or 'tests' in directory:
+        return sub_folders, files
 
     for f in os.scandir(directory):
         if f.is_dir():
             sub_folders.append(f.path)
         if f.is_file():
             if os.path.splitext(f.name)[1].lower() in ext:
                 files[f.name] = f.path
```

### Comparing `analogic-framework-4.1.1/analogic/analogic_tm1_service.py` & `analogic-framework-4.1.2/analogic/analogic_tm1_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from TM1py import TM1Service
 from TM1py.Services import HierarchyService, SecurityService, ApplicationService, SubsetService, ServerService, \
     MonitoringService, ProcessService, PowerBiService, AnnotationService, ViewService, RestService, CellService, \
     ChoreService, DimensionService, CubeService, ElementService, SandboxService, GitService
+from TM1py.Services.FileService import FileService
 from TM1py.Utils import case_and_space_insensitive_equals
-from typing import Union
+import json
+from json import JSONDecodeError
 from requests import Session as BaseSession
 from requests.adapters import HTTPAdapter as BaseHTTPAdapter
-from requests.adapters import (DEFAULT_POOLBLOCK, DEFAULT_POOLSIZE, DEFAULT_RETRIES, DEFAULT_POOL_TIMEOUT)
+from requests.adapters import (DEFAULT_POOLBLOCK, DEFAULT_POOLSIZE, DEFAULT_RETRIES)
 from requests import Request
 from requests import Response as BaseResponse
 import http.client as http_client
+import socket
+import requests
 
-from urllib3.response import HTTPResponse
+import urllib3
 from urllib3.util import Timeout as TimeoutSauce
 from urllib3.exceptions import ClosedPoolError
 from urllib3.exceptions import ConnectTimeoutError
 from urllib3.exceptions import HTTPError as _HTTPError
 from urllib3.exceptions import MaxRetryError
 from urllib3.exceptions import NewConnectionError
 from urllib3.exceptions import ProxyError as _ProxyError
@@ -57,15 +61,15 @@
             allow_redirects=True,
             proxies=None,
             hooks=None,
             stream=None,
             verify=None,
             cert=None,
             json=None,
-            decode_content=True
+            decode_content=True  # mod
     ):
         """Constructs a :class:`Request <Request>`, prepares it and sends it.
         Returns :class:`Response <Response>` object.
 
         :param method: method for the new :class:`Request` object.
         :param url: URL for the new :class:`Request` object.
         :param params: (optional) Dictionary or bytes to be sent in the query
@@ -125,26 +129,26 @@
             prep.url, proxies, stream, verify, cert
         )
 
         # Send the request.
         send_kwargs = {
             "timeout": timeout,
             "allow_redirects": allow_redirects,
-            "decode_content": decode_content
+            "decode_content": decode_content  # mod
         }
         send_kwargs.update(settings)
         resp = self.send(prep, **send_kwargs)
 
         return resp
 
 
 class Response(BaseResponse):
-    def __init__(self, decode_content=True):
+    def __init__(self, decode_content=True):  # mod
         super().__init__()
-        self._decode_content = decode_content
+        self._decode_content = decode_content  # mod
 
     def iter_content(self, chunk_size=1, decode_unicode=False):
         """Iterates over the response data.  When stream=True is set on the
         request, this avoids reading the content at once into memory for
         large responses.  The chunk size is the number of bytes it should
         read into memory.  This is not necessarily the length of each item
         returned as decoding can take place.
@@ -159,30 +163,30 @@
         available encoding based on the response.
         """
 
         def generate():
             # Special case for urllib3.
             if hasattr(self.raw, "stream"):
                 try:
-                    yield from self.raw.stream(chunk_size, decode_content=self._decode_content)
+                    yield from self.raw.stream(chunk_size, decode_content=self._decode_content)  # mod
                 except ProtocolError as e:
                     raise ChunkedEncodingError(e)
                 except DecodeError as e:
                     raise ContentDecodingError(e)
                 except ReadTimeoutError as e:
                     raise ConnectionError(e)
                 except SSLError as e:
                     raise RequestsSSLError(e)
             else:
                 # Standard file-like object.
                 while True:
-                    if self._decode_content:
-                        chunk = self.raw.read(chunk_size)
-                    else:
-                        chunk = self.raw.read(chunk_size, decode_content=False)
+                    if self._decode_content:  # mod
+                        chunk = self.raw.read(chunk_size)  # mod
+                    else:  # mod
+                        chunk = self.raw.read(chunk_size, decode_content=False)  # mod
                     if not chunk:
                         break
                     yield chunk
 
             self._content_consumed = True
 
         if self._content_consumed and isinstance(self._content, bool):
@@ -199,15 +203,15 @@
         chunks = reused_chunks if self._content_consumed else stream_chunks
 
         if decode_unicode:
             chunks = stream_decode_response_unicode(chunks, self)
 
         return chunks
 
-    def get_decompressed_data(self):
+    def get_decompressed_data(self):  # mod add
         text = ''
         try:
             gzip_decoder = GzipDecoder()
             text = gzip_decoder.decompress(self.content).decode('utf-8')
         except Exception:
             logging.getLogger(__name__).error('Failed to decompress data')
         return text
@@ -217,15 +221,15 @@
 
     def __init__(self, pool_connections=DEFAULT_POOLSIZE,
                  pool_maxsize=DEFAULT_POOLSIZE, max_retries=DEFAULT_RETRIES,
                  pool_block=DEFAULT_POOLBLOCK):
         super().__init__(pool_connections, pool_maxsize, max_retries, pool_block)
 
     def send(
-            self, request, stream=False, timeout=None, verify=True, cert=None, proxies=None, decode_content=True
+            self, request, stream=False, timeout=None, verify=True, cert=None, proxies=None, decode_content=True  # mod
     ):
         """Sends PreparedRequest object. Returns Response object.
 
         :param request: The :class:`PreparedRequest <PreparedRequest>` being sent.
         :param stream: (optional) Whether to stream the request content.
         :param timeout: (optional) How long to wait for the server to send
             data before giving up, as a float, or a :ref:`(connect timeout,
@@ -268,71 +272,27 @@
                 )
         elif isinstance(timeout, TimeoutSauce):
             pass
         else:
             timeout = TimeoutSauce(connect=timeout, read=timeout)
 
         try:
-            if not chunked:
-                resp = conn.urlopen(
-                    method=request.method,
-                    url=url,
-                    body=request.body,
-                    headers=request.headers,
-                    redirect=False,
-                    assert_same_host=False,
-                    preload_content=False,
-                    decode_content=False,
-                    retries=self.max_retries,
-                    timeout=timeout,
-                )
-
-            # Send the request.
-            else:
-                if hasattr(conn, "proxy_pool"):
-                    conn = conn.proxy_pool
-
-                low_conn = conn._get_conn(timeout=DEFAULT_POOL_TIMEOUT)
-
-                try:
-                    skip_host = "Host" in request.headers
-                    low_conn.putrequest(
-                        request.method,
-                        url,
-                        skip_accept_encoding=True,
-                        skip_host=skip_host,
-                    )
-
-                    for header, value in request.headers.items():
-                        low_conn.putheader(header, value)
-
-                    low_conn.endheaders()
-
-                    for i in request.body:
-                        low_conn.send(hex(len(i))[2:].encode("utf-8"))
-                        low_conn.send(b"\r\n")
-                        low_conn.send(i)
-                        low_conn.send(b"\r\n")
-                    low_conn.send(b"0\r\n\r\n")
-
-                    # Receive the response from the server
-                    r = low_conn.getresponse()
-
-                    resp = HTTPResponse.from_httplib(
-                        r,
-                        pool=conn,
-                        connection=low_conn,
-                        preload_content=False,
-                        decode_content=False,
-                    )
-                except Exception:
-                    # If we hit any problems here, clean up the connection.
-                    # Then, raise so that we can handle the actual exception.
-                    low_conn.close()
-                    raise
+            resp = conn.urlopen(
+                method=request.method,
+                url=url,
+                body=request.body,
+                headers=request.headers,
+                redirect=False,
+                assert_same_host=False,
+                preload_content=False,
+                decode_content=False,
+                retries=self.max_retries,
+                timeout=timeout,
+                chunked=chunked,
+            )
 
         except (ProtocolError, OSError) as err:
             raise ConnectionError(err, request=request)
 
         except MaxRetryError as e:
             if isinstance(e.reason, ConnectTimeoutError):
                 # TODO: Remove this in 3.0.0: see #2811
@@ -364,27 +324,27 @@
             elif isinstance(e, ReadTimeoutError):
                 raise ReadTimeout(e, request=request)
             elif isinstance(e, _InvalidHeader):
                 raise InvalidHeader(e, request=request)
             else:
                 raise
 
-        return self.build_response(request, resp, decode_content)
+        return self.build_response(request, resp, decode_content)  # mod
 
-    def build_response(self, req, resp, decode_content=True):
+    def build_response(self, req, resp, decode_content=True):  # mod
         """Builds a :class:`Response <requests.Response>` object from a urllib3
         response. This should not be called from user code, and is only exposed
         for use when subclassing the
         :class:`HTTPAdapter <requests.adapters.HTTPAdapter>`
 
         :param req: The :class:`PreparedRequest <PreparedRequest>` used to generate the response.
         :param resp: The urllib3 response object.
         :rtype: requests.Response
         """
-        response = Response(decode_content=decode_content)
+        response = Response(decode_content=decode_content)  # mod
 
         # Fallback to None if there's no status_code, for whatever reason.
         response.status_code = getattr(resp, "status", None)
 
         # Make headers case-insensitive.
         response.headers = CaseInsensitiveDict(getattr(resp, "headers", {}))
 
@@ -404,14 +364,25 @@
         # Give the Response some context.
         response.request = req
         response.connection = self
 
         return response
 
 
+class HTTPAdapterWithSocketOptions(HTTPAdapter):  # mod added for our adapter
+    def __init__(self, *args, **kwargs):
+        self.socket_options = kwargs.pop("socket_options", None)
+        super(HTTPAdapterWithSocketOptions, self).__init__(*args, **kwargs)
+
+    def init_poolmanager(self, *args, **kwargs):
+        if self.socket_options is not None:
+            kwargs["socket_options"] = self.socket_options
+        super(HTTPAdapterWithSocketOptions, self).init_poolmanager(*args, **kwargs)
+
+
 class AnalogicRestService(RestService):
 
     def __init__(self, **kwargs):
         """ Create an instance of RESTService
         :param address: String - address of the TM1 instance
         :param port: Int - HTTPPortNumber as specified in the tm1s.cfg
         :param base_url - base url e.g. https://localhost:12354/api/v1
@@ -419,39 +390,71 @@
         :param password String - password of the user
         :param decode_b64 - whether password argument is b64 encoded
         :param namespace String - optional CAM namespace
         :param ssl: boolean -  as specified in the tm1s.cfg
         :param cam_passport: String - the cam passport
         :param session_id: String - TM1SessionId e.g. q7O6e1w49AixeuLVxJ1GZg
         :param session_context: String - Name of the Application. Controls "Context" column in Arc / TM1top.
-        If None, use default: TM1py
+                If None, use default: TM1py
         :param verify: path to .cer file or 'True' / True / 'False' / False (if no ssl verification is required)
         :param logging: boolean - switch on/off verbose http logging into sys.stdout
         :param timeout: Float - Number of seconds that the client will wait to receive the first byte.
+        :param cancel_at_timeout: Abort operation in TM1 when timeout is reached
         :param async_requests_mode: changes internal REST execution mode to avoid 60s timeout on IBM cloud
-        :param connection_pool_size - In a multithreaded environment, you should set this value to a
-        higher number, such as the number of threads
+        :param tcp_keepalive: maintain the TCP connection all the time, users should choose either async_requests_mode or tcp_keepalive to run a long-run request
+                If both are True, use async_requests_mode by default
+        :param connection_pool_size - In a multi threaded environment, you should set this value to a
+                higher number, such as the number of threads
         :param integrated_login: True for IntegratedSecurityMode3
         :param integrated_login_domain: NT Domain name.
                 Default: '.' for local account.
         :param integrated_login_service: Kerberos Service type for remote Service Principal Name.
                 Default: 'HTTP'
         :param integrated_login_host: Host name for Service Principal Name.
                 Default: Extracted from request URI
         :param integrated_login_delegate: Indicates that the user's credentials are to be delegated to the server.
                 Default: False
         :param impersonate: Name of user to impersonate
+        :param re_connect_on_session_timeout: attempt to reconnect once if session is timed out
+        :param proxies: pass a dictionary with proxies e.g.
+                {'http': 'http://proxy.example.com:8080', 'https': 'http://secureproxy.example.com:8090'}
         """
+        # store kwargs for future use e.g. re_connect on 401 session timeout
         self._kwargs = kwargs
+
         self._ssl = self.translate_to_boolean(kwargs.get('ssl', True))
         self._address = kwargs.get('address', None)
         self._port = kwargs.get('port', None)
         self._verify = False
         self._timeout = None if kwargs.get('timeout', None) is None else float(kwargs.get('timeout'))
+        self._cancel_at_timeout = kwargs.get('cancel_at_timeout', False)
         self._async_requests_mode = self.translate_to_boolean(kwargs.get('async_requests_mode', False))
+        # Set tcp_keepalive to False explicitly to turn it off when async_requests_mode is enabled
+        self._tcp_keepalive = self.translate_to_boolean(
+            kwargs.get('tcp_keepalive', False)) \
+            if self._async_requests_mode is not True \
+            else False
+        self._connection_pool_size = kwargs.get('connection_pool_size', None)
+        self._re_connect_on_session_timeout = kwargs.get('re_connect_on_session_timeout', True)
+
+        # Logging
+        if 'logging' in kwargs:
+            if self.translate_to_boolean(value=kwargs['logging']):
+                http_client.HTTPConnection.debuglevel = 1
+
+        self._proxies = kwargs.get('proxies', None)
+        # handle invalid types and potential string argument
+        if not isinstance(self._proxies, (dict, str, type(None))):
+            raise ValueError("Argument of 'proxies' must be None, dictionary or JSON string")
+        elif isinstance(self._proxies, str):
+            try:
+                self._proxies = json.loads(self._proxies)
+            except JSONDecodeError:
+                raise ValueError("Invalid JSON passed for argument 'proxies': %s", self._proxies)
+
         # populated on the fly
         if kwargs.get('user'):
             self._is_admin = True if case_and_space_insensitive_equals(kwargs.get('user'), 'ADMIN') else None
         else:
             self._is_admin = None
 
         if 'verify' in kwargs:
@@ -479,59 +482,107 @@
 
         self._version = None
         self._headers = self.HEADERS.copy()
         if "session_context" in kwargs:
             self._headers["TM1-SessionContext"] = kwargs["session_context"]
 
         self.disable_http_warnings()
-        # re-use or create tm1 http session
-        self._s = Session()
 
-        # manage connection pool
-        if "connection_pool_size" in kwargs:
-            self._manage_http_connection_pool(kwargs.get("connection_pool_size"))
+        self._s = Session()  # mod out Session
 
-        if "session_id" in kwargs:
-            self._s.cookies.set("TM1SessionId", kwargs["session_id"])
-        else:
-            self._start_session(
-                user=kwargs.get("user", None),
-                password=kwargs.get("password", None),
-                namespace=kwargs.get("namespace", None),
-                gateway=kwargs.get("gateway", None),
-                cam_passport=kwargs.get("cam_passport", None),
-                decode_b64=self.translate_to_boolean(kwargs.get("decode_b64", False)),
-                integrated_login=self.translate_to_boolean(kwargs.get("integrated_login", False)),
-                integrated_login_domain=kwargs.get("integrated_login_domain"),
-                integrated_login_service=kwargs.get("integrated_login_service"),
-                integrated_login_host=kwargs.get("integrated_login_host"),
-                integrated_login_delegate=kwargs.get("integrated_login_delegate"),
-                impersonate=kwargs.get("impersonate", None))
+        if self._tcp_keepalive or self._connection_pool_size is not None: #mod move from end of method
+            self._manage_http_adapter()
+
+        if self._proxies:
+            self._s.proxies = self._proxies
+
+        self.connect()
 
         if not self._version:
             self.set_version()
 
+        # is retrieved on demand and cached
         self._sandboxing_disabled = None
 
-        # Logging
-        if 'logging' in kwargs:
-            if self.translate_to_boolean(value=kwargs['logging']):
-                http_client.HTTPConnection.debuglevel = 1
+    def _manage_http_adapter(self):  # mod override for using our base adapter
+        if self._tcp_keepalive:
+            # SO_KEEPALIVE: set 1 to enable TCP keepalive
+            socket_options = urllib3.connection.HTTPConnection.default_socket_options + [
+                (socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1),
+                (socket.IPPROTO_TCP, socket.TCP_KEEPIDLE, self.TCP_SOCKET_OPTIONS['TCP_KEEPIDLE']),
+                (socket.IPPROTO_TCP, socket.TCP_KEEPINTVL, self.TCP_SOCKET_OPTIONS['TCP_KEEPINTVL']),
+                (socket.IPPROTO_TCP, socket.TCP_KEEPCNT, self.TCP_SOCKET_OPTIONS['TCP_KEEPCNT'])]
+
+            if self._connection_pool_size is not None:
+                adapter = HTTPAdapterWithSocketOptions(
+                    pool_connections=int(self._connection_pool_size),
+                    pool_maxsize=int(self._connection_pool_size),
+                    socket_options=socket_options)
+            else:
+                adapter = HTTPAdapterWithSocketOptions(socket_options=socket_options)
 
-    def _manage_http_connection_pool(self, connection_pool_size: Union[str, int]):
-        self._s.mount(
-            self._base_url,
-            HTTPAdapter(
-                pool_connections=int(connection_pool_size),
-                pool_maxsize=int(connection_pool_size)))
+        else:
+            adapter = HTTPAdapterWithSocketOptions(
+                pool_connections=int(self._connection_pool_size),
+                pool_maxsize=int(self._connection_pool_size))
+
+        self._s.mount(self._base_url, adapter)
+
+    # @staticmethod
+    # def build_response_from_raw_bytes(data: bytes) -> Response:
+    #     urllib_response = RestService.urllib3_response_from_bytes(data)
+    #
+    #     adapter = HTTPAdapter()
+    #     requests_response = adapter.build_response(requests.PreparedRequest(), urllib_response)
+    #     # actual content of response needs to be set explicitly
+    #     requests_response._content = urllib_response.data
+    #
+    #     return requests_response
 
 
 class AnalogicTM1Service(TM1Service):
 
     def __init__(self, **kwargs):
+        """ Initiate the TM1Service
+
+            :param address: String - address of the TM1 instance
+            :param port: Int - HTTPPortNumber as specified in the tm1s.cfg
+            :param base_url - base url e.g. https://localhost:12354/api/v1
+            :param user: String - name of the user
+            :param password String - password of the user
+            :param decode_b64 - whether password argument is b64 encoded
+            :param namespace String - optional CAM namespace
+            :param ssl: boolean -  as specified in the tm1s.cfg
+            :param cam_passport: String - the cam passport
+            :param session_id: String - TM1SessionId e.g. q7O6e1w49AixeuLVxJ1GZg
+            :param session_context: String - Name of the Application. Controls "Context" column in Arc / TM1top.
+                If None, use default: TM1py
+            :param verify: path to .cer file or 'True' / True / 'False' / False (if no ssl verification is required)
+            :param logging: boolean - switch on/off verbose http logging into sys.stdout
+            :param timeout: Float - Number of seconds that the client will wait to receive the first byte.
+            :param cancel_at_timeout: Abort operation in TM1 when timeout is reached
+            :param async_requests_mode: changes internal REST execution mode to avoid 60s timeout on IBM cloud
+            :param tcp_keepalive: maintain the TCP connection all the time, users should choose either async_requests_mode or tcp_keepalive to run a long-run request
+                    If both are True, use async_requests_mode by default
+            :param connection_pool_size - In a multi threaded environment, you should set this value to a
+                    higher number, such as the number of threads
+            :param integrated_login: True for IntegratedSecurityMode3
+            :param integrated_login_domain: NT Domain name.
+                    Default: '.' for local account.
+            :param integrated_login_service: Kerberos Service type for remote Service Principal Name.
+                    Default: 'HTTP'
+            :param integrated_login_host: Host name for Service Principal Name.
+                    Default: Extracted from request URI
+            :param integrated_login_delegate: Indicates that the user's credentials are to be delegated to the server.
+                    Default: False
+            :param impersonate: Name of user to impersonate
+            :param re_connect_on_session_timeout: attempt to reconnect once if session is timed out
+            :param proxies: pass a dictionary with proxies e.g.
+                    {'http': 'http://proxy.example.com:8080', 'https': 'http://secureproxy.example.com:8090'}
+            """
         self._tm1_rest = AnalogicRestService(**kwargs)
         self.annotations = AnnotationService(self._tm1_rest)
         self.cells = CellService(self._tm1_rest)
         self.chores = ChoreService(self._tm1_rest)
         self.cubes = CubeService(self._tm1_rest)
         self.dimensions = DimensionService(self._tm1_rest)
         self.elements = ElementService(self._tm1_rest)
@@ -542,18 +593,19 @@
         self.processes = ProcessService(self._tm1_rest)
         self.security = SecurityService(self._tm1_rest)
         self.server = ServerService(self._tm1_rest)
         self.subsets = SubsetService(self._tm1_rest)
         self.applications = ApplicationService(self._tm1_rest)
         self.views = ViewService(self._tm1_rest)
         self.sandboxes = SandboxService(self._tm1_rest)
-        self.git = GitService(self._tm1_rest)
+        self.files = FileService(self._tm1_rest)
 
-    def re_authenticate(self):
-        self._tm1_rest = AnalogicRestService(**self.connection._kwargs)
-        self._instantiate_services()
+    # def re_authenticate(self):
+    #     # self._tm1_rest = AnalogicRestService(**self.connection._kwargs)
+    #     # self._instantiate_services()
+    #     self._tm1_rest.connect()
 
     def get_session(self):
         return self._tm1_rest._s
 
     def close_session(self):
         self._tm1_rest._s.close()
```

### Comparing `analogic-framework-4.1.1/analogic/authentication_provider.py` & `analogic-framework-4.1.2/analogic/cam.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,100 @@
-from flask import session, current_app, send_file, request, jsonify
-from analogic.loader import ClassLoader
-import analogic.pivot as PivotApi
-from analogic.exceptions import AnalogicProxyException
-import logging
-import pandas as pd
-from abc import ABC, abstractmethod
-from functools import wraps
+from analogic.authentication_provider import AuthenticationProvider
+from flask import render_template, request, make_response, redirect, session, Response, send_file
+from analogic.analogic_tm1_service import AnalogicTM1Service
 import orjson
+import analogic.pivot as PivotApi
+from analogic.exceptions import AnalogicTM1ServiceException
+from analogic.loader import ClassLoader
+from analogic.authentication_provider import login_required
+
+
+class Cam(AuthenticationProvider):
 
-pd.set_option('display.float_format', lambda x: '%.3f' % x)
+    def __init__(self, setting):
+        super().__init__(setting)
 
+    def index(self):
+        authenticated = request.cookies.get('authenticated') is not None and self.check_app_authenticated()
+        return render_template('index.html', authenticated=authenticated, cnf=self.setting.get_config())
 
-def get_authentication_provider():
-    return current_app.get_authentication_provider()
+    def auth(self):
+        resp = make_response(redirect(self.setting.get_base_url()))
+        resp.set_cookie('camPassport', request.form.get('c_pp'))
 
+        cam_name = self.set_tm1_service(request.form.get('c_pp'))
+        session[self.logged_in_user_session_name] = cam_name
+        self.load_permissions()
+        return self._add_authenticated_cookies(resp)
 
-def endpoint_login_required(f):
-    @wraps(f)
-    def decorated_function(*args, **kwargs):
-        auth_provider = get_authentication_provider()
-        if auth_provider.check_app_authenticated is False:
-            return auth_provider.get_authentication_required_response()
-        return f(*args, **kwargs)
+    def get_base_url(self):
+        return self.setting.get_config()['apiHost']
 
-    return decorated_function
+    def set_tm1_service(self, cam_passport):
+        cnf = self.setting.get_config()
 
+        tm1_service = AnalogicTM1Service(base_url=self.get_base_url(),
+                                         cam_passport=cam_passport,
+                                         connection_pool_size=100,
+                                         ssl=self.setting.get_ssl_verify())
 
-def login_required(f):
-    @wraps(f)
-    def decorated_function(*args, **kwargs):
-        auth_provider = args[0]
-        if auth_provider.check_app_authenticated is False:
-            return auth_provider.get_authentication_required_response()
-        return f(*args, **kwargs)
+        response = tm1_service.get_session().request('GET', self.get_base_url() + cnf['apiSubPath'] + 'ActiveUser',
+                                                     headers=self.HEADERS, verify=self.setting.get_ssl_verify())
 
-    return decorated_function
+        json_object = response.json()
+        cam_name = json_object['Name']
 
+        existing_tm1_service = self.setting.get_tm1_service(cam_name)
 
-class AuthenticationProvider(ABC):
-    HEADERS = {'Connection': 'keep-alive',
-               'User-Agent': 'Analogic',
-               'Content-Type': 'application/json; odata.streaming=true; charset=utf-8',
-               'Accept': 'application/json;odata.metadata=none,text/plain',
-               'Accept-Encoding': 'gzip, deflate, br',
-               'TM1-SessionContext': 'Analogic'}
+        if existing_tm1_service is not None:
+            try:
+                existing_tm1_service.close_session()
+            except Exception as e:
+                self._logger.error('exception while closing session: ' + str(e))
 
-    def __init__(self, setting):
-        self.setting = setting
-        self.logged_in_user_session_name = self.setting.get_instance() + '_logged_in_user_name'
-        self._logger = logging.getLogger(self.setting.get_instance())
+        self.setting.set_tm1_service(cam_name, tm1_service)
 
-    def initialize(self):
-        self.setting.initialize()
+        return cam_name
 
-    def get_setting(self):
-        return self.setting
+    def _create_request_with_authenticated_user(self, url, method, mdx, headers, cookies, decode_content=True):
+        tm1_service = self.setting.get_tm1_service(session.get(self.logged_in_user_session_name))
+        if tm1_service is None:
+            return Response('Unauthorized', status=401, mimetype='application/json')
 
-    def get_logged_in_user_name(self):
-        return session.get(self.logged_in_user_session_name)
+        response = tm1_service.get_session().request(method, url, data=mdx, headers=headers,
+                                                     verify=self.setting.get_ssl_verify(), decode_content=decode_content)
+        if response.status_code == 401:
+            try:
+                tm1_service.re_authenticate()
+            except Exception as e:
+                self._logger.error('exception while re-authenticating: ' + str(e))
+                return Response('Unauthorized', status=401, mimetype='application/json')
+            response = tm1_service.get_session().request(method, url, data=mdx, headers=headers,
+                                                         verify=self.setting.get_ssl_verify(), decode_content=decode_content)
+        return response
+
+    def _get_server_side_mdx(self, force_server_side_query=False):
+        mdx = request.data
+        if request.args.get('server') is not None:
+            body = orjson.loads(request.data)
+            key = body['key']
+            if body.get('key_suffix') is not None:
+                key = key + '_' + body['key_suffix']
+            mdx = self.setting.get_mdx(key)
+            mdx = self._set_custom_mdx_data(mdx)
+            for k in body:
+                mdx = mdx.replace('$' + k, body[k].replace('"', '\\"'))
+
+            return mdx.encode('utf-8')
+
+        return mdx
+
+    def check_app_authenticated(self):
+        return session.get(self.logged_in_user_session_name, '') != '' and self.setting.get_tm1_service(
+            session.get(self.logged_in_user_session_name)) is not None
 
     @login_required
     def pivot(self):
         username = self.get_logged_in_user_name()
 
         v = request.values
         cube_name = v.get('cube_name')
@@ -70,15 +103,20 @@
         subset_name = v.get('subset_name')
         element_names = v.getlist('element_names[]')
         subset_name_to_remove = v.get('subset_name_to_remove')
         selected_cards = v.get('selected_cards')
         options = orjson.loads(v.get('options', '{}'))
         export_data = v.get('export_data')
 
-        return PivotApi.call(self.get_tm1_service(), username, cube_name, dimension_name, hierarchy_name, subset_name,
+        try:
+            tm1_service = self.get_tm1_service()
+        except AnalogicTM1ServiceException as e:
+            return Response('Unauthorized', status=401, mimetype='application/json')
+
+        return PivotApi.call(tm1_service, username, cube_name, dimension_name, hierarchy_name, subset_name,
                              element_names, subset_name_to_remove, selected_cards, options, export_data)
 
     @login_required
     def export(self):
 
         file_name = request.args.get('file_name', default='export.xlsx')
         export_key = request.args.get('export_key')
@@ -87,137 +125,43 @@
             return self.get_not_found_response()
 
         export_description = self.setting.get_custom_object_description(export_key)
 
         if export_description is None:
             return self.get_not_found_response()
 
-        return send_file(ClassLoader().call(export_description, request, self.get_tm1_service(), self.setting, self),
-                         attachment_filename=file_name,
-                         as_attachment=True,
-                         cache_timeout=0,
-                         mimetype='application/vnd.openxmlformats-officedocument.spreadsheetml.sheet')
-
-    @login_required
-    def middleware(self):
-        key = request.args.get('key')
-
-        if key is None:
-            return self.get_not_found_response()
-
-        description = self.setting.get_custom_object_description(key)
-
-        return ClassLoader().call(description, request, self.get_tm1_service(), self.setting, self)
-
-    def _get_server_side_mdx(self):
-        mdx = request.data
-        if request.args.get('server') is not None:
-            body = orjson.loads(request.data)
-            key = body['key']
-            if body.get('key_suffix') is not None:
-                key = key + '_' + body['key_suffix']
-            mdx = self.setting.get_mdx(key)
-            mdx = self._set_custom_mdx_data(mdx)
-            for k in body:
-                mdx = mdx.replace('$' + k, body[k].replace('"', '\\"'))
-
-            return mdx.encode('utf-8')
-
-        return mdx
-
-    @abstractmethod
-    def index(self):
-        pass
-
-    @abstractmethod
-    def check_app_authenticated(self):
-        return True
-
-    @abstractmethod
-    def get_authentication_required_response(self):
-        pass
-
-    def get_not_found_response(self):
-        return 'Not found', 404, {'Content-Type': 'application/json'}
-
-    def _add_authenticated_cookies(self, response, max_age=None):
-        m = max_age
-        if max_age is None:
-            cnf = self.setting.get_config()
-            m = cnf['sessionExpiresInMinutes'] * 60
-        # TODO secure, httpOnly!!!
-        response.set_cookie('authenticated', 'authenticated', max_age=m)
-        return response
-
-    def _set_custom_mdx_data(self, mdx):
-        return mdx
-
-    @login_required
-    def proxy(self, sub_path):
-
-        self._extend_login_session()
-
-        target_url = self.setting.get_proxy_target_url()
-
-        mdx = self._get_server_side_mdx()
-
-        url = target_url + "/" + sub_path + (
-            "?" + request.query_string.decode('UTF-8') if len(
-                request.query_string) > 0 else "")
-
-        method = request.method
-
-        headers: dict[str, str] = self.HEADERS.copy()
-        cookies: dict[str, str] = {}
-
         try:
-            response = self.do_proxy_request(url, method, mdx, headers, cookies, False)
-        except AnalogicProxyException as e:
-            self._logger.error(e)
-            return 'Something went wrong', 500, {'Content-Type': 'application/json'}
-
-        if response.status_code == 400 or response.status_code == 500:
-            self._logger.error('MDX error: ' + response.get_decompressed_data())
-            self._logger.error('MDX: ' + mdx.decode('utf-8'))
-
-        if response.status_code == 401:
-            return 'Authentication required', 401, {'Content-Type': 'application/json'}
-
-        return response.content, response.status_code, {
-            'Content-Type': 'application/json; odata.metadata=minimal; odata.streaming=true; charset=utf-8',
-            'Content-Encoding': 'gzip'}
-
-    def do_proxy_request(self, url, method, mdx, headers=None, cookies=None, decode_content=True):
-
-        if headers is None:
-            headers: dict[str, str] = self.HEADERS.copy()
+            tm1_service = self.get_tm1_service()
+        except AnalogicTM1ServiceException as e:
+            return Response('Unauthorized', status=401, mimetype='application/json')
 
-        if cookies is None:
-            cookies: dict[str, str] = {}
-
-        return self._create_request_with_authenticated_user(url, method, mdx, headers, cookies, decode_content)
+        try:
+            response = ClassLoader().call(export_description, request, tm1_service, self.setting, self)
+        except Exception as e:
+            self.getLogger().error(e, exc_info=True)
+            return {'message': str(e)}, 404, {'Content-type': 'application/json'}
 
-    @abstractmethod
-    def _create_request_with_authenticated_user(self, url, method, mdx, headers, cookies, decode_content=True):
-        pass
+        return send_file(response,
+                         download_name=file_name,
+                         as_attachment=True,
+                         max_age=0,
+                         mimetype='application/vnd.openxmlformats-officedocument.spreadsheetml.sheet')
 
-    @abstractmethod
-    def _extend_login_session(self):
-        pass
+    def get_authentication_required_response(self):
+        return 'Authentication required', 401, {'Content-Type': 'application/json'}
 
-    @abstractmethod
     def get_tm1_service(self):
-        pass
-
-    @login_required
-    def active_user(self):
-        return jsonify({'username': self.get_logged_in_user_name()})
+        tm1_service = self.setting.get_tm1_service(session[self.logged_in_user_session_name])
+        if tm1_service is None:
+            raise AnalogicTM1ServiceException('Unauthorized')
+
+        if tm1_service.connection.is_connected() is False:
+            try:
+                tm1_service.re_authenticate()
+            except Exception as e:
+                self._logger.error('exception while re-authenticating: ' + str(e))
+                raise AnalogicTM1ServiceException('Unauthorized')
 
-    def logout(self):
-        session.clear()
-        return 'ok'
+        return tm1_service
 
-    def getLogger(self):
-        return self._logger
-
-    def on_exit(self):
-        pass
+    def _extend_login_session(self):
+        session.modified = True
```

### Comparing `analogic-framework-4.1.1/analogic/camsecure.py` & `analogic-framework-4.1.2/analogic/camsecure.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,11 +8,12 @@
         super().__init__(setting)
 
     def auth(self):
         resp = make_response(redirect(self.setting.get_base_url()))
 
         cam_name = self.set_tm1_service(request.form.get('c_pp'))
         session[self.logged_in_user_session_name] = cam_name
+        self.load_permissions()
         return self._add_authenticated_cookies(resp)
 
     def get_base_url(self):
         return self.setting.get_proxy_target_url()
```

### Comparing `analogic-framework-4.1.1/analogic/core_endpoints.py` & `analogic-framework-4.1.2/analogic/core_endpoints.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/email.py` & `analogic-framework-4.1.2/analogic/email.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/endpoint.py` & `analogic-framework-4.1.2/analogic/endpoint.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/loader.py` & `analogic-framework-4.1.2/analogic/loader.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/logging.json` & `analogic-framework-4.1.2/analogic/logging.json`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/loginbasic.py` & `analogic-framework-4.1.2/analogic/loginbasic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from analogic.authentication_provider import AuthenticationProvider
 from analogic.analogic_tm1_service import AnalogicTM1Service
+from analogic.exceptions import AnalogicTM1ServiceException
 from flask import render_template, request, make_response, redirect, session, Response
 
 
 class LoginBasic(AuthenticationProvider):
 
     def __init__(self, setting):
         super().__init__(setting)
@@ -44,19 +45,20 @@
                         except Exception as e:
                             self._logger.error('exception while closing session: ' + str(e))
 
                     tm1_service = AnalogicTM1Service(**p)
                     self.setting.set_tm1_service(user_name, tm1_service)
 
                 session[self.logged_in_user_session_name] = user_name
+                self.load_permissions()
                 resp = make_response(redirect(self.setting.get_base_url()))
                 return self._add_authenticated_cookies(resp)
 
             except Exception as e:
-                self._logger.error(e)
+                self._logger.error(e, exc_info=True)
 
         return render_template('login.html', cnf=cnf)
 
     def _create_request_with_authenticated_user(self, url, method, mdx, headers, cookies, decode_content=True):
         user_name = session[self.logged_in_user_session_name]
         tm1_service = self.setting.get_tm1_service(user_name)
         if tm1_service is None:
@@ -75,9 +77,20 @@
     def get_authentication_required_response(self):
         return redirect(self.setting.get_base_url('login'))
 
     def _extend_login_session(self):
         session.modified = True
 
     def get_tm1_service(self):
-        return self.setting.get_tm1_service(session[self.logged_in_user_session_name])
+        tm1_service = self.setting.get_tm1_service(session[self.logged_in_user_session_name])
+        if tm1_service is None:
+            raise AnalogicTM1ServiceException('Unauthorized')
+
+        if tm1_service.connection.is_connected() is False:
+            try:
+                tm1_service.re_authenticate()
+            except Exception as e:
+                self._logger.error('exception while re-authenticating: ' + str(e))
+                raise AnalogicTM1ServiceException('Unauthorized')
+
+        return tm1_service
```

### Comparing `analogic-framework-4.1.1/analogic/nologin.py` & `analogic-framework-4.1.2/analogic/nologin.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/pivot.py` & `analogic-framework-4.1.2/analogic/pivot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 import re
 import io
 import xlsxwriter
+import orjson
 
-from TM1py.Objects import Subset
+from TM1py.Objects import Subset, Hierarchy
 from TM1py.Services import TM1Service
+from TM1py.Utils import format_url
 from flask import jsonify, send_file, current_app
 
 
 def call(tm1:TM1Service, username, cube_name=None, dimension_name=None, hierarchy_name=None, subset_name=None, element_names=None, subset_name_to_remove=None, selected_cards=None, options=None, export_data=None):
     data = {}
 
     username = ''.join(ch for ch in username if ch.isalnum())
@@ -18,56 +20,62 @@
         selected_cards_data = json.loads(selected_cards)
         mdx = create_mdx(options, cube_name, selected_cards_data, username)
         cell_count = tm1.cells.execute_mdx_cellcount(mdx)
         if cell_count < cell_limit:
             data = get_pivot_data(tm1, mdx, selected_cards_data, bool(export_data))
         if export_data:
             return export_to_excel(selected_cards_data, data, json.loads(export_data))
-        return jsonify({'mdx': mdx, 'cell_count': cell_count, 'data': data})
+        return orjson.dumps({'mdx': mdx, 'cell_count': cell_count, 'data': data}), 200, {'Content-Type': 'application/json'}
     elif element_names:
         subset_name = username + '_' + subset_name
         new_subset = Subset(subset_name, dimension_name, hierarchy_name, None, None, element_names)
         tm1.subsets.update_or_create(new_subset, True)
-        hierarchy = tm1.hierarchies.get(dimension_name, hierarchy_name)
-        data['defaultMember'] = hierarchy.default_member
+        hierarchy = get_hierarchy(tm1, dimension_name, hierarchy_name)
+        data['defaultMember'] = hierarchy['DefaultMember']['Name']
         data['aliasAttributeNames'] = get_alias_attribute_names(hierarchy)
         children, data['privateSubsets'] = get_public_and_private_subsets(tm1, dimension_name, hierarchy_name, username, options)
     elif subset_name_to_remove:
         tm1.subsets.delete(username + '_' + subset_name_to_remove, dimension_name, hierarchy_name, True)
-        hierarchy = tm1.hierarchies.get(dimension_name, hierarchy_name)
-        data['defaultMember'] = hierarchy.default_member
+        hierarchy = get_hierarchy(tm1, dimension_name, hierarchy_name)
+        data['defaultMember'] = hierarchy['DefaultMember']['Name']
         data['aliasAttributeNames'] = get_alias_attribute_names(hierarchy)
         children, data['privateSubsets'] = get_public_and_private_subsets(tm1, dimension_name, hierarchy_name, username, options)
     elif 'process' in options:
         p = options['processParams']
         p['pUser'] = username
         p['pValue'] = json.dumps(p['pValue'])
         r = tm1.processes.execute_with_return(options['process'], **p)
-        return jsonify(r)
+        return orjson.dumps(r), 200, {'Content-Type': 'application/json'}
     elif dimension_name is None:
         children = tm1.cubes.get_dimension_names(cube_name)
         data = get_presets_data(tm1, username, options['widgetId'])
     elif hierarchy_name is None:
         children = tm1.hierarchies.get_all_names(dimension_name)
     elif subset_name is None:
-        hierarchy = tm1.hierarchies.get(dimension_name, hierarchy_name)
-        data['defaultMember'] = hierarchy.default_member
+        hierarchy = get_hierarchy(tm1, dimension_name, hierarchy_name)
+        data['defaultMember'] = hierarchy['DefaultMember']['Name']
         data['aliasAttributeNames'] = get_alias_attribute_names(hierarchy)
         children, data['privateSubsets'] = get_public_and_private_subsets(tm1, dimension_name, hierarchy_name, username, options)
     else:
-        current_app.config['JSON_SORT_KEYS'] = False
+        #current_app.config['JSON_SORT_KEYS'] = False
         children = []
         is_private_subset = options['isPrivateSubset']
         if is_private_subset:
             subset_name = username + '_' + subset_name
         subset = tm1.subsets.get(subset_name, dimension_name, hierarchy_name, is_private_subset)
         data['defaultAliasAttributeName'] = subset.alias
         data['children'] = get_elements_with_aliases(tm1, subset, is_private_subset)
+    return orjson.dumps({'children': children, 'data': data}, option=orjson.OPT_NON_STR_KEYS), 200, {'Content-Type': 'application/json'}
 
-    return jsonify({'children': children, 'data': data})
+def get_hierarchy(tm1:TM1Service, dimension_name, hierarchy_name, **kwargs):
+    url = format_url(
+        "/api/v1/Dimensions('{}')/Hierarchies('{}')?$expand=ElementAttributes,Subsets,DefaultMember",
+        dimension_name,
+        hierarchy_name)
+    return tm1._tm1_rest.GET(url, **kwargs).json()
 
 def get_presets_data(tm1, username, widget_id):
     mdx = """WITH
 MEMBER [Measures zSYS Analogic Pivot Presets].[Measures zSYS Analogic Pivot Presets].[sType]
 AS [zSYS Analogic Pivot Presets].[zSYS Analogic Pivot Presets].CurrentMember.Properties('Type')
 MEMBER [Measures zSYS Analogic Pivot Presets].[Measures zSYS Analogic Pivot Presets].[sOwner]
 AS
@@ -127,39 +135,42 @@
     if filter_term:
         filtered_subsets = list(filter(re.compile(filter_term).match, filtered_subsets))
 
     return filtered_subsets
 
 
 def get_elements_with_aliases(tm1:TM1Service, subset:Subset, is_private_subset):
-    d = []
+    hierarchy = get_hierarchy(tm1, subset.dimension_name, subset.hierarchy_name)
+    alias_attribute_names = get_alias_attribute_names(hierarchy)
+    alias_attributes = 'Attributes/' + ',Attributes/'.join(alias_attribute_names)
 
-    element_names = subset.elements
-    hierarchy = tm1.hierarchies.get(subset.dimension_name, subset.hierarchy_name)
+    if subset.is_static:
+        epx_prefix = '[' + subset.dimension_name + '].[' + subset.hierarchy_name + '].['
+        expression = '{'
+        for e in subset.elements:
+            expression += epx_prefix + e + '],'
+        expression = expression[:-1] + '}'
+    else:
+        expression = subset.expression
 
-    if not element_names:
-        element_names = tm1.subsets.get_element_names(subset.dimension_name, hierarchy.name, subset.name, is_private_subset)
+    names_and_aliases = tm1.elements.execute_set_mdx(expression, None, ['Name', alias_attributes], None, None)
 
-    alias_attribute_names = get_alias_attribute_names(hierarchy)
+    d = []
 
-    for element_name in element_names:
-        element = hierarchy.get_element(element_name)
-        aliases = {0: element_name}
-        for alias_attribute_name in alias_attribute_names:
-            aliases[alias_attribute_name] = element.element_attributes[alias_attribute_name]
-        d.append(aliases)
+    for e in names_and_aliases:
+        d.append(e[0]['Attributes'] | {0: e[0]['Name']})
 
     return d
 
 
 def get_alias_attribute_names(hierarchy):
     d = []
-    for attribute in hierarchy.element_attributes:
-        if 'Alias' == attribute.attribute_type:
-            d.append(attribute.name)
+    for attribute in hierarchy['ElementAttributes']:
+        if 'Alias' == attribute['Type']:
+            d.append(attribute['Name'])
     return d
 
 
 def create_mdx(options, cube_name, selected_cards_data, username):
     mdx = 'SELECT ' + ('NON EMPTY ' if options.get('nonEmptyColumns', False) else '')
 
     props = ''
@@ -350,9 +361,9 @@
         i += 1
 
     workbook.close()
     output.seek(0)
     return send_file(output,
                      download_name='pivot_export.xlsx',
                      as_attachment=True,
-                     cache_timeout=0,
+                     max_age=0,
                      mimetype='application/vnd.openxmlformats-officedocument.spreadsheetml.sheet')
```

### Comparing `analogic-framework-4.1.1/analogic/setting.py` & `analogic-framework-4.1.2/analogic/setting.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     def _get_repository(self):
         if self.repository is not None:
             return self.repository
         return self._get_yaml_setting(os.path.join('server', 'configs', 'repository'))
 
     def get_mdx(self, key):
         repository = self._get_repository()
-        mdx = repository[key]
+        mdx = repository.get(key)
         return mdx
 
     def _get_json_setting(self, file_name):
 
         json_url = os.path.join(self.site_root, file_name + '.json')
         with open(json_url, encoding="utf-8") as f:
             setting = json.load(f)
@@ -106,31 +106,31 @@
                 setting['useMinifiedAssets'] = False
 
             if setting.get('ssl_verify') is None:
                 setting['ssl_verify'] = True
 
         return setting
 
-    def save_config_js(self):
+    def save_config_js(self, exclude=[]):
         js_url = os.path.join(self.site_root, 'static', 'assets', 'js', 'config.js')
         with open(js_url, 'w', encoding="utf-8") as f:
-            f.write(render_template('config.html', cnf=self.config))
+            f.write(render_template('config.html', cnf=self.config, exclude=exclude))
 
     def _get_yaml_setting(self, file_path):
         with open(os.path.join(self.site_root, file_path + '.yml'), encoding="utf-8") as file:
             setting = yaml.safe_load(file)
         return setting
 
     def _create_custom_objects(self):
         return self._get_json_setting(os.path.join('server', 'configs', 'custom_objects'))
 
     def get_custom_object_description(self, key):
         if self.custom_objects is None:
             self.custom_objects = self._create_custom_objects()
-        return self.custom_objects[key]
+        return self.custom_objects.get(key)
 
     def set_tm1_service(self, user_name, tm1_service):
         self.tm1_services[user_name] = tm1_service
 
     def get_tm1_service(self, user_name):
         return self.tm1_services.get(user_name)
```

### Comparing `analogic-framework-4.1.1/analogic/static/assets/css/bootstrap-grid.min.css` & `analogic-framework-4.1.2/analogic/static/assets/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/css/bootstrap-grid.min.css.map` & `analogic-framework-4.1.2/analogic/static/assets/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/css/lib/Chart-2.9.3.min.css` & `analogic-framework-4.1.2/analogic/static/assets/css/lib/Chart-2.9.3.min.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/css/lib/nouislider.min.css` & `analogic-framework-4.1.2/analogic/static/assets/css/lib/nouislider.min.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/css/style.css` & `analogic-framework-4.1.2/analogic/static/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/css/widgets/simulation-panel-slider.css` & `analogic-framework-4.1.2/analogic/static/assets/css/widgets/simulation-panel-slider.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/images/loading.gif` & `analogic-framework-4.1.2/analogic/static/assets/images/loading.gif`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/images/loading2.gif` & `analogic-framework-4.1.2/analogic/static/assets/images/loading2.gif`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/images/loading2_transparent.gif` & `analogic-framework-4.1.2/analogic/static/assets/images/loading2_transparent.gif`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/images/triangle.png` & `analogic-framework-4.1.2/analogic/static/assets/images/triangle.png`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/api.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/api.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -689,8 +689,16 @@
 
         if (arg.length > 2) {
             for (let i = 2; i < arg.length; ++i) {
                 Api.forceRefresh(arg[i]);
             }
         }
     }
+};
+
+Api.logout = function logout() {
+    return Auth.logout();
+};
+
+Api.goToStartPage = function goToStartPage() {
+    Auth.goToStartPage();
 };
```

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/app.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/app.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/authentication.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/authentication.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -7,14 +7,26 @@
     return $.ajax({
         url: app.assetsUrl + '/js/widgets/default/' + arg + '.json',
         dataType: 'json',
         cache: false
     });
 };
 
+Auth.logout = () => {
+    return $.ajax({
+        url: 'logout',
+        method: 'GET'
+    });
+};
+
+Auth.goToStartPage = () => {
+    window.onbeforeunload = null;
+    Api.goToUrl('');
+};
+
 Auth.getAjaxRequest = (url, data, type, widgetId = '', resent = false, eventMapId = '') => {
     let urlWithWidgetId = url + (url.includes('?') ? '&' : '?') + 'widgetid=' + widgetId;
     return $.ajax({
         cache: true,
         type: type,
         url: urlWithWidgetId,
         headers: Auth.getHeader(),
```

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/array.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/load-executor/array.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/base.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/load-executor/base.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/load-executor/factory.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/load-executor/factory.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/base.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/parsing-control/base.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/factory.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/parsing-control/factory.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/parsing-control/matrix.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/parsing-control/matrix.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/pivot.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/pivot.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/query-builder.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/query-builder.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/server.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/server.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/utils.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/utils.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -611,11 +611,14 @@
         return value.includes('CAMID') ? value : value.replace(/\\/g, '/');
     },
     checkScreenResolution() {
         if (!app.checkScreenResolutionWarningDisplayed && $('body').width() - 100 > window.innerWidth) {
             Api.showPopup('Your current screen resolution is below the recommended 1920*1080. For optimal user experience please lower your browser zoom to 90% or 80%.');
             app.checkScreenResolutionWarningDisplayed = true;
         }
+    },
+    undefinedOrFalse(val) {
+        return typeof val === 'undefined' || val === false;
     }
 };
 
 app.utils = Utils;
```

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/base.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/write-executor/base.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/factory.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/write-executor/factory.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/function.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/write-executor/function.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/framework/write-executor/grid-table.js` & `analogic-framework-4.1.2/analogic/static/assets/js/framework/write-executor/grid-table.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/lib/Chart-2.9.3.min.js` & `analogic-framework-4.1.2/analogic/static/assets/js/lib/Chart-2.9.3.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/lib/Sortable.min.js` & `analogic-framework-4.1.2/analogic/static/assets/js/lib/Sortable.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js` & `analogic-framework-4.1.2/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js` & `analogic-framework-4.1.2/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js` & `analogic-framework-4.1.2/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js` & `analogic-framework-4.1.2/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery.actual.min.js` & `analogic-framework-4.1.2/analogic/static/assets/js/lib/jquery/jquery.actual.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery.cookie.js` & `analogic-framework-4.1.2/analogic/static/assets/js/lib/jquery/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/jquery.doubletap.js` & `analogic-framework-4.1.2/analogic/static/assets/js/lib/jquery/jquery.doubletap.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/lib/jquery/tableSort.js` & `analogic-framework-4.1.2/analogic/static/assets/js/lib/jquery/tableSort.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/lib/nouislider.min.js` & `analogic-framework-4.1.2/analogic/static/assets/js/lib/nouislider.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/base/widget.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/base/widget.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -765,8 +765,12 @@
     static setOrRemoveStyle(element, styleName, value) {
         value ? element.css(styleName, value) : Widget.removeStyle(element, styleName);
     }
 
     static setOrRemoveMeasure(element, measureName, value) {
         Widget.setOrRemoveStyle(element, measureName, value ? Widget.getPercentOrPixel(value) : false);
     }
+
+    static addOrRemoveClass(element, className, add) {
+        add ? !element.hasClass(className) && element.addClass(className) : element.removeClass(className);
+    }
 }
```

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/button.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/button.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/combo-chart.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/combo-chart.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -194,15 +194,19 @@
 
         this.value = v;
         return v;
     }
 
     updateHtml(data) {
         this.getParameters(data);
-        this.initEventHandlers();
+        let c = ComboChartWidget.getChartConfig(this.value);
+        this.chart.data = c.data;
+        this.chart.options = c.options;
+
+        this.chart.update();
     }
 
     initEventHandlers() {
         const canvas = $('#' + this.options.id + 'Canvas'),
             ctx = canvas[0].getContext('2d'),
             c = new Chart(ctx, ComboChartWidget.getChartConfig(this.value));
 
@@ -210,14 +214,15 @@
             let legend = $(e.target).closest('.ks-legend-item'),
                 id = legend.toggleClass('off').data('id');
 
             c.getDatasetMeta(id).hidden = !c.getDatasetMeta(id).hidden;
 
             c.update();
         });
+        this.chart = c;
     }
 
     static getChartConfig(v) {
         let data = v.data;
 
         for (let f = 0; f < v.datasets.length; ++f) {
             if (v.datasets[f].data) {
```

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/container.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/container.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/datepicker.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/datepicker.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -12,21 +12,24 @@
             monthPicker = this.getRealValue('monthPicker', d, false);
 
         const v = {
             allowEmptyDate: this.getRealValue('allowEmptyDate', d, false),
             closeAfterSelectingTheDate: this.getRealValue('closeAfterSelectingTheDate', d, false),
             datePicked: this.getRealValue('datePicked', d, DatePickerWidget.getStandardizedDateString(new Date(), monthPicker)),
             editable: this.getRealValue('editable', d, true),
+            fullYearButtonText: this.getRealValue('fullYearButtonText', d, 'Full year'),
+            fullYearButtonVisible: this.getRealValue('fullYearButtonVisible', d, false),
             local: this.getRealValue('local', d, false),
-            skin: this.getRealValue('skin', d, 'standard'),
             maxDate: this.getRealValue('maxDate', d, false),
             minDate: this.getRealValue('minDate', d, false),
+            monthLocale: this.getRealValue('monthLocale', d, 'en-US'), //[] - browser default
             monthPicker: monthPicker,
             ordinal: this.getRealValue('ordinal', d, ''),
             panelFixed: this.getRealValue('panelFixed', d, false),
+            skin: this.getRealValue('skin', d, 'standard'),
             title: this.getRealValue('title', d, ''),
             titleVisible: this.getRealValue('titleVisible', d, true)
         };
 
         let date = DatePickerWidget.getDateFromString(v.datePicked, v.monthPicker),
             dateText = DatePickerWidget.getFormattedDateString(date, v.monthPicker, v.local),
             minDate = v.minDate ? DatePickerWidget.getDateFromString(v.minDate, v.monthPicker) : '',
@@ -38,29 +41,33 @@
 
         this.value = v.datePicked;
         this.minDate = minDate;
         this.maxDate = maxDate;
         this.panelFixed = v.panelFixed;
         this.local = v.local;
         this.closeAfterSelectingTheDate = v.closeAfterSelectingTheDate;
+        this.isMonthPicker = v.monthPicker;
+        this.fullYearButtonVisible = v.fullYearButtonVisible;
 
 
         const months = ['JAN', 'FEB', 'MAR', 'APR', 'MAY', 'JUN', 'JUL', 'AUG', 'SEP', 'OCT', 'NOV', 'DEC'];
 
         let monthsHtml = months.map((month, i) => {
             let ym = new Date(date.getFullYear(), i),
                 disabled = '',
                 min = new Date(minDate),
                 max = new Date(maxDate);
 
             if ((ym < min.setMonth(min.getMonth() - 1)) || (ym > max)) {
                 disabled = 'disabled';
             }
 
-            return '<div data-month=' + i + ' class="' + disabled + ' ks-datepicker-panel-month-item ' + ((i === date.getMonth()) ? 'on' : '') + '">' + month + '</div>';
+            return '<div data-month=' + i + ' class="' + disabled + ' ks-datepicker-panel-month-item ' + ((i === date.getMonth()) ? 'on' : '') + '">' + ym.toLocaleString(v.monthLocale, {
+                month: 'short'
+            }).substring(0, 3) + '</div>';
         });
 
         const html = `
 <div class="ks-datepicker dropdown-type ks-datepicker-${v.skin}" style="${mainDivStyle.join('')}" data-ordinal="${v.ordinal}" data-monthpicker="${v.monthPicker || false}" data-min-date="${v.minDate || ''}" data-max-date="${v.maxDate || ''}">
     <div class="ks-datepicker-inner" style="${innerStyle.join('')}">
         <div class="ks-datepicker-title"  style="${titleStyles.join('')}">
             ${v.titleVisible ? v.title : ''}
@@ -69,24 +76,25 @@
             <div class="ks-datepicker-field-inner">
                 <div class="ks-datepicker-icon icon-date"></div>
                 <input type="text" class="ks-datepicker-input" placeholder="Choose..." value="${dateText}" ${v.editable ? '' : `disabled`}>
             </div>
         </div>
     </div>
     ${v.editable ?
-            `<div class="ks-datepicker-panel holder" ${v.panelFixed ? '' : 'style="display:none;'}">
+            `<div class="ks-datepicker-panel holder" ${v.panelFixed ? '' : 'style="display:none;"'}>
         <div class="ks-datepicker-panel-header">
             <div class="ks-datepicker-panel-header-inner">
                 <div class="ks-datepicker-panel-pager ks-left"></div>
                 <div class="ks-datepicker-panel-year" data-year="${date.getFullYear()}">${date.getFullYear()}</div>
                 <div class="ks-datepicker-panel-pager ks-right"></div>
             </div>
         </div>
-        <div class="ks-datepicker-panel-months">${monthsHtml.join('')}</div>
-        <div class="ks-datepicker-panel-days">${DatePickerWidget.getPickerHolderDaysHtml(date, minDate, maxDate)}</div>
+        <div class="ks-datepicker-full-year-button" ${v.fullYearButtonVisible ? '' : 'style="display:none;"'}>${v.fullYearButtonText}</div>
+        <div class="ks-datepicker-panel-months" >${monthsHtml.join('')}</div>
+        <div class="ks-datepicker-panel-days" ${v.monthPicker ? 'style="display:none;"' : ''}>${v.monthPicker ? '' : DatePickerWidget.getPickerHolderDaysHtml(date, minDate, maxDate)}</div>
     </div>` : ''}
 </div>`;
 
         return html;
     }
 
     static getPickerHolderDaysHtml(date, minDate, maxDate) {
@@ -116,14 +124,15 @@
             dateInput = $('#' + id + ' .ks-datepicker-input'),
             _this = this;
 
         let date = DatePickerWidget.getDateFromString(_this.value, datePicker.data('monthpicker')),
             yearHolder = $('#' + id + ' .ks-datepicker-panel-year'),
             monthHolders = $('#' + id + ' .ks-datepicker-panel-month-item'),
             dayHolders = $('#' + id + ' .ks-datepicker-panel-day-item'),
+            yearButton = $('#' + id + ' .ks-datepicker-full-year-button'),
             target;
 
         datePicker.on('click touch', e => {
             Doc.find(".dropdown-type .holder").not(datePicker).each((i, el) => {
                 if ($(el).is(':visible')) {
                     DatePickerWidget.triggerPickEvent($(el).closest('section').attr('id'), $(el), e);
                 }
@@ -139,15 +148,15 @@
                     }));
                 } else {
                     pickerHolder.slideDown(50);
                 }
             }
 
             return false;
-        }).on('dateChange.' + id, (_, date) => {
+        }).on('dateChange.' + id, (_, date, source) => {
             let m = datePicker.data('monthpicker'),
                 minDateStr = String(datePicker.data('min-date')),
                 maxDateStr = String(datePicker.data('max-date')),
                 minDate = minDateStr ? DatePickerWidget.getDateFromString(minDateStr, m) : '',
                 maxDate = maxDateStr ? DatePickerWidget.getDateFromString(maxDateStr, m) : '';
 
             if (minDateStr && DatePickerWidget.isValidDateString(minDateStr, m)) {
@@ -160,14 +169,16 @@
             if (maxDateStr && DatePickerWidget.isValidDateString(maxDateStr, m)) {
                 if (date > maxDate) {
                     date = maxDate;
                     dateInput.val(DatePickerWidget.getFormattedDateString(date, m, _this.local));
                 }
             }
 
+            _this.fullYearButtonVisible && yearButton.removeClass('on');
+
             _this.value = DatePickerWidget.getStandardizedDateString(date, m);
 
             $('#' + id + ' .ks-datepicker-panel-days').empty().append(DatePickerWidget.getPickerHolderDaysHtml(date, minDate, maxDate));
             yearHolder.data('year', date.getFullYear()).text(date.getFullYear());
             monthHolders.removeClass('on').filter(`[data-month='${date.getMonth()}']`).addClass('on');
             dayHolders.removeClass('on').filter(`[data-day='${date.getDate()}']`).addClass('on');
 
@@ -179,72 +190,109 @@
                     target.toggleClass('disabled', ym < min.setMonth(min.getMonth() - 1));
                 }
                 if (maxDate) {
                     target.toggleClass('disabled', ym > maxDate);
                 }
             });
 
-            if (_this.panelFixed || _this.closeAfterSelectingTheDate) {
-                DatePickerWidget.triggerPickEvent(id, pickerHolder, {});
-                if (_this.closeAfterSelectingTheDate) {
+            if (_this.closeAfterSelectingTheDate) {
+                const triggerEvent = _this.isMonthPicker && source === 'month' ? true : !_this.isMonthPicker && source === 'day';
+                if (triggerEvent) {
+                    DatePickerWidget.triggerPickEvent(id, pickerHolder, {});
                     pickerHolder.slideUp(50);
                 }
             }
+
+            if (_this.panelFixed) {
+                DatePickerWidget.triggerPickEvent(id, pickerHolder, {});
+            }
         });
 
+        let source = '';
+
         const pickerHolder = $('#' + id + ' .ks-datepicker-panel').on('click touch', '.ks-datepicker-panel-pager', e => {
             let mod = $(e.currentTarget).hasClass('ks-left') ? -1 : 1;
-            date = DatePickerWidget.getDateFromString(_this.value, datePicker.data('monthpicker'));
-            date.setYear(Number(date.getFullYear()) + mod);
+            if (_this.fullYearButtonVisible && yearButton.hasClass('on')) {
+                e.stopPropagation();
+                let year = Number(yearHolder.data('year')) + mod;
+                yearHolder.data('year', year + '').text(year);
+                handleYearButtonClick();
+            } else {
+                date = DatePickerWidget.getDateFromString(_this.value, datePicker.data('monthpicker'));
+                date.setYear(Number(date.getFullYear()) + mod);
+                source = 'pager';
+            }
         }).on('click touch', '.ks-datepicker-panel-month-item', e => {
             target = $(e.currentTarget);
             date = DatePickerWidget.getDateFromString(_this.value, datePicker.data('monthpicker'));
             date.setMonth(target.data('month'));
+            source = 'month';
         }).on('click touch', '.ks-datepicker-panel-day-item[data-enabled="true"]', e => {
             target = $(e.currentTarget);
             date = DatePickerWidget.getDateFromString(_this.value, datePicker.data('monthpicker'));
             date.setDate(target.data('day'));
+            source = 'day';
+        }).on('click touch', '.ks-datepicker-full-year-button', e => {
+            e.stopPropagation();
+            handleYearButtonClick();
+
         }).on('click touch', e => {
             e.stopPropagation();
             $('#' + id + ' .ks-datepicker-input').val(DatePickerWidget.getFormattedDateString(date, datePicker.data('monthpicker'), Widgets[id].local));
-            datePicker.trigger('dateChange.' + id, [date]);
+            datePicker.trigger('dateChange.' + id, [date, source]);
         });
 
         dateInput.on('input', e => {
             let date = DatePickerWidget.getDateFromString($(e.currentTarget).val(), $(e.currentTarget).data('monthpicker'));
             if (!date) {
                 return false;
             }
+            source = 'input';
 
-            datePicker.trigger('dateChange.' + id, [date]);
+            datePicker.trigger('dateChange.' + id, [date, source]);
         }).on('focusout', e => {
             let date = DatePickerWidget.getDateFromString($(e.currentTarget).val(), $(e.currentTarget).data('monthpicker'));
             $('#' + id + ' .ks-datepicker-input').val(DatePickerWidget.getFormattedDateString(date, datePicker.data('monthpicker'), _this.local));
         }).on('keypress', e => {
             if (e.which === 13) {
                 $(e.currentTarget).blur();
-                let element = $('<div>');
+                let element = $('<div>'),
+                    value = $('#' + id + ' .ks-datepicker-input').val();
                 element.data({
                     action: 'pick',
                     id: id,
-                    value: $('#' + id + ' .ks-datepicker-input').val().slice(0, -1),
+                    value: value.length !== 4 ? value.slice(0, -1) : value,
                     ordinal: $('#' + id + ' .ks-datepicker').data('ordinal')
                 });
                 Widget.doHandleSystemEvent(element, e, true);
             }
         });
 
+        const handleYearButtonClick = () => {
+            let year = yearHolder.data('year');
+            $('#' + id + ' .ks-datepicker-input').val(year);
+            _this.value = year;
+            monthHolders.removeClass('on');
+            dayHolders.removeClass('on');
+            yearButton.addClass('on');
+            if (_this.closeAfterSelectingTheDate) {
+                DatePickerWidget.triggerPickEvent(id, pickerHolder, {});
+                pickerHolder.slideUp(50);
+            }
+        };
+
         const catcher = Doc.not(datePicker).on('click touch', e => {
             if (pickerHolder.is(':visible') && !_this.panelFixed) {
                 if (!_this.closeAfterSelectingTheDate) {
-                    let element = $('<div>');
+                    let element = $('<div>'),
+                        value = $('#' + id + ' .ks-datepicker-input').val();
                     element.data({
                         action: 'pick',
                         id: id,
-                        value: $('#' + id + ' .ks-datepicker-input').val().slice(0, -1),
+                        value: value.length !== 4 ? value.slice(0, -1) : value,
                         ordinal: $('#' + id + ' .ks-datepicker').data('ordinal')
                     });
                     Widget.doHandleSystemEvent(element, e, true);
                 }
                 pickerHolder.slideUp(50);
             }
         });
@@ -256,22 +304,24 @@
 
     reset() {
         delete this.value;
         delete this.minDate;
         delete this.maxDate;
         delete this.panelFixed;
         delete this.local;
+        delete this.fullYearButtonVisible;
     }
 
     static triggerPickEvent(id, pickerHolder, e) {
-        let element = $('<div>');
+        let element = $('<div>'),
+            value = $('#' + id + ' .ks-datepicker-input').val();
         element.data({
             action: 'pick',
             id: id,
-            value: $('#' + id + ' .ks-datepicker-input').val().slice(0, -1),
+            value: value.length !== 4 ? value.slice(0, -1) : value,
             ordinal: $('#' + id + ' .ks-datepicker').data('ordinal')
         });
         Widget.doHandleSystemEvent(element, e, true);
         if (!Widgets[id].panelFixed) {
             pickerHolder.slideUp(50);
         }
     }
```

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/default/ScrollTableWidget.json` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/default/ScrollTableWidget.json`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/dropbox.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/dropbox.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -36,15 +36,15 @@
     <div class="ks-dropbox-inner">
         <div class="ks-dropbox-title" style="${titleStyles.join('')}">
             <span class="ks-dropbox-title-primary">${v.titleVisible ? v.title : ''}</span>
             <span class="ks-dropbox-title-secondary"></span>
         </div>
         <div class="ks-dropbox-field ${v.editable === false ? 'readonly' : ''}">
             <div class="ks-dropbox-field-inner">
-                <input ${v.editable === false ? 'readonly' : ''} style="${textStyles.join('')}" type="text" class="ks-dropbox-input search-text" placeholder="${pi.selectedItems !== '' ? pi.selectedItems : v.placeHolder}">
+                <input ${v.editable === false || v.disableSearch === true  ? 'readonly' : ''} style="${textStyles.join('')}" type="text" class="ks-dropbox-input search-text" placeholder="${pi.selectedItems !== '' ? pi.selectedItems : v.placeHolder}">
                 <div class="ks-dropbox-icon"></div>
             </div>
         </div>
     </div>
     <div class="ks-dropbox-panel" style="${panelStyles.join('')}">
         ${v.backdrop ? '<div class="ks-dropbox-backdrop"><\/div>' : ''}
         <div class="ks-dropbox-panel-inner">${this.getItems(pi.data, v)}</div>
@@ -114,14 +114,15 @@
 </div>`;
         }).join('');
     }
 
     getParameters(d) {
         return {
             backdrop: this.getRealValue('backdrop', d, false),
+            disableSearch: this.getRealValue('disableSearch', d, false),
             editable: this.getRealValue('editable', d, true),
             itemIconOff: this.getRealValue('itemIconOff', d, false),
             itemIconOn: this.getRealValue('itemIconOn', d, false),
             hideIfNoData: this.getRealValue('hideIfNoData', d, false),
             panelWidth: this.getRealValue('panelWidth', d, false),
             placeHolder: this.getRealValue('placeHolder', d, ''),
             selectFirst: this.getRealValue('selectFirst', d, false),
@@ -144,15 +145,17 @@
             section = this.getSection(),
             inner = section.find('.ks-dropbox-panel-inner'),
             input = section.find('.ks-dropbox-input');
         if (this.state.serverSideFilter) {
             let previouslySelected = this.items.filter(e => e.on === true),
                 previouslySelectedName = previouslySelected.map(e => e.name);
             this.items = previouslySelected.concat(data.items.filter(e => !previouslySelectedName.includes(e.name)));
-            inner.html(this.getItems(data, p));
+            inner.html(this.getItems({
+                items: this.items
+            }, p));
         } else {
             const pi = this.processItems(data, this.options, p);
             inner.html(this.getItems(pi.data, p));
             input.attr('placeholder', pi.selectedItems !== '' ? pi.selectedItems : p.placeHolder);
         }
     }
 
@@ -174,14 +177,19 @@
         const dropbox = $('#' + id + ' .ks-dropbox-field-inner').on('click', (e) => {
             Doc.find(".ks-dropbox .ks-dropbox-panel").not(dropbox).each((i, el) => $(el).is(':visible') ? $(el).slideUp(50) : false);
 
             itemHolder.is(':visible') ? itemHolder.slideUp(50) : itemHolder.slideDown(50, function() {
                 // $(e.currentTarget).parent().get(0).scrollIntoView({behavior: "smooth", block: "start"});
             });
 
+            if (state.serverSideFilter) {
+                const previousFilterValue = v(id + '.filter.value');
+                section.find('input[type="text"]').val(previousFilterValue !== false ? previousFilterValue : '');
+            }
+
             return false;
         });
 
         section.find('input[type="text"]').on('input', i => {
             let e = $(i.currentTarget),
                 term = e.val(),
                 f;
@@ -211,14 +219,17 @@
         const itemHolder = $('#' + id + ' .ks-dropbox-panel'). /*on('click', false).*/ on('click', '.ks-dropbox-panel-item ', e => {
             const clickedItem = $(e.currentTarget);
             DropBoxWidget.handleClick(state, w, e, itemHolder, section, id, clickedItem, $(e.target).hasClass('ks-dropbox-panel-item-checkbox'), amIOnGridtable);
         });
 
         const catcher = Doc.not(dropbox).on('touch click', e => {
             itemHolder.is(':visible') ? itemHolder.slideUp(50) : false;
+            if (itemHolder.is(':visible') && state.serverSideFilter) {
+                section.find('input[type="text"]').val('');
+            }
         });
 
         itemHolder.hide();
     }
 
     reset() {
         delete this.value;
```

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/gauge.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/gauge.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid/grid-cell.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid/grid-cell.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid/grid-row.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid/grid-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid/grid.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid/grid.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -61,30 +61,37 @@
             childrenData['originalId'] = widgetOptions['id'];
             Widgets[childrenData['id']].updateHtml(childrenData);
         }
         this.updateHtml(childrenData);
     }
 
     updateHtml(data) {
+        delete data['skin'];
         const o = this.options,
             p = this.getParameters(data),
-            mainDiv = $('#' + p.cellId);
+            mainDiv = $('#' + p.cellId),
+            content = mainDiv.find('.ks-grid-table-cell-content');
         p.cellVisible === false ? mainDiv.css('display', 'none') : mainDiv.css('display', 'block');
         p.cellWidth && mainDiv.css('width', Widget.getPercentOrPixel(p.cellWidth));
         let paddingRight, paddingLeft;
 
         Widget.setOrRemoveStyle(mainDiv, 'background-color', p.cellBackgroundColor);
 
         paddingRight = p.cellPaddingRight !== false ? p.cellPaddingRight : o.paddingRight ? o.paddingRight : false;
         Widget.setOrRemoveMeasure(mainDiv, 'padding-right', paddingRight);
 
         paddingLeft = p.cellPaddingLeft !== false ? p.cellPaddingLeft : o.paddingLeft ? o.paddingLeft : false;
         Widget.setOrRemoveMeasure(mainDiv, 'padding-left', paddingLeft);
 
         Widget.setSkin(mainDiv, 'ks-grid-table-cell-', p.cellSkin ? p.cellSkin : p.skin);
+
+        Widget.addOrRemoveClass(mainDiv, 'border-right', p.borderRight);
+        Widget.addOrRemoveClass(mainDiv, 'border-left', p.borderLeft);
+
+        Widget.addOrRemoveClass(content, 'ks-pos-' + p.alignment, true);
     }
 
     render(withState, childrenData) {
         this.isRendering = true;
         const o = {
                 ...this.options,
                 ...childrenData
```

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/grid-table/grid-table.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/grid-table/grid-table.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -60,15 +60,15 @@
                     hw = w.title.split('|').map(e => '<div>' + e + '</div>').join('');
                 }
                 c.push(this.buildTableHeaderCellHtml(hw, w.width, w.borderLeft, w.borderRight, w.headerAlignment ? w.headerAlignment : w.alignment));
             }
 
             th = this.buildTableHeadHtml(this.buildTableHeaderRowHtml(c.join(''), v.rowHeight, v.borderTop, v.borderBottom));
         }
-        return this.getWidgetHtml(this.buildTableHtml([th, tb].join(''), v.skin), o.title, mainDivStyle);
+        return this.getWidgetHtml(this.buildTableHtml([th, tb].join(''), v.skin), o.title || '', mainDivStyle);
     }
 
     getParameters(data) {
         return {
             allowFullContentUpdated: this.getRealValue('allowFullContentUpdated', data, false),
             allowChangedDataUpdate: this.getRealValue('allowChangedDataUpdate', data, true),
             borderBottom: this.getRealValue('borderBottom', data, true),
```

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/histogram-combo-chart.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/histogram-combo-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontal-bar-chart.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/horizontal-bar-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontal-table.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/horizontal-table.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/image.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/image.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/line-area-chart.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/line-area-chart.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -2,32 +2,64 @@
 
 'use strict';
 
 class LineAreaChartWidget extends Widget {
 
     getHtml(verticalLineBoxWidget, d) {
         const o = this.options,
+            v = this.getParameters(d);
+
+        return `
+<div class="ks-line-area-chart ks-line-area-chart-${v.skin}" style="${this.getGeneralStyles(v.data, {width: 450, height: 450}).join('')}">
+    ${verticalLineBoxWidget.join('')}
+    <div class="ks-line-area-chart-widget">
+        <canvas id="${o.id}Canvas"></canvas>
+    </div>
+    <div class="ks-legend ks-legend-${v.legendSkin}"></div>
+</div>`;
+    }
+
+    updateHtml(data) {
+        this.getParameters(data);
+
+        let c = this.getChartConfig();
+
+        this.chart.data = c.data;
+        this.chart.options = c.options;
+
+        this.chart.update();
+    }
+
+    getParameters(d) {
+        const o = this.options,
             f = this.getRealValue('defaultFontFamily', d, 'imago, sans-serif'),
             c = '#A6A7A7',
             b = '#000',
             e = 'bold';
 
-        const defaultDatasets = [{
+        const demoDatasets = [{
             borderColor: 'black',
+            labelBorderColor: '#000000',
+            labelBackgroundColor: '#FFFFFF',
+            labelColor: 'blue',
+            labelBorderWidth: 2,
             borderWidth: 3,
             backgroundColor: 'rgba(255, 10, 13, 0.4)',
-            fill: true,
-            lineTension: 0.5
+            fill: false,
+            legendLabel: 'Legend1',
+            labelVisible: true,
+            borderDash: [5, 5]
         }, {
             legendLabel: 'Legend2',
             borderWidth: 2,
             borderColor: 'red',
             backgroundColor: 'rgba(10, 255, 13, 0.4)',
             fill: true,
-            lineTension: 0.5
+            lineTension: 0.5,
+            labelVisible: true
         }, {
             legendLabel: 'Legend3',
             borderColor: 'blue',
             backgroundColor: 'blue',
             fill: true,
             lineTension: 0.5
         }, {
@@ -40,15 +72,15 @@
             legendLabel: 'Legend5',
             borderColor: 'orange',
             backgroundColor: 'orange',
             fill: true,
             lineTension: 0.5
         }];
 
-        const defaultData = [
+        const demoData = [
             [{
                 label: '2019'
             }, {
                 label: '2020'
             }, {
                 label: '2021'
             }, {
@@ -137,17 +169,17 @@
                     value: 78
                 }, {
                     value: 80
                 }]
             ]
         ];
 
-        const data = $.extend(true, [], o.data || [], d.data.length ? d.data : defaultData);
+        const data = $.extend(true, [], o.data || [], d.data.length ? d.data : demoData);
 
-        const datasets = !o.datasets && !d.datasets ? defaultDatasets : $.extend(true, [], o.datasets || [], d.datasets || []);
+        const datasets = !o.datasets && !d.datasets ? demoDatasets : $.extend(true, [], o.datasets || [], d.datasets || []);
 
         const v = {
             data: data,
             datasets: datasets,
             legendSkin: this.getRealValue('legendSkin', d, 'standard'),
             skin: this.getRealValue('skin', d, 'standard'),
             xAxisLabel: this.getRealValue('xAxisLabel', d),
@@ -179,38 +211,43 @@
             xAxesLabelDisplay: this.getRealValue('xAxesLabelDisplay', d, true),
             xAxesLabelFontSize: this.getRealValue('xAxesLabelFontSize', d, 14),
             xAxesLabelFontFamily: this.getRealValue('xAxesLabelFontFamily', d, f),
             xAxesLabelFontColor: this.getRealValue('xAxesLabelFontColor', d, b),
             xAxesLabelFontStyle: this.getRealValue('xAxesLabelFontStyle', d, e),
             xAxesLabelPadding: this.getRealValue('xAxesLabelPadding', d, 0),
             xAxesLabelRotation: this.getRealValue('xAxesLabelRotation', d, 0),
+            xMin: this.getRealValue('xMin', d, false),
+            xMax: this.getRealValue('xMax', d, false),
+            xAxesOffset: this.getRealValue('xAxesOffset', d, 0),
+            xAxesOffsetRight: this.getRealValue('xAxesOffsetRight', d, 0),
+            xAxesOffsetLeft: this.getRealValue('xAxesOffsetLeft', d, 0),
             yAxesLabelDisplay: this.getRealValue('yAxesLabelDisplay', d, true),
             yAxesLabelFontSize: this.getRealValue('yAxesLabelFontSize', d, 14),
             yAxesLabelFontFamily: this.getRealValue('yAxesLabelFontFamily', d, f),
             yAxesLabelFontColor: this.getRealValue('yAxesLabelFontColor', d, b),
             yAxesLabelFontStyle: this.getRealValue('yAxesLabelFontStyle', d, e),
             yAxesLabelPadding: this.getRealValue('yAxesLabelPadding', d, 0),
             yAxesLabelRotation: this.getRealValue('yAxesLabelRotation', d, 0),
+            yAxesStacked: this.getRealValue('yAxesStacked', d, false),
+            yAxesUnit: this.getRealValue('yAxesUnit', d, ''),
+            yAxesDecimalNum: parseInt(this.getRealValue('yAxesDecimalNum', d, 2)),
+            yAxesSeparatesThousands: this.getRealValue('yAxesSeparatesThousands', d, false),
+            yAxesTicksPrecisionFixed: this.getRealValue('yAxesTicksPrecisionFixed', d, false),
+
             tooltipsEnabled: this.getRealValue('tooltipsEnabled', d, true),
             tooltipsMode: this.getRealValue('tooltipsMode', d, 'index'),
             tooltipsIntersect: this.getRealValue('tooltipsIntersect', d, false),
             aspectRatio: this.getRealValue('aspectRatio', d, null),
-            maintainAspectRatio: this.getRealValue('maintainAspectRatio', d, true)
+            maintainAspectRatio: this.getRealValue('maintainAspectRatio', d, true),
+            defaultBezierCurveTension: this.getRealValue('defaultBezierCurveTension', d, 0)
         };
 
         this.value = v;
 
-        return `
-<div class="ks-line-area-chart ks-line-area-chart-${v.skin}" style="${this.getGeneralStyles(v.data, {width: 450, height: 450}).join('')}">
-    ${verticalLineBoxWidget.join('')}
-    <div class="ks-line-area-chart-widget">
-        <canvas id="${o.id}Canvas"></canvas>
-    </div>
-    <div class="ks-legend ks-legend-${v.legendSkin}"></div>
-</div>`;
+        return v;
     }
 
     initEventHandlers() {
         const o = this.options,
             a = $('#' + o.id + 'Canvas');
 
         const c = new Chart(a[0].getContext('2d'), this.getChartConfig(this.value));
@@ -225,60 +262,69 @@
         });
 
         this.chart = c;
         this.canvas = a;
 
         if (o.widgets) {
             this.verticalLineBox = this.getSection().find('.ks-vertical-line-box');
-            app.q = this.verticalLineBox;
             this.verticalLines = this.verticalLineBox.children('.ks-vertical-line');
 
             this.adjustVerticalLineBox();
         }
     }
 
     getChartConfig(v) {
         let datasets = v.datasets,
             d = v.data[v.data.length - 1],
-            j, i, e;
-
-        for (i = 0; i < d.length; ++i) {
-            for (j = 0; j < datasets.length; ++j) {
-                e = datasets[j];
-
-                if (!datasets[j].data) {
-                    datasets[j].data = [];
-                }
+            j, i, xValues = v.data[0].map(e => e.label),
+            data, len = d.length;
 
-                datasets[j].data.push(Utils.parseNumber(d[i][j].value || '0'));
+        const yAxesUnit = v.yAxesUnit,
+            yAxesDecimalNum = v.yAxesDecimalNum,
+            yAxesSeparatesThousands = v.yAxesSeparatesThousands,
+            yAxesTicksPrecisionFixed = v.yAxesTicksPrecisionFixed;
+
+        for (i = 0; i < datasets.length; ++i) {
+            data = [];
+
+            for (j = 0; j < len; ++j) {
+                data.push({
+                    x: parseInt(xValues[j]),
+                    y: Utils.parseNumber(d[j][i].value || '0')
+                });
             }
+
+            datasets[i].data = data;
         }
 
         return {
             type: 'line',
             data: {
-                labels: v.data[0].map(item => item.label),
+                labels: xValues,
                 datasets: datasets
             },
             options: {
                 scales: {
                     xAxes: [{
+                        type: 'linear',
                         offset: false,
                         display: v.xAxesDisplay,
                         gridLines: {
                             display: v.xAxesGridLinesDisplay,
                             drawTicks: v.xAxesTicksDisplay,
                             drawOnChartArea: v.xAxesGridLinesDisplay,
                             drawBorder: v.yAxesGridLinesDrawBorder,
                             color: v.xAxesGridLinesColor,
                             zeroLineColor: v.xAxesGridLinesColor,
                             offsetGridLines: false
                         },
                         ticks: {
                             display: v.xAxesTicksLabelDisplay,
+                            min: parseFloat($.isNumeric(v.xMin) ? v.xMin : xValues[0]) - (v.xAxesOffsetLeft || v.xAxesOffset),
+                            max: parseFloat($.isNumeric(v.xMax) ? v.xMax : xValues.slice(-1)) + (v.xAxesOffsetRight || v.xAxesOffset),
                             fontSize: v.xAxesTicksFontSize,
                             fontFamily: v.xAxesTicksFontFamily,
                             fontStyle: v.xAxesTicksFontStyle,
                             fontColor: v.xAxesTicksFontColor,
                             autoSkip: true,
                             minRotation: v.xAxesLabelRotation,
                             maxRotation: v.xAxesLabelRotation,
@@ -304,14 +350,15 @@
                             color: v.xAxesGridLinesColor,
                             lineWidth: 1.5,
                             drawOnChartArea: false,
                             drawTicks: false
                         }
                     }],
                     yAxes: [{
+                        stacked: v.yAxesStacked,
                         display: v.yAxesDisplay,
                         offset: false,
                         gridLines: {
                             lineWidth: v.yAxesGridLinesDrawBorder ? [] : [0],
                             display: v.yAxesGridLinesDisplay,
                             color: v.yAxesGridLinesColor,
                             zeroLineColor: v.yAxesGridLinesColor,
@@ -325,15 +372,20 @@
                             padding: v.yAxesTicksPadding,
                             fontSize: v.yAxesTicksFontSize,
                             fontFamily: v.yAxesTicksFontFamily,
                             fontStyle: v.yAxesTicksFontStyle,
                             fontColor: v.yAxesTicksFontColor,
                             minRotation: v.yAxesLabelRotation,
                             maxRotation: v.yAxesLabelRotation,
-                            autoSkip: true
+                            autoSkip: true,
+                            callback: v => {
+                                v = Utils.precisionRound(v, yAxesDecimalNum, yAxesTicksPrecisionFixed);
+
+                                return (yAxesSeparatesThousands ? Utils.separatesThousands(v) : v) + yAxesUnit;
+                            }
                         },
                         scaleLabel: {
                             display: v.yAxesLabelDisplay,
                             labelString: v.yAxisLabel,
                             fontSize: v.yAxesLabelFontSize,
                             fontFamily: v.yAxesLabelFontFamily,
                             fontColor: v.yAxesLabelFontColor,
@@ -347,57 +399,78 @@
                         align: 'top',
                         offset: 0,
                         anchor: 'end',
                         clamp: true,
                         clip: false,
                         display: c => v.tooltipsEnabled ? false : (c.active ? true : (datasets[c.datasetIndex].labelVisible ? 'auto' : false)),
                         borderRadius: 5,
-                        borderWidth: 0,
+                        borderWidth: c => datasets[c.datasetIndex].labelBorderWidth || 0,
+                        borderColor: c => datasets[c.datasetIndex].labelBorderColor,
                         color: c => {
                             c = datasets[c.datasetIndex];
                             return c.labelColor || v.yAxesTicksFontColor || c.borderColor;
                         },
                         backgroundColor: c => {
                             c = datasets[c.datasetIndex];
                             return c.labelBackgroundColor || c.backgroundColor || c.borderColor;
                         },
                         font: {
                             size: v.yAxesTicksFontSize,
-                            color: v.yAxesTicksFontColor,
+                            weight: 'normal',
                             style: v.yAxesTicksFontStyle,
                             family: v.yAxesTicksFontFamily,
                             lineHeight: 1
                         },
                         padding: {
                             top: 7,
                             left: 10,
-                            right: 10
+                            right: 10,
+                            bottom: 0
                         },
-                        formatter: p => 'object' === typeof p ? p.y : p[1]
+                        formatter: v => {
+                            v = Utils.precisionRound('number' === typeof v ? v : v.y, yAxesDecimalNum, yAxesTicksPrecisionFixed);
+
+                            return (yAxesSeparatesThousands ? Utils.separatesThousands(v) : v) + yAxesUnit;
+                        }
                     }
                 },
                 tooltips: {
                     enabled: v.tooltipsEnabled,
                     mode: v.tooltipsMode,
-                    intersect: v.tooltipsIntersect
+                    intersect: v.tooltipsIntersect,
+                    callbacks: {
+                        label: d => {
+                            d = Utils.precisionRound(d.value, yAxesDecimalNum, yAxesTicksPrecisionFixed);
+
+                            return (yAxesSeparatesThousands ? Utils.separatesThousands(d) : d) + yAxesUnit;
+                        }
+                    }
                 },
                 legend: {
                     display: false
                 },
                 title: {
                     display: false
                 },
                 elements: {
                     line: {
-                        tension: 0
+                        tension: v.defaultBezierCurveTension
                     }
                 },
                 animation: {
                     duration: 0
                 },
+                layout: {
+                    padding: {
+                        left: 0,
+                        right: 0,
+                        top: 0,
+                        bottom: 0
+                    }
+                },
                 hover: {
                     mode: 'nearest',
                     intersect: false,
                     animationDuration: 0
                 },
                 onResize: () => setTimeout(() => this.adjustVerticalLineBox(), 100),
                 responsiveAnimationDuration: 0,
@@ -414,15 +487,15 @@
                     for (i = 0; i < d.length; ++i) {
                         e = d[i];
                         c = e.backgroundColor;
 
                         h.push(`<div data-id="${i}" class="ks-legend-item"><div class="ks-legend-item-inner"><div style="color: ${c};" class="ks-legend-icon"></div><div style="color: ${c};" class="ks-legend-label">${e.legendLabel}</div></div></div>`);
                     }
 
-                    return h.join('') + '<\/div>';
+                    return h.join('') + '</div>';
                 }
             }
         };
     }
 
     adjustVerticalLineBox() {
         if (!this.verticalLines || !this.verticalLines.length) {
@@ -453,8 +526,8 @@
 
         for (i = 0; i < len; ++i) {
             i < 2 ? d.data.push(data[i]) : d.datasets = data[i];
         }
 
         return d;
     }
-};
+}
```

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/line-scatter-combo.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/line-scatter-combo.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/loader.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/loader.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/page.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/page.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/pie-chart.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/pie-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/pivot-table.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/pivot-table.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1702,14 +1702,19 @@
 
             for (j = 0, len = cards.length; j < len; ++j) {
                 n = cards.eq(j).data();
                 cardData = {
                     ...n
                 };
 
+                cardData.dimension += '';
+                cardData.hierarchy += '';
+                cardData.subset += '';
+                cardData.element += '';
+
                 if (i) {
                     n = cardData.dimension;
 
                     cardData.expanded_collapsed_members = this.expandedCollapsedMembers[i - 1][n] || {};
                 }
 
                 v.push(cardData);
```

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/popup.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/popup.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/radar-chart.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/radar-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/scroll-table.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/scroll-table.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/segmented-bar.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/segmented-bar.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/segmented-control-item.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/segmented-control-item.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/segmented-control.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/segmented-control.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/simulation-panel-slider.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/simulation-panel-slider.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/simulation-panel.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/simulation-panel.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/slider.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/slider.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/swipe.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/swipe.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/system-popup.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/system-popup.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/text.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/text.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/textarea.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/textarea.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/textbox.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/textbox.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/toggle.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/toggle.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/tornado-chart.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/tornado-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/js/widgets/vertical-line-box.js` & `analogic-framework-4.1.2/analogic/static/assets/js/widgets/vertical-line-box.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-button.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-button.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-container.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-container.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-dropbox.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-dropbox.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-grid-table.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-grid-table.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-grid.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-grid.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-horizontal-table.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-horizontal-table.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-horizontalbarchart.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-horizontalbarchart.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-line-scatter-combo.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-line-scatter-combo.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-pivot-table.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-pivot-table.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-popup.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-popup.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-scrolltable.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-scrolltable.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-segmentedbar.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-segmentedbar.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-slider-touch.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-slider-touch.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-slider.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-slider.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-text.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-text.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-textarea.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-textarea.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-textbox.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-textbox.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-toggle.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-toggle.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-tornado.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-tornado.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/css/ks-vertical-line-box.css` & `analogic-framework-4.1.2/analogic/static/assets/skin/css/ks-vertical-line-box.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.eot` & `analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Bold.eot`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.svg` & `analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Bold.svg`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.ttf` & `analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Bold.ttf`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff` & `analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff2` & `analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff2`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.eot` & `analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Medium.eot`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.svg` & `analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Medium.svg`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.ttf` & `analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Medium.ttf`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff` & `analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff2` & `analogic-framework-4.1.2/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff2`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.eot` & `analogic-framework-4.1.2/analogic/static/assets/skin/fonts/pivot.eot`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.svg` & `analogic-framework-4.1.2/analogic/static/assets/skin/fonts/pivot.svg`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.ttf` & `analogic-framework-4.1.2/analogic/static/assets/skin/fonts/pivot.ttf`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/static/assets/skin/fonts/pivot.woff` & `analogic-framework-4.1.2/analogic/static/assets/skin/fonts/pivot.woff`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/templates/authenticated.html` & `analogic-framework-4.1.2/analogic/templates/authenticated.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/templates/config.html` & `analogic-framework-4.1.2/analogic/templates/config.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 let app = {};
 app = {id: 0, isMobile: null, isTouched: false, url: {}};
 app.assetsUrl = '{{ url_for('static', filename='assets') }}';
 app.applicationAssetsUrl = '{{ url_for(cnf.blueprint_static, filename='assets') }}';
 app.tm1CellsetId = (cellsetId) => `Cellsets('${cellsetId}')?`;
 app.handled401 = false;
 app.pingTime = new Date().getTime();
-{% for key, value in cnf.items() %}
+{% for key, value in cnf.items() if key not in exclude%}
     {% if value is string %}
         app['{{ key }}'] = '{{ value|safe }}';
     {% endif %}
 
     {% if value is integer %}
         app['{{ key }}'] = {{ value }};
     {% endif %}
```

### Comparing `analogic-framework-4.1.1/analogic/templates/css.html` & `analogic-framework-4.1.2/analogic/templates/css.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/templates/javascripts.html` & `analogic-framework-4.1.2/analogic/templates/javascripts.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,118 @@
 <!-- libs -->
-<script  src="{{ url_for('static', filename='assets/js/lib/jquery/jquery-3.6.0.min.js')}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/lib/jquery/jquery.doubletap.js')}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/lib/jquery/jquery.cookie.js')}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/lib/jquery/tableSort.js')}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/lib/debounceAndThrottle.1.8.3.min.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/lib/jquery/jquery.actual.min.js')}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/lib/Chart-2.9.3.min.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/lib/chartjs-plugin-datalabels.min.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/lib/chartjs-plugin-dragdata.min.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/lib/nouislider.min.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/lib/Sortable.min.js')}}?v={{cnf.version}}"></script>
+<script src="{{ url_for('static', filename='assets/js/lib/chartjs4/chart.umd.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/lib/chartjs4/chartjs-plugin-datalabels.min.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/lib/chartjs4/init.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/lib/jquery/jquery-3.6.0.min.js') }}"></script>
+<script src="{{ url_for('static', filename='assets/js/lib/jquery/jquery.doubletap.js') }}"></script>
+<script src="{{ url_for('static', filename='assets/js/lib/jquery/jquery.cookie.js') }}"></script>
+<script src="{{ url_for('static', filename='assets/js/lib/jquery/tableSort.js') }}"></script>
+<script src="{{ url_for('static', filename='assets/js/lib/debounceAndThrottle.1.8.3.min.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/lib/jquery/jquery.actual.min.js') }}"></script>
+<script src="{{ url_for('static', filename='assets/js/lib/Chart-2.9.3.min.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/lib/chartjs-plugin-datalabels.min.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/lib/chartjs-plugin-dragdata.min.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/lib/nouislider.min.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/lib/Sortable.min.js') }}?v={{ cnf.version }}"></script>
 
-<script  src="{{ url_for(cnf.blueprint_static, filename='assets/js/config.js')}}?v={{cnf.version}}"></script>
+<script src="{{ url_for(cnf.blueprint_static, filename='assets/js/config.js') }}?v={{ cnf.version }}"></script>
 <!-- end libs -->
 
 <!-- framework -->
-<script  src="{{ url_for('static', filename='assets/js/framework/app.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/utils.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/render.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/listener.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/api.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/authentication.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/rest-request.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/write-executor/factory.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/write-executor/base.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/write-executor/download.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/write-executor/grid-table.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/write-executor/function.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/write-executor/skip.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/load-executor/factory.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/load-executor/base.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/load-executor/default.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/load-executor/skip.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/load-executor/state.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/load-executor/array.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/parsing-control/factory.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/parsing-control/base.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/parsing-control/skip.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/parsing-control/list.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/parsing-control/matrix.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/parsing-control/object.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/parsing-control/script.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/query-builder.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/server.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/pivot.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/extensions/authentication-provider.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/framework/extensions/write-executor.js')}}?v={{cnf.version}}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/app.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/utils.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/render.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/listener.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/api.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/authentication.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/rest-request.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/write-executor/factory.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/write-executor/base.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/write-executor/download.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/write-executor/grid-table.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/write-executor/function.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/write-executor/skip.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/load-executor/factory.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/load-executor/base.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/load-executor/default.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/load-executor/skip.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/load-executor/state.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/load-executor/array.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/parsing-control/factory.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/parsing-control/base.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/parsing-control/skip.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/parsing-control/list.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/parsing-control/matrix.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/parsing-control/object.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/parsing-control/script.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/query-builder.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/server.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/pivot.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/extensions/authentication-provider.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/framework/extensions/write-executor.js') }}?v={{ cnf.version }}"></script>
 <!-- end framework -->
 
 <!-- widgets -->
-<script  src="{{ url_for('static', filename='assets/js/widgets/base/widget.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/loader.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/container.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/popup.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/swipe.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/simulation-panel.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/scroll-table.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/datepicker.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/combo-chart.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/simulation-panel-slider.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/water-fall.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/grid-table/grid-table.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/grid-table/grid-table-cell.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/grid-table/grid-table-header-row.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/grid-table/grid-table-header-cell.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/button.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/text.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/textbox.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/dropbox.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/toggle.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/slider.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/gauge.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/histogram-combo-chart.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/line-scatter-combo.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/segmented-bar.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/tornado-chart.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/page.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/image.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/segmented-control.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/segmented-control-item.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/horizontal-table.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/horizontaltable/radio-button-row.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/horizontaltable/action-button-row.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/horizontaltable/delete-button-row.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/textarea.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/system-popup.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/pie-chart.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/radar-chart.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/line-area-chart.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/vertical-line-box.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/shadow.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/pivot-table.js')}}?v={{cnf.version}}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/base/widget.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/loader.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/container.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/popup.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/swipe.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/simulation-panel.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/scroll-table.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/datepicker.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/combo-chart.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/simulation-panel-slider.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/water-fall.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/grid-table/grid-table.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/grid-table/grid-table-cell.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/grid-table/grid-table-header-row.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/grid-table/grid-table-header-cell.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/button.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/text.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/textbox.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/dropbox.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/toggle.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/slider.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/gauge.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/histogram-combo-chart.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/line-scatter-combo.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/segmented-bar.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/tornado-chart.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/page.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/image.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/segmented-control.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/segmented-control-item.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/horizontal-table.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/horizontaltable/radio-button-row.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/horizontaltable/action-button-row.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/horizontaltable/delete-button-row.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/textarea.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/system-popup.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/pie-chart.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/radar-chart.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/line-area-chart.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/stacked-column-chart.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/vertical-line-box.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/shadow.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/pivot-table.js') }}?v={{ cnf.version }}"></script>
 
-<script  src="{{ url_for('static', filename='assets/js/widgets/horizontal-bar-chart.js')}}?v={{cnf.version}}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/horizontal-bar-chart.js') }}?v={{ cnf.version }}"></script>
 
 {% for asset_name in cnf.extension_js_asset_names %}
-    <script  src="{{ url_for('extension_asset', asset_name=asset_name)}}&v={{cnf.version}}"></script>
+    <script src="{{ url_for('extension_asset', asset_name=asset_name) }}&v={{ cnf.version }}"></script>
 {% endfor %}
 
 <!-- end widgets -->
 
 <!-- layouts -->
-<script  src="{{ url_for('static', filename='assets/js/widgets/grid/grid.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/grid/grid-row.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/grid/grid-cell.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for('static', filename='assets/js/widgets/panel.js')}}?v={{cnf.version}}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/grid/grid.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/grid/grid-row.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/grid/grid-cell.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for('static', filename='assets/js/widgets/panel.js') }}?v={{ cnf.version }}"></script>
 <!-- end layouts -->
 
 <!-- configs -->
-<script  src="{{ url_for(cnf.blueprint_static, filename='assets/js/configs/repository.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for(cnf.blueprint_static, filename='assets/js/configs/widget-config.js')}}?v={{cnf.version}}"></script>
-<script  src="{{ url_for(cnf.blueprint_static, filename='assets/js/configs/event-map.js')}}?v={{cnf.version}}"></script>
+<script src="{{ url_for(cnf.blueprint_static, filename='assets/js/configs/repository.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for(cnf.blueprint_static, filename='assets/js/configs/widget-config.js') }}?v={{ cnf.version }}"></script>
+<script src="{{ url_for(cnf.blueprint_static, filename='assets/js/configs/event-map.js') }}?v={{ cnf.version }}"></script>
 <!-- end configs -->
```

### Comparing `analogic-framework-4.1.1/analogic/templates/login.html` & `analogic-framework-4.1.2/analogic/templates/login.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/templates/redirect.html` & `analogic-framework-4.1.2/analogic/templates/redirect.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic/templates/sso_error.html` & `analogic-framework-4.1.2/analogic/templates/sso_error.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.1.1/analogic_framework.egg-info/SOURCES.txt` & `analogic-framework-4.1.2/analogic_framework.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -69,14 +69,18 @@
 analogic/static/assets/js/framework/write-executor/skip.js
 analogic/static/assets/js/lib/Chart-2.9.3.min.js
 analogic/static/assets/js/lib/Sortable.min.js
 analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js
 analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js
 analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js
 analogic/static/assets/js/lib/nouislider.min.js
+analogic/static/assets/js/lib/chartjs4/chart.umd.js
+analogic/static/assets/js/lib/chartjs4/chart.umd.js.map
+analogic/static/assets/js/lib/chartjs4/chartjs-plugin-datalabels.min.js
+analogic/static/assets/js/lib/chartjs4/init.js
 analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js
 analogic/static/assets/js/lib/jquery/jquery.actual.min.js
 analogic/static/assets/js/lib/jquery/jquery.cookie.js
 analogic/static/assets/js/lib/jquery/jquery.doubletap.js
 analogic/static/assets/js/lib/jquery/tableSort.js
 analogic/static/assets/js/widgets/button.js
 analogic/static/assets/js/widgets/combo-chart.js
@@ -101,14 +105,15 @@
 analogic/static/assets/js/widgets/segmented-bar.js
 analogic/static/assets/js/widgets/segmented-control-item.js
 analogic/static/assets/js/widgets/segmented-control.js
 analogic/static/assets/js/widgets/shadow.js
 analogic/static/assets/js/widgets/simulation-panel-slider.js
 analogic/static/assets/js/widgets/simulation-panel.js
 analogic/static/assets/js/widgets/slider.js
+analogic/static/assets/js/widgets/stacked-column-chart.js
 analogic/static/assets/js/widgets/swipe.js
 analogic/static/assets/js/widgets/system-popup.js
 analogic/static/assets/js/widgets/text.js
 analogic/static/assets/js/widgets/textarea.js
 analogic/static/assets/js/widgets/textbox.js
 analogic/static/assets/js/widgets/toggle.js
 analogic/static/assets/js/widgets/tornado-chart.js
```

### Comparing `analogic-framework-4.1.1/setup.py` & `analogic-framework-4.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,18 @@
     python_requires='>=3.9',
     packages=[
         'analogic'
     ],
     include_package_data=True,
     package_data={'': ['version.config']},
     install_requires=[
-        'Flask==2.1.2',
-        'Flask-Caching==2.0.0',
-        'TM1py==1.9.1',
+        'Flask==2.3.2',
+        'TM1py==1.11.3',
         'PyJWT==2.4.0',
-        'requests==2.28.1',
+        'requests==2.31.0',
         'numpy==1.23.1',
         'pandas==1.4.3',
         'XlsxWriter==1.3.7',
         'matplotlib==3.5.2',
         'PyYaml==6.0',
         'xlrd==2.0.1',
         'openpyxl==3.0.10',
```

