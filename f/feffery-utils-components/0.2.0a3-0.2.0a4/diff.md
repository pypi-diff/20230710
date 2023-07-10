# Comparing `tmp/feffery_utils_components-0.2.0a3.tar.gz` & `tmp/feffery_utils_components-0.2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feffery_utils_components-0.2.0a3.tar", last modified: Fri Jun 16 02:38:24 2023, max compression
+gzip compressed data, was "feffery_utils_components-0.2.0a4.tar", last modified: Mon Jul 10 09:50:53 2023, max compression
```

## Comparing `feffery_utils_components-0.2.0a3.tar` & `feffery_utils_components-0.2.0a4.tar`

### file list

```diff
@@ -1,88 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.909885 feffery_utils_components-0.2.0a3/
--rw-rw-rw-   0        0        0     1087 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a3/LICENSE
--rw-rw-rw-   0        0        0      484 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a3/MANIFEST.in
--rw-rw-rw-   0        0        0      342 2023-06-16 02:38:24.907714 feffery_utils_components-0.2.0a3/PKG-INFO
--rw-rw-rw-   0        0        0     1432 2023-05-28 10:44:03.000000 feffery_utils_components-0.2.0a3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.896794 feffery_utils_components-0.2.0a3/feffery_utils_components/
--rw-rw-rw-   0        0        0     1877 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyAutoAnimate.py
--rw-rw-rw-   0        0        0     2015 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyBlockColorPicker.py
--rw-rw-rw-   0        0        0     2093 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyCaptcha.py
--rw-rw-rw-   0        0        0     2207 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyCircleColorPicker.py
--rw-rw-rw-   0        0        0     2784 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyCompareSlider.py
--rw-rw-rw-   0        0        0     2049 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyCookie.py
--rw-rw-rw-   0        0        0     1616 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyCountDown.py
--rw-rw-rw-   0        0        0     2508 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyCountUp.py
--rw-rw-rw-   0        0        0     1431 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyCssVar.py
--rw-rw-rw-   0        0        0     2078 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyDeviceDetect.py
--rw-rw-rw-   0        0        0     4313 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyDiv.py
--rw-rw-rw-   0        0        0     1556 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyDocumentVisibility.py
--rw-rw-rw-   0        0        0     1449 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyExecuteJs.py
--rw-rw-rw-   0        0        0     1610 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyExternalCss.py
--rw-rw-rw-   0        0        0     1602 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyExternalJs.py
--rw-rw-rw-   0        0        0     2390 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyExtraSpinner.py
--rw-rw-rw-   0        0        0     1526 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyEyeDropper.py
--rw-rw-rw-   0        0        0     2687 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyFancyButton.py
--rw-rw-rw-   0        0        0     2816 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyFancyMessage.py
--rw-rw-rw-   0        0        0     3737 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyFancyNotification.py
--rw-rw-rw-   0        0        0     1733 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyFullscreen.py
--rw-rw-rw-   0        0        0     1483 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyGeolocation.py
--rw-rw-rw-   0        0        0     2037 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyGithubColorPicker.py
--rw-rw-rw-   0        0        0     5043 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyGrid.py
--rw-rw-rw-   0        0        0     1749 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyGridItem.py
--rw-rw-rw-   0        0        0     3888 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyGuide.py
--rw-rw-rw-   0        0        0     1727 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyHexColorPicker.py
--rw-rw-rw-   0        0        0     2498 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyHighlightWords.py
--rw-rw-rw-   0        0        0     1529 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyIdle.py
--rw-rw-rw-   0        0        0     1728 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyImagePaste.py
--rw-rw-rw-   0        0        0     1713 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyInViewport.py
--rw-rw-rw-   0        0        0     3879 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyJsonViewer.py
--rw-rw-rw-   0        0        0     1704 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyKeyPress.py
--rw-rw-rw-   0        0        0     2109 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyLazyLoad.py
--rw-rw-rw-   0        0        0     1809 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyListenPaste.py
--rw-rw-rw-   0        0        0     1538 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyListenScroll.py
--rw-rw-rw-   0        0        0     1462 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyListenUnload.py
--rw-rw-rw-   0        0        0     2108 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyLocation.py
--rw-rw-rw-   0        0        0     3312 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyMotion.py
--rw-rw-rw-   0        0        0     1463 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyMousePosition.py
--rw-rw-rw-   0        0        0     2479 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyQRCode.py
--rw-rw-rw-   0        0        0     1449 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyRawHTML.py
--rw-rw-rw-   0        0        0     1505 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyReload.py
--rw-rw-rw-   0        0        0     3724 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyResizable.py
--rw-rw-rw-   0        0        0     1459 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyResponsive.py
--rw-rw-rw-   0        0        0     1737 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyRgbColorPicker.py
--rw-rw-rw-   0        0        0     2653 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyScroll.py
--rw-rw-rw-   0        0        0     2531 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyScrollbars.py
--rw-rw-rw-   0        0        0     1651 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySessionStorage.py
--rw-rw-rw-   0        0        0     1433 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySetTitle.py
--rw-rw-rw-   0        0        0     1753 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyShadowDom.py
--rw-rw-rw-   0        0        0     3498 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyShortcutPanel.py
--rw-rw-rw-   0        0        0     1358 2023-06-15 10:22:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySortable.py
--rw-rw-rw-   0        0        0     1945 2023-06-13 03:49:15.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySortableContainer.py
--rw-rw-rw-   0        0        0     1698 2023-06-13 03:49:15.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySortableItem.py
--rw-rw-rw-   0        0        0     2966 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySortableList.py
--rw-rw-rw-   0        0        0     2472 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySplit.py
--rw-rw-rw-   0        0        0     1686 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySplitPane.py
--rw-rw-rw-   0        0        0     1874 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySticky.py
--rw-rw-rw-   0        0        0     1433 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyStyle.py
--rw-rw-rw-   0        0        0     1533 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyTimeout.py
--rw-rw-rw-   0        0        0     2845 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyTopProgress.py
--rw-rw-rw-   0        0        0     2057 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyTwitterColorPicker.py
--rw-rw-rw-   0        0        0     1606 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyUnmount.py
--rw-rw-rw-   0        0        0     2050 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyVirtualList.py
--rw-rw-rw-   0        0        0     2311 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyWebSocket.py
--rw-rw-rw-   0        0        0     1629 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyWheelColorPicker.py
--rw-rw-rw-   0        0        0     1528 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyWindowSize.py
--rw-rw-rw-   0        0        0     2610 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/__init__.py
--rw-rw-rw-   0        0        0     4888 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/_imports_.py
--rw-rw-rw-   0        0        0  1378706 2023-06-16 02:38:21.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/feffery_utils_components.min.js
--rw-rw-rw-   0        0        0   206765 2023-06-16 02:38:23.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/metadata.json
--rw-rw-rw-   0        0        0     4067 2023-06-16 02:38:22.000000 feffery_utils_components-0.2.0a3/feffery_utils_components/package-info.json
-drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.905511 feffery_utils_components-0.2.0a3/feffery_utils_components.egg-info/
--rw-rw-rw-   0        0        0      342 2023-06-16 02:38:24.000000 feffery_utils_components-0.2.0a3/feffery_utils_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3639 2023-06-16 02:38:24.000000 feffery_utils_components-0.2.0a3/feffery_utils_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 02:38:24.000000 feffery_utils_components-0.2.0a3/feffery_utils_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-16 02:38:24.000000 feffery_utils_components-0.2.0a3/feffery_utils_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-16 02:38:24.000000 feffery_utils_components-0.2.0a3/feffery_utils_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4067 2023-06-16 02:36:52.000000 feffery_utils_components-0.2.0a3/package.json
--rw-rw-rw-   0        0        0       42 2023-06-16 02:38:24.909885 feffery_utils_components-0.2.0a3/setup.cfg
--rw-rw-rw-   0        0        0      729 2023-06-16 02:37:57.000000 feffery_utils_components-0.2.0a3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:50:53.369332 feffery_utils_components-0.2.0a4/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a4/LICENSE
+-rw-rw-rw-   0        0        0      484 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a4/MANIFEST.in
+-rw-rw-rw-   0        0        0      342 2023-07-10 09:50:53.369332 feffery_utils_components-0.2.0a4/PKG-INFO
+-rw-rw-rw-   0        0        0     1432 2023-05-28 10:44:03.000000 feffery_utils_components-0.2.0a4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 09:50:53.357375 feffery_utils_components-0.2.0a4/feffery_utils_components/
+-rw-rw-rw-   0        0        0     1877 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyAutoAnimate.py
+-rw-rw-rw-   0        0        0     2015 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyBlockColorPicker.py
+-rw-rw-rw-   0        0        0     2093 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCaptcha.py
+-rw-rw-rw-   0        0        0     2207 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCircleColorPicker.py
+-rw-rw-rw-   0        0        0     2784 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCompareSlider.py
+-rw-rw-rw-   0        0        0     2049 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCookie.py
+-rw-rw-rw-   0        0        0     1616 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCountDown.py
+-rw-rw-rw-   0        0        0     2508 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCountUp.py
+-rw-rw-rw-   0        0        0     1431 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCssVar.py
+-rw-rw-rw-   0        0        0     2078 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyDeviceDetect.py
+-rw-rw-rw-   0        0        0     4313 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyDiv.py
+-rw-rw-rw-   0        0        0     1556 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyDocumentVisibility.py
+-rw-rw-rw-   0        0        0     1449 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExecuteJs.py
+-rw-rw-rw-   0        0        0     1610 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExternalCss.py
+-rw-rw-rw-   0        0        0     1602 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExternalJs.py
+-rw-rw-rw-   0        0        0     2390 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExtraSpinner.py
+-rw-rw-rw-   0        0        0     1526 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyEyeDropper.py
+-rw-rw-rw-   0        0        0     2687 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFancyButton.py
+-rw-rw-rw-   0        0        0     2816 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFancyMessage.py
+-rw-rw-rw-   0        0        0     3737 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFancyNotification.py
+-rw-rw-rw-   0        0        0     1733 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFullscreen.py
+-rw-rw-rw-   0        0        0     1483 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGeolocation.py
+-rw-rw-rw-   0        0        0     2037 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGithubColorPicker.py
+-rw-rw-rw-   0        0        0     5043 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGrid.py
+-rw-rw-rw-   0        0        0     1749 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGridItem.py
+-rw-rw-rw-   0        0        0     3888 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGuide.py
+-rw-rw-rw-   0        0        0     1727 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyHexColorPicker.py
+-rw-rw-rw-   0        0        0     2498 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyHighlightWords.py
+-rw-rw-rw-   0        0        0     1529 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyIdle.py
+-rw-rw-rw-   0        0        0     1728 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyImagePaste.py
+-rw-rw-rw-   0        0        0     1713 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyInViewport.py
+-rw-rw-rw-   0        0        0     3879 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyJsonViewer.py
+-rw-rw-rw-   0        0        0     1704 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyKeyPress.py
+-rw-rw-rw-   0        0        0     2109 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyLazyLoad.py
+-rw-rw-rw-   0        0        0     1809 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyListenPaste.py
+-rw-rw-rw-   0        0        0     1538 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyListenScroll.py
+-rw-rw-rw-   0        0        0     1462 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyListenUnload.py
+-rw-rw-rw-   0        0        0     1748 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyLocalStorage.py
+-rw-rw-rw-   0        0        0     2108 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyLocation.py
+-rw-rw-rw-   0        0        0     3312 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyMotion.py
+-rw-rw-rw-   0        0        0     1463 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyMousePosition.py
+-rw-rw-rw-   0        0        0     1577 2023-07-08 13:15:23.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyPopout.py
+-rw-rw-rw-   0        0        0     2479 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyQRCode.py
+-rw-rw-rw-   0        0        0     1449 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyRawHTML.py
+-rw-rw-rw-   0        0        0     1505 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyReload.py
+-rw-rw-rw-   0        0        0     3724 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyResizable.py
+-rw-rw-rw-   0        0        0     1459 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyResponsive.py
+-rw-rw-rw-   0        0        0     1737 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyRgbColorPicker.py
+-rw-rw-rw-   0        0        0     2653 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyScroll.py
+-rw-rw-rw-   0        0        0     2531 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyScrollbars.py
+-rw-rw-rw-   0        0        0     1756 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySessionStorage.py
+-rw-rw-rw-   0        0        0     1433 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySetTitle.py
+-rw-rw-rw-   0        0        0     1753 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyShadowDom.py
+-rw-rw-rw-   0        0        0     3498 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyShortcutPanel.py
+-rw-rw-rw-   0        0        0     1358 2023-06-15 10:22:23.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySortable.py
+-rw-rw-rw-   0        0        0     1945 2023-06-13 03:49:15.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySortableContainer.py
+-rw-rw-rw-   0        0        0     1698 2023-06-13 03:49:15.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySortableItem.py
+-rw-rw-rw-   0        0        0     3103 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySortableList.py
+-rw-rw-rw-   0        0        0     2472 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySplit.py
+-rw-rw-rw-   0        0        0     1686 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySplitPane.py
+-rw-rw-rw-   0        0        0     1874 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySticky.py
+-rw-rw-rw-   0        0        0     1433 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyStyle.py
+-rw-rw-rw-   0        0        0     1533 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyTimeout.py
+-rw-rw-rw-   0        0        0     2845 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyTopProgress.py
+-rw-rw-rw-   0        0        0     2057 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyTwitterColorPicker.py
+-rw-rw-rw-   0        0        0     1606 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyUnmount.py
+-rw-rw-rw-   0        0        0     2050 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyVirtualList.py
+-rw-rw-rw-   0        0        0     2311 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyWebSocket.py
+-rw-rw-rw-   0        0        0     1629 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyWheelColorPicker.py
+-rw-rw-rw-   0        0        0     1528 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyWindowSize.py
+-rw-rw-rw-   0        0        0     2610 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/__init__.py
+-rw-rw-rw-   0        0        0     4970 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/_imports_.py
+-rw-rw-rw-   0        0        0  1380501 2023-07-10 09:50:49.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/feffery_utils_components.min.js
+-rw-rw-rw-   0        0        0   209192 2023-07-10 09:50:52.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/metadata.json
+-rw-rw-rw-   0        0        0     4130 2023-07-10 09:50:50.000000 feffery_utils_components-0.2.0a4/feffery_utils_components/package-info.json
+drwxrwxrwx   0        0        0        0 2023-07-10 09:50:53.367219 feffery_utils_components-0.2.0a4/feffery_utils_components.egg-info/
+-rw-rw-rw-   0        0        0      342 2023-07-10 09:50:53.000000 feffery_utils_components-0.2.0a4/feffery_utils_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3729 2023-07-10 09:50:53.000000 feffery_utils_components-0.2.0a4/feffery_utils_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 09:50:53.000000 feffery_utils_components-0.2.0a4/feffery_utils_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-10 09:50:53.000000 feffery_utils_components-0.2.0a4/feffery_utils_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-10 09:50:53.000000 feffery_utils_components-0.2.0a4/feffery_utils_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4130 2023-07-10 09:17:35.000000 feffery_utils_components-0.2.0a4/package.json
+-rw-rw-rw-   0        0        0       42 2023-07-10 09:50:53.370469 feffery_utils_components-0.2.0a4/setup.cfg
+-rw-rw-rw-   0        0        0      729 2023-06-16 02:41:22.000000 feffery_utils_components-0.2.0a4/setup.py
```

### Comparing `feffery_utils_components-0.2.0a3/LICENSE` & `feffery_utils_components-0.2.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/README.md` & `feffery_utils_components-0.2.0a4/README.md`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyAutoAnimate.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyAutoAnimate.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyBlockColorPicker.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyBlockColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyCaptcha.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCaptcha.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyCircleColorPicker.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCircleColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyCompareSlider.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCompareSlider.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyCookie.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCookie.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyCountDown.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCountDown.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyCountUp.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCountUp.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyCssVar.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyCssVar.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyDeviceDetect.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyDeviceDetect.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyDiv.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyDiv.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyDocumentVisibility.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyDocumentVisibility.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyExecuteJs.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExecuteJs.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyExternalCss.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExternalCss.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyExternalJs.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExternalJs.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyExtraSpinner.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyExtraSpinner.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyEyeDropper.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyEyeDropper.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyFancyButton.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFancyButton.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyFancyMessage.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFancyMessage.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyFancyNotification.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFancyNotification.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyFullscreen.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyFullscreen.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyGeolocation.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGeolocation.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyGithubColorPicker.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGithubColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyGrid.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGrid.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyGridItem.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGridItem.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyGuide.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyGuide.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyHexColorPicker.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyHexColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyHighlightWords.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyHighlightWords.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyIdle.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyIdle.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyImagePaste.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyImagePaste.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyInViewport.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyInViewport.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyJsonViewer.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyJsonViewer.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyKeyPress.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyKeyPress.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyLazyLoad.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyLazyLoad.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyListenPaste.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyListenPaste.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyListenScroll.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyListenScroll.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyListenUnload.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyListenUnload.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyLocation.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyLocation.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyMotion.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyMotion.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyMousePosition.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyMousePosition.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyQRCode.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyQRCode.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyRawHTML.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyRawHTML.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyReload.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyReload.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyResizable.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyResizable.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyResponsive.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyResponsive.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyRgbColorPicker.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyRgbColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyScroll.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyScroll.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyScrollbars.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyScrollbars.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySessionStorage.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySessionStorage.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 Keyword arguments:
 
 - id (string; required)
 
 - data (boolean | number | string | dict | list; optional)
 
+- initialSync (boolean; default False)
+
 - loading_state (dict; optional)
 
     `loading_state` is a dict with keys:
 
     - component_name (string; optional):
         Holds the name of the component that is loading.
 
@@ -26,18 +28,18 @@
     - prop_name (string; optional):
         Holds which property is loading."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_utils_components'
     _type = 'FefferySessionStorage'
     @_explicitize_args
-    def __init__(self, id=Component.REQUIRED, data=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'data', 'loading_state']
+    def __init__(self, id=Component.REQUIRED, data=Component.UNDEFINED, initialSync=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'data', 'initialSync', 'loading_state']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'data', 'loading_state']
+        self.available_properties = ['id', 'data', 'initialSync', 'loading_state']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         for k in ['id']:
```

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySetTitle.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySetTitle.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyShadowDom.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyShadowDom.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyShortcutPanel.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyShortcutPanel.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySortable.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySortable.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySortableContainer.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySortableContainer.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySortableItem.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySortableItem.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySortableList.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySplit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,63 @@
 # AUTO GENERATED FILE - DO NOT EDIT
 
 from dash.development.base_component import Component, _explicitize_args
 
 
-class FefferySortableList(Component):
-    """A FefferySortableList component.
+class FefferySplit(Component):
+    """A FefferySplit component.
 
 
 Keyword arguments:
 
-- id (string; optional)
-
-- className (string | dict; optional)
-
-- currentOrder (list of number | strings; optional)
-
-- handleClassName (string | dict; optional)
-
-- handlePosition (a value equal to: 'start', 'end'; default 'end')
-
-- handleStyle (dict; optional)
-
-- handleType (a value equal to: 'holder', 'menu', 'drag'; default 'holder')
-
-- itemDraggingScale (number; default 1)
+- children (a list of or a singular dash component, string or number; optional)
 
-- items (list of dicts; required)
-
-    `items` is a list of dicts with keys:
-
-    - className (string | dict; optional)
+- id (string; optional)
 
-    - content (a list of or a singular dash component, string or number; optional)
+- className (string; optional)
 
-    - draggingClassName (string | dict; optional)
+- cursor (string; optional)
 
-    - draggingStyle (dict; optional)
+- direction (a value equal to: 'horizontal', 'vertical'; default 'horizontal')
 
-    - key (number | string; required)
+- dragInterval (number; optional)
 
-    - style (dict; optional)
+- expandToMin (boolean; optional)
 
-- key (string; optional)
+- gutterSize (number; optional)
 
 - loading_state (dict; optional)
 
     `loading_state` is a dict with keys:
 
     - component_name (string; optional):
         Holds the name of the component that is loading.
 
     - is_loading (boolean; optional):
         Determines if the component is loading or not.
 
     - prop_name (string; optional):
         Holds which property is loading.
 
+- maxSize (number | list of numbers; optional)
+
+- minSize (number | list of numbers; optional)
+
+- sizes (list of numbers; optional)
+
 - style (dict; optional)"""
-    _children_props = ['items[].content']
+    _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_utils_components'
-    _type = 'FefferySortableList'
+    _type = 'FefferySplit'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, style=Component.UNDEFINED, handleStyle=Component.UNDEFINED, handleClassName=Component.UNDEFINED, className=Component.UNDEFINED, key=Component.UNDEFINED, items=Component.REQUIRED, itemDraggingScale=Component.UNDEFINED, handlePosition=Component.UNDEFINED, handleType=Component.UNDEFINED, currentOrder=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'className', 'currentOrder', 'handleClassName', 'handlePosition', 'handleStyle', 'handleType', 'itemDraggingScale', 'items', 'key', 'loading_state', 'style']
+    def __init__(self, children=None, id=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, sizes=Component.UNDEFINED, minSize=Component.UNDEFINED, maxSize=Component.UNDEFINED, expandToMin=Component.UNDEFINED, gutterSize=Component.UNDEFINED, dragInterval=Component.UNDEFINED, direction=Component.UNDEFINED, cursor=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['children', 'id', 'className', 'cursor', 'direction', 'dragInterval', 'expandToMin', 'gutterSize', 'loading_state', 'maxSize', 'minSize', 'sizes', 'style']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'className', 'currentOrder', 'handleClassName', 'handlePosition', 'handleStyle', 'handleType', 'itemDraggingScale', 'items', 'key', 'loading_state', 'style']
+        self.available_properties = ['children', 'id', 'className', 'cursor', 'direction', 'dragInterval', 'expandToMin', 'gutterSize', 'loading_state', 'maxSize', 'minSize', 'sizes', 'style']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
-        args = {k: _locals[k] for k in _explicit_args}
-
-        for k in ['items']:
-            if k not in args:
-                raise TypeError(
-                    'Required argument `' + k + '` was not specified.')
+        args = {k: _locals[k] for k in _explicit_args if k != 'children'}
 
-        super(FefferySortableList, self).__init__(**args)
+        super(FefferySplit, self).__init__(children=children, **args)
```

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySplit.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyVirtualList.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,56 @@
 # AUTO GENERATED FILE - DO NOT EDIT
 
 from dash.development.base_component import Component, _explicitize_args
 
 
-class FefferySplit(Component):
-    """A FefferySplit component.
+class FefferyVirtualList(Component):
+    """A FefferyVirtualList component.
 
 
 Keyword arguments:
 
 - children (a list of or a singular dash component, string or number; optional)
 
 - id (string; optional)
 
 - className (string; optional)
 
-- cursor (string; optional)
+- height (number; required)
 
-- direction (a value equal to: 'horizontal', 'vertical'; default 'horizontal')
-
-- dragInterval (number; optional)
-
-- expandToMin (boolean; optional)
-
-- gutterSize (number; optional)
+- itemHeight (number; required)
 
 - loading_state (dict; optional)
 
     `loading_state` is a dict with keys:
 
     - component_name (string; optional):
         Holds the name of the component that is loading.
 
     - is_loading (boolean; optional):
         Determines if the component is loading or not.
 
     - prop_name (string; optional):
         Holds which property is loading.
 
-- maxSize (number | list of numbers; optional)
-
-- minSize (number | list of numbers; optional)
-
-- sizes (list of numbers; optional)
-
 - style (dict; optional)"""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_utils_components'
-    _type = 'FefferySplit'
+    _type = 'FefferyVirtualList'
     @_explicitize_args
-    def __init__(self, children=None, id=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, sizes=Component.UNDEFINED, minSize=Component.UNDEFINED, maxSize=Component.UNDEFINED, expandToMin=Component.UNDEFINED, gutterSize=Component.UNDEFINED, dragInterval=Component.UNDEFINED, direction=Component.UNDEFINED, cursor=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['children', 'id', 'className', 'cursor', 'direction', 'dragInterval', 'expandToMin', 'gutterSize', 'loading_state', 'maxSize', 'minSize', 'sizes', 'style']
+    def __init__(self, children=None, id=Component.UNDEFINED, style=Component.UNDEFINED, className=Component.UNDEFINED, height=Component.REQUIRED, itemHeight=Component.REQUIRED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['children', 'id', 'className', 'height', 'itemHeight', 'loading_state', 'style']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['children', 'id', 'className', 'cursor', 'direction', 'dragInterval', 'expandToMin', 'gutterSize', 'loading_state', 'maxSize', 'minSize', 'sizes', 'style']
+        self.available_properties = ['children', 'id', 'className', 'height', 'itemHeight', 'loading_state', 'style']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args if k != 'children'}
 
-        super(FefferySplit, self).__init__(children=children, **args)
+        for k in ['height', 'itemHeight']:
+            if k not in args:
+                raise TypeError(
+                    'Required argument `' + k + '` was not specified.')
+
+        super(FefferyVirtualList, self).__init__(children=children, **args)
```

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySplitPane.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySplitPane.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferySticky.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferySticky.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyStyle.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyStyle.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyTimeout.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyTimeout.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyTopProgress.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyTopProgress.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyTwitterColorPicker.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyTwitterColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyUnmount.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyUnmount.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyVirtualList.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyWindowSize.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,45 @@
 # AUTO GENERATED FILE - DO NOT EDIT
 
 from dash.development.base_component import Component, _explicitize_args
 
 
-class FefferyVirtualList(Component):
-    """A FefferyVirtualList component.
+class FefferyWindowSize(Component):
+    """A FefferyWindowSize component.
 
 
 Keyword arguments:
 
-- children (a list of or a singular dash component, string or number; optional)
-
 - id (string; optional)
 
-- className (string; optional)
-
-- height (number; required)
+- _height (number; optional)
 
-- itemHeight (number; required)
+- _width (number; optional)
 
 - loading_state (dict; optional)
 
     `loading_state` is a dict with keys:
 
     - component_name (string; optional):
         Holds the name of the component that is loading.
 
     - is_loading (boolean; optional):
         Determines if the component is loading or not.
 
     - prop_name (string; optional):
-        Holds which property is loading.
-
-- style (dict; optional)"""
+        Holds which property is loading."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_utils_components'
-    _type = 'FefferyVirtualList'
+    _type = 'FefferyWindowSize'
     @_explicitize_args
-    def __init__(self, children=None, id=Component.UNDEFINED, style=Component.UNDEFINED, className=Component.UNDEFINED, height=Component.REQUIRED, itemHeight=Component.REQUIRED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['children', 'id', 'className', 'height', 'itemHeight', 'loading_state', 'style']
+    def __init__(self, id=Component.UNDEFINED, _width=Component.UNDEFINED, _height=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', '_height', '_width', 'loading_state']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['children', 'id', 'className', 'height', 'itemHeight', 'loading_state', 'style']
+        self.available_properties = ['id', '_height', '_width', 'loading_state']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
-        args = {k: _locals[k] for k in _explicit_args if k != 'children'}
-
-        for k in ['height', 'itemHeight']:
-            if k not in args:
-                raise TypeError(
-                    'Required argument `' + k + '` was not specified.')
+        args = {k: _locals[k] for k in _explicit_args}
 
-        super(FefferyVirtualList, self).__init__(children=children, **args)
+        super(FefferyWindowSize, self).__init__(**args)
```

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyWebSocket.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyWebSocket.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyWheelColorPicker.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyWheelColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/FefferyWindowSize.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/FefferyPopout.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # AUTO GENERATED FILE - DO NOT EDIT
 
 from dash.development.base_component import Component, _explicitize_args
 
 
-class FefferyWindowSize(Component):
-    """A FefferyWindowSize component.
+class FefferyPopout(Component):
+    """A FefferyPopout component.
 
 
 Keyword arguments:
 
-- id (string; optional)
-
-- _height (number; optional)
+- children (a list of or a singular dash component, string or number; optional)
 
-- _width (number; optional)
+- id (string; optional)
 
 - loading_state (dict; optional)
 
     `loading_state` is a dict with keys:
 
     - component_name (string; optional):
         Holds the name of the component that is loading.
 
     - is_loading (boolean; optional):
         Determines if the component is loading or not.
 
     - prop_name (string; optional):
-        Holds which property is loading."""
+        Holds which property is loading.
+
+- url (string; optional)"""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_utils_components'
-    _type = 'FefferyWindowSize'
+    _type = 'FefferyPopout'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, _width=Component.UNDEFINED, _height=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', '_height', '_width', 'loading_state']
+    def __init__(self, children=None, id=Component.UNDEFINED, url=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['children', 'id', 'loading_state', 'url']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', '_height', '_width', 'loading_state']
+        self.available_properties = ['children', 'id', 'loading_state', 'url']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
-        args = {k: _locals[k] for k in _explicit_args}
+        args = {k: _locals[k] for k in _explicit_args if k != 'children'}
 
-        super(FefferyWindowSize, self).__init__(**args)
+        super(FefferyPopout, self).__init__(children=children, **args)
```

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/__init__.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/__init__.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/_imports_.py` & `feffery_utils_components-0.2.0a4/feffery_utils_components/_imports_.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 from .FefferyResponsive import FefferyResponsive
 from .FefferyWindowSize import FefferyWindowSize
 from .FefferyResizable import FefferyResizable
 from .FefferySortableList import FefferySortableList
 from .FefferySplit import FefferySplit
 from .FefferySplitPane import FefferySplitPane
 from .FefferyCookie import FefferyCookie
+from .FefferyLocalStorage import FefferyLocalStorage
 from .FefferySessionStorage import FefferySessionStorage
 
 __all__ = [
     "FefferyAutoAnimate",
     "FefferyMotion",
     "FefferyBlockColorPicker",
     "FefferyCircleColorPicker",
@@ -123,9 +124,10 @@
     "FefferyResponsive",
     "FefferyWindowSize",
     "FefferyResizable",
     "FefferySortableList",
     "FefferySplit",
     "FefferySplitPane",
     "FefferyCookie",
+    "FefferyLocalStorage",
     "FefferySessionStorage"
 ]
```

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/feffery_utils_components.min.js` & `feffery_utils_components-0.2.0a4/feffery_utils_components/feffery_utils_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -57,15 +57,15 @@
         return Object.defineProperty(o, "p", {
             get: (e = i().src.split("/").slice(0, -1).join("/") + "/", function() {
                 return e
             })
         }), "undefined" != typeof jsonpScriptSrc && (a = jsonpScriptSrc, jsonpScriptSrc = function(e) {
             var t, n = /\/_dash-component-suites\//.test(i().src),
                 e = a(e);
-            return n ? ((t = (n = e.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_0-a3m1686883076"), n.splice(-1, 1, t.join(".")), n.join("/")) : e
+            return n ? ((t = (n = e.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_0-a4m1688982631"), n.splice(-1, 1, t.join(".")), n.join("/")) : e
         }), o(o.s = 493)
     }([function(e, t) {
                 e.exports = window.PropTypes
             }, function(e, t) {
                 e.exports = window.React
             }, function(e, t, n) {
                 "use strict";
@@ -250,310 +250,14 @@
 
                 function u(e, t, n) {
                     if (n || 2 === arguments.length)
                         for (var r, o = 0, i = t.length; o < i; o++) !r && o in t || ((r = r || Array.prototype.slice.call(t, 0, o))[o] = t[o]);
                     return e.concat(r || Array.prototype.slice.call(t))
                 }
                 Object.create, Object.create
-            }, function(e, t, n) {
-                "use strict";
-                n.d(t, "a", function() {
-                    return l
-                }), n.d(t, "b", function() {
-                    return s
-                }), n.d(t, "c", function() {
-                    return b
-                }), n.d(t, "d", function() {
-                    return m
-                }), n.d(t, "e", function() {
-                    return a
-                }), n.d(t, "f", function() {
-                    return p
-                }), n.d(t, "g", function() {
-                    return c
-                }), n.d(t, "h", function() {
-                    return h
-                }), n.d(t, "i", function() {
-                    return f
-                }), n.d(t, "j", function() {
-                    return u
-                }), n.d(t, "k", function() {
-                    return d
-                });
-                var t = n(1),
-                    i = n.n(t);
-                const r = {
-                    a: {
-                        content: 9,
-                        self: !1,
-                        type: 105
-                    },
-                    address: {
-                        invalid: ["h1", "h2", "h3", "h4", "h5", "h6", "address", "article", "aside", "section", "div", "header", "footer"],
-                        self: !1
-                    },
-                    audio: {
-                        children: ["track", "source"]
-                    },
-                    br: {
-                        type: 9,
-                        void: !0
-                    },
-                    body: {
-                        content: 127
-                    },
-                    button: {
-                        content: 8,
-                        type: 105
-                    },
-                    caption: {
-                        content: 1,
-                        parent: ["table"]
-                    },
-                    col: {
-                        parent: ["colgroup"],
-                        void: !0
-                    },
-                    colgroup: {
-                        children: ["col"],
-                        parent: ["table"]
-                    },
-                    details: {
-                        children: ["summary"],
-                        type: 97
-                    },
-                    dd: {
-                        content: 1,
-                        parent: ["dl"]
-                    },
-                    dl: {
-                        children: ["dt", "dd"],
-                        type: 1
-                    },
-                    dt: {
-                        content: 1,
-                        invalid: ["footer", "header"],
-                        parent: ["dl"]
-                    },
-                    figcaption: {
-                        content: 1,
-                        parent: ["figure"]
-                    },
-                    footer: {
-                        invalid: ["footer", "header"]
-                    },
-                    header: {
-                        invalid: ["footer", "header"]
-                    },
-                    hr: {
-                        type: 1,
-                        void: !0
-                    },
-                    img: {
-                        void: !0
-                    },
-                    li: {
-                        content: 1,
-                        parent: ["ul", "ol", "menu"]
-                    },
-                    main: {
-                        self: !1
-                    },
-                    ol: {
-                        children: ["li"],
-                        type: 1
-                    },
-                    picture: {
-                        children: ["source", "img"],
-                        type: 25
-                    },
-                    rb: {
-                        parent: ["ruby", "rtc"]
-                    },
-                    rp: {
-                        parent: ["ruby", "rtc"]
-                    },
-                    rt: {
-                        content: 8,
-                        parent: ["ruby", "rtc"]
-                    },
-                    rtc: {
-                        content: 8,
-                        parent: ["ruby"]
-                    },
-                    ruby: {
-                        children: ["rb", "rp", "rt", "rtc"]
-                    },
-                    source: {
-                        parent: ["audio", "video", "picture"],
-                        void: !0
-                    },
-                    summary: {
-                        content: 8,
-                        parent: ["details"]
-                    },
-                    table: {
-                        children: ["caption", "colgroup", "thead", "tbody", "tfoot", "tr"],
-                        type: 1
-                    },
-                    tbody: {
-                        parent: ["table"],
-                        children: ["tr"]
-                    },
-                    td: {
-                        content: 1,
-                        parent: ["tr"]
-                    },
-                    tfoot: {
-                        parent: ["table"],
-                        children: ["tr"]
-                    },
-                    th: {
-                        content: 1,
-                        parent: ["tr"]
-                    },
-                    thead: {
-                        parent: ["table"],
-                        children: ["tr"]
-                    },
-                    tr: {
-                        parent: ["table", "tbody", "thead", "tfoot"],
-                        children: ["th", "td"]
-                    },
-                    track: {
-                        parent: ["audio", "video"],
-                        void: !0
-                    },
-                    ul: {
-                        children: ["li"],
-                        type: 1
-                    },
-                    video: {
-                        children: ["track", "source"]
-                    },
-                    wbr: {
-                        type: 9,
-                        void: !0
-                    }
-                };
-
-                function o(t) {
-                    return e => {
-                        r[e] = {
-                            ...t,
-                            ...r[e]
-                        }
-                    }
-                } ["address", "main", "div", "figure", "p", "pre"].forEach(o({
-                    content: 1,
-                    type: 65
-                })), ["abbr", "b", "bdi", "bdo", "cite", "code", "data", "dfn", "em", "i", "kbd", "mark", "q", "ruby", "samp", "strong", "sub", "sup", "time", "u", "var"].forEach(o({
-                    content: 8,
-                    type: 73
-                })), ["p", "pre"].forEach(o({
-                    content: 8,
-                    type: 65
-                })), ["s", "small", "span", "del", "ins"].forEach(o({
-                    content: 8,
-                    type: 9
-                })), ["article", "aside", "footer", "header", "nav", "section", "blockquote"].forEach(o({
-                    content: 1,
-                    type: 67
-                })), ["h1", "h2", "h3", "h4", "h5", "h6"].forEach(o({
-                    content: 8,
-                    type: 69
-                })), ["audio", "canvas", "iframe", "img", "video"].forEach(o({
-                    type: 89
-                }));
-                const a = Object.freeze(r),
-                    s = ["applet", "base", "body", "command", "embed", "frame", "frameset", "head", "html", "link", "meta", "noscript", "object", "script", "style", "title"],
-                    l = Object.keys(a).filter(e => "canvas" !== e && "iframe" !== e),
-                    c = 2,
-                    u = 3,
-                    f = 4,
-                    d = 5,
-                    p = Object.freeze({
-                        alt: 1,
-                        cite: 1,
-                        class: 1,
-                        colspan: u,
-                        controls: f,
-                        datetime: 1,
-                        default: f,
-                        disabled: f,
-                        dir: 1,
-                        height: 1,
-                        href: 1,
-                        id: 1,
-                        kind: 1,
-                        label: 1,
-                        lang: 1,
-                        loading: 1,
-                        loop: f,
-                        media: 1,
-                        muted: f,
-                        poster: 1,
-                        rel: 1,
-                        role: 1,
-                        rowspan: u,
-                        scope: 1,
-                        sizes: 1,
-                        span: u,
-                        start: u,
-                        style: d,
-                        src: 1,
-                        srclang: 1,
-                        srcset: 1,
-                        tabindex: 1,
-                        target: 1,
-                        title: 1,
-                        type: 1,
-                        width: 1
-                    }),
-                    h = Object.freeze({
-                        class: "className",
-                        colspan: "colSpan",
-                        datetime: "dateTime",
-                        rowspan: "rowSpan",
-                        srclang: "srcLang",
-                        srcset: "srcSet",
-                        tabindex: "tabIndex"
-                    });
-
-                function g() {
-                    return (g = Object.assign || function(e) {
-                        for (var t = 1; t < arguments.length; t++) {
-                            var n, r = arguments[t];
-                            for (n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
-                        }
-                        return e
-                    }).apply(this, arguments)
-                }
-
-                function b({
-                    attributes: e = {},
-                    className: t,
-                    children: n = null,
-                    selfClose: r = !1,
-                    tagName: o
-                }) {
-                    return r ? i.a.createElement(o, g({
-                        className: t
-                    }, e)) : i.a.createElement(o, g({
-                        className: t
-                    }, e), n)
-                }
-                class m {
-                    attribute(e, t) {
-                        return t
-                    }
-                    node(e, t) {
-                        return t
-                    }
-                }
             }, function(e, O, E) {
                 ! function(w, _) {
                     var x;
                     ! function() {
                         var Ai = "Expected a function",
                             Ri = "__lodash_placeholder__",
                             ca = [
@@ -618,16 +322,16 @@
                             Va = /\$\{([^\\}]*(?:\\.[^\\}]*)*)\}/g,
                             $a = /\w*$/,
                             qa = /^[-+]0x[0-9a-f]+$/i,
                             Ya = /^0b[01]+$/i,
                             Ka = /^\[object .+?Constructor\]$/,
                             Xa = /^0o[0-7]+$/i,
                             Ga = /^(?:0|[1-9]\d*)$/,
-                            Za = /[\xc0-\xd6\xd8-\xf6\xf8-\xff\u0100-\u017f]/g,
-                            Ja = /($^)/,
+                            Ja = /[\xc0-\xd6\xd8-\xf6\xf8-\xff\u0100-\u017f]/g,
+                            Za = /($^)/,
                             Qa = /['\n\r\u2028\u2029\\]/g,
                             s = "\\u0300-\\u036f\\ufe20-\\ufe2f\\u20d0-\\u20ff",
                             e = "\\xac\\xb1\\xd7\\xf7\\x00-\\x2f\\x3a-\\x40\\x5b-\\x60\\x7b-\\xbf\\u2000-\\u206f \\t\\x0b\\f\\xa0\\ufeff\\n\\r\\u2028\\u2029\\u1680\\u180e\\u2000\\u2001\\u2002\\u2003\\u2004\\u2005\\u2006\\u2007\\u2008\\u2009\\u200a\\u202f\\u205f\\u3000",
                             l = "[" + e + "]",
                             t = "[" + s + "]",
                             c = "[a-z\\xdf-\\xf6\\xf8-\\xff]",
                             e = "[^\\ud800-\\udfff" + e + "\\d+\\u2700-\\u27bfa-z\\xdf-\\xf6\\xf8-\\xffA-Z\\xc0-\\xd6\\xd8-\\xde]",
@@ -676,15 +380,15 @@
                             cs = n && n.isArrayBuffer,
                             us = n && n.isDate,
                             fs = n && n.isMap,
                             ds = n && n.isRegExp,
                             ps = n && n.isSet,
                             hs = n && n.isTypedArray;
 
-                        function Zi(e, t, n) {
+                        function Ji(e, t, n) {
                             switch (n.length) {
                                 case 0:
                                     return e.call(t);
                                 case 1:
                                     return e.call(t, n[0]);
                                 case 2:
                                     return e.call(t, n[0], n[1]);
@@ -698,15 +402,15 @@
                             for (var o = -1, i = null == e ? 0 : e.length; ++o < i;) {
                                 var a = e[o];
                                 t(r, a, n(a), e)
                             }
                             return r
                         }
 
-                        function Ji(e, t) {
+                        function Zi(e, t) {
                             for (var n = -1, r = null == e ? 0 : e.length; ++n < r && !1 !== t(e[n], n, e););
                             return e
                         }
 
                         function bs(e, t) {
                             for (var n = -1, r = null == e ? 0 : e.length; ++n < r;)
                                 if (!t(e[n], n, e)) return !1;
@@ -1131,16 +835,16 @@
                                     $ = m.prototype,
                                     q = e["__core-js_shared__"],
                                     Y = V.toString,
                                     k = $.hasOwnProperty,
                                     K = 0,
                                     X = (V = /[^.]+$/.exec(q && q.keys && q.keys.IE_PROTO || "")) ? "Symbol(src)_1." + V : "",
                                     G = $.toString,
-                                    Z = Y.call(m),
-                                    J = Gi._,
+                                    J = Y.call(m),
+                                    Z = Gi._,
                                     Q = F("^" + Y.call(k).replace(Da, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
                                     V = ls ? e.Buffer : void 0,
                                     t = e.Symbol,
                                     ee = e.Uint8Array,
                                     te = V ? V.allocUnsafe : void 0,
                                     ne = Us(m.getPrototypeOf, m),
                                     re = m.create,
@@ -1300,20 +1004,20 @@
                                         configurable: !0,
                                         enumerable: !0,
                                         value: n,
                                         writable: !0
                                     }) : e[t] = n
                                 }
 
-                                function Ze(e, t) {
+                                function Je(e, t) {
                                     for (var n = -1, r = t.length, o = P(r), i = null == e; ++n < r;) o[n] = i ? void 0 : Lo(e, t[n]);
                                     return o
                                 }
 
-                                function Je(e, t, n) {
+                                function Ze(e, t, n) {
                                     return e = e == e && (void 0 !== n && (e = e <= n ? e : n), void 0 !== t) ? t <= e ? e : t : e
                                 }
 
                                 function v(n, r, o, e, t, i) {
                                     var a, s = 1 & r,
                                         l = 2 & r,
                                         c = 4 & r;
@@ -1369,15 +1073,15 @@
                                         if (g) return g;
                                         i.set(n, a), _o(n) ? n.forEach(function(e) {
                                             a.add(v(e, r, o, e, n, i))
                                         }) : mo(n) && n.forEach(function(e, t) {
                                             a.set(t, v(e, r, o, t, n, i))
                                         });
                                         var b = e ? void 0 : (c ? l ? Nn : Ln : l ? S : E)(n);
-                                        Ji(b || n, function(e, t) {
+                                        Zi(b || n, function(e, t) {
                                             b && (e = n[t = e]), qe(a, t, v(e, r, o, t, n, i))
                                         })
                                     }
                                     return a
                                 }
 
                                 function Qe(e, t, n) {
@@ -1611,15 +1315,15 @@
                                         }
                                     }
                                     return c
                                 }
 
                                 function vt(e, t, n) {
                                     t = null == (e = or(e, t = Qt(t, e))) ? e : e[hr(r(t))];
-                                    return null == t ? void 0 : Zi(t, e, n)
+                                    return null == t ? void 0 : Ji(t, e, n)
                                 }
 
                                 function yt(e) {
                                     return i(e) && n(e) == Di
                                 }
 
                                 function wt(e, t, n, r, o) {
@@ -1757,15 +1461,15 @@
                                     var n = Hn(t);
                                     return 1 == n.length && n[0][2] ? nr(n[0][0], n[0][1]) : function(e) {
                                         return e === t || _t(e, t, n)
                                     }
                                 }
 
                                 function Ct(n, r) {
-                                    return Zn(n) && tr(r) ? nr(hr(n), r) : function(e) {
+                                    return Jn(n) && tr(r) ? nr(hr(n), r) : function(e) {
                                         var t = Lo(e, n);
                                         return void 0 === t && t === r ? No(e, n) : wt(r, t, 3)
                                     }
                                 }
 
                                 function zt(g, b, m, v, y) {
                                     g !== b && st(b, function(e, t) {
@@ -1996,24 +1700,24 @@
                                     for (var r = -1, o = e.length, i = t.length, a = {}; ++r < o;) {
                                         var s = r < i ? t[r] : void 0;
                                         n(a, e[r], s)
                                     }
                                     return a
                                 }
 
-                                function Zt(e) {
+                                function Jt(e) {
                                     return w(e) ? e : []
                                 }
 
-                                function Jt(e) {
+                                function Zt(e) {
                                     return "function" == typeof e ? e : j
                                 }
 
                                 function Qt(e, t) {
-                                    return D(e) ? e : Zn(e, t) ? [e] : pr(p(e))
+                                    return D(e) ? e : Jn(e, t) ? [e] : pr(p(e))
                                 }
                                 var en = a;
 
                                 function tn(e, t, n) {
                                     var r = e.length;
                                     return n = void 0 === n ? r : n, !t && r <= n ? e : s(e, t, n)
                                 }
@@ -2134,15 +1838,15 @@
                                             t = t ? tn(t, 1).join("") : e.slice(1);
                                         return n[r]() + t
                                     }
                                 }
 
                                 function bn(t) {
                                     return function(e) {
-                                        return ys(ai(Jo(e).replace(es, "")), t, "")
+                                        return ys(ai(Zo(e).replace(es, "")), t, "")
                                     }
                                 }
 
                                 function mn(r) {
                                     return function() {
                                         var e = arguments;
                                         switch (e.length) {
@@ -2187,15 +1891,15 @@
                                         for (l && o.reverse(); e--;) {
                                             var n = o[e];
                                             if ("function" != typeof n) throw new T(Ai);
                                             t && !s && "wrapper" == Bn(n) && (s = new g([], !0))
                                         }
                                         for (e = s ? e : i; ++e < i;) var r = Bn(n = o[e]),
                                             a = "wrapper" == r ? Un(n) : void 0,
-                                            s = a && Jn(a[0]) && 424 == a[1] && !a[4].length && 1 == a[9] ? s[Bn(a[0])].apply(s, a[3]) : 1 == n.length && Jn(n) ? s[r]() : s.thru(n);
+                                            s = a && Zn(a[0]) && 424 == a[1] && !a[4].length && 1 == a[9] ? s[Bn(a[0])].apply(s, a[3]) : 1 == n.length && Zn(n) ? s[r]() : s.thru(n);
                                         return function() {
                                             var e = arguments,
                                                 t = e[0];
                                             if (s && 1 == e.length && D(t)) return s.plant(t).value();
                                             for (var n = 0, r = i ? o[n].apply(this, e) : t; ++n < i;) r = o[n].call(this, r);
                                             return r
                                         }
@@ -2246,15 +1950,15 @@
                                 }
 
                                 function On(r) {
                                     return In(function(e) {
                                         return e = ea(e, ra(u())), a(function(t) {
                                             var n = this;
                                             return r(e, function(e) {
-                                                return Zi(e, n, t)
+                                                return Ji(e, n, t)
                                             })
                                         })
                                     })
                                 }
 
                                 function En(e, t) {
                                     var n = (t = void 0 === t ? " " : c(t)).length;
@@ -2275,15 +1979,15 @@
                                     }
                                 }
 
                                 function kn(e, t, n, r, o, i, a, s, l, c) {
                                     var u = 8 & t,
                                         o = (4 & (t = (t | (u ? 32 : 64)) & ~(u ? 64 : 32)) || (t &= -4), [e, t, o, u ? i : void 0, u ? a : void 0, u ? void 0 : i, u ? void 0 : a, s, l, c]),
                                         i = n.apply(void 0, o);
-                                    return Jn(e) && ar(i, o), i.placeholder = r, cr(i, e, t)
+                                    return Zn(e) && ar(i, o), i.placeholder = r, cr(i, e, t)
                                 }
 
                                 function Cn(e) {
                                     var r = B[e];
                                     return function(e, t) {
                                         var n;
                                         return e = O(e), (t = null == t ? 0 : A(I(t), 292)) && be(e) ? (n = (p(e) + "e").split("e"), +((n = (p(r(n[0] + "e" + (+n[1] + t))) + "e").split("e"))[0] + "e" + (+n[1] - t))) : r(e)
@@ -2305,19 +2009,19 @@
                                 }
 
                                 function Tn(e, t, n, r, o, i, a, s) {
                                     var l, c, u, f, d, p, h, g, b, m, v, y, w, _, x, O, E, S, j, k, C, z = 2 & t;
                                     if (z || "function" == typeof e) return (l = r ? r.length : 0) || (t &= -97, r = o = void 0), a = void 0 === a ? a : M(I(a), 0), s = void 0 === s ? s : I(s), l -= o ? o.length : 0, 64 & t && (u = r, E = o, r = o = void 0), c = z ? void 0 : Un(e), u = [e, t, n, r, o, u, E, i, a, s], c && (E = c, a = (i = u)[1], j = E[1], k = a | j, C = 128 == j && 8 == a || 128 == j && 256 == a && i[7].length <= E[8] || 384 == j && E[7].length <= E[8] && 8 == a, k < 131 || C) && (1 & j && (i[2] = E[2], k |= 1 & a ? 0 : 4), (C = E[3]) && (S = i[3], i[3] = S ? ln(S, C, E[4]) : C, i[4] = S ? aa(i[3], Ri) : E[4]), (C = E[5]) && (S = i[5], i[5] = S ? cn(S, C, E[6]) : C, i[6] = S ? aa(i[5], Ri) : E[6]), (C = E[7]) && (i[7] = C), 128 & j && (i[8] = null == i[8] ? E[8] : A(i[8], E[8])), null == i[9] && (i[9] = E[9]), i[0] = E[0], i[1] = k), e = u[0], t = u[1], n = u[2], r = u[3], o = u[4], !(s = u[9] = void 0 === u[9] ? z ? 0 : e.length : M(u[9] - l, 0)) && 24 & t && (t &= -25), a = t && 1 != t ? 8 == t || 16 == t ? (_ = t, x = s, O = mn(w = e), function e() {
                                         for (var t = arguments.length, n = P(t), r = t, o = Fn(e); r--;) n[r] = arguments[r];
                                         o = t < 3 && n[0] !== o && n[t - 1] !== o ? [] : aa(n, o);
-                                        return (t -= o.length) < x ? kn(w, _, wn, e.placeholder, void 0, n, o, void 0, void 0, x - t) : Zi(this && this !== Gi && this instanceof e ? O : w, this, n)
+                                        return (t -= o.length) < x ? kn(w, _, wn, e.placeholder, void 0, n, o, void 0, void 0, x - t) : Ji(this && this !== Gi && this instanceof e ? O : w, this, n)
                                     }) : 32 != t && 33 != t || o.length ? wn.apply(void 0, u) : (b = n, m = r, v = 1 & t, y = mn(g = e), function e() {
                                         for (var t = -1, n = arguments.length, r = -1, o = m.length, i = P(o + n), a = this && this !== Gi && this instanceof e ? y : g; ++r < o;) i[r] = m[r];
                                         for (; n--;) i[r++] = arguments[++t];
-                                        return Zi(a, v ? b : this, i)
+                                        return Ji(a, v ? b : this, i)
                                     }) : (d = n, p = 1 & t, h = mn(f = e), function e() {
                                         return (this && this !== Gi && this instanceof e ? h : f).apply(p ? d : this, arguments)
                                     }), cr((c ? Nt : ar)(a, u), e, t);
                                     throw new T(Ai)
                                 }
 
                                 function Mn(e, t, n, r) {
@@ -2451,20 +2155,20 @@
                                 }
 
                                 function f(e, t, n) {
                                     var r;
                                     return !!_(n) && !!("number" == (r = typeof t) ? d(n) && Gn(t, n.length) : "string" == r && t in n) && R(n[t], e)
                                 }
 
-                                function Zn(e, t) {
+                                function Jn(e, t) {
                                     var n;
                                     if (!D(e)) return "number" == (n = typeof e) || "symbol" == n || "boolean" == n || null == e || y(e) || Aa.test(e) || !Ma.test(e) || null != t && e in m(t)
                                 }
 
-                                function Jn(e) {
+                                function Zn(e) {
                                     var t = Bn(e),
                                         n = h[t];
                                     return "function" == typeof n && t in b.prototype && (e === n || (t = Un(n)) && e === t[0])
                                 }(L && z(new L(new ArrayBuffer(1))) != Yi || Oe && z(new Oe) != Ui || Ee && "[object Promise]" != z(Ee.resolve()) || Se && z(new Se) != Hi || e && z(new e) != $i) && (z = function(e) {
                                     var t = n(e),
                                         e = t == Fi ? e.constructor : void 0,
                                         e = e ? gr(e) : "";
@@ -2500,15 +2204,15 @@
                                 }
 
                                 function rr(i, a, s) {
                                     return a = M(void 0 === a ? i.length - 1 : a, 0),
                                         function() {
                                             for (var e = arguments, t = -1, n = M(e.length - a, 0), r = P(n); ++t < n;) r[t] = e[a + t];
                                             for (var t = -1, o = P(a + 1); ++t < a;) o[t] = e[t];
-                                            return o[a] = s(r), Zi(i, this, o)
+                                            return o[a] = s(r), Ji(i, this, o)
                                         }
                                 }
 
                                 function or(e, t) {
                                     return t.length < 2 ? e : dt(e, s(t, 0, -1))
                                 }
 
@@ -2519,15 +2223,15 @@
                                     sr = de || function(e, t) {
                                         return Gi.setTimeout(e, t)
                                     },
                                     lr = ur(t);
 
                                 function cr(e, t, n) {
                                     var r, o, i, t = t + "";
-                                    return lr(e, (t = (e = t).match(Ua), o = t ? t[1].split(Ba) : [], i = n, Ji(ca, function(e) {
+                                    return lr(e, (t = (e = t).match(Ua), o = t ? t[1].split(Ba) : [], i = n, Zi(ca, function(e) {
                                         var t = "_." + e[0];
                                         i & e[1] && !ms(o, t) && o.push(t)
                                     }), t = o.sort(), (n = t.length) ? (t[r = n - 1] = (1 < n ? "& " : "") + t[r], t = t.join(2 < n ? ", " : " "), e.replace(Na, "{\n/* [wrapped with " + t + "] */\n")) : e))
                                 }
 
                                 function ur(n) {
                                     var r = 0,
@@ -2608,38 +2312,38 @@
                                     return null != e && e.length ? l(e, 1) : []
                                 }
 
                                 function wr(e) {
                                     return e && e.length ? e[0] : void 0
                                 }
                                 q = a(function(e) {
-                                    var t = ea(e, Zt);
+                                    var t = ea(e, Jt);
                                     return t.length && t[0] === e[0] ? mt(t) : []
                                 }), de = a(function(e) {
                                     var t = r(e),
-                                        n = ea(e, Zt);
+                                        n = ea(e, Jt);
                                     return t === r(n) ? t = void 0 : n.pop(), n.length && n[0] === e[0] ? mt(n, u(t, 2)) : []
                                 }), t = a(function(e) {
                                     var t = r(e),
-                                        n = ea(e, Zt);
+                                        n = ea(e, Jt);
                                     return (t = "function" == typeof t ? t : void 0) && n.pop(), n.length && n[0] === e[0] ? mt(n, void 0, t) : []
                                 });
 
                                 function r(e) {
                                     var t = null == e ? 0 : e.length;
                                     return t ? e[t - 1] : void 0
                                 }
                                 ue = a(_r);
 
                                 function _r(e, t) {
                                     return e && e.length && t && t.length ? At(e, t) : e
                                 }
                                 var xr = In(function(e, t) {
                                     var n = null == e ? 0 : e.length,
-                                        r = Ze(e, t);
+                                        r = Je(e, t);
                                     return Rt(e, ea(t, function(e) {
                                         return Gn(e, n) ? +e : e
                                     }).sort(sn)), r
                                 });
 
                                 function Or(e) {
                                     return null == e ? e : xe.call(e)
@@ -2663,15 +2367,15 @@
                                     }), Ps(n, function(e) {
                                         return ea(t, ks(e))
                                     })) : []
                                 }
 
                                 function Cr(e, t) {
                                     return e && e.length ? (e = kr(e), null == t ? e : ea(e, function(e) {
-                                        return Zi(t, void 0, e)
+                                        return Ji(t, void 0, e)
                                     })) : []
                                 }
                                 var zr = a(function(e, t) {
                                         return w(e) ? tt(e, t) : []
                                     }),
                                     Pr = a(function(e) {
                                         return Xt(Qi(e, w))
@@ -2697,15 +2401,15 @@
                                 }
 
                                 function Ir(e, t) {
                                     return t(e)
                                 }
                                 var Lr = In(function(t) {
                                         function e(e) {
-                                            return Ze(e, t)
+                                            return Je(e, t)
                                         }
                                         var n = t.length,
                                             r = n ? t[0] : 0,
                                             o = this.__wrapped__;
                                         return !(1 < n || this.__actions__.length) && o instanceof b && Gn(r) ? ((o = o.slice(r, +r + (n ? 1 : 0))).__actions__.push({
                                             func: Ir,
                                             args: [e],
@@ -2717,15 +2421,15 @@
                                     Nr = fn(function(e, t, n) {
                                         k.call(e, n) ? ++e[n] : Ge(e, n, 1)
                                     }),
                                     Ur = vn(mr),
                                     Br = vn(vr);
 
                                 function Fr(e, t) {
-                                    return (D(e) ? Ji : nt)(e, u(t, 3))
+                                    return (D(e) ? Zi : nt)(e, u(t, 3))
                                 }
 
                                 function Wr(e, t) {
                                     return (D(e) ? function(e, t) {
                                         for (var n = null == e ? 0 : e.length; n-- && !1 !== t(e[n], n, e););
                                         return e
                                     } : rt)(e, u(t, 3))
@@ -2734,15 +2438,15 @@
                                         k.call(e, n) ? e[n].push(t) : Ge(e, n, [t])
                                     }),
                                     Vr = a(function(e, t, n) {
                                         var r = -1,
                                             o = "function" == typeof t,
                                             i = d(e) ? P(e.length) : [];
                                         return nt(e, function(e) {
-                                            i[++r] = o ? Zi(t, e, n) : vt(e, t, n)
+                                            i[++r] = o ? Ji(t, e, n) : vt(e, t, n)
                                         }), i
                                     }),
                                     $r = fn(function(e, t, n) {
                                         Ge(e, n, t)
                                     });
 
                                 function qr(e, t) {
@@ -2764,25 +2468,25 @@
                                         return Gi.Date.now()
                                     };
 
                                 function Gr(e, t, n) {
                                     return t = n ? void 0 : t, Tn(e, 128, void 0, void 0, void 0, void 0, t = e && null == t ? e.length : t)
                                 }
 
-                                function Zr(e, t) {
+                                function Jr(e, t) {
                                     var n;
                                     if ("function" != typeof t) throw new T(Ai);
                                     return e = I(e),
                                         function() {
                                             return 0 < --e && (n = t.apply(this, arguments)), e <= 1 && (t = void 0), n
                                         }
                                 }
-                                var Jr = a(function(e, t, n) {
+                                var Zr = a(function(e, t, n) {
                                         var r, o = 1;
-                                        return n.length && (r = aa(n, Fn(Jr)), o |= 32), Tn(e, o, t, n, r)
+                                        return n.length && (r = aa(n, Fn(Zr)), o |= 32), Tn(e, o, t, n, r)
                                     }),
                                     Qr = a(function(e, t, n) {
                                         var r, o = 3;
                                         return n.length && (r = aa(n, Fn(Qr)), o |= 32), Tn(t, o, e, n, r)
                                     });
 
                                 function eo(r, n, e) {
@@ -2865,15 +2569,15 @@
                                     }
                                 }
                                 no.Cache = Fe;
                                 var en = en(function(r, o) {
                                         var i = (o = 1 == o.length && D(o[0]) ? ea(o[0], ra(u())) : ea(l(o, 1), ra(u()))).length;
                                         return a(function(e) {
                                             for (var t = -1, n = A(e.length, i); ++t < n;) e[t] = o[t].call(this, e[t]);
-                                            return Zi(r, this, e)
+                                            return Ji(r, this, e)
                                         })
                                     }),
                                     oo = a(function(e, t) {
                                         return Tn(e, 32, void 0, t, aa(t, Fn(oo)))
                                     }),
                                     io = a(function(e, t) {
                                         return Tn(e, 64, void 0, t, aa(t, Fn(io)))
@@ -2941,15 +2645,15 @@
                                 };
 
                                 function vo(e) {
                                     return "number" == typeof e || i(e) && n(e) == Bi
                                 }
 
                                 function yo(e) {
-                                    return !(!i(e) || n(e) != Fi) && (null === (e = ne(e)) || "function" == typeof(e = k.call(e, "constructor") && e.constructor) && e instanceof e && Y.call(e) == Z)
+                                    return !(!i(e) || n(e) != Fi) && (null === (e = ne(e)) || "function" == typeof(e = k.call(e, "constructor") && e.constructor) && e instanceof e && Y.call(e) == J)
                                 }
                                 var wo = ds ? ra(ds) : function(e) {
                                         return i(e) && n(e) == Wi
                                     },
                                     _o = ps ? ra(ps) : function(e) {
                                         return i(e) && z(e) == Hi
                                     };
@@ -2987,15 +2691,15 @@
                                 function I(e) {
                                     var e = ko(e),
                                         t = e % 1;
                                     return e == e ? t ? e - t : e : 0
                                 }
 
                                 function Co(e) {
-                                    return e ? Je(I(e), 0, 4294967295) : 0
+                                    return e ? Ze(I(e), 0, 4294967295) : 0
                                 }
 
                                 function O(e) {
                                     if ("number" == typeof e) return e;
                                     if (y(e)) return NaN;
                                     if ("string" != typeof(e = _(e) ? _(t = "function" == typeof e.valueOf ? e.valueOf() : e) ? t + "" : t : e)) return 0 === e ? e : +e;
                                     e = Ts(e);
@@ -3020,30 +2724,30 @@
                                     }),
                                     Mo = dn(function(e, t, n, r) {
                                         un(t, S(t), e, r)
                                     }),
                                     Ao = dn(function(e, t, n, r) {
                                         un(t, E(t), e, r)
                                     }),
-                                    Ro = In(Ze),
+                                    Ro = In(Je),
                                     Do = a(function(e, t) {
                                         e = m(e);
                                         var n = -1,
                                             r = t.length,
                                             o = 2 < r ? t[2] : void 0;
                                         for (o && f(t[0], t[1], o) && (r = 1); ++n < r;)
                                             for (var i = t[n], a = S(i), s = -1, l = a.length; ++s < l;) {
                                                 var c = a[s],
                                                     u = e[c];
                                                 (void 0 === u || R(u, $[c]) && !k.call(e, c)) && (e[c] = i[c])
                                             }
                                         return e
                                     }),
                                     Io = a(function(e) {
-                                        return e.push(void 0, An), Zi(Ho, void 0, e)
+                                        return e.push(void 0, An), Ji(Ho, void 0, e)
                                     });
 
                                 function Lo(e, t, n) {
                                     e = null == e ? void 0 : dt(e, t);
                                     return void 0 === e ? n : e
                                 }
 
@@ -3111,23 +2815,23 @@
                                 var Yo = Pn(E),
                                     Ko = Pn(S);
 
                                 function Xo(e) {
                                     return null == e ? [] : Ms(e, E(e))
                                 }
                                 var Go = bn(function(e, t, n) {
-                                    return t = t.toLowerCase(), e + (n ? Zo(t) : t)
+                                    return t = t.toLowerCase(), e + (n ? Jo(t) : t)
                                 });
 
-                                function Zo(e) {
+                                function Jo(e) {
                                     return ii(p(e).toLowerCase())
                                 }
 
-                                function Jo(e) {
-                                    return (e = p(e)) && e.replace(Za, Ds).replace(ts, "")
+                                function Zo(e) {
+                                    return (e = p(e)) && e.replace(Ja, Ds).replace(ts, "")
                                 }
                                 var Qo = bn(function(e, t, n) {
                                         return e + (n ? "-" : "") + t.toLowerCase()
                                     }),
                                     ei = bn(function(e, t, n) {
                                         return e + (n ? " " : "") + t.toLowerCase()
                                     }),
@@ -3144,22 +2848,22 @@
                                     ii = gn("toUpperCase");
 
                                 function ai(e, t, n) {
                                     return e = p(e), void 0 === (t = n ? void 0 : t) ? (n = e, rs.test(n) ? e.match(ns) || [] : e.match(Fa) || []) : e.match(t) || []
                                 }
                                 var si = a(function(e, t) {
                                         try {
-                                            return Zi(e, void 0, t)
+                                            return Ji(e, void 0, t)
                                         } catch (e) {
                                             return po(e) ? e : new N(e)
                                         }
                                     }),
                                     li = In(function(t, e) {
-                                        return Ji(e, function(e) {
-                                            e = hr(e), Ge(t, e, Jr(t[e], t))
+                                        return Zi(e, function(e) {
+                                            e = hr(e), Ge(t, e, Zr(t[e], t))
                                         }), t
                                     });
 
                                 function ci(e) {
                                     return function() {
                                         return e
                                     }
@@ -3186,15 +2890,15 @@
                                     });
 
                                 function gi(r, t, e) {
                                     var n = E(t),
                                         o = ft(t, n),
                                         i = (null != e || _(t) && (o.length || !n.length) || (e = t, t = r, r = this, o = ft(t, E(t))), !(_(e) && "chain" in e && !e.chain)),
                                         a = ho(r);
-                                    return Ji(o, function(e) {
+                                    return Zi(o, function(e) {
                                         var n = t[e];
                                         r[e] = n, a && (r.prototype[e] = function() {
                                             var e, t = this.__chain__;
                                             return i || t ? (((e = r(this.__wrapped__)).__actions__ = x(this.__actions__)).push({
                                                 func: n,
                                                 args: arguments,
                                                 thisArg: r
@@ -3205,15 +2909,15 @@
 
                                 function bi() {}
                                 var mi = On(ea),
                                     vi = On(bs),
                                     yi = On(_s);
 
                                 function wi(e) {
-                                    return Zn(e) ? ks(hr(e)) : (t = e, function(e) {
+                                    return Jn(e) ? ks(hr(e)) : (t = e, function(e) {
                                         return dt(e, t)
                                     });
                                     var t
                                 }
                                 var _i = Sn(),
                                     xi = Sn(!0);
 
@@ -3241,15 +2945,15 @@
                                     }, 0);
                                 return h.after = function(e, t) {
                                     if ("function" != typeof t) throw new T(Ai);
                                     return e = I(e),
                                         function() {
                                             if (--e < 1) return t.apply(this, arguments)
                                         }
-                                }, h.ary = Gr, h.assign = Po, h.assignIn = To, h.assignInWith = Mo, h.assignWith = Ao, h.at = Ro, h.before = Zr, h.bind = Jr, h.bindAll = li, h.bindKey = Qr, h.castArray = function() {
+                                }, h.ary = Gr, h.assign = Po, h.assignIn = To, h.assignInWith = Mo, h.assignWith = Ao, h.at = Ro, h.before = Jr, h.bind = Zr, h.bindAll = li, h.bindKey = Qr, h.castArray = function() {
                                     var e;
                                     return arguments.length ? D(e = arguments[0]) ? e : [e] : []
                                 }, h.chain = Dr, h.chunk = function(e, t, n) {
                                     t = (n ? f(e, t, n) : void 0 === t) ? 1 : M(I(t), 0);
                                     var r = null == e ? 0 : e.length;
                                     if (!r || t < 1) return [];
                                     for (var o = 0, i = 0, a = P(pe(r / t)); o < r;) a[i++] = s(e, o, o += t);
@@ -3270,15 +2974,15 @@
                                         t = u();
                                     return r = o ? ea(r, function(e) {
                                         if ("function" != typeof e[1]) throw new T(Ai);
                                         return [t(e[0]), e[1]]
                                     }) : [], a(function(e) {
                                         for (var t = -1; ++t < o;) {
                                             var n = r[t];
-                                            if (Zi(n[0], this, e)) return Zi(n[1], this, e)
+                                            if (Ji(n[0], this, e)) return Ji(n[1], this, e)
                                         }
                                     })
                                 }, h.conforms = function(e) {
                                     return t = v(e, 1), n = E(t),
                                         function(e) {
                                             return Qe(e, t, n)
                                         };
@@ -3358,15 +3062,15 @@
                                 }, h.memoize = no, h.merge = Wo, h.mergeWith = Ho, h.method = pi, h.methodOf = hi, h.mixin = gi, h.negate = ro, h.nthArg = function(t) {
                                     return t = I(t), a(function(e) {
                                         return Pt(e, t)
                                     })
                                 }, h.omit = Vo, h.omitBy = function(e, t) {
                                     return qo(e, ro(u(t)))
                                 }, h.once = function(e) {
-                                    return Zr(2, e)
+                                    return Jr(2, e)
                                 }, h.orderBy = function(e, t, n, r) {
                                     return null == e ? [] : Tt(e, t = D(t) ? t : null == t ? [] : [t], n = D(n = r ? void 0 : n) ? n : null == n ? [] : [n])
                                 }, h.over = mi, h.overArgs = en, h.overEvery = vi, h.overSome = yi, h.partial = oo, h.partialRight = io, h.partition = Yr, h.pick = $o, h.pickBy = qo, h.property = wi, h.propertyOf = function(t) {
                                     return function(e) {
                                         return null == t ? void 0 : dt(t, e)
                                     }
                                 }, h.pull = ue, h.pullAll = _r, h.pullAllBy = function(e, t, n) {
@@ -3389,17 +3093,17 @@
                                     }
                                     return n
                                 }, h.rest = function(e, t) {
                                     if ("function" != typeof e) throw new T(Ai);
                                     return a(e, t = void 0 === t ? t : I(t))
                                 }, h.reverse = Or, h.sampleSize = function(e, t, n) {
                                     return t = (n ? f(e, t, n) : void 0 === t) ? 1 : I(t), (D(e) ? function(e, t) {
-                                        return fr(x(e), Je(t, 0, e.length))
+                                        return fr(x(e), Ze(t, 0, e.length))
                                     } : function(e, t) {
-                                        return fr(e = Xo(e), Je(t, 0, e.length))
+                                        return fr(e = Xo(e), Ze(t, 0, e.length))
                                     })(e, t)
                                 }, h.set = function(e, t, n) {
                                     return null == e ? e : Lt(e, t, n)
                                 }, h.setWith = function(e, t, n, r) {
                                     return r = "function" == typeof r ? r : void 0, null == e ? e : Lt(e, t, n, r)
                                 }, h.shuffle = function(e) {
                                     return (D(e) ? function(e) {
@@ -3417,15 +3121,15 @@
                                 }, h.split = function(e, t, n) {
                                     return n && "number" != typeof n && f(e, t, n) && (t = n = void 0), (n = void 0 === n ? 4294967295 : n >>> 0) ? (e = p(e)) && ("string" == typeof t || null != t && !wo(t)) && !(t = c(t)) && ia(e) ? tn(la(e), 0, n) : e.split(t, n) : []
                                 }, h.spread = function(n, r) {
                                     if ("function" != typeof n) throw new T(Ai);
                                     return r = null == r ? 0 : M(I(r), 0), a(function(e) {
                                         var t = e[r],
                                             e = tn(e, 0, r);
-                                        return t && ta(e, t), Zi(n, this, e)
+                                        return t && ta(e, t), Ji(n, this, e)
                                     })
                                 }, h.tail = function(e) {
                                     var t = null == e ? 0 : e.length;
                                     return t ? s(e, 1, t) : []
                                 }, h.take = function(e, t, n) {
                                     return e && e.length ? s(e, 0, (t = n || void 0 === t ? 1 : I(t)) < 0 ? 0 : t) : []
                                 }, h.takeRight = function(e, t, n) {
@@ -3447,57 +3151,57 @@
                                         trailing: o
                                     })
                                 }, h.thru = Ir, h.toArray = jo, h.toPairs = Yo, h.toPairsIn = Ko, h.toPath = function(e) {
                                     return D(e) ? ea(e, hr) : y(e) ? [e] : x(pr(p(e)))
                                 }, h.toPlainObject = zo, h.transform = function(e, r, o) {
                                     var t, n = D(e),
                                         i = n || fo(e) || Oo(e);
-                                    return r = u(r, 4), null == o && (t = e && e.constructor, o = i ? n ? new t : [] : _(e) && ho(t) ? Ie(ne(e)) : {}), (i ? Ji : ct)(e, function(e, t, n) {
+                                    return r = u(r, 4), null == o && (t = e && e.constructor, o = i ? n ? new t : [] : _(e) && ho(t) ? Ie(ne(e)) : {}), (i ? Zi : ct)(e, function(e, t, n) {
                                         return r(o, e, t, n)
                                     }), o
                                 }, h.unary = function(e) {
                                     return Gr(e, 1)
                                 }, h.union = Er, h.unionBy = Sr, h.unionWith = jr, h.uniq = function(e) {
                                     return e && e.length ? Vt(e) : []
                                 }, h.uniqBy = function(e, t) {
                                     return e && e.length ? Vt(e, u(t, 2)) : []
                                 }, h.uniqWith = function(e, t) {
                                     return t = "function" == typeof t ? t : void 0, e && e.length ? Vt(e, void 0, t) : []
                                 }, h.unset = function(e, t) {
                                     return null == e || $t(e, t)
                                 }, h.unzip = kr, h.unzipWith = Cr, h.update = function(e, t, n) {
-                                    return null == e ? e : qt(e, t, Jt(n))
+                                    return null == e ? e : qt(e, t, Zt(n))
                                 }, h.updateWith = function(e, t, n, r) {
-                                    return r = "function" == typeof r ? r : void 0, null == e ? e : qt(e, t, Jt(n), r)
+                                    return r = "function" == typeof r ? r : void 0, null == e ? e : qt(e, t, Zt(n), r)
                                 }, h.values = Xo, h.valuesIn = function(e) {
                                     return null == e ? [] : Ms(e, S(e))
                                 }, h.without = zr, h.words = ai, h.wrap = function(e, t) {
-                                    return oo(Jt(t), e)
+                                    return oo(Zt(t), e)
                                 }, h.xor = Pr, h.xorBy = Tr, h.xorWith = Mr, h.zip = Ar, h.zipObject = function(e, t) {
                                     return Gt(e || [], t || [], qe)
                                 }, h.zipObjectDeep = function(e, t) {
                                     return Gt(e || [], t || [], Lt)
-                                }, h.zipWith = Rr, h.entries = Yo, h.entriesIn = Ko, h.extend = To, h.extendWith = Mo, gi(h, h), h.add = ji, h.attempt = si, h.camelCase = Go, h.capitalize = Zo, h.ceil = ki, h.clamp = function(e, t, n) {
-                                    return void 0 === n && (n = t, t = void 0), void 0 !== n && (n = (n = O(n)) == n ? n : 0), void 0 !== t && (t = (t = O(t)) == t ? t : 0), Je(O(e), t, n)
+                                }, h.zipWith = Rr, h.entries = Yo, h.entriesIn = Ko, h.extend = To, h.extendWith = Mo, gi(h, h), h.add = ji, h.attempt = si, h.camelCase = Go, h.capitalize = Jo, h.ceil = ki, h.clamp = function(e, t, n) {
+                                    return void 0 === n && (n = t, t = void 0), void 0 !== n && (n = (n = O(n)) == n ? n : 0), void 0 !== t && (t = (t = O(t)) == t ? t : 0), Ze(O(e), t, n)
                                 }, h.clone = function(e) {
                                     return v(e, 4)
                                 }, h.cloneDeep = function(e) {
                                     return v(e, 5)
                                 }, h.cloneDeepWith = function(e, t) {
                                     return v(e, 5, t = "function" == typeof t ? t : void 0)
                                 }, h.cloneWith = function(e, t) {
                                     return v(e, 4, t = "function" == typeof t ? t : void 0)
                                 }, h.conformsTo = function(e, t) {
                                     return null == t || Qe(e, t, E(t))
-                                }, h.deburr = Jo, h.defaultTo = function(e, t) {
+                                }, h.deburr = Zo, h.defaultTo = function(e, t) {
                                     return null == e || e != e ? t : e
                                 }, h.divide = Ci, h.endsWith = function(e, t, n) {
                                     e = p(e), t = c(t);
                                     var r = e.length,
-                                        r = n = void 0 === n ? r : Je(I(n), 0, r);
+                                        r = n = void 0 === n ? r : Ze(I(n), 0, r);
                                     return 0 <= (n -= t.length) && e.slice(n, r) == t
                                 }, h.eq = R, h.escape = function(e) {
                                     return (e = p(e)) && Ca.test(e) ? e.replace(ja, Is) : e
                                 }, h.escapeRegExp = function(e) {
                                     return (e = p(e)) && Ia.test(e) ? e.replace(Da, "\\$&") : e
                                 }, h.every = function(e, t, n) {
                                     return (D(e) ? bs : ot)(e, u(t = n && f(e, t, n) ? void 0 : t, 3))
@@ -3599,15 +3303,15 @@
                                 }, h.stubString = function() {
                                     return ""
                                 }, h.stubTrue = function() {
                                     return !0
                                 }, h.multiply = Pi, h.nth = function(e, t) {
                                     return e && e.length ? Pt(e, I(t)) : void 0
                                 }, h.noConflict = function() {
-                                    return Gi._ === this && (Gi._ = J), this
+                                    return Gi._ === this && (Gi._ = Z), this
                                 }, h.noop = bi, h.now = Xr, h.pad = function(e, t, n) {
                                     e = p(e);
                                     var r = (t = I(t)) ? sa(e) : 0;
                                     return !t || t <= r ? e : En(he(t = (t - r) / 2), n) + e + En(pe(t), n)
                                 }, h.padEnd = function(e, t, n) {
                                     e = p(e);
                                     var r = (t = I(t)) ? sa(e) : 0;
@@ -3670,29 +3374,29 @@
                                 }, h.sortedLastIndexOf = function(e, t) {
                                     if (null != e && e.length) {
                                         var n = Bt(e, t, !0) - 1;
                                         if (R(e[n], t)) return n
                                     }
                                     return -1
                                 }, h.startCase = ri, h.startsWith = function(e, t, n) {
-                                    return e = p(e), n = null == n ? 0 : Je(I(n), 0, e.length), t = c(t), e.slice(n, n + t.length) == t
+                                    return e = p(e), n = null == n ? 0 : Ze(I(n), 0, e.length), t = c(t), e.slice(n, n + t.length) == t
                                 }, h.subtract = Mi, h.sum = function(e) {
                                     return e && e.length ? zs(e, j) : 0
                                 }, h.sumBy = function(e, t) {
                                     return e && e.length ? zs(e, u(t, 2)) : 0
                                 }, h.template = function(a, e, t) {
                                     var n = h.templateSettings;
                                     t && f(a, e, t) && (e = void 0), a = p(a), e = Mo({}, e, n, Mn);
                                     var s, l, t = Mo({}, e.imports, n.imports, Mn),
                                         r = E(t),
                                         o = Ms(t, r),
                                         c = 0,
-                                        n = e.interpolate || Ja,
+                                        n = e.interpolate || Za,
                                         u = "__p += '",
-                                        t = F((e.escape || Ja).source + "|" + n.source + "|" + (n === Ta ? Va : Ja).source + "|" + (e.evaluate || Ja).source + "|$", "g"),
+                                        t = F((e.escape || Za).source + "|" + n.source + "|" + (n === Ta ? Va : Za).source + "|" + (e.evaluate || Za).source + "|$", "g"),
                                         i = "//# sourceURL=" + (k.call(e, "sourceURL") ? (e.sourceURL + "").replace(/\s/g, " ") : "lodash.templateSources[" + ++is + "]") + "\n",
                                         n = (a.replace(t, function(e, t, n, r, o, i) {
                                             return n = n || r, u += a.slice(c, i).replace(Qa, Ls), t && (s = !0, u += "' +\n__e(" + t + ") +\n'"), o && (l = !0, u += "';\n" + o + ";\n__p += '"), n && (u += "' +\n((__t = (" + n + ")) == null ? '' : __t) +\n'"), c = i + e.length, e
                                         }), u += "';\n", k.call(e, "variable") && e.variable);
                                     if (n) {
                                         if (Wa.test(n)) throw new N("Invalid `variable` option passed into `_.template`")
                                     } else u = "with (obj) {\n" + u + "\n}\n";
@@ -3708,15 +3412,15 @@
                                         r = A(e, 4294967295);
                                     e -= 4294967295;
                                     for (r = Ps(r, t = u(t)); ++n < e;) t(n);
                                     return r
                                 }, h.toFinite = ko, h.toInteger = I, h.toLength = Co, h.toLower = function(e) {
                                     return p(e).toLowerCase()
                                 }, h.toNumber = O, h.toSafeInteger = function(e) {
-                                    return e ? Je(I(e), -9007199254740991, 9007199254740991) : 0 === e ? e : 0
+                                    return e ? Ze(I(e), -9007199254740991, 9007199254740991) : 0 === e ? e : 0
                                 }, h.toString = p, h.toUpper = function(e) {
                                     return p(e).toUpperCase()
                                 }, h.trim = function(e, t, n) {
                                     return (e = p(e)) && (n || void 0 === t) ? Ts(e) : e && (t = c(t)) ? tn(n = la(e), As(n, t = la(t)), Rs(n, t) + 1).join("") : e
                                 }, h.trimEnd = function(e, t, n) {
                                     return (e = p(e)) && (n || void 0 === t) ? e.slice(0, Fs(e) + 1) : e && (t = c(t)) ? tn(n = la(e), 0, Rs(n, la(t)) + 1).join("") : e
                                 }, h.trimStart = function(e, t, n) {
@@ -3743,43 +3447,43 @@
                                 }, h.uniqueId = function(e) {
                                     var t = ++K;
                                     return p(e) + t
                                 }, h.upperCase = oi, h.upperFirst = ii, h.each = Fr, h.eachRight = Wr, h.first = wr, gi(h, (Si = {}, ct(h, function(e, t) {
                                     k.call(h.prototype, t) || (Si[t] = e)
                                 }), Si), {
                                     chain: !1
-                                }), h.VERSION = "4.17.21", Ji(["bind", "bindKey", "curry", "curryRight", "partial", "partialRight"], function(e) {
+                                }), h.VERSION = "4.17.21", Zi(["bind", "bindKey", "curry", "curryRight", "partial", "partialRight"], function(e) {
                                     h[e].placeholder = h
-                                }), Ji(["drop", "take"], function(n, r) {
+                                }), Zi(["drop", "take"], function(n, r) {
                                     b.prototype[n] = function(e) {
                                         e = void 0 === e ? 1 : M(I(e), 0);
                                         var t = this.__filtered__ && !r ? new b(this) : this.clone();
                                         return t.__filtered__ ? t.__takeCount__ = A(e, t.__takeCount__) : t.__views__.push({
                                             size: A(e, 4294967295),
                                             type: n + (t.__dir__ < 0 ? "Right" : "")
                                         }), t
                                     }, b.prototype[n + "Right"] = function(e) {
                                         return this.reverse()[n](e).reverse()
                                     }
-                                }), Ji(["filter", "map", "takeWhile"], function(e, t) {
+                                }), Zi(["filter", "map", "takeWhile"], function(e, t) {
                                     var n = t + 1,
                                         r = 1 == n || 3 == n;
                                     b.prototype[e] = function(e) {
                                         var t = this.clone();
                                         return t.__iteratees__.push({
                                             iteratee: u(e, 3),
                                             type: n
                                         }), t.__filtered__ = t.__filtered__ || r, t
                                     }
-                                }), Ji(["head", "last"], function(e, t) {
+                                }), Zi(["head", "last"], function(e, t) {
                                     var n = "take" + (t ? "Right" : "");
                                     b.prototype[e] = function() {
                                         return this[n](1).value()[0]
                                     }
-                                }), Ji(["initial", "tail"], function(e, t) {
+                                }), Zi(["initial", "tail"], function(e, t) {
                                     var n = "drop" + (t ? "" : "Right");
                                     b.prototype[e] = function() {
                                         return this.__filtered__ ? new b(this) : this[n](1)
                                     }
                                 }), b.prototype.compact = function() {
                                     return this.filter(j)
                                 }, b.prototype.find = function(e) {
@@ -3820,15 +3524,15 @@
                                             o = o && !i;
                                         return !p && a ? (n = o ? n : new b(this), (t = c.apply(n, r)).__actions__.push({
                                             func: Ir,
                                             args: [e],
                                             thisArg: void 0
                                         }), new g(t, s)) : l && o ? c.apply(this, r) : (t = this.thru(e), l ? f ? t.value()[0] : t.value() : t)
                                     })
-                                }), Ji(["pop", "push", "shift", "sort", "splice", "unshift"], function(e) {
+                                }), Zi(["pop", "push", "shift", "sort", "splice", "unshift"], function(e) {
                                     var n = H[e],
                                         r = /^(?:push|sort|unshift)$/.test(e) ? "tap" : "thru",
                                         o = /^(?:pop|shift)$/.test(e);
                                     h.prototype[e] = function() {
                                         var e, t = arguments;
                                         return o && !this.__chain__ ? (e = this.value(), n.apply(D(e) ? e : [], t)) : this[r](function(e) {
                                             return n.apply(D(e) ? e : [], t)
@@ -3934,14 +3638,310 @@
                             }();
                         Gi._ = Hs, void 0 !== (x = function() {
                             return Hs
                         }.call(O, E, O, _)) && (_.exports = x)
                     }.call(this)
                 }.call(this, E(27), E(60)(e))
             }, function(e, t, n) {
+                "use strict";
+                n.d(t, "a", function() {
+                    return l
+                }), n.d(t, "b", function() {
+                    return s
+                }), n.d(t, "c", function() {
+                    return b
+                }), n.d(t, "d", function() {
+                    return m
+                }), n.d(t, "e", function() {
+                    return a
+                }), n.d(t, "f", function() {
+                    return p
+                }), n.d(t, "g", function() {
+                    return c
+                }), n.d(t, "h", function() {
+                    return h
+                }), n.d(t, "i", function() {
+                    return f
+                }), n.d(t, "j", function() {
+                    return u
+                }), n.d(t, "k", function() {
+                    return d
+                });
+                var t = n(1),
+                    i = n.n(t);
+                const r = {
+                    a: {
+                        content: 9,
+                        self: !1,
+                        type: 105
+                    },
+                    address: {
+                        invalid: ["h1", "h2", "h3", "h4", "h5", "h6", "address", "article", "aside", "section", "div", "header", "footer"],
+                        self: !1
+                    },
+                    audio: {
+                        children: ["track", "source"]
+                    },
+                    br: {
+                        type: 9,
+                        void: !0
+                    },
+                    body: {
+                        content: 127
+                    },
+                    button: {
+                        content: 8,
+                        type: 105
+                    },
+                    caption: {
+                        content: 1,
+                        parent: ["table"]
+                    },
+                    col: {
+                        parent: ["colgroup"],
+                        void: !0
+                    },
+                    colgroup: {
+                        children: ["col"],
+                        parent: ["table"]
+                    },
+                    details: {
+                        children: ["summary"],
+                        type: 97
+                    },
+                    dd: {
+                        content: 1,
+                        parent: ["dl"]
+                    },
+                    dl: {
+                        children: ["dt", "dd"],
+                        type: 1
+                    },
+                    dt: {
+                        content: 1,
+                        invalid: ["footer", "header"],
+                        parent: ["dl"]
+                    },
+                    figcaption: {
+                        content: 1,
+                        parent: ["figure"]
+                    },
+                    footer: {
+                        invalid: ["footer", "header"]
+                    },
+                    header: {
+                        invalid: ["footer", "header"]
+                    },
+                    hr: {
+                        type: 1,
+                        void: !0
+                    },
+                    img: {
+                        void: !0
+                    },
+                    li: {
+                        content: 1,
+                        parent: ["ul", "ol", "menu"]
+                    },
+                    main: {
+                        self: !1
+                    },
+                    ol: {
+                        children: ["li"],
+                        type: 1
+                    },
+                    picture: {
+                        children: ["source", "img"],
+                        type: 25
+                    },
+                    rb: {
+                        parent: ["ruby", "rtc"]
+                    },
+                    rp: {
+                        parent: ["ruby", "rtc"]
+                    },
+                    rt: {
+                        content: 8,
+                        parent: ["ruby", "rtc"]
+                    },
+                    rtc: {
+                        content: 8,
+                        parent: ["ruby"]
+                    },
+                    ruby: {
+                        children: ["rb", "rp", "rt", "rtc"]
+                    },
+                    source: {
+                        parent: ["audio", "video", "picture"],
+                        void: !0
+                    },
+                    summary: {
+                        content: 8,
+                        parent: ["details"]
+                    },
+                    table: {
+                        children: ["caption", "colgroup", "thead", "tbody", "tfoot", "tr"],
+                        type: 1
+                    },
+                    tbody: {
+                        parent: ["table"],
+                        children: ["tr"]
+                    },
+                    td: {
+                        content: 1,
+                        parent: ["tr"]
+                    },
+                    tfoot: {
+                        parent: ["table"],
+                        children: ["tr"]
+                    },
+                    th: {
+                        content: 1,
+                        parent: ["tr"]
+                    },
+                    thead: {
+                        parent: ["table"],
+                        children: ["tr"]
+                    },
+                    tr: {
+                        parent: ["table", "tbody", "thead", "tfoot"],
+                        children: ["th", "td"]
+                    },
+                    track: {
+                        parent: ["audio", "video"],
+                        void: !0
+                    },
+                    ul: {
+                        children: ["li"],
+                        type: 1
+                    },
+                    video: {
+                        children: ["track", "source"]
+                    },
+                    wbr: {
+                        type: 9,
+                        void: !0
+                    }
+                };
+
+                function o(t) {
+                    return e => {
+                        r[e] = {
+                            ...t,
+                            ...r[e]
+                        }
+                    }
+                } ["address", "main", "div", "figure", "p", "pre"].forEach(o({
+                    content: 1,
+                    type: 65
+                })), ["abbr", "b", "bdi", "bdo", "cite", "code", "data", "dfn", "em", "i", "kbd", "mark", "q", "ruby", "samp", "strong", "sub", "sup", "time", "u", "var"].forEach(o({
+                    content: 8,
+                    type: 73
+                })), ["p", "pre"].forEach(o({
+                    content: 8,
+                    type: 65
+                })), ["s", "small", "span", "del", "ins"].forEach(o({
+                    content: 8,
+                    type: 9
+                })), ["article", "aside", "footer", "header", "nav", "section", "blockquote"].forEach(o({
+                    content: 1,
+                    type: 67
+                })), ["h1", "h2", "h3", "h4", "h5", "h6"].forEach(o({
+                    content: 8,
+                    type: 69
+                })), ["audio", "canvas", "iframe", "img", "video"].forEach(o({
+                    type: 89
+                }));
+                const a = Object.freeze(r),
+                    s = ["applet", "base", "body", "command", "embed", "frame", "frameset", "head", "html", "link", "meta", "noscript", "object", "script", "style", "title"],
+                    l = Object.keys(a).filter(e => "canvas" !== e && "iframe" !== e),
+                    c = 2,
+                    u = 3,
+                    f = 4,
+                    d = 5,
+                    p = Object.freeze({
+                        alt: 1,
+                        cite: 1,
+                        class: 1,
+                        colspan: u,
+                        controls: f,
+                        datetime: 1,
+                        default: f,
+                        disabled: f,
+                        dir: 1,
+                        height: 1,
+                        href: 1,
+                        id: 1,
+                        kind: 1,
+                        label: 1,
+                        lang: 1,
+                        loading: 1,
+                        loop: f,
+                        media: 1,
+                        muted: f,
+                        poster: 1,
+                        rel: 1,
+                        role: 1,
+                        rowspan: u,
+                        scope: 1,
+                        sizes: 1,
+                        span: u,
+                        start: u,
+                        style: d,
+                        src: 1,
+                        srclang: 1,
+                        srcset: 1,
+                        tabindex: 1,
+                        target: 1,
+                        title: 1,
+                        type: 1,
+                        width: 1
+                    }),
+                    h = Object.freeze({
+                        class: "className",
+                        colspan: "colSpan",
+                        datetime: "dateTime",
+                        rowspan: "rowSpan",
+                        srclang: "srcLang",
+                        srcset: "srcSet",
+                        tabindex: "tabIndex"
+                    });
+
+                function g() {
+                    return (g = Object.assign || function(e) {
+                        for (var t = 1; t < arguments.length; t++) {
+                            var n, r = arguments[t];
+                            for (n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
+                        }
+                        return e
+                    }).apply(this, arguments)
+                }
+
+                function b({
+                    attributes: e = {},
+                    className: t,
+                    children: n = null,
+                    selfClose: r = !1,
+                    tagName: o
+                }) {
+                    return r ? i.a.createElement(o, g({
+                        className: t
+                    }, e)) : i.a.createElement(o, g({
+                        className: t
+                    }, e), n)
+                }
+                class m {
+                    attribute(e, t) {
+                        return t
+                    }
+                    node(e, t) {
+                        return t
+                    }
+                }
+            }, function(e, t, n) {
                 var r, o, i, a = t,
                     s = (o = [function(e, t) {
                         e.exports = n(1)
                     }, function(e, t) {
                         e.exports = n(0)
                     }, function(e, t) {
                         e.exports = n(333)
@@ -7701,19 +7701,19 @@
                     return e.name === A.MAC_OS
                 }
 
                 function G(e) {
                     return e.name === A.WindowsPhone
                 }
 
-                function Z(e) {
+                function J(e) {
                     return e.name === A.IOS
                 }
 
-                function J(e) {
+                function Z(e) {
                     return e = e.version, x(e)
                 }
 
                 function Q(e) {
                     return e = e.name, x(e)
                 }
 
@@ -7863,21 +7863,21 @@
                         isMobile: U(t) || z(),
                         isMobileOnly: E(t),
                         isTablet: S(t) || z(),
                         isBrowser: j(t),
                         isDesktop: j(t),
                         isAndroid: Y(r),
                         isWinPhone: G(r),
-                        isIOS: Z(r) || z(),
+                        isIOS: J(r) || z(),
                         isChrome: ee(n),
                         isFirefox: te(n),
                         isSafari: oe(n),
                         isOpera: ae(n),
                         isIE: se(n),
-                        osVersion: J(r),
+                        osVersion: Z(r),
                         osName: Q(r),
                         fullBrowserVersion: ue(n),
                         browserVersion: fe(n),
                         browserName: de(n),
                         mobileVendor: V(t),
                         mobileModel: $(t),
                         engineName: pe(o),
@@ -7908,36 +7908,36 @@
                     D = U(l) || z(),
                     ke = E(l),
                     Ce = S(l) || z(),
                     ze = j(l),
                     Pe = j(l),
                     Te = Y(u),
                     Me = G(u),
-                    Ae = Z(u) || z(),
+                    Ae = J(u) || z(),
                     Re = ee(s),
                     De = te(s),
                     Ie = oe(s),
                     Le = ae(s),
                     Ne = se(s),
-                    Ue = J(u),
+                    Ue = Z(u),
                     Be = Q(u),
                     Fe = ue(s),
                     We = fe(s),
                     He = de(s),
                     Ve = V(l),
                     $e = $(l),
                     qe = pe(c),
                     c = he(c),
                     Ye = ye(f),
                     Ke = k(s) || C(f),
                     Xe = re(s),
                     l = q(l),
                     Ge = be(),
-                    Ze = z(),
-                    Je = me(),
+                    Je = z(),
+                    Ze = me(),
                     Qe = ve(),
                     et = ge(),
                     tt = C(f),
                     f = k(s) && !C(f),
                     nt = K(u),
                     u = X(u),
                     rt = le(s),
@@ -8102,15 +8102,15 @@
                         device: (e = b(e)).device,
                         browser: e.browser,
                         os: e.os,
                         engine: e.engine,
                         ua: e.ua
                     });
                     console.error("No valid user agent string was provided")
-                }, e.getUA = Ye, e.isAndroid = Te, e.isBrowser = ze, e.isChrome = Re, e.isChromium = je, e.isConsole = Oe, e.isDesktop = Pe, e.isEdge = Ke, e.isEdgeChromium = tt, e.isElectron = et, e.isEmbedded = t, e.isFirefox = De, e.isIE = Ne, e.isIOS = Ae, e.isIOS13 = Ge, e.isIPad13 = Ze, e.isIPhone13 = Je, e.isIPod13 = Qe, e.isLegacyEdge = f, e.isMIUI = rt, e.isMacOs = u, e.isMobile = D, e.isMobileOnly = ke, e.isMobileSafari = Se, e.isOpera = Le, e.isSafari = Ie, e.isSamsungBrowser = s, e.isSmartTV = xe, e.isTablet = Ce, e.isWearable = Ee, e.isWinPhone = Me, e.isWindows = nt, e.isYandex = Xe, e.mobileModel = $e, e.mobileVendor = Ve, e.osName = Be, e.osVersion = Ue, e.parseUserAgent = b, e.setUserAgent = n, e.useDeviceData = ot, e.useDeviceSelectors = function(e) {
+                }, e.getUA = Ye, e.isAndroid = Te, e.isBrowser = ze, e.isChrome = Re, e.isChromium = je, e.isConsole = Oe, e.isDesktop = Pe, e.isEdge = Ke, e.isEdgeChromium = tt, e.isElectron = et, e.isEmbedded = t, e.isFirefox = De, e.isIE = Ne, e.isIOS = Ae, e.isIOS13 = Ge, e.isIPad13 = Je, e.isIPhone13 = Ze, e.isIPod13 = Qe, e.isLegacyEdge = f, e.isMIUI = rt, e.isMacOs = u, e.isMobile = D, e.isMobileOnly = ke, e.isMobileSafari = Se, e.isOpera = Le, e.isSafari = Ie, e.isSamsungBrowser = s, e.isSmartTV = xe, e.isTablet = Ce, e.isWearable = Ee, e.isWinPhone = Me, e.isWindows = nt, e.isYandex = Xe, e.mobileModel = $e, e.mobileVendor = Ve, e.osName = Be, e.osVersion = Ue, e.parseUserAgent = b, e.setUserAgent = n, e.useDeviceData = ot, e.useDeviceSelectors = function(e) {
                     e = ot(e || window.navigator.userAgent);
                     return [_e(e), e]
                 }, e.useMobileOrientation = function() {
                     t = i.useState(function() {
                         var e = window.innerWidth > window.innerHeight ? 90 : 0;
                         return {
                             isPortrait: 0 == e,
@@ -10156,15 +10156,15 @@
                     B = l,
                     c = {
                         CheckmarkIcon: () => M,
                         ErrorIcon: () => P,
                         LoaderIcon: () => T,
                         ToastBar: () => R,
                         ToastIcon: () => A,
-                        Toaster: () => J,
+                        Toaster: () => Z,
                         default: () => Q,
                         resolveValue: () => f,
                         toast: () => _,
                         useToaster: () => O,
                         useToasterStore: () => y
                     };
                 for (n in c) i(B, n, {
@@ -10664,21 +10664,21 @@
                         }, [n, r]);
                         return D.createElement("div", {
                             ref: i,
                             className: e,
                             style: t
                         }, o)
                     }),
-                    Z = C.css`
+                    J = C.css`
   z-index: 9999;
   > * {
     pointer-events: auto;
   }
 `,
-                    J = ({
+                    Z = ({
                         reverseOrder: a,
                         position: s = "top-center",
                         toastOptions: e,
                         gutter: l,
                         children: c,
                         containerStyle: t,
                         containerClassName: n
@@ -10725,15 +10725,15 @@
                                     ...r,
                                     ...t
                                 });
                             return D.createElement(G, {
                                 id: e.id,
                                 key: e.id,
                                 onHeightUpdate: u.updateHeight,
-                                className: e.visible ? Z : "",
+                                className: e.visible ? J : "",
                                 style: i
                             }, "custom" === e.type ? f(e.message, e) : c ? c(e) : D.createElement(R, {
                                 toast: e,
                                 position: o
                             }))
                         }))
                     },
@@ -12519,16 +12519,16 @@
                         f = O(r, "Promise"),
                         h = O(r, "Set"),
                         r = O(r, "WeakMap"),
                         g = O(Object, "create"),
                         K = E(o),
                         X = E(p),
                         G = E(f),
-                        Z = E(h),
-                        J = E(r),
+                        J = E(h),
+                        Z = E(r),
                         c = c ? c.prototype : void 0,
                         M = c ? c.valueOf : void 0;
 
                     function b(e) {
                         var t = -1,
                             n = null == e ? 0 : e.length;
                         for (this.clear(); ++t < n;) {
@@ -12853,17 +12853,17 @@
                         if (e) switch (e) {
                             case K:
                                 return "[object DataView]";
                             case X:
                                 return C;
                             case G:
                                 return "[object Promise]";
-                            case Z:
-                                return P;
                             case J:
+                                return P;
+                            case Z:
                                 return "[object WeakMap]"
                         }
                         return t
                     });
                     var se = ee(function() {
                             return arguments
                         }()) ? ee : function(e) {
@@ -13224,16 +13224,16 @@
                         V = 32,
                         $ = 45,
                         q = 42,
                         Y = 44,
                         K = 58,
                         X = 47,
                         G = 1,
-                        Z = 1,
-                        J = 0,
+                        J = 1,
+                        Z = 0,
                         Q = 1,
                         ee = 1,
                         te = 1,
                         g = 0,
                         me = 0,
                         ne = 0,
                         re = [],
@@ -13334,15 +13334,15 @@
                                                 case 115:
                                                 case $:
                                                     i = t;
                                                     break;
                                                 default:
                                                     i = re
                                             }
-                                            if (S = (P = ye(t, i, P, d, o + 1)).length, 0 < ne && 0 === S && (S = z.length), 0 < oe && (a = ue(3, P, i = we(re, z, E), t, Z, G, S, d, o, r), z = i.join(""), void 0 !== a) && 0 === (S = (P = a.trim()).length) && (d = 0, P = ""), 0 < S) switch (d) {
+                                            if (S = (P = ye(t, i, P, d, o + 1)).length, 0 < ne && 0 === S && (S = z.length), 0 < oe && (a = ue(3, P, i = we(re, z, E), t, J, G, S, d, o, r), z = i.join(""), void 0 !== a) && 0 === (S = (P = a.trim()).length) && (d = 0, P = ""), 0 < S) switch (d) {
                                                 case 115:
                                                     z = z.replace(be, xe);
                                                 case 100:
                                                 case 109:
                                                 case $:
                                                     P = z + "{" + P + "}";
                                                     break;
@@ -13353,15 +13353,15 @@
                                                     P = z + P, 112 === r && (T += P, P = "")
                                             } else P = ""
                                         } else P = ye(t, we(t, z, E), P, r, o + 1);
                                         M += P, y = E = x = w = O = v = 0, P = z = "", p = n.charCodeAt(++_);
                                         break;
                                     case N:
                                     case L:
-                                        if (1 < (S = (z = (0 < x ? z.replace(R, "") : z).trim()).length)) switch (0 === w && ((f = z.charCodeAt(0)) === $ || 96 < f && f < 123) && (S = (z = z.replace(" ", ":")).length), 0 < oe && void 0 !== (a = ue(1, z, t, e, Z, G, T.length, r, o, r)) && 0 === (S = (z = a.trim()).length) && (z = "\0\0"), f = z.charCodeAt(0), d = z.charCodeAt(1), f) {
+                                        if (1 < (S = (z = (0 < x ? z.replace(R, "") : z).trim()).length)) switch (0 === w && ((f = z.charCodeAt(0)) === $ || 96 < f && f < 123) && (S = (z = z.replace(" ", ":")).length), 0 < oe && void 0 !== (a = ue(1, z, t, e, J, G, T.length, r, o, r)) && 0 === (S = (z = a.trim()).length) && (z = "\0\0"), f = z.charCodeAt(0), d = z.charCodeAt(1), f) {
                                             case 0:
                                                 break;
                                             case 64:
                                                 if (105 === d || 99 === d) {
                                                     A += z + n.charAt(_);
                                                     break
                                                 }
@@ -13390,15 +13390,15 @@
                                         case L:
                                         case U:
                                         case N:
                                             break;
                                         default:
                                             0 < w && (O = 1)
                                     }
-                                    l === X ? l = 0 : Q + v === 0 && 107 !== r && 0 < z.length && (x = 1, z += "\0"), 0 < oe * ve && ue(0, z, t, e, Z, G, T.length, r, o, r), G = 1, Z++;
+                                    l === X ? l = 0 : Q + v === 0 && 107 !== r && 0 < z.length && (x = 1, z += "\0"), 0 < oe * ve && ue(0, z, t, e, J, G, T.length, r, o, r), G = 1, J++;
                                     break;
                                 case L:
                                 case N:
                                     if (l + u + c + s === 0) {
                                         G++;
                                         break
                                     }
@@ -13426,19 +13426,19 @@
                                         case 11:
                                             C = "\\v";
                                             break;
                                         case 38:
                                             u + l + s === 0 && 0 < Q && (x = E = 1, C = "\f" + C);
                                             break;
                                         case 108:
-                                            if (u + l + s + J === 0 && 0 < w) switch (_ - w) {
+                                            if (u + l + s + Z === 0 && 0 < w) switch (_ - w) {
                                                 case 2:
-                                                    112 === h && n.charCodeAt(_ - 3) === K && (J = h);
+                                                    112 === h && n.charCodeAt(_ - 3) === K && (Z = h);
                                                 case 8:
-                                                    111 === g && (J = g)
+                                                    111 === g && (Z = g)
                                             }
                                             break;
                                         case K:
                                             u + l + s === 0 && (w = _);
                                             break;
                                         case Y:
                                             l + c + u + s === 0 && (x = 1, C += "\r");
@@ -13574,24 +13574,24 @@
                                                     default:
                                                         n = 1 < a && 0 < n.indexOf(":") ? t + n.replace(ge, "$1" + se + "$2") : t + n + se
                                                 }
                                                 u += n
                                             } i[r] = u.replace(R, "").trim()
                                     }
                                     return i
-                                }(t) : t, 0 < oe && void 0 !== (a = ue(2, T, i, e, Z, G, S, r, o, r)) && 0 === (T = a).length) return A + T + M;
-                            if (T = i.join(",") + "{" + T + "}", ee * J != 0) {
-                                switch (J = 2 !== ee || ce(T, 2) ? J : 0) {
+                                }(t) : t, 0 < oe && void 0 !== (a = ue(2, T, i, e, J, G, S, r, o, r)) && 0 === (T = a).length) return A + T + M;
+                            if (T = i.join(",") + "{" + T + "}", ee * Z != 0) {
+                                switch (Z = 2 !== ee || ce(T, 2) ? Z : 0) {
                                     case 111:
                                         T = T.replace(he, ":-moz-$1") + T;
                                         break;
                                     case 112:
                                         T = T.replace(D, "::" + I + "input-$1") + T.replace(D, "::-moz-$1") + T.replace(D, ":-ms-input-$1") + T
                                 }
-                                J = 0
+                                Z = 0
                             }
                         }
                         return A + T + M
                     }
 
                     function we(e, t, n) {
                         var r = t.trim().split(f),
@@ -13827,16 +13827,16 @@
                     }
 
                     function p(e, t) {
                         if (void 0 !== this && this.constructor === p) return o(e);
                         var n = e.charCodeAt(0);
                         n < 33 && (n = (e = e.trim()).charCodeAt(0)), 0 < ie && (ae = e.replace(s, 91 === n ? "" : "-")), (n = 1) === Q ? le = e : se = e;
                         var r, e = [le],
-                            t = (0 < oe && void 0 !== (r = ue(-1, t, e, e, Z, G, 0, 0, 0, 0)) && "string" == typeof r && (t = r), ye(re, e, t, 0, 0));
-                        return 0 < oe && void 0 !== (r = ue(-2, t, e, e, Z, G, t.length, 0, 0, 0)) && "string" != typeof(t = r) && (n = 0), se = le = ae = "", G = Z = 1, g * n == (J = 0) ? t : t.replace(R, "").replace(l, "").replace(c, "$1").replace(u, "$1").replace(d, " ")
+                            t = (0 < oe && void 0 !== (r = ue(-1, t, e, e, J, G, 0, 0, 0, 0)) && "string" == typeof r && (t = r), ye(re, e, t, 0, 0));
+                        return 0 < oe && void 0 !== (r = ue(-2, t, e, e, J, G, t.length, 0, 0, 0)) && "string" != typeof(t = r) && (n = 0), se = le = ae = "", G = J = 1, g * n == (Z = 0) ? t : t.replace(R, "").replace(l, "").replace(c, "$1").replace(u, "$1").replace(d, " ")
                     }
                     return p.use = function e(t) {
                         switch (t) {
                             case void 0:
                             case null:
                                 oe = b.length = 0;
                                 break;
@@ -13939,15 +13939,15 @@
                 t.a = r
             }, , function(module, __webpack_exports__, __webpack_require__) {
                 "use strict";
                 var react__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(1),
                     react__WEBPACK_IMPORTED_MODULE_0___default = __webpack_require__.n(react__WEBPACK_IMPORTED_MODULE_0__),
                     prop_types__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(0),
                     prop_types__WEBPACK_IMPORTED_MODULE_1___default = __webpack_require__.n(prop_types__WEBPACK_IMPORTED_MODULE_1__),
-                    lodash__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(4),
+                    lodash__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(3),
                     lodash__WEBPACK_IMPORTED_MODULE_2___default = __webpack_require__.n(lodash__WEBPACK_IMPORTED_MODULE_2__),
                     ninja_keys__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(494),
                     _FefferyStyle_react__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(55);
 
                 function _typeof(e) {
                     return (_typeof = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
@@ -14201,15 +14201,15 @@
             }, function(module, __webpack_exports__, __webpack_require__) {
                 "use strict";
                 var react__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(1),
                     react__WEBPACK_IMPORTED_MODULE_0___default = __webpack_require__.n(react__WEBPACK_IMPORTED_MODULE_0__),
                     byte_guide__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(242),
                     prop_types__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(0),
                     prop_types__WEBPACK_IMPORTED_MODULE_2___default = __webpack_require__.n(prop_types__WEBPACK_IMPORTED_MODULE_2__),
-                    lodash__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(4),
+                    lodash__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(3),
                     lodash__WEBPACK_IMPORTED_MODULE_3___default = __webpack_require__.n(lodash__WEBPACK_IMPORTED_MODULE_3__),
                     _styles_css__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(29),
                     _styles_css__WEBPACK_IMPORTED_MODULE_4___default = __webpack_require__.n(_styles_css__WEBPACK_IMPORTED_MODULE_4__),
                     FefferyGuide = function FefferyGuide(props) {
                         var id = props.id,
                             className = props.className,
                             style = props.style,
@@ -16497,21 +16497,21 @@
                         Y = ((e = Q.prototype).insertRule = function(e, t) {
                             return e <= this.length && 0 <= e && (t = document.createTextNode(t), e = this.nodes[e], this.element.insertBefore(t, e || null), this.length++, !0)
                         }, e.deleteRule = function(e) {
                             this.element.removeChild(this.nodes[e]), this.length--
                         }, e.getRule = function(e) {
                             return e < this.length ? this.nodes[e].textContent : ""
                         }, Q),
-                        K = ((e = J.prototype).insertRule = function(e, t) {
+                        K = ((e = Z.prototype).insertRule = function(e, t) {
                             return e <= this.length && (this.rules.splice(e, 0, t), this.length++, !0)
                         }, e.deleteRule = function(e) {
                             this.rules.splice(e, 1), this.length--
                         }, e.getRule = function(e) {
                             return e < this.length ? this.rules[e] : ""
-                        }, J),
+                        }, Z),
                         X = u,
                         G = {
                             isServer: !u,
                             useCSSOMInjection: !t
                         },
                         v = (y.registerId = r, (e = y.prototype).reconstructWithOptions = function(e, t) {
                             return void 0 === t && (t = !0), new y(O({}, this.options, {}, e), this.gs, t && this.names || void 0)
@@ -16539,15 +16539,15 @@
                                 var i, a, s, l = f.get(l);
                                 void 0 !== l && (i = e.names.get(l), a = t.getGroup(o), i) && a && i.size && (l = c + ".g" + o + '[id="' + l + '"]', s = "", void 0 !== i && i.forEach(function(e) {
                                     0 < e.length && (s += e + ",")
                                 }), r += a + l + '{content:"' + s + '"}/*!sc*/\n')
                             }
                             return r
                         }, y),
-                        Z = /(a)(d)/gi;
+                        J = /(a)(d)/gi;
 
                     function y(e, t, n) {
                         if (void 0 === e && (e = E), void 0 === t && (t = {}), this.options = O({}, G, {}, e), this.gs = t, this.names = new Map(n), this.server = !!e.isServer, !this.server && u && X) {
                             X = !1;
                             for (var r = this, o = document.querySelectorAll(H), i = 0, a = o.length; i < a; i++) {
                                 var s = o[i];
                                 s && "active" !== s.getAttribute(c) && (function(e, t) {
@@ -16556,15 +16556,15 @@
                                         c && ((a = c.match(V)) ? (s = 0 | parseInt(a[1], 10), l = a[2], 0 != s && (W(l, s), $(e, l, a[3]), e.getTag().insertRules(s, r)), r.length = 0) : r.push(c))
                                     }
                                 }(r, s), s.parentNode) && s.parentNode.removeChild(s)
                             }
                         }
                     }
 
-                    function J(e) {
+                    function Z(e) {
                         this.rules = [], this.length = 0
                     }
 
                     function Q(e) {
                         e = this.element = n(e);
                         this.nodes = e.childNodes, this.length = 0
                     }
@@ -16583,15 +16583,15 @@
 
                     function te(e) {
                         this.groupSizes = new Uint32Array(512), this.length = 512, this.tag = e
                     }
 
                     function w(e) {
                         for (var t = "", n = Math.abs(e); 52 < n; n = n / 52 | 0) t = B(n % 52) + t;
-                        return (B(n % 52) + t).replace(Z, "$1-$2")
+                        return (B(n % 52) + t).replace(J, "$1-$2")
                     }
 
                     function j(e, t) {
                         for (var n = t.length; n;) e = 33 * e ^ t.charCodeAt(--n);
                         return e
                     }
 
@@ -17504,15 +17504,15 @@
 
                 function s(e, t) {
                     var n, r, t = (t = void 0 === t ? {} : t).insertAt;
                     e && "undefined" != typeof document && (n = document.head || document.getElementsByTagName("head")[0], (r = document.createElement("style")).type = "text/css", "top" === t && n.firstChild ? n.insertBefore(r, n.firstChild) : n.appendChild(r), r.styleSheet ? r.styleSheet.cssText = e : r.appendChild(document.createTextNode(e)))
                 }
                 s(".guide-mask {\n  position: absolute;\n  left: 0;\n  top: 0;\n  border-color: rgba(0, 0, 0, 0.6);\n  border-style: solid;\n  z-index: 1001;\n  box-sizing: border-box;\n}\n.guide-mask::after {\n  content: '';\n  display: block;\n  position: absolute;\n  top: -1px;\n  left: -1px;\n  width: 100%;\n  height: 100%;\n  border-radius: 4px;\n  border: 1px solid #fff;\n  box-shadow: 0 0 0 1px #fff;\n  background: transparent;\n}\n");
 
-                function Z(e) {
+                function J(e) {
                     function t() {
                         t = $(e = s), n = t.scrollWidth, r = t.scrollHeight, a = t.scrollTop, t.style.overflow = "hidden", e = (t = e.getBoundingClientRect()).height, o = t.width, i = t.left, t = t.top + a;
                         var e, t, n, r, o, i, a = {
                             width: n,
                             height: r,
                             borderTopWidth: Math.max(t, 0),
                             borderBottomWidth: Math.max(r - e - t, 0),
@@ -17542,15 +17542,15 @@
                             }
                     }, [o, s]), s ? N.a.createPortal(L.a.createElement("div", {
                         className: "guide-mask ".concat(r),
                         style: i
                     }), D(s).body) : null
                 }
 
-                function J(e) {
+                function Z(e) {
                     var t = void 0 === (t = e.size) ? "16" : t,
                         n = void 0 === (n = e.fill) ? "#666" : n,
                         r = e.onClick,
                         e = e.className;
                     return L.a.createElement("div", {
                         onClick: void 0 === r ? function() {} : r,
                         className: void 0 === e ? "" : e
@@ -17781,15 +17781,15 @@
                         style: P
                     }), f && L.a.createElement("div", {
                         className: "".concat(ee, "-hotspot"),
                         style: M
                     }), e ? L.a.createElement("div", {
                         className: "".concat(ee, "-close-icon"),
                         onClick: p
-                    }, e) : d ? L.a.createElement(J, {
+                    }, e) : d ? L.a.createElement(Z, {
                         className: "".concat(ee, "-close-icon"),
                         onClick: p
                     }) : null, L.a.createElement("div", {
                         className: "".concat(ee, "-title")
                     }, x.title), L.a.createElement("div", {
                         className: "".concat(ee, "-content")
                     }, "function" == typeof x.content ? x.content() : x.content), L.a.createElement("div", {
@@ -17917,15 +17917,15 @@
                             })).observe(document, {
                                 childList: !0,
                                 subtree: !0
                             }),
                             function() {
                                 e.disconnect()
                             }
-                    }, [E, C]), a && !j || !e ? null : L.a.createElement(L.a.Fragment, null, a && L.a.createElement(Z, {
+                    }, [E, C]), a && !j || !e ? null : L.a.createElement(L.a.Fragment, null, a && L.a.createElement(J, {
                         className: u,
                         anchorEl: T,
                         realWindow: M
                     }), L.a.createElement(Q, {
                         anchorEl: T,
                         parentEl: e,
                         realWindow: M,
@@ -19302,15 +19302,15 @@
                 }()
             }, function(e, c, u) {
                 "use strict";
                 ! function(r) {
                     u.d(c, "a", function() {
                         return t
                     });
-                    var p = u(3),
+                    var p = u(4),
                         e = u(1),
                         y = u.n(e),
                         e = u(256),
                         o = u.n(e);
 
                     function i(e, t, n) {
                         t in e ? Object.defineProperty(e, t, {
@@ -20253,15 +20253,15 @@
                             K = "undefined" != typeof window,
                             X = K && "ontouchstart" in window || K && 0 < navigator.maxTouchPoints,
                             G = W.forwardRef(function(e, t) {
                                 return (0, F.jsx)("a", Y({
                                     ref: t
                                 }, e))
                             }),
-                            Z = W.forwardRef(function(e, t) {
+                            J = W.forwardRef(function(e, t) {
                                 return (0, F.jsx)("button", Y({
                                     ref: t
                                 }, e))
                             });
                         const x = function(e) {
                             var t = e.active,
                                 c = void 0 !== t && t,
@@ -20320,15 +20320,15 @@
                                 C = W.useRef(null),
                                 z = W.useRef(null),
                                 O = W.useRef(null),
                                 P = W.useRef(!1),
                                 T = W.useRef(0),
                                 M = W.useRef(null),
                                 A = W.useRef(0),
-                                e = s || (p ? G : Z),
+                                e = s || (p ? G : J),
                                 s = {
                                     href: p
                                 },
                                 R = W.useMemo(function() {
                                     return !0 === w && !i || l
                                 }, [w, i, l]);
                             W.useEffect(function() {
@@ -21753,20 +21753,20 @@
 
                     function o(e, t) {
                         var n;
                         if (e = v(e), t = y(t, !0), e !== T || !c(z, t) || c(P, t)) return !(n = G(e, t)) || !c(z, t) || c(e, k) && e[k][t] || (n.enumerable = !0), n
                     }
 
                     function i(e) {
-                        for (var t, n = Z(v(e)), r = [], o = 0; n.length > o;) c(z, t = n[o++]) || t == k || t == N || r.push(t);
+                        for (var t, n = J(v(e)), r = [], o = 0; n.length > o;) c(z, t = n[o++]) || t == k || t == N || r.push(t);
                         return r
                     }
 
                     function s(e) {
-                        for (var t, n = e === T, r = Z(n ? P : v(e)), o = [], i = 0; r.length > i;) !c(z, t = r[i++]) || n && !c(T, t) || o.push(z[t]);
+                        for (var t, n = e === T, r = J(n ? P : v(e)), o = [], i = 0; r.length > i;) !c(z, t = r[i++]) || n && !c(T, t) || o.push(z[t]);
                         return o
                     }
                     var l = e(3),
                         c = e(5),
                         u = e(4),
                         f = e(15),
                         d = e(37),
@@ -21790,20 +21790,20 @@
                         q = e(71),
                         Y = e(72),
                         x = e(32),
                         K = e(7),
                         X = e(13),
                         G = Y.f,
                         O = K.f,
-                        Z = q.f,
+                        J = q.f,
                         E = l.Symbol,
                         S = l.JSON,
                         j = S && S.stringify,
                         k = b("_hidden"),
-                        J = b("toPrimitive"),
+                        Z = b("toPrimitive"),
                         Q = {}.propertyIsEnumerable,
                         C = h("symbol-registry"),
                         z = h("symbols"),
                         P = h("op-symbols"),
                         T = Object.prototype,
                         h = "function" == typeof E && !!x.f,
                         M = l.QObject,
@@ -21884,15 +21884,15 @@
                     })), "JSON", {
                         stringify: function(e) {
                             for (var t, n, r = [e], o = 1; o < arguments.length;) r.push(arguments[o++]);
                             if (n = t = r[1], (V(t) || void 0 !== e) && !D(e)) return H(t) || (t = function(e, t) {
                                 if ("function" == typeof n && (t = n.call(this, e, t)), !D(t)) return t
                             }), r[1] = t, j.apply(S, r)
                         }
-                    }), E.prototype[J] || e(6)(E.prototype, J, E.prototype.valueOf), g(E, "Symbol"), g(Math, "Math", !0), g(l.JSON, "JSON", !0)
+                    }), E.prototype[Z] || e(6)(E.prototype, Z, E.prototype.valueOf), g(E, "Symbol"), g(Math, "Math", !0), g(l.JSON, "JSON", !0)
                 }, function(e, t, n) {
                     function r(e) {
                         s(e, o, {
                             value: {
                                 i: "O" + ++l,
                                 w: {}
                             }
@@ -24090,25 +24090,25 @@
                                 n = e.displayDataTypes,
                                 e = e.theme;
                             return n ? g.a.createElement("span", Object.assign({
                                 className: "data-type-label"
                             }, b(e, "data-type-label")), t) : null
                         }
                     }]);
-                    var Z, J, Q, ee, s = p,
+                    var J, Z, Q, ee, s = p,
                         te = (n(d, g.a.PureComponent), Q = r(d), t(d, [{
                             key: "render",
                             value: function() {
                                 var e = this.props;
                                 return g.a.createElement("div", b(e.theme, "boolean"), g.a.createElement(s, Object.assign({
                                     type_name: "bool"
                                 }, e)), e.value ? "true" : "false")
                             }
                         }]), d),
-                        ne = (n(c, g.a.PureComponent), J = r(c), t(c, [{
+                        ne = (n(c, g.a.PureComponent), Z = r(c), t(c, [{
                             key: "render",
                             value: function() {
                                 var e = this.props;
                                 return g.a.createElement("div", b(e.theme, "date"), g.a.createElement(s, Object.assign({
                                     type_name: "date"
                                 }, e)), g.a.createElement("span", Object.assign({
                                     className: "date-value"
@@ -24118,30 +24118,30 @@
                                     month: "short",
                                     day: "numeric",
                                     hour: "2-digit",
                                     minute: "2-digit"
                                 })))
                             }
                         }]), c),
-                        re = (n(l, g.a.PureComponent), Z = r(l), t(l, [{
+                        re = (n(l, g.a.PureComponent), J = r(l), t(l, [{
                             key: "render",
                             value: function() {
                                 var e = this.props;
                                 return g.a.createElement("div", b(e.theme, "float"), g.a.createElement(s, Object.assign({
                                     type_name: "float"
                                 }, e)), this.props.value)
                             }
                         }]), l);
 
                     function l() {
-                        return o(this, l), Z.apply(this, arguments)
+                        return o(this, l), J.apply(this, arguments)
                     }
 
                     function c() {
-                        return o(this, c), J.apply(this, arguments)
+                        return o(this, c), Z.apply(this, arguments)
                     }
 
                     function d() {
                         return o(this, d), Q.apply(this, arguments)
                     }
 
                     function p() {
@@ -24619,30 +24619,30 @@
                                     viewBox: "0 0 15 15",
                                     fill: "currentColor"
                                 }, g.a.createElement("path", {
                                     d: "M0 5l6 6 6-6z"
                                 })))
                             }
                         }]), at),
-                        Ze = (n(it, g.a.PureComponent), Ne = r(it), t(it, [{
+                        Je = (n(it, g.a.PureComponent), Ne = r(it), t(it, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.style,
                                     e = f(e, ["style"]);
                                 return g.a.createElement("span", e, g.a.createElement("svg", Object.assign({}, A(t), {
                                     viewBox: "0 0 40 40",
                                     fill: "currentColor",
                                     preserveAspectRatio: "xMidYMid meet"
                                 }), g.a.createElement("g", null, g.a.createElement("path", {
                                     d: "m30 35h-25v-22.5h25v7.5h2.5v-12.5c0-1.4-1.1-2.5-2.5-2.5h-7.5c0-2.8-2.2-5-5-5s-5 2.2-5 5h-7.5c-1.4 0-2.5 1.1-2.5 2.5v27.5c0 1.4 1.1 2.5 2.5 2.5h25c1.4 0 2.5-1.1 2.5-2.5v-5h-2.5v5z m-20-27.5h2.5s2.5-1.1 2.5-2.5 1.1-2.5 2.5-2.5 2.5 1.1 2.5 2.5 1.3 2.5 2.5 2.5h2.5s2.5 1.1 2.5 2.5h-20c0-1.5 1.1-2.5 2.5-2.5z m-2.5 20h5v-2.5h-5v2.5z m17.5-5v-5l-10 7.5 10 7.5v-5h12.5v-5h-12.5z m-17.5 10h7.5v-2.5h-7.5v2.5z m12.5-17.5h-12.5v2.5h12.5v-2.5z m-7.5 5h-5v2.5h5v-2.5z"
                                 }))))
                             }
                         }]), it),
-                        Je = (n(ot, g.a.PureComponent), Le = r(ot), t(ot, [{
+                        Ze = (n(ot, g.a.PureComponent), Le = r(ot), t(ot, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.style,
                                     e = f(e, ["style"]);
                                 return g.a.createElement("span", e, g.a.createElement("svg", Object.assign({}, A(t), {
                                     viewBox: "0 0 40 40",
@@ -24932,15 +24932,15 @@
                                 i = t.src,
                                 a = t.rjvId;
                             if (1 !== r.length) return g.a.createElement("span", {
                                 className: "click-to-remove",
                                 style: {
                                     display: e ? "inline-block" : "none"
                                 }
-                            }, g.a.createElement(Je, Object.assign({
+                            }, g.a.createElement(Ze, Object.assign({
                                 className: "click-to-remove-icon"
                             }, b(n, "removeVarIcon"), {
                                 onClick: function() {
                                     v.dispatch({
                                         name: "VARIABLE_REMOVED",
                                         rjvId: a,
                                         data: {
@@ -25038,15 +25038,15 @@
                                 o = e.rjvId;
                             return g.a.createElement("div", {
                                 className: "click-to-remove",
                                 style: {
                                     verticalAlign: "top",
                                     display: a.state.hovered ? "inline-block" : "none"
                                 }
-                            }, g.a.createElement(Je, Object.assign({
+                            }, g.a.createElement(Ze, Object.assign({
                                 className: "click-to-remove-icon"
                             }, b(r, "removeVarIcon"), {
                                 onClick: function() {
                                     v.dispatch({
                                         name: "VARIABLE_REMOVED",
                                         rjvId: o,
                                         data: {
@@ -25135,15 +25135,15 @@
                                         case "Enter":
                                             (e.ctrlKey || e.metaKey) && a.submitEdit(!0)
                                     }
                                     e.stopPropagation()
                                 },
                                 placeholder: "",
                                 minRows: 2
-                            }, b(e, "edit-input"))), g.a.createElement("div", b(e, "edit-icon-container"), g.a.createElement(Je, Object.assign({
+                            }, b(e, "edit-input"))), g.a.createElement("div", b(e, "edit-icon-container"), g.a.createElement(Ze, Object.assign({
                                 className: "edit-cancel"
                             }, b(e, "cancel-icon"), {
                                 onClick: function() {
                                     a.setState({
                                         editMode: !1,
                                         editValue: ""
                                     })
@@ -25288,17 +25288,17 @@
                                     src: r,
                                     namespace: o,
                                     name: o[o.length - 1]
                                 })
                             })
                         }, i.getClippyIcon = function() {
                             var e = i.props.theme;
-                            return i.state.copied ? g.a.createElement("span", null, g.a.createElement(Ze, Object.assign({
+                            return i.state.copied ? g.a.createElement("span", null, g.a.createElement(Je, Object.assign({
                                 className: "copy-icon"
-                            }, b(e, "copy-icon"))), g.a.createElement("span", b(e, "copy-icon-copied"), "✔")) : g.a.createElement(Ze, Object.assign({
+                            }, b(e, "copy-icon"))), g.a.createElement("span", b(e, "copy-icon-copied"), "✔")) : g.a.createElement(Je, Object.assign({
                                 className: "copy-icon"
                             }, b(e, "copy-icon")))
                         }, i.clipboardValue = function(e) {
                             switch (u(e)) {
                                 case "function":
                                 case "regexp":
                                     return e.toString();
@@ -27791,19 +27791,19 @@
                         }), pt.d(dt, "css", function() {
                             return j
                         }), pt.d(dt, "isStyledComponent", function() {
                             return w
                         }), pt.d(dt, "keyframes", function() {
                             return ct
                         }), pt.d(dt, "ServerStyleSheet", function() {
-                            return Ze
+                            return Je
                         }), pt.d(dt, "StyleSheetConsumer", function() {
                             return Qe
                         }), pt.d(dt, "StyleSheetContext", function() {
-                            return Je
+                            return Ze
                         }), pt.d(dt, "StyleSheetManager", function() {
                             return et
                         }), pt.d(dt, "ThemeConsumer", function() {
                             return P
                         }), pt.d(dt, "ThemeContext", function() {
                             return z
                         }), pt.d(dt, "ThemeProvider", function() {
@@ -27896,23 +27896,23 @@
                         var o, E = void 0 !== e && (e.env.REACT_APP_SC_ATTR || e.env.SC_ATTR) || "data-styled",
                             S = "undefined" != typeof window && "HTMLElement" in window,
                             Y = "boolean" == typeof SC_DISABLE_SPEEDY && SC_DISABLE_SPEEDY || void 0 !== e && (e.env.REACT_APP_SC_DISABLE_SPEEDY || e.env.SC_DISABLE_SPEEDY) || !1,
                             K = {},
                             x = (o = Error, c(a, o), a),
                             X = /^[^\S\n]*?\/\* sc-component-id:\s*(\S+)\s+\*\//gm,
                             G = /^\s*\/\/.*$/gm,
-                            Z = new t.a({
+                            J = new t.a({
                                 global: !1,
                                 cascade: !0,
                                 keyframe: !1,
                                 prefix: !1,
                                 compress: !1,
                                 semicolon: !0
                             }),
-                            J = new t.a({
+                            Z = new t.a({
                                 global: !1,
                                 cascade: !0,
                                 keyframe: !1,
                                 prefix: !0,
                                 compress: !1,
                                 semicolon: !1
                             }),
@@ -27926,21 +27926,21 @@
 
                         function a(e) {
                             l(this, a);
                             for (var t = arguments.length, n = Array(1 < t ? t - 1 : 0), r = 1; r < t; r++) n[r - 1] = arguments[r];
                             e = f(this, o.call(this, "An error occurred. See https://github.com/styled-components/styled-components/blob/master/packages/styled-components/src/utils/errors.md#" + e + " for more information." + (0 < n.length ? " Additional arguments: " + n.join(", ") : "")));
                             return f(e)
                         }
-                        J.use([function(e, t, n) {
+                        Z.use([function(e, t, n) {
                             2 === e && n.length && 0 < n[0].lastIndexOf(i) && (n[0] = n[0].replace(ee, q))
-                        }, e, $]), Z.use([e, $]);
+                        }, e, $]), J.use([e, $]);
 
                         function te(e, t, n, r) {
                             r = 3 < arguments.length && void 0 !== r ? r : "&", e = e.join("").replace(G, ""), e = t && n ? n + " " + t + " { " + e + " }" : e;
-                            return Q = r, i = t, ee = new RegExp("\\" + i + "\\b", "g"), J(n || !t ? "" : t, e)
+                            return Q = r, i = t, ee = new RegExp("\\" + i + "\\b", "g"), Z(n || !t ? "" : t, e)
                         }
 
                         function ne(e) {
                             var t, n = "";
                             for (t in e) n += Object.keys(e[t]).join(" ") + " ";
                             return n.trim()
                         }
@@ -28180,15 +28180,15 @@
                                         }
                                         var f = t.length;
                                         if (f) {
                                             for (var d = this.makeTag(null), p = d, h = e, g = t, b = 0, m = g.length; b < m; b += 1) {
                                                 var v = g[b],
                                                     y = v.componentId,
                                                     v = v.cssFromDOM,
-                                                    v = Z("", v);
+                                                    v = J("", v);
                                                 p.insertRules(y, v)
                                             }
                                             for (var w = 0, _ = h.length; w < _; w += 1) {
                                                 var x = h[w];
                                                 x.parentNode && x.parentNode.removeChild(x)
                                             }
                                             this.capacity = Math.max(1, me - f), this.tags.push(d);
@@ -28436,41 +28436,41 @@
                             }, A.prototype.getTheme = function(e, t) {
                                 if (p(e)) return e(t);
                                 if (null === e || Array.isArray(e) || "object" !== (void 0 === e ? "undefined" : W(e))) throw new x(8);
                                 return m({}, t, e)
                             }, A.prototype.getContext = function(e, t) {
                                 return this.getTheme(e, t)
                             }, A),
-                            Ze = (M.prototype.seal = function() {
+                            Je = (M.prototype.seal = function() {
                                 var e;
                                 this.sealed || (e = this.masterSheet.clones.indexOf(this.instance), this.masterSheet.clones.splice(e, 1), this.sealed = !0)
                             }, M.prototype.collectStyles = function(e) {
                                 if (this.sealed) throw new x(2);
                                 return b.a.createElement(et, {
                                     sheet: this.instance
                                 }, e)
                             }, M.prototype.getStyleTags = function() {
                                 return this.seal(), this.instance.toHTML()
                             }, M.prototype.getStyleElement = function() {
                                 return this.seal(), this.instance.toReactElements()
                             }, M.prototype.interleaveWithNodeStream = function(e) {
                                 throw new x(3)
                             }, M),
-                            Je = Object(u.createContext)(),
-                            Qe = Je.Consumer,
+                            Ze = Object(u.createContext)(),
+                            Qe = Ze.Consumer,
                             et = (Ke = u.Component, c(T, Ke), T.prototype.getContext = function(e, t) {
                                 if (e) return e;
                                 if (t) return new h(t);
                                 throw new x(4)
                             }, T.prototype.render = function() {
                                 var e = this.props,
                                     t = e.children,
                                     n = e.sheet,
                                     e = e.target;
-                                return b.a.createElement(Je.Provider, {
+                                return b.a.createElement(Ze.Provider, {
                                     value: this.getContext(n, e)
                                 }, t)
                             }, T),
                             tt = {};
 
                         function T(e) {
                             l(this, T);
@@ -30459,16 +30459,16 @@
                     O = e(36),
                     Y = e(130),
                     E = e(49),
                     S = e(85),
                     K = e(68),
                     X = e(84),
                     G = e(15),
-                    Z = e(229),
-                    J = e(230),
+                    J = e(229),
+                    Z = e(230),
                     Q = e(460),
                     ee = e(90),
                     j = e(42),
                     k = e(124).forEach,
                     C = S("hidden"),
                     te = j.set,
                     ne = j.getterFor("Symbol"),
@@ -30509,15 +30509,15 @@
                         configurable: !0,
                         set: n
                     }), r(t, e)
                 }).prototype, "toString", function() {
                     return ne(this).tag
                 }), O(e, "withoutSetter", function(e) {
                     return r(X(e), e)
-                }), q.f = i, x.f = o, $.f = n, _.f = t, H.f = w.f = a, V.f = s, Z.f = function(e) {
+                }), q.f = i, x.f = o, $.f = n, _.f = t, H.f = w.f = a, V.f = s, J.f = function(e) {
                     return r(G(e), e)
                 }, f && (Y(P, "description", {
                     configurable: !0,
                     get: function() {
                         return ne(this).description
                     }
                 }), U || O(z, "propertyIsEnumerable", i, {
@@ -30527,15 +30527,15 @@
                     constructor: !0,
                     wrap: !0,
                     forced: !d,
                     sham: !d
                 }, {
                     Symbol: e
                 }), k(y(j), function(e) {
-                    J(e)
+                    Z(e)
                 }), l({
                     target: "Symbol",
                     stat: !0,
                     forced: !d
                 }, {
                     useSetter: function() {
                         R = !0
@@ -33420,15 +33420,15 @@
                         bgColor: s,
                         fontSize: l,
                         onChange: f,
                         "data-dash-is-loading": e && e.is_loading || void 0
                     })
                 }
                 var T = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "p", "q", "r", "s", "t", "u", "v", "w", "x", "y", "z"],
-                    D = o(4),
+                    D = o(3),
                     n = o(23),
                     Te = o.n(n),
                     M = Object(ze.forwardRef)(function(e, t) {
                         var n = e.height,
                             s = void 0 === n ? 40 : n,
                             n = e.width,
                             l = void 0 === n ? 100 : n,
@@ -33810,16 +33810,16 @@
                     excludeProps: [],
                     includeProps: [],
                     debug: !1,
                     color: "#29d",
                     zIndex: 99999
                 };
                 var G = W,
-                    Z = o(164),
-                    J = o(165),
+                    J = o(164),
+                    Z = o(165),
                     Q = "undefined" != typeof window ? window : null,
                     ee = null === Q,
                     te = ee ? void 0 : Q.document,
                     ne = ee ? "calc" : ["", "-webkit-", "-moz-", "-o-"].filter(function(e) {
                         var t = te.createElement("div");
                         return t.style.cssText = "width:" + e + "calc(9px)", !!t.style.length
                     }).shift() + "calc",
@@ -34287,19 +34287,19 @@
                 function Be(e) {
                     var t;
                     return e instanceof Element || !!((t = null == (t = null == e ? void 0 : e.ownerDocument) ? void 0 : t.defaultView) && e instanceof t.Element)
                 }
 
                 function Fe(e, t) {
                     var n, r, o, i, a, s, l, c, u, f, d, p;
-                    return void 0 === t && (t = !1), tt.has(e) && !t ? tt.get(e) : Qe(e) ? (tt.set(e, st), st) : (t = getComputedStyle(e), p = Je(e) && e.ownerSVGElement && e.getBBox(), l = !ot && "border-box" === t.boxSizing, n = rt.test(t.writingMode || ""), c = !p && nt.test(t.overflowY || ""), u = !p && nt.test(t.overflowX || ""), r = p ? 0 : it(t.paddingTop), f = p ? 0 : it(t.paddingRight), i = p ? 0 : it(t.paddingBottom), o = p ? 0 : it(t.paddingLeft), a = p ? 0 : it(t.borderTopWidth), d = p ? 0 : it(t.borderRightWidth), s = p ? 0 : it(t.borderBottomWidth), f = o + f, i = r + i, d = (p ? 0 : it(t.borderLeftWidth)) + d, a = a + s, s = u ? e.offsetHeight - a - e.clientHeight : 0, u = c ? e.offsetWidth - d - e.clientWidth : 0, c = l ? f + d : 0, l = l ? i + a : 0, f = (c = p ? p.width : it(t.width) - c - u) + f + u + d, d = (u = p ? p.height : it(t.height) - l - s) + i + s + a, p = Ge({
+                    return void 0 === t && (t = !1), tt.has(e) && !t ? tt.get(e) : Qe(e) ? (tt.set(e, st), st) : (t = getComputedStyle(e), p = Ze(e) && e.ownerSVGElement && e.getBBox(), l = !ot && "border-box" === t.boxSizing, n = rt.test(t.writingMode || ""), c = !p && nt.test(t.overflowY || ""), u = !p && nt.test(t.overflowX || ""), r = p ? 0 : it(t.paddingTop), f = p ? 0 : it(t.paddingRight), i = p ? 0 : it(t.paddingBottom), o = p ? 0 : it(t.paddingLeft), a = p ? 0 : it(t.borderTopWidth), d = p ? 0 : it(t.borderRightWidth), s = p ? 0 : it(t.borderBottomWidth), f = o + f, i = r + i, d = (p ? 0 : it(t.borderLeftWidth)) + d, a = a + s, s = u ? e.offsetHeight - a - e.clientHeight : 0, u = c ? e.offsetWidth - d - e.clientWidth : 0, c = l ? f + d : 0, l = l ? i + a : 0, f = (c = p ? p.width : it(t.width) - c - u) + f + u + d, d = (u = p ? p.height : it(t.height) - l - s) + i + s + a, p = Ge({
                         devicePixelContentBoxSize: at(Math.round(c * devicePixelRatio), Math.round(u * devicePixelRatio), n),
                         borderBoxSize: at(f, d, n),
                         contentBoxSize: at(c, u, n),
-                        contentRect: new Ze(o, r, c, u)
+                        contentRect: new Je(o, r, c, u)
                     }), tt.set(e, p), p)
                 }
 
                 function We(e, t, n) {
                     var r = (e = Fe(e, n)).borderBoxSize,
                         o = e.contentBoxSize,
                         i = e.devicePixelContentBoxSize;
@@ -34340,34 +34340,34 @@
                     for (var n = 0; n < e.length; n += 1)
                         if (e[n].target === t) return n;
                     return -1
                 }
                 var Xe, Ge = function(e) {
                         return Object.freeze(e)
                     },
-                    Ze = (St.prototype.toJSON = function() {
+                    Je = (St.prototype.toJSON = function() {
                         return {
                             x: this.x,
                             y: this.y,
                             top: this.top,
                             right: this.right,
                             bottom: this.bottom,
                             left: this.left,
                             width: this.width,
                             height: this.height
                         }
                     }, St.fromRect = function(e) {
                         return new St(e.x, e.y, e.width, e.height)
                     }, St),
-                    Je = function(e) {
+                    Ze = function(e) {
                         return e instanceof SVGElement && "getBBox" in e
                     },
                     Qe = function(e) {
                         var t, n;
-                        return Je(e) ? (t = (n = e.getBBox()).width, n = n.height, !t && !n) : (t = e.offsetWidth, n = e.offsetHeight, !(t || n || e.getClientRects().length))
+                        return Ze(e) ? (t = (n = e.getBBox()).width, n = n.height, !t && !n) : (t = e.offsetWidth, n = e.offsetHeight, !(t || n || e.getClientRects().length))
                     },
                     et = "undefined" != typeof window ? window : {},
                     tt = new WeakMap,
                     nt = /auto|scroll/,
                     rt = /^tb|vertical/,
                     ot = /msie|trident/i.test(et.navigator && et.navigator.userAgent),
                     it = function(e) {
@@ -34376,15 +34376,15 @@
                     at = function(e, t, n) {
                         return void 0 === e && (e = 0), void 0 === t && (t = 0), new Ue(((n = void 0 === n ? !1 : n) ? t : e) || 0, (n ? e : t) || 0)
                     },
                     st = Ge({
                         devicePixelContentBoxSize: at(),
                         borderBoxSize: at(),
                         contentBoxSize: at(),
-                        contentRect: new Ze(0, 0, 0, 0)
+                        contentRect: new Je(0, 0, 0, 0)
                     }),
                     lt = function() {
                         var o = 1 / 0,
                             t = [];
                         Le.forEach(function(e) {
                             var r;
                             0 !== e.activeTargets.length && (r = [], e.activeTargets.forEach(function(e) {
@@ -34464,15 +34464,15 @@
                         this.stopped || (this.observer && this.observer.disconnect(), pt.forEach(function(e) {
                             return et.removeEventListener(e, t.listener, !0)
                         }), this.stopped = !0)
                     }, new Et),
                     bt = (Ot.prototype.isActive = function() {
                         var e = We(this.target, this.observedBox, !0),
                             t = this.target;
-                        return Je(t) || function(e) {
+                        return Ze(t) || function(e) {
                             switch (e.tagName) {
                                 case "INPUT":
                                     if ("image" !== e.type) break;
                                 case "VIDEO":
                                 case "AUDIO":
                                 case "EMBED":
                                 case "OBJECT":
@@ -35332,34 +35332,34 @@
                         value: n,
                         enumerable: !0,
                         configurable: !0,
                         writable: !0
                     }) : e[t] = n, e
                 }
 
-                function Zt(t, e) {
+                function Jt(t, e) {
                     var n, r = Object.keys(t);
                     return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(t), e && (n = n.filter(function(e) {
                         return Object.getOwnPropertyDescriptor(t, e).enumerable
                     })), r.push.apply(r, n)), r
                 }
 
                 function Pe(t) {
                     for (var e = 1; e < arguments.length; e++) {
                         var n = null != arguments[e] ? arguments[e] : {};
-                        e % 2 ? Zt(Object(n), !0).forEach(function(e) {
+                        e % 2 ? Jt(Object(n), !0).forEach(function(e) {
                             Gt(t, e, n[e])
-                        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(t, Object.getOwnPropertyDescriptors(n)) : Zt(Object(n)).forEach(function(e) {
+                        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(t, Object.getOwnPropertyDescriptors(n)) : Jt(Object(n)).forEach(function(e) {
                             Object.defineProperty(t, e, Object.getOwnPropertyDescriptor(n, e))
                         })
                     }
                     return t
                 }
 
-                function Jt(e, t) {
+                function Zt(e, t) {
                     (null == t || t > e.length) && (t = e.length);
                     for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
                     return r
                 }
 
                 function Qt(e, t) {
                     return function(e) {
@@ -35385,15 +35385,15 @@
                                     if (c) throw o
                                 }
                             }
                             return s
                         }
                     }(e, t) || function(e, t) {
                         var n;
-                        if (e) return "string" == typeof e ? Jt(e, t) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(e).slice(8, -1)) && e.constructor ? e.constructor.name : n) || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Jt(e, t) : void 0
+                        if (e) return "string" == typeof e ? Zt(e, t) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(e).slice(8, -1)) && e.constructor ? e.constructor.name : n) || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Zt(e, t) : void 0
                     }(e, t) || function() {
                         throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                     }()
                 }
 
                 function en(e, t) {
                     if (null == e) return {};
@@ -35932,20 +35932,20 @@
                         function g(t) {
                             H(function(e) {
                                 e = "function" == typeof t ? t(e) : t, Number.isNaN(pe.current) || (e = Math.min(e, pe.current));
                                 e = Math.max(e, 0);
                                 return p.current.scrollTop = e
                             })
                         }
-                        var b, K, X, G, Z, J, Q, ee, m, v, y, o = Object(ze.useRef)({
+                        var b, K, X, G, J, Z, Q, ee, m, v, y, o = Object(ze.useRef)({
                                 start: 0,
                                 end: d.length
                             }),
                             w = Object(ze.useRef)(),
-                            _ = Qt((b = d, K = h, _ = Qt(ze.useState(b), 2), G = _[0], Z = _[1], x = (_ = Qt(ze.useState(null), 2))[0], J = _[1], ze.useEffect(function() {
+                            _ = Qt((b = d, K = h, _ = Qt(ze.useState(b), 2), G = _[0], J = _[1], x = (_ = Qt(ze.useState(null), 2))[0], Z = _[1], ze.useEffect(function() {
                                 var e = function(e, t, n) {
                                     var r, o = e.length,
                                         i = t.length;
                                     if (0 === o && 0 === i) return null;
                                     var a = o < i ? (r = e, t) : (r = t, e),
                                         s = {
                                             __EMPTY_ITEM__: !0
@@ -35962,15 +35962,15 @@
                                         }
                                     }
                                     return null === c ? null : {
                                         index: c,
                                         multiple: u
                                     }
                                 }(G || [], b || [], K);
-                                void 0 !== (null == e ? void 0 : e.index) && (null != X && X(e.index), J(b[e.index])), Z(b)
+                                void 0 !== (null == e ? void 0 : e.index) && (null != X && X(e.index), Z(b[e.index])), J(b)
                             }, [b]), [x]), 1)[0],
                             _ = (w.current = _, Q = h, x = Qt(ze.useState(0), 2), w = x[0], ee = x[1], m = Object(ze.useRef)(new Map), v = Object(ze.useRef)(new Un), y = Object(ze.useRef)(), Object(ze.useEffect)(function() {
                                 return ne
                             }, []), [function(e, t) {
                                 e = Q(e);
                                 m.current.get(e);
                                 t ? (m.current.set(e, t), re()) : m.current.delete(e)
@@ -36181,27 +36181,27 @@
                         loading_state: t.a.shape({
                             is_loading: t.a.bool,
                             prop_name: t.a.string,
                             component_name: t.a.string
                         })
                     }, Kn.defaultProps = {}, Kn),
                     L = o(2),
-                    Zn = (o(338), function(e) {
+                    Jn = (o(338), function(e) {
                         return "function" == typeof e
                     }),
-                    Jn = function(e) {
+                    Zn = function(e) {
                         return "string" == typeof e
                     },
                     Qn = function(e) {
                         return "number" == typeof e
                     },
                     er = !("undefined" == typeof window || !window.document || !window.document.createElement);
 
                 function N(e, t) {
-                    if (er) return e ? Zn(e) ? e() : "current" in e ? e.current : e : t
+                    if (er) return e ? Jn(e) ? e() : "current" in e ? e.current : e : t
                 }
                 var tr = function(e) {
                         var t = Object(ze.useRef)(e);
                         return t.current = e, t
                     },
                     nr = function(e) {
                         var t = tr(e);
@@ -36742,21 +36742,21 @@
                     return xe.a.createElement(Xr, cr({}, e, {
                         colorModel: Gr
                     }))
                 }
 
                 function Br(e) {
                     return xe.a.createElement(Xr, cr({}, e, {
-                        colorModel: Zr
+                        colorModel: Jr
                     }))
                 }
 
                 function Fr(e) {
                     return xe.a.createElement(Yr, cr({}, e, {
-                        colorModel: Jr
+                        colorModel: Zr
                     }))
                 }
 
                 function Wr(e) {
                     var t = e.id,
                         n = e.className,
                         r = e.style,
@@ -36903,24 +36903,24 @@
                     },
                     Gr = {
                         defaultColor: "0001",
                         toHsva: yr,
                         fromHsva: wr,
                         equal: Cr
                     },
-                    Zr = {
+                    Jr = {
                         defaultColor: "rgba(0, 0, 0, 1)",
                         toHsva: Sr,
                         fromHsva: function(e) {
                             e = Er(e);
                             return "rgba(" + e.r + ", " + e.g + ", " + e.b + ", " + e.a + ")"
                         },
                         equal: kr
                     },
-                    Jr = {
+                    Zr = {
                         defaultColor: "rgb(0, 0, 0)",
                         toHsva: r,
                         fromHsva: function(e) {
                             e = Er(e);
                             return "rgb(" + e.r + ", " + e.g + ", " + e.b + ")"
                         },
                         equal: kr
@@ -37332,15 +37332,15 @@
 
                 function Go(t, n) {
                     return function(e) {
                         return null != e && e[t] === n && (void 0 !== n || t in Object(e))
                     }
                 }
 
-                function Zo(t) {
+                function Jo(t) {
                     var n = function(e) {
                         for (var t = $o(e), n = t.length; n--;) {
                             var r = t[n],
                                 o = e[r];
                             t[n] = [r, o, Xo(o)]
                         }
                         return t
@@ -37367,21 +37367,21 @@
                                 }
                             }
                             return !0
                         }(e, t, n)
                     }
                 }
 
-                function Jo(e) {
+                function Zo(e) {
                     return "symbol" == typeof e || Wo(e) && "[object Symbol]" == ao(e)
                 }
 
                 function Qo(e, t) {
                     var n;
-                    return !oi(e) && (!("number" != (n = typeof e) && "symbol" != n && "boolean" != n && null != e && !Jo(e)) || Ai.test(e) || !Mi.test(e) || null != t && e in Object(t))
+                    return !oi(e) && (!("number" != (n = typeof e) && "symbol" != n && "boolean" != n && null != e && !Zo(e)) || Ai.test(e) || !Mi.test(e) || null != t && e in Object(t))
                 }
                 var ei, ti = No,
                     ni = co.a.Uint8Array,
                     i = r ? r.prototype : void 0,
                     ri = i ? i.valueOf : void 0,
                     oi = Array.isArray,
                     ii = Object.prototype.propertyIsEnumerable,
@@ -37494,24 +37494,24 @@
                     }
                     return i.cache = new(Ri.Cache || Do), i
                 }
                 Ri.Cache = Do;
 
                 function Di(e) {
                     var t;
-                    return "string" == typeof e ? e : oi(e) ? no(e, Di) + "" : Jo(e) ? Ki ? Ki.call(e) : "" : "0" == (t = e + "") && 1 / e == -1 / 0 ? "-0" : t
+                    return "string" == typeof e ? e : oi(e) ? no(e, Di) + "" : Zo(e) ? Ki ? Ki.call(e) : "" : "0" == (t = e + "") && 1 / e == -1 / 0 ? "-0" : t
                 }
 
                 function Ii(e, t) {
                     return oi(e) ? e : Qo(e, t) ? [e] : Yi(null == (t = e) ? "" : Di(t))
                 }
 
                 function Li(e) {
                     var t;
-                    return "string" == typeof e || Jo(e) ? e : "0" == (t = e + "") && 1 / e == -1 / 0 ? "-0" : t
+                    return "string" == typeof e || Zo(e) ? e : "0" == (t = e + "") && 1 / e == -1 / 0 ? "-0" : t
                 }
 
                 function Ni(e, t) {
                     for (var n = 0, r = (t = Ii(t, e)).length; null != e && n < r;) e = e[Li(t[n++])];
                     return n && n == r ? e : void 0
                 }
 
@@ -37561,39 +37561,39 @@
                         }), o
                     }, function(e) {
                         return 500 === Vi.size && Vi.clear(), e
                     })).cache, i),
                     a = r ? r.prototype : void 0,
                     Ki = a ? a.toString : void 0,
                     Xi = function(e) {
-                        return "function" == typeof e ? e : null == e ? Wi : "object" == typeof e ? oi(e) ? Fi(e[0], e[1]) : Zo(e) : Hi(e)
+                        return "function" == typeof e ? e : null == e ? Wi : "object" == typeof e ? oi(e) ? Fi(e[0], e[1]) : Jo(e) : Hi(e)
                     },
                     Gi = function(e, t, n) {
                         for (var r = -1, o = Object(e), i = n(e), a = i.length; a--;) {
                             var s = i[++r];
                             if (!1 === t(o[s], s, o)) break
                         }
                         return e
                     },
-                    Zi = function(e, t) {
+                    Ji = function(e, t) {
                         if (null != e) {
                             if (!Oi(e)) return r = t, (n = e) && Gi(n, r, $o);
                             for (var n, r, o = e.length, i = -1, a = Object(e); ++i < o && !1 !== t(a[i], i, a););
                         }
                         return e
                     },
-                    Ji = function(e, r) {
+                    Zi = function(e, r) {
                         var o = -1,
                             i = Oi(e) ? Array(e.length) : [];
-                        return Zi(e, function(e, t, n) {
+                        return Ji(e, function(e, t, n) {
                             i[++o] = r(e, t, n)
                         }), i
                     },
                     Qi = function(e, t) {
-                        return (oi(e) ? no : Ji)(e, Xi(t, 3))
+                        return (oi(e) ? no : Zi)(e, Xi(t, 3))
                     },
                     ea = function() {
                         try {
                             var e = so(Object, "defineProperty");
                             return e({}, "", {}), e
                         } catch (e) {}
                     }(),
@@ -38209,31 +38209,31 @@
                             style: n.slider
                         }))))
                     }
                 }]);
 
                 function Xa(e) {
                     return e && e.slice(0, function(e) {
-                        for (var t = e.length; t-- && Za.test(e.charAt(t)););
+                        for (var t = e.length; t-- && Ja.test(e.charAt(t)););
                         return t
-                    }(e) + 1).replace(Ja, "")
+                    }(e) + 1).replace(Za, "")
                 }
                 t.a.string, t.a.oneOf([0, 1, 2, 3, 4, 5]), t.a.number, t.a.object;
                 var Ga = function() {
                         return co.a.Date.now()
                     },
-                    Za = /\s/,
-                    Ja = /^\s+/,
+                    Ja = /\s/,
+                    Za = /^\s+/,
                     Qa = /^[-+]0x[0-9a-f]+$/i,
                     es = /^0b[01]+$/i,
                     ts = /^0o[0-7]+$/i,
                     ns = parseInt,
                     rs = function(e) {
                         if ("number" == typeof e) return e;
-                        if (Jo(e)) return NaN;
+                        if (Zo(e)) return NaN;
                         if (vo(e) && (t = "function" == typeof e.valueOf ? e.valueOf() : e, e = vo(t) ? t + "" : t), "string" != typeof e) return 0 === e ? e : +e;
                         e = Xa(e);
                         var t = es.test(e);
                         return t || ts.test(e) ? ns(e.slice(2), t ? 2 : 8) : Qa.test(e) ? NaN : +e
                     },
                     os = Math.max,
                     is = Math.min,
@@ -38437,15 +38437,15 @@
                     var t;
                     return "transparent" === e || (t = "#" === String(e).charAt(0) ? 1 : 0, e.length !== 4 + t && e.length < 7 + t && ds()(e).isValid())
                 }
                 var fs = function(e, t) {
                         return (oi(e) ? function(e, t) {
                             for (var n = -1, r = null == e ? 0 : e.length; ++n < r && !1 !== t(e[n], n, e););
                             return e
-                        } : Zi)(e, "function" == typeof(e = t) ? e : Wi)
+                        } : Ji)(e, "function" == typeof(e = t) ? e : Wi)
                     },
                     d = o(74),
                     ds = o.n(d),
                     ps = function(e, t) {
                         var n = e.hex ? ds()(e.hex) : ds()(e),
                             r = n.toHsl(),
                             o = n.toHsv(),
@@ -39482,17 +39482,17 @@
                                 l.r = o, l.g = i, l.b = a
                         }
                         return l.r = Math.round(l.r), l.g = Math.round(l.g), l.b = Math.round(l.b), qs()({}, l, {
                             a: r
                         })
                     },
                     Gs = e => Ys(Xs(e)),
-                    Zs = e => /^#?([A-Fa-f0-9]{3,4}){1,2}$/.test(e),
+                    Js = e => /^#?([A-Fa-f0-9]{3,4}){1,2}$/.test(e),
                     i = o(159),
-                    Js = o.n(i),
+                    Zs = o.n(i),
                     r = o(251),
                     Qs = o.n(r);
 
                 function el(e) {
                     var n = Object(ze.useRef)(e);
                     return Object(ze.useEffect)(() => {
                         n.current = e
@@ -39532,17 +39532,17 @@
                             e(s.current ? "touchmove" : "mousemove", d), e(s.current ? "touchend" : "mouseup", p)
                         }, []), o = (Object(ze.useEffect)(() => (h(l), () => {
                             l && h(!1)
                         }), [l, h]), Object(ze.useCallback)(e => {
                             var t;
                             rl(e.nativeEvent), t = e.nativeEvent, s.current && !nl(t) || (s.current = nl(t), 0) || (f && f(ol(a.current, e.nativeEvent), e.nativeEvent), c(!0))
                         }, [f]));
-                        return Object(il.jsx)("div", Js()({}, e, {
+                        return Object(il.jsx)("div", Zs()({}, e, {
                             className: [n, r || ""].filter(Boolean).join(" "),
-                            style: Js()({}, e.style, {
+                            style: Zs()({}, e.style, {
                                 touchAction: "none"
                             }),
                             ref: a,
                             tabIndex: 0,
                             onMouseDown: o,
                             onTouchStart: o
                         }))
@@ -39784,15 +39784,15 @@
                             style: i,
                             width: u = 200,
                             height: f = 200,
                             direction: a = "anticlockwise",
                             angle: s = 180,
                             color: l,
                             onChange: d
-                        } = e, e = $s()(e, wl), p = "string" == typeof l && Zs(l) ? Ks(l) : l || {}, l = l ? Gs(p) : "", c = function(e) {
+                        } = e, e = $s()(e, wl), p = "string" == typeof l && Js(l) ? Ks(l) : l || {}, l = l ? Gs(p) : "", c = function(e) {
                             var {
                                 cx: t,
                                 cy: n
                             } = ul(e), r = fl(e), o = (180 + dl(e, p.h, !0)) * (cl / 360), r = p.s / 100 * r, e = "clockwise" === e.direction ? -1 : 1;
                             return {
                                 x: t + r * Math.cos(o) * e,
                                 y: n + r * Math.sin(o) * e
@@ -39818,15 +39818,15 @@
                                 }, u - e.x, f - e.y),
                                 e = {
                                     h: e.h,
                                     s: e.s,
                                     v: p.v,
                                     a: p.a
                                 };
-                            d && d(("string" == typeof(e = e) && Zs(e) ? (s = Ks(e), l = e) : "string" != typeof e && (s = e), s && (o = (() => {
+                            d && d(("string" == typeof(e = e) && Js(e) ? (s = Ks(e), l = e) : "string" != typeof e && (s = e), s && (o = (() => {
                                 var {
                                     h: e,
                                     s: t,
                                     v: n
                                 } = s;
                                 return {
                                     h: e,
@@ -40205,15 +40205,15 @@
 
                 function $l(e) {
                     for (var t = [], n = 1; n < arguments.length; n++) t[n - 1] = arguments[n];
                     e && e.removeEventListener && e.removeEventListener.apply(e, t)
                 }
 
                 function ql(b, e, m) {
-                    void 0 === b && (b = 6e4), void 0 === e && (e = !1), void 0 === m && (m = Zl);
+                    void 0 === b && (b = 6e4), void 0 === e && (e = !1), void 0 === m && (m = Jl);
                     var v = (e = Object(ze.useState)(e))[0],
                         y = e[1];
                     return Object(ze.useEffect)(function() {
                         for (var e, a, s, l, c, u, f, d, t = !0, n = v, r = function(e) {
                                 t && y(n = e)
                             }, o = (a = 50, f = !(s = function() {
                                 n && r(!1), clearTimeout(e), e = setTimeout(function() {
@@ -40305,16 +40305,16 @@
                         })
                     }, [a, s]), React.createElement("div", {
                         id: r,
                         "data-dash-is-loading": e && e.is_loading || void 0
                     })
                 }
                 var Gl = "undefined" != typeof window,
-                    Zl = ["mousemove", "mousedown", "resize", "keydown", "touchstart", "wheel"],
-                    Jl = (Yl.propTypes = {
+                    Jl = ["mousemove", "mousedown", "resize", "keydown", "touchstart", "wheel"],
+                    Zl = (Yl.propTypes = {
                         id: t.a.string,
                         isIdle: t.a.bool,
                         waitDuration: t.a.number,
                         setProps: t.a.func,
                         loading_state: t.a.shape({
                             is_loading: t.a.bool,
                             prop_name: t.a.string,
@@ -40511,15 +40511,15 @@
                         d = tr(t),
                         p = tr(e);
                     nc(function() {
                         var e, t, n, a = N(c, window);
                         if (a) {
                             var s = function(e) {
                                 var t, n, r;
-                                return n = p.current, r = u, !(Zn(n) ? n : Jn(n) || Qn(n) ? function(e) {
+                                return n = p.current, r = u, !(Jn(n) ? n : Zn(n) || Qn(n) ? function(e) {
                                     return ic(e, n, r)
                                 } : Array.isArray(n) ? function(t) {
                                     return n.some(function(e) {
                                         return ic(t, e, r)
                                     })
                                 } : function() {
                                     return Boolean(n)
@@ -41535,15 +41535,15 @@
                     Vc = e.containerId || e, $c.set(Vc, e), qc.forEach(e => {
                         Rc.emit(0, e.content, e.options)
                     }), qc = []
                 }).on(3, e => {
                     $c.delete(e.containerId || e), 0 === $c.size && Rc.off(0).off(1).off(5)
                 }), o(444);
 
-                function Zc(e) {
+                function Jc(e) {
                     var t = e.id,
                         n = e.children,
                         r = e.key,
                         o = e.className,
                         i = e.style,
                         a = e.type,
                         s = e.visible,
@@ -41595,15 +41595,15 @@
                         containerId: _,
                         enableMultiContainer: !0,
                         limit: x,
                         theme: O,
                         "data-dash-is-loading": e && e.is_loading || void 0
                     })
                 }
-                Zc.propTypes = {
+                Jc.propTypes = {
                     children: t.a.node,
                     id: t.a.string,
                     key: t.a.string,
                     className: t.a.string,
                     style: t.a.object,
                     type: t.a.oneOf(["info", "success", "warning", "error"]),
                     visible: t.a.bool,
@@ -41625,19 +41625,19 @@
                     theme: t.a.oneOf(["light", "dark", "colored"]),
                     setProps: t.a.func,
                     loading_state: t.a.shape({
                         is_loading: t.a.bool,
                         prop_name: t.a.string,
                         component_name: t.a.string
                     })
-                }, Zc.defaultProps = {
+                }, Jc.defaultProps = {
                     visible: !0,
                     closable: !0
                 };
-                var Jc = Zc,
+                var Zc = Jc,
                     Qc = Object.defineProperty,
                     eu = Object.getOwnPropertySymbols,
                     tu = Object.prototype.hasOwnProperty,
                     nu = Object.prototype.propertyIsEnumerable,
                     ru = (e, t, n) => t in e ? Qc(e, t, {
                         enumerable: !0,
                         configurable: !0,
@@ -42548,15 +42548,15 @@
                             var e = Gu[t].indexOf(n);
                             Gu[t].splice(e, 1)
                         }
                 }
                 var Ku = new Map,
                     Xu = new Map,
                     Gu = {},
-                    Zu = function(r, e) {
+                    Ju = function(r, e) {
                         function o(e, t) {
                             var n, r, o, i, a;
                             l ? l(t) : (r = e, o = s, i = t, a = void(null != (a = Ku.get(r)) && a.timer && clearTimeout(a.timer)), -1 < o && (a = setTimeout(function() {
                                 Ku.delete(r)
                             }, o)), Ku.set(r, Object(L.a)(Object(L.a)({}, i), {
                                 timer: a
                             }))), n = t.data, Gu[e] && Gu[e].forEach(function(e) {
@@ -42632,28 +42632,28 @@
                                         data: e
                                     })
                                 }))
                             }
                         } : {}
                     },
                     a = o(153),
-                    Ju = o.n(a),
+                    Zu = o.n(a),
                     Qu = function(t, e) {
                         var n = e.debounceWait,
                             r = e.debounceLeading,
                             o = e.debounceTrailing,
                             i = e.debounceMaxWait,
                             a = Object(ze.useRef)(),
                             s = Object(ze.useMemo)(function() {
                                 var e = {};
                                 return void 0 !== r && (e.leading = r), void 0 !== o && (e.trailing = o), void 0 !== i && (e.maxWait = i), e
                             }, [r, o, i]);
                         return Object(ze.useEffect)(function() {
                             var o;
-                            if (n) return o = t.runAsync.bind(t), a.current = Ju()(function(e) {
+                            if (n) return o = t.runAsync.bind(t), a.current = Zu()(function(e) {
                                     e()
                                 }, n, s), t.runAsync = function() {
                                     for (var r = [], e = 0; e < arguments.length; e++) r[e] = arguments[e];
                                     return new Promise(function(e, t) {
                                         var n;
                                         null != (n = a.current) && n.call(a, function() {
                                             o.apply(void 0, Object(L.g)([], Object(L.e)(r), !1)).then(e).catch(t)
@@ -42883,15 +42883,15 @@
                             loading: !1
                         }), this.runPluginHandler("onCancel")
                     }, ff.prototype.refresh = function() {
                         this.run.apply(this, Object(L.g)([], Object(L.e)(this.state.params || []), !1))
                     }, ff.prototype.refreshAsync = function() {
                         return this.runAsync.apply(this, Object(L.g)([], Object(L.e)(this.state.params || []), !1))
                     }, ff.prototype.mutate = function(e) {
-                        e = Zn(e) ? e(this.state.data) : e;
+                        e = Jn(e) ? e(this.state.data) : e;
                         this.runPluginHandler("onMutate", e), this.setState({
                             data: e
                         })
                     }, ff);
 
                 function ff(e, t, n, r) {
                     void 0 === r && (r = {}), this.serviceRef = e, this.options = t, this.subscribe = n, this.initState = r, this.count = 0, this.state = {
@@ -42901,15 +42901,15 @@
                         error: void 0
                     }, this.state = Object(L.a)(Object(L.a)(Object(L.a)({}, this.state), {
                         loading: !t.manual
                     }), r)
                 }
 
                 function df(e, t, n) {
-                    return pf(e, t, Object(L.g)(Object(L.g)([], Object(L.e)(n || []), !1), [Qu, ef, rf, af, cf, $u, Zu, sf], !1))
+                    return pf(e, t, Object(L.g)(Object(L.g)([], Object(L.e)(n || []), !1), [Qu, ef, rf, af, cf, $u, Ju, sf], !1))
                 }
                 var pf = function(e, t, n) {
                     void 0 === n && (n = []);
                     var r, o, i = (t = void 0 === t ? {} : t).manual,
                         a = void 0 !== i && i,
                         i = Object(L.f)(t, ["manual"]),
                         s = Object(L.a)({
@@ -43505,16 +43505,16 @@
                         s = 0;
                     return function() {
                         o = this, i = arguments, s = s || $f()(n)
                     }
                 }
                 var Xf = Af.connections,
                     Gf = Af.EE,
-                    Zf = Af.listeners,
-                    Jf = Af.removers,
+                    Jf = Af.listeners,
+                    Zf = Af.removers,
                     i = void 0,
                     Tf = void 0,
                     d = void 0,
                     Qf = 0;
 
                 function ed(e) {
                     return e.id || "target-id-" + Qf++
@@ -43523,18 +43523,18 @@
                 function td(t, n, r, o) {
                     return Gf.on(t, n || Nf.a, r), Xf[o = o || t] = (Xf[o] || 0) + 1, {
                         _type: t,
                         _cb: n,
                         _ctx: r,
                         unsubscribe: function() {
                             if (this._type) {
-                                Gf.removeListener(t, n, r), Xf[o]--, 0 === Xf[o] && (Zf[o].remove(), Zf[o] = void 0), this._type = void 0, this._cb = void 0, this._ctx = void 0;
-                                for (var e = Jf.length - 1; 0 <= e; e--)
-                                    if (Jf[e] === this) {
-                                        Jf.splice(e, 1);
+                                Gf.removeListener(t, n, r), Xf[o]--, 0 === Xf[o] && (Jf[o].remove(), Jf[o] = void 0), this._type = void 0, this._cb = void 0, this._ctx = void 0;
+                                for (var e = Zf.length - 1; 0 <= e; e--)
+                                    if (Zf[e] === this) {
+                                        Zf.splice(e, 1);
                                         break
                                     }
                             }
                         }
                     }
                 }
 
@@ -43544,27 +43544,27 @@
                             n = n.target,
                             s = n && ed(n),
                             s = s ? ":" + s : "",
                             l = h + "Start:" + t + s,
                             c = h + "End:" + t + s,
                             u = h + ":" + t + s,
                             s = td(g + ":" + t + s, e, a, u);
-                        return Jf.push(s), Zf[u] || (o = {
+                        return Zf.push(s), Jf[u] || (o = {
                             start: new Vf({
                                 mainType: h,
                                 subType: "start"
                             }),
                             main: new Vf({
                                 mainType: h
                             }),
                             end: new Vf({
                                 mainType: h,
                                 subType: "end"
                             })
-                        }, i = void("raf" === t ? (t = 16, d = Kf(d)) : 0 < t && (d = lf()(d, t))), Zf[u] = Mf(n || p, h, d, r)), s;
+                        }, i = void("raf" === t ? (t = 16, d = Kf(d)) : 0 < t && (d = lf()(d, t))), Jf[u] = Mf(n || p, h, d, r)), s;
 
                         function f(e) {
                             o.end.update(e), Gf.emit(c, e, o.end), i = null
                         }
 
                         function d(e) {
                             i || (o.start.update(e), Gf.emit(l, e, o.start)), clearTimeout(i), o.main.update(e), Gf.emit(u, e, o.main), i = If ? setTimeout(function() {
@@ -43577,17 +43577,17 @@
                 function rd(l, c) {
                     return function(e, t, n, r) {
                         var o, i = n.context,
                             n = n.target,
                             a = n && ed(n),
                             s = c + ":0" + (a ? ":" + a : ""),
                             a = td(s, t, i);
-                        return Jf.push(a), Zf[s] || (o = new Vf({
+                        return Zf.push(a), Jf[s] || (o = new Vf({
                             mainType: c
-                        }), Zf[s] = Mf(n || l, c, function(e) {
+                        }), Jf[s] = Mf(n || l, c, function(e) {
                             o.update(e), Gf.emit(s, e, o)
                         }, r)), a
                     }
                 }
                 "undefined" != typeof window && (d = (i = (Tf = window).document || document).body);
                 var od = {
                     scrollStart: nd(Tf, "scroll", "scrollStart"),
@@ -43692,27 +43692,33 @@
                         "data-dash-is-loading": e && e.is_loading || void 0
                     }, n)
                 }
 
                 function gd(e) {
                     var t = e.id,
                         n = e.data,
-                        r = e.setProps,
+                        r = e.initialSync,
+                        o = e.setProps,
                         e = e.loading_state;
                     return Object(ze.useEffect)(function() {
                         function e(e) {
-                            e.triggerKey === t && (e = sessionStorage.getItem(t)) && r({
+                            e.triggerKey === t && (e = sessionStorage.getItem(t)) && o({
                                 data: JSON.parse(e)
                             })
                         }
                         return window.addEventListener("sessionStorageSetItem", e),
                             function() {
                                 window.removeEventListener("sessionStorageSetItem", e)
                             }
                     }, []), Object(ze.useEffect)(function() {
+                        var e;
+                        r && (e = sessionStorage.getItem(t)) && o({
+                            data: JSON.parse(e)
+                        })
+                    }, []), Object(ze.useEffect)(function() {
                         Object(D.isUndefined)(n) || sessionStorage.setItem(t, JSON.stringify(n))
                     }, [n]), xe.a.createElement("div", {
                         id: t,
                         "data-dash-is-loading": e && e.is_loading || void 0
                     })
                 }
                 var bd, md, vd, yd, wd, _d = "transform",
@@ -43970,21 +43976,24 @@
                     }, hd.defaultProps = {
                         enabled: !0,
                         top: 0
                     }, hd);
                 gd.propTypes = {
                     id: t.a.string.isRequired,
                     data: t.a.any,
+                    initialSync: t.a.bool,
                     loading_state: t.a.shape({
                         is_loading: t.a.bool,
                         prop_name: t.a.string,
                         component_name: t.a.string
                     }),
                     setProps: t.a.func
-                }, gd.defaultProps = {};
+                }, gd.defaultProps = {
+                    initialSync: !1
+                };
 
                 function kd(e) {
                     var t, n, r, o, i, a, s, l, c, u, f, d, p, h, g, b, m, v, y, w = e.id,
                         _ = e.socketUrl,
                         x = e.reconnectLimit,
                         O = e.reconnectInterval,
                         E = e.operation,
@@ -44533,18 +44542,18 @@
                         editable: !1,
                         addible: !1,
                         deletable: !1,
                         sortKeys: !1,
                         quotesOnKeys: !0,
                         displayArrayKey: !0
                     }, Wd),
-                    Zd = o(269);
+                    Jd = o(269);
 
-                function Jd(e) {
-                    return (Jd = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                function Zd(e) {
+                    return (Zd = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                     })(e)
                 }
 
                 function Qd() {
@@ -44666,15 +44675,15 @@
                         var t;
                         c(this, "_invoke", {
                             value: function(n, r) {
                                 function e() {
                                     return new s(function(e, t) {
                                         ! function t(e, n, r, o) {
                                             var i, e = u(a[e], a, n);
-                                            return "throw" !== e.type ? (n = (i = e.arg).value) && "object" == Jd(n) && l.call(n, "__await") ? s.resolve(n.__await).then(function(e) {
+                                            return "throw" !== e.type ? (n = (i = e.arg).value) && "object" == Zd(n) && l.call(n, "__await") ? s.resolve(n.__await).then(function(e) {
                                                 t("next", e, r, o)
                                             }, function(e) {
                                                 t("throw", e, r, o)
                                             }) : s.resolve(n).then(function(e) {
                                                 i.value = e, r(i)
                                             }, function(e) {
                                                 return t("throw", e, r, o)
@@ -44910,15 +44919,15 @@
                                 }.apply(this, arguments)
                             }
                         }(), []);
                     return xe.a.createElement("div", {
                         id: t,
                         key: n,
                         "data-dash-is-loading": e && e.is_loading || void 0
-                    }, xe.a.createElement(Zd.Gluejar, {
+                    }, xe.a.createElement(Jd.Gluejar, {
                         onPaste: function(e) {
                             r || i(e)
                         },
                         onError: function() {
                             return null
                         },
                         container: document.querySelector("#container")
@@ -45327,16 +45336,16 @@
                     },
                     Kp = {
                         ...qp,
                         default: 1
                     },
                     Xp = e => Math.round(1e5 * e) / 1e5,
                     Gp = /(-)?([\d]*\.?[\d])+/g,
-                    Zp = /(#[0-9a-f]{3,8}|(rgb|hsl)a?\((-?[\d\.]+%?[,\s]+){2}(-?[\d\.]+%?)\s*[\,\/]?\s*[\d\.]*%?\))/gi,
-                    Jp = /^(#[0-9a-f]{3,8}|(rgb|hsl)a?\((-?[\d\.]+%?[,\s]+){2}(-?[\d\.]+%?)\s*[\,\/]?\s*[\d\.]*%?\))$/i;
+                    Jp = /(#[0-9a-f]{3,8}|(rgb|hsl)a?\((-?[\d\.]+%?[,\s]+){2}(-?[\d\.]+%?)\s*[\,\/]?\s*[\d\.]*%?\))/gi,
+                    Zp = /^(#[0-9a-f]{3,8}|(rgb|hsl)a?\((-?[\d\.]+%?[,\s]+){2}(-?[\d\.]+%?)\s*[\,\/]?\s*[\d\.]*%?\))$/i;
 
                 function Qp(e) {
                     return "string" == typeof e
                 }
                 const eh = t => ({
                         test: e => Qp(e) && e.endsWith(t) && 1 === e.split(" ").length,
                         parse: parseFloat,
@@ -45773,18 +45782,18 @@
                     Yh = (...e) => e.reduce(qh),
                     Kh = new WeakMap,
                     Xh = new WeakMap,
                     Gh = e => {
                         var t = Kh.get(e.target);
                         t && t(e)
                     },
-                    Zh = e => {
+                    Jh = e => {
                         e.forEach(Gh)
                     };
-                const Jh = {
+                const Zh = {
                     some: 0,
                     all: 1
                 };
 
                 function Qh(s, l, c, {
                     root: u,
                     margin: f,
@@ -45792,25 +45801,25 @@
                     once: p
                 }) {
                     Object(ze.useEffect)(() => {
                         if (s && c.current) {
                             var e, t, n, r = {
                                 root: null == u ? void 0 : u.current,
                                 rootMargin: f,
-                                threshold: "number" == typeof d ? d : Jh[d]
+                                threshold: "number" == typeof d ? d : Zh[d]
                             }; {
                                 var o = c.current,
                                     i = e => {
                                         var t, n = e["isIntersecting"];
                                         l.isInView !== n && (l.isInView = n, !p || n || !l.hasEnteredView) && (n && (l.hasEnteredView = !0), c.animationState && c.animationState.setActive(v.InView, n), t = c.getProps(), n = n ? t.onViewportEnter : t.onViewportLeave) && n(e)
                                     };
                                 ({
                                     root: r,
                                     ...e
-                                } = r), t = r || document, Xh.has(t) || Xh.set(t, {}), t = Xh.get(t), n = JSON.stringify(e), t[n] || (t[n] = new IntersectionObserver(Zh, {
+                                } = r), t = r || document, Xh.has(t) || Xh.set(t, {}), t = Xh.get(t), n = JSON.stringify(e), t[n] || (t[n] = new IntersectionObserver(Jh, {
                                     root: r,
                                     ...e
                                 }));
                                 const a = t[n];
                                 return Kh.set(o, i), a.observe(o), () => {
                                     Kh.delete(o), a.unobserve(o)
                                 }
@@ -46089,15 +46098,15 @@
                         this.clearListeners(), this.stop(), this.stopPassiveEffect && this.stopPassiveEffect()
                     }
                 }
 
                 function _0(e, t) {
                     return new w0(e, t)
                 }
-                const x0 = (t, n) => e => Boolean(Qp(e) && Jp.test(e) && e.startsWith(t) || n && Object.prototype.hasOwnProperty.call(e, n)),
+                const x0 = (t, n) => e => Boolean(Qp(e) && Zp.test(e) && e.startsWith(t) || n && Object.prototype.hasOwnProperty.call(e, n)),
                     O0 = (i, a, s) => e => {
                         var t, n, r, o;
                         return Qp(e) ? ([t, n, r, o] = e.match(Gp), {
                             [i]: parseFloat(t),
                             [a]: parseFloat(n),
                             [s]: parseFloat(r),
                             alpha: void 0 !== o ? parseFloat(o) : 1
@@ -46151,16 +46160,16 @@
                         transform: e => Qp(e) ? e : (e.hasOwnProperty("red") ? S0 : k0).transform(e)
                     };
 
                 function z0(e) {
                     var t = [];
                     let n = 0,
                         r = 0;
-                    var o = (e = "number" == typeof e ? "" + e : e).match(Zp),
-                        o = (o && (n = o.length, e = e.replace(Zp, "${c}"), t.push(...o.map(C0.parse))), e.match(Gp));
+                    var o = (e = "number" == typeof e ? "" + e : e).match(Jp),
+                        o = (o && (n = o.length, e = e.replace(Jp, "${c}"), t.push(...o.map(C0.parse))), e.match(Gp));
                     return o && (r = o.length, e = e.replace(Gp, "${n}"), t.push(...o.map(qp.parse))), {
                         values: t,
                         numColors: n,
                         numNumbers: r,
                         tokenised: e
                     }
                 }
@@ -46181,15 +46190,15 @@
                         return n
                     }
                 }
                 const M0 = e => "number" == typeof e ? 0 : e,
                     A0 = {
                         test: function(e) {
                             var t;
-                            return isNaN(e) && Qp(e) && 0 < ((null == (t = e.match(Gp)) ? void 0 : t.length) || 0) + ((null == (t = e.match(Zp)) ? void 0 : t.length) || 0)
+                            return isNaN(e) && Qp(e) && 0 < ((null == (t = e.match(Gp)) ? void 0 : t.length) || 0) + ((null == (t = e.match(Jp)) ? void 0 : t.length) || 0)
                         },
                         parse: P0,
                         createTransformer: T0,
                         getAnimatableNone: function(e) {
                             var t = P0(e);
                             return T0(e)(t.map(M0))
                         }
@@ -46268,19 +46277,19 @@
 
                 function Y0(e) {
                     return Boolean(Bp(e) && e.add)
                 }
                 const K0 = "data-" + wh("framerAppearId");
                 var X0 = o(11);
                 const G0 = e => 1e3 * e,
-                    Z0 = t => e => e <= .5 ? t(2 * e) / 2 : (2 - t(2 * (1 - e))) / 2,
-                    J0 = t => e => 1 - t(1 - e),
+                    J0 = t => e => e <= .5 ? t(2 * e) / 2 : (2 - t(2 * (1 - e))) / 2,
+                    Z0 = t => e => 1 - t(1 - e),
                     Q0 = e => e * e,
-                    eg = J0(Q0),
-                    tg = Z0(Q0),
+                    eg = Z0(Q0),
+                    tg = J0(Q0),
                     y = (e, t, n) => -n * e + n * t + e;
 
                 function ng(e, t, n) {
                     return n < 0 && (n += 1), 1 < n && --n, n < 1 / 6 ? e + 6 * (t - e) * n : n < .5 ? t : n < 2 / 3 ? e + (t - e) * (2 / 3 - n) * 6 : e
                 }
                 const rg = (e, t, n) => {
                         e *= e;
@@ -46406,19 +46415,19 @@
                             let e, t, n = 0;
                             for (; t = i + (a - i) / 2, 0 < (e = gg(t, s, l) - o) ? a = t : i = t, 1e-7 < Math.abs(e) && ++n < 12;);
                             return t
                         }
                     })(e), t, n)
                 }
                 const mg = e => 1 - Math.sin(Math.acos(e)),
-                    vg = J0(mg),
-                    yg = Z0(vg),
+                    vg = Z0(mg),
+                    yg = J0(vg),
                     wg = bg(.33, 1.53, .69, .99),
-                    _g = J0(wg),
-                    xg = Z0(_g),
+                    _g = Z0(wg),
+                    xg = J0(_g),
                     Og = {
                         linear: hg,
                         easeIn: Q0,
                         easeInOut: tg,
                         easeOut: eg,
                         circIn: mg,
                         circInOut: yg,
@@ -46847,31 +46856,31 @@
                     },
                     Xg = (e, t) => !("zIndex" === e || "number" != typeof t && !Array.isArray(t) && ("string" != typeof t || !A0.test(t) || t.startsWith("url(")));
 
                 function Gg(e) {
                     return 0 === e || "string" == typeof e && 0 === parseFloat(e) && -1 === e.indexOf(" ")
                 }
 
-                function Zg(e) {
+                function Jg(e) {
                     return "number" == typeof e ? 0 : B0("", e)
                 }
 
-                function Jg(e, t) {
+                function Zg(e, t) {
                     return e[t] || e.default || e
                 }
                 const Qg = (L, N, U, B = {}) => e => {
-                    const t = Jg(B, L) || {},
+                    const t = Zg(B, L) || {},
                         n = t.delay || B.delay || 0;
                     var r, o, i, a, s, l, c, u, f, d, p, h, g, {
                             elapsed: b = 0
                         } = B,
                         m = (b -= G0(n), function(e, t, n, r) {
                             var o = Xg(t, n);
                             let i = void 0 !== r.from ? r.from : e.get();
-                            return "none" === i && o && "string" == typeof n ? i = B0(t, n) : Gg(i) && "string" == typeof n ? i = Zg(n) : !Array.isArray(n) && Gg(n) && "string" == typeof i && (n = Zg(i)), Array.isArray(n) ? (null === n[0] && (n[0] = i), n) : [i, n]
+                            return "none" === i && o && "string" == typeof n ? i = B0(t, n) : Gg(i) && "string" == typeof n ? i = Jg(n) : !Array.isArray(n) && Gg(n) && "string" == typeof i && (n = Jg(i)), Array.isArray(n) ? (null === n[0] && (n[0] = i), n) : [i, n]
                         }(N, L, U, t)),
                         v = m[0],
                         y = m[m.length - 1],
                         w = Xg(L, v),
                         _ = Xg(L, y);
                     Object(X0.warning)(w === _, `You are trying to animate ${L} from "${v}" to "${y}". ${v} is not an animatable value - to enable this animation set ${v} to a value animatable to ${y} via the \`style\` property.`);
                     let x = {
@@ -47802,16 +47811,16 @@
 
                 function Gb(e, t, n = 1) {
                     Object(X0.invariant)(n <= 4, `Max CSS variable fallback depth detected in property "${e}". This may indicate a circular fallback dependency.`);
                     e = e;
                     var [e, r] = (e = Xb.exec(e)) ? ([, e, r] = e, [e, r]) : [, ];
                     if (e) return (e = window.getComputedStyle(t).getPropertyValue(e)) ? e.trim() : Kb(r) ? Gb(r, t, n + 1) : r
                 }
-                const Zb = new Set(["width", "height", "top", "left", "right", "bottom", "x", "y"]),
-                    Jb = e => Zb.has(e),
+                const Jb = new Set(["width", "height", "top", "left", "right", "bottom", "x", "y"]),
+                    Zb = e => Jb.has(e),
                     Qb = e => e === qp || e === m,
                     em = (0, (e, t) => parseFloat(e.split(", ")[t])),
                     tm = (r, o) => (e, {
                         transform: t
                     }) => {
                         if ("none" === t || !t) return 0;
                         var n = t.match(/^matrix3d\((.+)\)$/);
@@ -47856,15 +47865,15 @@
                     },
                     im = (a, s, l = {}, c = {}) => {
                         s = {
                             ...s
                         }, c = {
                             ...c
                         };
-                        const e = Object.keys(s).filter(Jb);
+                        const e = Object.keys(s).filter(Zb);
                         let u = [],
                             f = !1;
                         const d = [];
                         if (e.forEach(r => {
                                 var o = a.getValue(r);
                                 if (a.hasValue(r)) {
                                     let e = l[r],
@@ -47937,15 +47946,15 @@
                                 }
                             }
                             return {
                                 target: t,
                                 transitionEnd: n
                             }
                         }(e, t, r);
-                        return e = e, t = t = o.target, n = n, o = r = o.transitionEnd, Object.keys(t).some(Jb) ? im(e, t, n, o) : {
+                        return e = e, t = t = o.target, n = n, o = r = o.transitionEnd, Object.keys(t).some(Zb) ? im(e, t, n, o) : {
                             target: t,
                             transitionEnd: o
                         }
                     },
                     sm = {
                         current: null
                     },
@@ -48626,15 +48635,15 @@
                                                 onLayoutAnimationComplete: s
                                             } = c.getProps(),
                                             l = !this.targetLayout || !Um(this.targetLayout, r) || n,
                                             n = !t && n;
                                         if (this.options.layoutRoot || null != (o = this.resumeFrom) && o.instance || n || t && (l || !this.currentAnimation)) {
                                             this.resumeFrom && (this.resumingFrom = this.resumeFrom, this.resumingFrom.resumingFrom = void 0), this.setAnimationOrigin(e, n);
                                             const t = {
-                                                ...Jg(i, "layout"),
+                                                ...Zg(i, "layout"),
                                                 onPlay: a,
                                                 onComplete: s
                                             };
                                             (c.shouldReduceMotion || this.options.layoutRoot) && (t.delay = 0, t.type = !1), this.startAnimation(t)
                                         } else t || 0 !== this.animationProgress || ev(this), !this.isLead() || null != (l = (o = this.options).onExitComplete) && l.call(o);
                                         this.targetLayout = r
                                     }
@@ -48678,18 +48687,18 @@
                                     layoutId: t,
                                     layout: n
                                 } = this.options;
                                 (void 0 !== t || n) && (this.prevTransformTemplateValue = null == (t = this.getTransformTemplate()) ? void 0 : t(this.latestValues, ""), this.updateSnapshot(), e) && this.notifyListeners("willUpdate")
                             }
                         }
                         didUpdate() {
-                            this.isUpdateBlocked() ? (this.unblockUpdate(), this.clearAllSnapshots(), this.nodes.forEach(Jm)) : this.isUpdating && (this.isUpdating = !1, this.potentialNodes.size && (this.potentialNodes.forEach(cv), this.potentialNodes.clear()), this.nodes.forEach(Qm), this.nodes.forEach(Km), this.nodes.forEach(Xm), this.clearAllSnapshots(), d0.update(), d0.preRender(), d0.render())
+                            this.isUpdateBlocked() ? (this.unblockUpdate(), this.clearAllSnapshots(), this.nodes.forEach(Zm)) : this.isUpdating && (this.isUpdating = !1, this.potentialNodes.size && (this.potentialNodes.forEach(cv), this.potentialNodes.clear()), this.nodes.forEach(Qm), this.nodes.forEach(Km), this.nodes.forEach(Xm), this.clearAllSnapshots(), d0.update(), d0.preRender(), d0.render())
                         }
                         clearAllSnapshots() {
-                            this.nodes.forEach(Zm), this.sharedNodes.forEach(ov)
+                            this.nodes.forEach(Jm), this.sharedNodes.forEach(ov)
                         }
                         scheduleUpdateProjection() {
                             u0.preRender(this.updateProjection, !1, !0)
                         }
                         scheduleCheckAfterUnmount() {
                             u0.postRender(() => {
                                 this.isLayoutDirty ? this.root.didUpdate() : this.root.checkUpdateFailed()
@@ -49182,15 +49191,15 @@
                         }
                         clearSnapshot() {
                             this.resumeFrom = this.snapshot = void 0
                         }
                         resetTree() {
                             this.root.nodes.forEach(e => {
                                 return null == (e = e.currentAnimation) ? void 0 : e.stop()
-                            }), this.root.nodes.forEach(Jm), this.root.sharedNodes.clear()
+                            }), this.root.nodes.forEach(Zm), this.root.sharedNodes.clear()
                         }
                     }
                 }
 
                 function Km(e) {
                     e.updateLayout()
                 }
@@ -49282,19 +49291,19 @@
                     t.options.transition = void 0
                 }
 
                 function Gm(e) {
                     e.isProjectionDirty || (e.isProjectionDirty = Boolean(e.parent && e.parent.isProjectionDirty)), e.isTransformDirty || (e.isTransformDirty = Boolean(e.parent && e.parent.isTransformDirty))
                 }
 
-                function Zm(e) {
+                function Jm(e) {
                     e.clearSnapshot()
                 }
 
-                function Jm(e) {
+                function Zm(e) {
                     e.clearMeasurements()
                 }
 
                 function Qm(e) {
                     var t = e.options["visualElement"];
                     null != t && t.getProps().onBeforeLayoutMeasure && t.notify("BeforeLayoutMeasure"), e.resetTransform()
                 }
@@ -49944,25 +49953,25 @@
                             }
                     }, [s]), React.createElement("div", {
                         id: t,
                         "data-dash-is-loading": e && e.is_loading || void 0
                     })
                 }
 
-                function Zv(r) {
+                function Jv(r) {
                     var e = window.history,
                         o = e[r];
                     e[r] = function(e) {
                         var t = o.apply(this, arguments),
                             n = new Event(r.toLowerCase());
                         return n.state = e, window.dispatchEvent(n), t
                     }
                 }
 
-                function Jv(e) {
+                function Zv(e) {
                     var t = (n = window.history).state,
                         n = n.length,
                         r = window.location;
                     return {
                         trigger: e,
                         state: t,
                         length: n,
@@ -50105,30 +50114,30 @@
                             prop_name: t.a.string,
                             component_name: t.a.string
                         })
                     }, Gv.defaultProps = {
                         pasteCount: 0,
                         enableListenPaste: !1
                     }, Gv),
-                    a = (Gl && (Zv("pushState"), Zv("replaceState")), "function" == typeof Event),
+                    a = (Gl && (Jv("pushState"), Jv("replaceState")), "function" == typeof Event),
                     ly = Gl && a ? function() {
-                        var e = Object(ze.useState)(Jv("load")),
+                        var e = Object(ze.useState)(Zv("load")),
                             t = e[0],
                             r = e[1];
                         return Object(ze.useEffect)(function() {
                             function e() {
-                                return r(Jv("popstate"))
+                                return r(Zv("popstate"))
                             }
 
                             function t() {
-                                return r(Jv("pushstate"))
+                                return r(Zv("pushstate"))
                             }
 
                             function n() {
-                                return r(Jv("replacestate"))
+                                return r(Zv("replacestate"))
                             }
                             return Vl(window, "popstate", e), Vl(window, "pushstate", t), Vl(window, "replacestate", n),
                                 function() {
                                     $l(window, "popstate", e), $l(window, "pushstate", t), $l(window, "replacestate", n)
                                 }
                         }, []), t
                     } : function() {
@@ -50177,18 +50186,18 @@
                     n = a, void 0 === (r = {
                         defaultValue: s,
                         expires: c && new Date(+new Date + 1e3 * c),
                         path: u,
                         secure: f
                     }) && (r = {}), a = Object(L.e)(Object(ze.useState)(function() {
                         var e = uy.a.get(n);
-                        return Jn(e) ? e : Zn(r.defaultValue) ? r.defaultValue() : r.defaultValue
+                        return Zn(e) ? e : Jn(r.defaultValue) ? r.defaultValue() : r.defaultValue
                     }), 2), o = a[0], i = a[1], a = fc(function(e, t) {
                         void 0 === t && (t = {});
-                        t = Object(L.a)(Object(L.a)({}, r), t), t.defaultValue, t = Object(L.f)(t, ["defaultValue"]), e = Zn(e) ? e(o) : e;
+                        t = Object(L.a)(Object(L.a)({}, r), t), t.defaultValue, t = Object(L.f)(t, ["defaultValue"]), e = Jn(e) ? e(o) : e;
                         i(e), void 0 === e ? uy.a.remove(n) : uy.a.set(n, e, t)
                     }), s = 2;
                     var p = (u = function(e) {
                             if (Array.isArray(e)) return e
                         }(c = [o, a]) || function(e, t) {
                             var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                             if (null != n) {
@@ -51271,15 +51280,15 @@
                     setProps: t.a.func
                 }, Xy.defaultProps = {
                     position: 50,
                     onlyHandleDraggable: !0,
                     boundsPadding: 0,
                     direction: "horizontal"
                 };
-                var Oe, Gy, x, Zy, O, Jy, Qy, e1, t1, n1, r1, o1 = xe.a.memo(Xy);
+                var Oe, Gy, x, Jy, O, Zy, Qy, e1, t1, n1, r1, o1 = xe.a.memo(Xy);
                 const i1 = "undefined" != typeof window && void 0 !== window.document && void 0 !== window.document.createElement;
 
                 function a1(e) {
                     e = Object.prototype.toString.call(e);
                     return "[object Window]" === e || "[object global]" === e
                 }
 
@@ -51785,22 +51794,22 @@
                     return i1 && e ? a1(e) ? e : s1(e) ? c1(e) || e === f1(e).scrollingElement ? window : u1(e) ? e : null : null : null
                 }
 
                 function G1(e) {
                     return a1(e) ? e.scrollX : e.scrollLeft
                 }
 
-                function Z1(e) {
+                function J1(e) {
                     return a1(e) ? e.scrollY : e.scrollTop
                 }
 
-                function J1(e) {
+                function Z1(e) {
                     return {
                         x: G1(e),
-                        y: Z1(e)
+                        y: J1(e)
                     }
                 }
 
                 function Q1(e) {
                     return i1 && e && e === document.scrollingElement
                 }
 
@@ -51831,22 +51840,22 @@
                 }(a = x = x || {})[a.Forward = 1] = "Forward", a[a.Backward = -1] = "Backward";
                 const tw = {
                     x: .2,
                     y: .2
                 };
 
                 function nw(e) {
-                    return e.reduce((e, t) => _1(e, J1(t)), I1)
+                    return e.reduce((e, t) => _1(e, Z1(t)), I1)
                 }
                 const rw = [
                     ["x", ["left", "right"], function(e) {
                         return e.reduce((e, t) => e + G1(t), 0)
                     }],
                     ["y", ["top", "bottom"], function(e) {
-                        return e.reduce((e, t) => e + Z1(t), 0)
+                        return e.reduce((e, t) => e + J1(t), 0)
                     }]
                 ];
                 class ow {
                     constructor(t, e) {
                         this.rect = void 0, this.width = void 0, this.height = void 0, this.top = void 0, this.bottom = void 0, this.right = void 0, this.left = void 0;
                         const n = Y1(e),
                             r = nw(n);
@@ -51890,30 +51899,30 @@
 
                 function sw(e) {
                     e.preventDefault()
                 }
 
                 function lw(e) {
                     e.stopPropagation()
-                }(n = Zy = Zy || {}).Click = "click", n.DragStart = "dragstart", n.Keydown = "keydown", n.ContextMenu = "contextmenu", n.Resize = "resize", n.SelectionChange = "selectionchange", n.VisibilityChange = "visibilitychange", (f = O = O || {}).Space = "Space", f.Down = "ArrowDown", f.Right = "ArrowRight", f.Left = "ArrowLeft", f.Up = "ArrowUp", f.Esc = "Escape", f.Enter = "Enter";
+                }(n = Jy = Jy || {}).Click = "click", n.DragStart = "dragstart", n.Keydown = "keydown", n.ContextMenu = "contextmenu", n.Resize = "resize", n.SelectionChange = "selectionchange", n.VisibilityChange = "visibilitychange", (f = O = O || {}).Space = "Space", f.Down = "ArrowDown", f.Right = "ArrowRight", f.Left = "ArrowLeft", f.Up = "ArrowUp", f.Esc = "Escape", f.Enter = "Enter";
                 const cw = {
                     start: [O.Space, O.Enter],
                     cancel: [O.Esc],
                     end: [O.Space, O.Enter]
                 };
                 class uw {
                     constructor(e) {
                         this.props = void 0, this.autoScrollEnabled = !1, this.referenceCoordinates = void 0, this.listeners = void 0, this.windowListeners = void 0;
                         var {
                             target: t
                         } = (this.props = e)["event"];
                         this.props = e, this.listeners = new iw(f1(t)), this.windowListeners = new iw(l1(t)), this.handleKeyDown = this.handleKeyDown.bind(this), this.handleCancel = this.handleCancel.bind(this), this.attach()
                     }
                     attach() {
-                        this.handleStart(), this.windowListeners.add(Zy.Resize, this.handleCancel), this.windowListeners.add(Zy.VisibilityChange, this.handleCancel), setTimeout(() => this.listeners.add(Zy.Keydown, this.handleKeyDown))
+                        this.handleStart(), this.windowListeners.add(Jy.Resize, this.handleCancel), this.windowListeners.add(Jy.VisibilityChange, this.handleCancel), setTimeout(() => this.listeners.add(Jy.Keydown, this.handleKeyDown))
                     }
                     handleStart() {
                         var e, t, n, r, {
                                 activeNode: o,
                                 onStart: i
                             } = this.props,
                             o = o.node.current;
@@ -52109,29 +52118,29 @@
                                 options: {
                                     activationConstraint: t
                                 }
                             }
                         } = this;
                         if (this.listeners.add(e.move.name, this.handleMove, {
                                 passive: !1
-                            }), this.listeners.add(e.end.name, this.handleEnd), this.windowListeners.add(Zy.Resize, this.handleCancel), this.windowListeners.add(Zy.DragStart, sw), this.windowListeners.add(Zy.VisibilityChange, this.handleCancel), this.windowListeners.add(Zy.ContextMenu, sw), this.documentListeners.add(Zy.Keydown, this.handleKeydown), t) {
+                            }), this.listeners.add(e.end.name, this.handleEnd), this.windowListeners.add(Jy.Resize, this.handleCancel), this.windowListeners.add(Jy.DragStart, sw), this.windowListeners.add(Jy.VisibilityChange, this.handleCancel), this.windowListeners.add(Jy.ContextMenu, sw), this.documentListeners.add(Jy.Keydown, this.handleKeydown), t) {
                             if (fw(t)) return;
                             if (dw(t)) return void(this.timeoutId = setTimeout(this.handleStart, t.delay))
                         }
                         this.handleStart()
                     }
                     detach() {
                         this.listeners.removeAll(), this.windowListeners.removeAll(), setTimeout(this.documentListeners.removeAll, 50), null !== this.timeoutId && (clearTimeout(this.timeoutId), this.timeoutId = null)
                     }
                     handleStart() {
                         var e = this["initialCoordinates"],
                             t = this.props["onStart"];
-                        e && (this.activated = !0, this.documentListeners.add(Zy.Click, lw, {
+                        e && (this.activated = !0, this.documentListeners.add(Jy.Click, lw, {
                             capture: !0
-                        }), this.removeTextSelection(), this.documentListeners.add(Zy.SelectionChange, this.removeTextSelection), t(e))
+                        }), this.removeTextSelection(), this.documentListeners.add(Jy.SelectionChange, this.removeTextSelection), t(e))
                     }
                     handleMove(e) {
                         var {
                             activated: t,
                             initialCoordinates: n,
                             props: r
                         } = this, {
@@ -52194,23 +52203,23 @@
                         move: {
                             name: "mousemove"
                         },
                         end: {
                             name: "mouseup"
                         }
                     },
-                    mw = (Jy = Jy || {}, Jy[Jy.RightClick = 2] = "RightClick", class extends pw {
+                    mw = (Zy = Zy || {}, Zy[Zy.RightClick = 2] = "RightClick", class extends pw {
                         constructor(e) {
                             super(e, bw, f1(e.event.target))
                         }
                     }.activators = [{
                         eventName: "onMouseDown",
                         handler: (e, t) => {
                             e = e.nativeEvent, t = t.onActivation;
-                            return e.button !== Jy.RightClick && (null != t && t({
+                            return e.button !== Zy.RightClick && (null != t && t({
                                 event: e
                             }), !0)
                         }
                     }], {
                         move: {
                             name: "touchmove"
                         },
@@ -52713,27 +52722,27 @@
                                     nodes: a,
                                     translate: b
                                 },
                                 droppable: {
                                     containers: s
                                 }
                             } = Y,
-                            Z = i ? a.get(i) : null,
-                            J = Object(ze.useRef)({
+                            J = i ? a.get(i) : null,
+                            Z = Object(ze.useRef)({
                                 initial: null,
                                 translated: null
                             }),
                             u = Object(ze.useMemo)(() => {
                                 var e;
                                 return null != i ? {
                                     id: i,
-                                    data: null != (e = null == Z ? void 0 : Z.data) ? e : Pw,
-                                    rect: J
+                                    data: null != (e = null == J ? void 0 : J.data) ? e : Pw,
+                                    rect: Z
                                 } : null
-                            }, [i, Z]),
+                            }, [i, J]),
                             f = Object(ze.useRef)(null),
                             [Q, ee] = Object(ze.useState)(null),
                             [d, te] = Object(ze.useState)(null),
                             p = h1($, Object.values($)),
                             ne = y1("DndDescribedBy", N),
                             re = Object(ze.useMemo)(() => s.getEnabled(), [s]),
                             m = (t = H, Object(ze.useMemo)(() => ({
@@ -52961,24 +52970,24 @@
                                 scrollableAncestorRects: j,
                                 windowRect: de
                             }),
                             pe = ie ? _1(ie, b) : null,
                             he = function(r) {
                                 const [e, o] = Object(ze.useState)(null), i = Object(ze.useRef)(r), a = Object(ze.useCallback)(e => {
                                     const t = X1(e.target);
-                                    t && o(e => e ? (e.set(t, J1(t)), new Map(e)) : null)
+                                    t && o(e => e ? (e.set(t, Z1(t)), new Map(e)) : null)
                                 }, []);
                                 return Object(ze.useEffect)(() => {
                                     const e = i.current;
                                     var t;
                                     return r !== e && (n(e), t = r.map(e => {
                                         e = X1(e);
                                         return e ? (e.addEventListener("scroll", a, {
                                             passive: !0
-                                        }), [e, J1(e)]) : null
+                                        }), [e, Z1(e)]) : null
                                     }).filter(e => null != e), o(t.length ? new Map(t) : null), i.current = r), () => {
                                         n(r), n(e)
                                     };
 
                                     function n(e) {
                                         e.forEach(e => {
                                             e = X1(e);
@@ -53026,15 +53035,15 @@
                                                         var n = a.get(t);
                                                         if (n) {
                                                             const r = p.current["onDragStart"],
                                                                 o = {
                                                                     active: {
                                                                         id: t,
                                                                         data: n.data,
-                                                                        rect: J
+                                                                        rect: Z
                                                                     }
                                                                 };
                                                             Object(sn.unstable_batchedUpdates)(() => {
                                                                 null != r && r(o), G(r1.Initializing), l({
                                                                     type: Oe.DragStart,
                                                                     initialCoordinates: e,
                                                                     active: t
@@ -53193,15 +53202,15 @@
                                 draggableNodes: a,
                                 draggingNode: O,
                                 draggingNodeRect: E,
                                 droppableContainers: s,
                                 over: T,
                                 scrollableAncestors: S,
                                 scrollAdjustedTranslate: C
-                            }, J.current = {
+                            }, Z.current = {
                                 initial: E,
                                 translated: z
                             }
                         }, [u, y, P, z, a, O, E, h, s, T, S, C]), vw({
                             ...ae,
                             delta: b,
                             draggingRect: z,
@@ -53265,86 +53274,122 @@
                     e = e.slice();
                     return e.splice(n < 0 ? e.length + n : n, 0, e.splice(t, 1)[0]), e
                 }
 
                 function $w(e) {
                     return null !== e && 0 <= e
                 }
-                const qw = e => {
+                const qw = {
+                        scaleX: 1,
+                        scaleY: 1
+                    },
+                    Yw = e => {
+                        var {
+                            rects: t,
+                            activeNodeRect: e,
+                            activeIndex: n,
+                            overIndex: r,
+                            index: o
+                        } = e, i = null != (i = t[n]) ? i : e;
+                        if (!i) return null;
+                        e = t[o], a = t[o - 1], s = t[o + 1];
+                        var a, s = e && (a || s) ? n < o ? a ? e.left - (a.left + a.width) : s.left - (e.left + e.width) : s ? s.left - (e.left + e.width) : e.left - (a.left + a.width) : 0;
+                        if (o !== n) return n < o && o <= r ? {
+                            x: -i.width - s,
+                            y: 0,
+                            ...qw
+                        } : o < n && r <= o ? {
+                            x: i.width + s,
+                            y: 0,
+                            ...qw
+                        } : {
+                            x: 0,
+                            y: 0,
+                            ...qw
+                        }; {
+                            const e = t[r];
+                            return e ? {
+                                x: n < r ? e.left + e.width - (i.left + i.width) : e.left - i.left,
+                                y: 0,
+                                ...qw
+                            } : null
+                        }
+                    },
+                    Kw = e => {
                         var {
                             rects: e,
                             activeIndex: t,
                             overIndex: n,
                             index: r
                         } = e, n = Vw(e, n, t), t = e[r], e = n[r];
                         return e && t ? {
                             x: e.left - t.left,
                             y: e.top - t.top,
                             scaleX: e.width / t.width,
                             scaleY: e.height / t.height
                         } : null
                     },
-                    Yw = {
+                    Xw = {
                         scaleX: 1,
                         scaleY: 1
                     },
-                    Kw = e => {
+                    Gw = e => {
                         var {
                             activeIndex: t,
                             activeNodeRect: e,
                             index: n,
                             rects: r,
                             overIndex: o
                         } = e, i = null != (i = r[t]) ? i : e;
                         if (!i) return null;
                         if (n === t) {
                             const e = r[o];
                             return e ? {
                                 x: 0,
                                 y: t < o ? e.top + e.height - (i.top + i.height) : e.top - i.top,
-                                ...Yw
+                                ...Xw
                             } : null
                         }
                         e = r[n], a = r[n - 1], r = r[n + 1];
                         var a, r = e ? t < n ? a ? e.top - (a.top + a.height) : r ? r.top - (e.top + e.height) : 0 : r ? r.top - (e.top + e.height) : a ? e.top - (a.top + a.height) : 0 : 0;
                         return t < n && n <= o ? {
                             x: 0,
                             y: -i.height - r,
-                            ...Yw
+                            ...Xw
                         } : n < t && o <= n ? {
                             x: 0,
                             y: i.height + r,
-                            ...Yw
+                            ...Xw
                         } : {
                             x: 0,
                             y: 0,
-                            ...Yw
+                            ...Xw
                         }
                     },
-                    Xw = xe.a.createContext({
+                    Jw = xe.a.createContext({
                         activeIndex: -1,
                         containerId: "Sortable",
                         disableTransforms: !1,
                         items: [],
                         overIndex: -1,
                         useDragOverlay: !1,
                         sortedRects: [],
-                        strategy: qw,
+                        strategy: Kw,
                         disabled: {
                             draggable: !1,
                             droppable: !1
                         }
                     });
 
-                function Gw(e) {
+                function Zw(e) {
                     let {
                         children: t,
                         id: n,
                         items: r,
-                        strategy: o = qw,
+                        strategy: o = Kw,
                         disabled: i = !1
                     } = e;
                     const {
                         active: a,
                         dragOverlay: s,
                         droppableRects: l,
                         over: c,
@@ -53378,77 +53423,77 @@
                                 t = r.get(t);
                                 return t && (e[n] = t), e
                             }, Array(e.length))),
                             strategy: o
                         };
                         var e, r
                     }, [g, f, w.draggable, w.droppable, y, p, b, l, d, o]);
-                    return xe.a.createElement(Xw.Provider, {
+                    return xe.a.createElement(Jw.Provider, {
                         value: e
                     }, t)
                 }
-                const Zw = e => {
+                const Qw = e => {
                         var {
                             id: e,
                             items: t,
                             activeIndex: n,
                             overIndex: r
                         } = e;
                         return Vw(t, n, r).indexOf(e)
                     },
-                    Jw = e => {
+                    e_ = e => {
                         var {
                             containerId: e,
                             isSorting: t,
                             wasDragging: n,
                             index: r,
                             items: o,
                             newIndex: i,
                             previousItems: a,
                             previousContainerId: s,
                             transition: l
                         } = e;
                         return !(!l || !n || a !== o && r === i || !t && (i === r || e !== s))
                     },
-                    Qw = {
+                    t_ = {
                         duration: 200,
                         easing: "ease"
                     },
-                    e_ = S1.Transition.toString({
+                    n_ = S1.Transition.toString({
                         property: "transform",
                         duration: 0,
                         easing: "linear"
                     }),
-                    t_ = {
+                    r_ = {
                         roleDescription: "sortable"
                     };
 
-                function n_(e) {
+                function o_(e) {
                     let {
-                        animateLayoutChanges: t = Jw,
+                        animateLayoutChanges: t = e_,
                         attributes: n,
                         disabled: r,
                         data: o,
-                        getNewIndex: i = Zw,
+                        getNewIndex: i = Qw,
                         id: x,
                         strategy: a,
                         resizeObserverConfig: O,
-                        transition: s = Qw
+                        transition: s = t_
                     } = e;
                     const {
                         items: l,
                         containerId: c,
                         activeIndex: u,
                         disabled: f,
                         disableTransforms: d,
                         sortedRects: p,
                         overIndex: h,
                         useDragOverlay: I,
                         strategy: L
-                    } = Object(ze.useContext)(Xw), E = "boolean" == typeof(e = r) ? {
+                    } = Object(ze.useContext)(Jw), E = "boolean" == typeof(e = r) ? {
                         draggable: e,
                         droppable: !1
                     } : {
                         draggable: null != (D = null == e ? void 0 : e.draggable) ? D : f.draggable,
                         droppable: null != (D = null == e ? void 0 : e.droppable) ? D : f.droppable
                     }, g = l.indexOf(x), S = Object(ze.useMemo)(() => ({
                         sortable: {
@@ -53620,15 +53665,15 @@
                             setActivatorNodeRef: _,
                             transform: m
                         }
                     }({
                         id: x,
                         data: S,
                         attributes: {
-                            ...t_,
+                            ...r_,
                             ...n
                         },
                         disabled: E.draggable
                     }), Y = function() {
                         for (var e = arguments.length, n = new Array(e), t = 0; t < e; t++) n[t] = arguments[t];
                         return Object(ze.useMemo)(() => t => {
                             n.forEach(e => e(t))
@@ -53726,22 +53771,22 @@
                         overIndex: h,
                         over: V,
                         setNodeRef: Y,
                         setActivatorNodeRef: $,
                         setDroppableNodeRef: v,
                         setDraggableNodeRef: w,
                         transform: null != R ? R : K,
-                        transition: R || X && M.current.newIndex === g ? e_ : C && !O1(B) || !s || !j && !A ? void 0 : S1.Transition.toString({
+                        transition: R || X && M.current.newIndex === g ? n_ : C && !O1(B) || !s || !j && !A ? void 0 : S1.Transition.toString({
                             ...s,
                             property: "transform"
                         })
                     }
                 }
                 O.Down, O.Right, O.Up, O.Left;
-                var r_ = {
+                var i_ = {
                         icon: {
                             tag: "svg",
                             attrs: {
                                 viewBox: "64 64 896 896",
                                 focusable: "false"
                             },
                             children: [{
@@ -53750,41 +53795,41 @@
                                     d: "M300 276.5a56 56 0 1056-97 56 56 0 00-56 97zm0 284a56 56 0 1056-97 56 56 0 00-56 97zM640 228a56 56 0 10112 0 56 56 0 00-112 0zm0 284a56 56 0 10112 0 56 56 0 00-112 0zM300 844.5a56 56 0 1056-97 56 56 0 00-56 97zM640 796a56 56 0 10112 0 56 56 0 00-112 0z"
                                 }
                             }]
                         },
                         name: "holder",
                         theme: "outlined"
                     },
-                    o_ = Object(ze.createContext)({});
+                    a_ = Object(ze.createContext)({});
 
-                function i_(e, t) {
+                function s_(e, t) {
                     var n = "string" == typeof(e = "string" == typeof(n = e) && -1 !== n.indexOf(".") && 1 === parseFloat(n) ? "100%" : e) && -1 !== e.indexOf("%");
                     return e = 360 === t ? e : Math.min(t, Math.max(0, parseFloat(e))), n && (e = parseInt(String(e * t), 10) / 100), Math.abs(e - t) < 1e-6 ? 1 : 360 === t ? (e < 0 ? e % t + t : e % t) / parseFloat(String(t)) : e % t / parseFloat(String(t))
                 }
 
-                function a_(e) {
+                function l_(e) {
                     return e <= 1 ? "".concat(100 * Number(e), "%") : e
                 }
 
-                function s_(e) {
+                function c_(e) {
                     return 1 === e.length ? "0" + e : String(e)
                 }
 
-                function l_(e, t, n) {
+                function u_(e, t, n) {
                     return n < 0 && (n += 1), 1 < n && --n, n < 1 / 6 ? e + 6 * n * (t - e) : n < .5 ? t : n < 2 / 3 ? e + (t - e) * (2 / 3 - n) * 6 : e
                 }
 
-                function c_(e) {
-                    return u_(e) / 255
+                function f_(e) {
+                    return d_(e) / 255
                 }
 
-                function u_(e) {
+                function d_(e) {
                     return parseInt(e, 16)
                 }
-                var f_ = {
+                var p_ = {
                     aliceblue: "#f0f8ff",
                     antiquewhite: "#faebd7",
                     aqua: "#00ffff",
                     aquamarine: "#7fffd4",
                     azure: "#f0ffff",
                     beige: "#f5f5dc",
                     bisque: "#ffe4c4",
@@ -53927,95 +53972,95 @@
                     wheat: "#f5deb3",
                     white: "#ffffff",
                     whitesmoke: "#f5f5f5",
                     yellow: "#ffff00",
                     yellowgreen: "#9acd32"
                 };
 
-                function d_(e) {
+                function h_(e) {
                     var t, n, r, o, i, a, s, l, c, u = {
                             r: 0,
                             g: 0,
                             b: 0
                         },
                         f = 1,
                         d = null,
                         p = !1,
                         h = !1;
                     return "object" == typeof(e = "string" == typeof e ? function(e) {
                         if (0 === (e = e.trim().toLowerCase()).length) return !1;
                         var t = !1;
-                        if (f_[e]) e = f_[e], t = !0;
+                        if (p_[e]) e = p_[e], t = !0;
                         else if ("transparent" === e) return {
                             r: 0,
                             g: 0,
                             b: 0,
                             a: 0,
                             format: "name"
                         };
-                        var n = p_.rgb.exec(e);
+                        var n = g_.rgb.exec(e);
                         return n ? {
                             r: n[1],
                             g: n[2],
                             b: n[3]
-                        } : (n = p_.rgba.exec(e)) ? {
+                        } : (n = g_.rgba.exec(e)) ? {
                             r: n[1],
                             g: n[2],
                             b: n[3],
                             a: n[4]
-                        } : (n = p_.hsl.exec(e)) ? {
+                        } : (n = g_.hsl.exec(e)) ? {
                             h: n[1],
                             s: n[2],
                             l: n[3]
-                        } : (n = p_.hsla.exec(e)) ? {
+                        } : (n = g_.hsla.exec(e)) ? {
                             h: n[1],
                             s: n[2],
                             l: n[3],
                             a: n[4]
-                        } : (n = p_.hsv.exec(e)) ? {
+                        } : (n = g_.hsv.exec(e)) ? {
                             h: n[1],
                             s: n[2],
                             v: n[3]
-                        } : (n = p_.hsva.exec(e)) ? {
+                        } : (n = g_.hsva.exec(e)) ? {
                             h: n[1],
                             s: n[2],
                             v: n[3],
                             a: n[4]
-                        } : (n = p_.hex8.exec(e)) ? {
-                            r: u_(n[1]),
-                            g: u_(n[2]),
-                            b: u_(n[3]),
-                            a: c_(n[4]),
+                        } : (n = g_.hex8.exec(e)) ? {
+                            r: d_(n[1]),
+                            g: d_(n[2]),
+                            b: d_(n[3]),
+                            a: f_(n[4]),
                             format: t ? "name" : "hex8"
-                        } : (n = p_.hex6.exec(e)) ? {
-                            r: u_(n[1]),
-                            g: u_(n[2]),
-                            b: u_(n[3]),
+                        } : (n = g_.hex6.exec(e)) ? {
+                            r: d_(n[1]),
+                            g: d_(n[2]),
+                            b: d_(n[3]),
                             format: t ? "name" : "hex"
-                        } : (n = p_.hex4.exec(e)) ? {
-                            r: u_(n[1] + n[1]),
-                            g: u_(n[2] + n[2]),
-                            b: u_(n[3] + n[3]),
-                            a: c_(n[4] + n[4]),
+                        } : (n = g_.hex4.exec(e)) ? {
+                            r: d_(n[1] + n[1]),
+                            g: d_(n[2] + n[2]),
+                            b: d_(n[3] + n[3]),
+                            a: f_(n[4] + n[4]),
                             format: t ? "name" : "hex8"
-                        } : !!(n = p_.hex3.exec(e)) && {
-                            r: u_(n[1] + n[1]),
-                            g: u_(n[2] + n[2]),
-                            b: u_(n[3] + n[3]),
+                        } : !!(n = g_.hex3.exec(e)) && {
+                            r: d_(n[1] + n[1]),
+                            g: d_(n[2] + n[2]),
+                            b: d_(n[3] + n[3]),
                             format: t ? "name" : "hex"
                         }
-                    }(e) : e) && (h_(e.r) && h_(e.g) && h_(e.b) ? (a = e.r, o = e.g, i = e.b, u = {
-                        r: 255 * i_(a, 255),
-                        g: 255 * i_(o, 255),
-                        b: 255 * i_(i, 255)
-                    }, p = !0, h = "%" === String(e.r).substr(-1) ? "prgb" : "rgb") : h_(e.h) && h_(e.s) && h_(e.v) ? (d = a_(e.s), a = a_(e.v), o = e.h, i = d, a = a, o = 6 * i_(o, 360), i = i_(i, 100), a = i_(a, 100), s = Math.floor(o), u = {
+                    }(e) : e) && (b_(e.r) && b_(e.g) && b_(e.b) ? (a = e.r, o = e.g, i = e.b, u = {
+                        r: 255 * s_(a, 255),
+                        g: 255 * s_(o, 255),
+                        b: 255 * s_(i, 255)
+                    }, p = !0, h = "%" === String(e.r).substr(-1) ? "prgb" : "rgb") : b_(e.h) && b_(e.s) && b_(e.v) ? (d = l_(e.s), a = l_(e.v), o = e.h, i = d, a = a, o = 6 * s_(o, 360), i = s_(i, 100), a = s_(a, 100), s = Math.floor(o), u = {
                         r: 255 * [a, c = a * (1 - (o -= s) * i), l = a * (1 - i), l, o = a * (1 - (1 - o) * i), a][i = s % 6],
                         g: 255 * [o, a, a, c, l, l][i],
                         b: 255 * [l, l, o, a, a, c][i]
-                    }, p = !0, h = "hsv") : h_(e.h) && h_(e.s) && h_(e.l) && (d = a_(e.s), s = a_(e.l), l = e.h, c = d, d = s, l = i_(l, 360), c = i_(c, 100), d = i_(d, 100), 0 === c ? t = r = n = d : (t = l_(c = 2 * d - (d = d < .5 ? d * (1 + c) : d + c - d * c), d, l + 1 / 3), n = l_(c, d, l), r = l_(c, d, l - 1 / 3)), u = {
+                    }, p = !0, h = "hsv") : b_(e.h) && b_(e.s) && b_(e.l) && (d = l_(e.s), s = l_(e.l), l = e.h, c = d, d = s, l = s_(l, 360), c = s_(c, 100), d = s_(d, 100), 0 === c ? t = r = n = d : (t = u_(c = 2 * d - (d = d < .5 ? d * (1 + c) : d + c - d * c), d, l + 1 / 3), n = u_(c, d, l), r = u_(c, d, l - 1 / 3)), u = {
                         r: 255 * t,
                         g: 255 * n,
                         b: 255 * r
                     }, p = !0, h = "hsl"), Object.prototype.hasOwnProperty.call(e, "a")) && (f = e.a), d = f, d = parseFloat(d), f = d = isNaN(d) || d < 0 || 1 < d ? 1 : d, {
                         ok: p,
                         format: e.format || h,
                         r: Math.min(255, Math.max(u.r, 0)),
@@ -54023,32 +54068,32 @@
                         b: Math.min(255, Math.max(u.b, 0)),
                         a: f
                     }
                 }
                 var r = "(?:".concat("[-\\+]?\\d*\\.\\d+%?", ")|(?:").concat("[-\\+]?\\d+%?", ")"),
                     a = "[\\s|\\(]+(".concat(r, ")[,|\\s]+(").concat(r, ")[,|\\s]+(").concat(r, ")\\s*\\)?"),
                     n = "[\\s|\\(]+(".concat(r, ")[,|\\s]+(").concat(r, ")[,|\\s]+(").concat(r, ")[,|\\s]+(").concat(r, ")\\s*\\)?"),
-                    p_ = {
+                    g_ = {
                         CSS_UNIT: new RegExp(r),
                         rgb: new RegExp("rgb" + a),
                         rgba: new RegExp("rgba" + n),
                         hsl: new RegExp("hsl" + a),
                         hsla: new RegExp("hsla" + n),
                         hsv: new RegExp("hsv" + a),
                         hsva: new RegExp("hsva" + n),
                         hex3: /^#?([0-9a-fA-F]{1})([0-9a-fA-F]{1})([0-9a-fA-F]{1})$/,
                         hex6: /^#?([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})$/,
                         hex4: /^#?([0-9a-fA-F]{1})([0-9a-fA-F]{1})([0-9a-fA-F]{1})([0-9a-fA-F]{1})$/,
                         hex8: /^#?([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})$/
                     };
 
-                function h_(e) {
-                    return Boolean(p_.CSS_UNIT.exec(String(e)))
+                function b_(e) {
+                    return Boolean(g_.CSS_UNIT.exec(String(e)))
                 }
-                var g_ = [{
+                var m_ = [{
                     index: 7,
                     opacity: .15
                 }, {
                     index: 6,
                     opacity: .25
                 }, {
                     index: 5,
@@ -54072,17 +54117,17 @@
                     index: 2,
                     opacity: .97
                 }, {
                     index: 1,
                     opacity: .98
                 }];
 
-                function b_(e) {
+                function v_(e) {
                     e = function(e, t, n) {
-                        e = i_(e, 255), t = i_(t, 255), n = i_(n, 255);
+                        e = s_(e, 255), t = s_(t, 255), n = s_(n, 255);
                         var r = Math.max(e, t, n),
                             o = Math.min(e, t, n),
                             i = 0,
                             a = r,
                             s = r - o,
                             l = 0 === r ? 0 : s / r;
                         if (r === o) i = 0;
@@ -54108,197 +54153,197 @@
                     return {
                         h: 360 * e.h,
                         s: e.s,
                         v: e.v
                     }
                 }
 
-                function m_(e) {
+                function y_(e) {
                     var n = e.r,
                         t = e.g,
                         e = e.b;
                     return "#".concat(function(e, t) {
-                        e = [s_(Math.round(n).toString(16)), s_(Math.round(e).toString(16)), s_(Math.round(t).toString(16))];
+                        e = [c_(Math.round(n).toString(16)), c_(Math.round(e).toString(16)), c_(Math.round(t).toString(16))];
                         return e.join("")
                     }(t, e))
                 }
 
-                function v_(e, t, n) {
+                function w_(e, t, n) {
                     return (n = 60 <= Math.round(e.h) && Math.round(e.h) <= 240 ? n ? Math.round(e.h) - 2 * t : Math.round(e.h) + 2 * t : n ? Math.round(e.h) + 2 * t : Math.round(e.h) - 2 * t) < 0 ? n += 360 : 360 <= n && (n -= 360), n
                 }
 
-                function y_(e, t, n) {
+                function __(e, t, n) {
                     return 0 === e.h && 0 === e.s ? e.s : (1 < (e = n ? e.s - .16 * t : 4 === t ? e.s + .16 : e.s + .05 * t) && (e = 1), (e = n && 5 === t && .1 < e ? .1 : e) < .06 && (e = .06), Number(e.toFixed(2)))
                 }
 
-                function w_(e, t, n) {
+                function x_(e, t, n) {
                     return 1 < (n = n ? e.v + .05 * t : e.v - .15 * t) && (n = 1), Number(n.toFixed(2))
                 }
 
-                function __(e, t) {
-                    for (var r = 1 < arguments.length && void 0 !== t ? t : {}, o = [], n = d_(e), i = 5; 0 < i; --i) {
-                        var a = b_(n),
-                            a = m_(d_({
-                                h: v_(a, i, !0),
-                                s: y_(a, i, !0),
-                                v: w_(a, i, !0)
+                function O_(e, t) {
+                    for (var r = 1 < arguments.length && void 0 !== t ? t : {}, o = [], n = h_(e), i = 5; 0 < i; --i) {
+                        var a = v_(n),
+                            a = y_(h_({
+                                h: w_(a, i, !0),
+                                s: __(a, i, !0),
+                                v: x_(a, i, !0)
                             }));
                         o.push(a)
                     }
-                    o.push(m_(n));
+                    o.push(y_(n));
                     for (var s = 1; s <= 4; s += 1) {
-                        var l = b_(n),
-                            l = m_(d_({
-                                h: v_(l, s),
-                                s: y_(l, s),
-                                v: w_(l, s)
+                        var l = v_(n),
+                            l = y_(h_({
+                                h: w_(l, s),
+                                s: __(l, s),
+                                v: x_(l, s)
                             }));
                         o.push(l)
                     }
-                    return "dark" === r.theme ? g_.map(function(e) {
+                    return "dark" === r.theme ? m_.map(function(e) {
                         var t, n = e.index,
                             e = e.opacity;
-                        return m_((t = d_(r.backgroundColor || "#141414"), n = d_(o[n]), e = 100 * e, e /= 100, {
+                        return y_((t = h_(r.backgroundColor || "#141414"), n = h_(o[n]), e = 100 * e, e /= 100, {
                             r: (n.r - t.r) * e + t.r,
                             g: (n.g - t.g) * e + t.g,
                             b: (n.b - t.b) * e + t.b
                         }))
                     }) : o
                 }
-                var x_ = {
+                var E_ = {
                         red: "#F5222D",
                         volcano: "#FA541C",
                         orange: "#FA8C16",
                         gold: "#FAAD14",
                         yellow: "#FADB14",
                         lime: "#A0D911",
                         green: "#52C41A",
                         cyan: "#13C2C2",
                         blue: "#1890FF",
                         geekblue: "#2F54EB",
                         purple: "#722ED1",
                         magenta: "#EB2F96",
                         grey: "#666666"
                     },
-                    O_ = {},
-                    E_ = {},
-                    S_ = (Object.keys(x_).forEach(function(e) {
-                        O_[e] = __(x_[e]), O_[e].primary = O_[e][5], E_[e] = __(x_[e], {
+                    S_ = {},
+                    j_ = {},
+                    k_ = (Object.keys(E_).forEach(function(e) {
+                        S_[e] = O_(E_[e]), S_[e].primary = S_[e][5], j_[e] = O_(E_[e], {
                             theme: "dark",
                             backgroundColor: "#141414"
-                        }), E_[e].primary = E_[e][5]
+                        }), j_[e].primary = j_[e][5]
                     }), new Map);
 
-                function j_(e) {
+                function C_(e) {
                     e = (0 < arguments.length && void 0 !== e ? e : {}).mark;
                     return e ? e.startsWith("data-") ? e : "data-".concat(e) : "rc-util-key"
                 }
 
-                function k_(e) {
+                function z_(e) {
                     return e.attachTo || document.querySelector("head") || document.body
                 }
 
-                function C_(e) {
-                    return Array.from((S_.get(e) || e).children).filter(function(e) {
+                function P_(e) {
+                    return Array.from((k_.get(e) || e).children).filter(function(e) {
                         return "STYLE" === e.tagName
                     })
                 }
 
-                function z_(e, t) {
+                function T_(e, t) {
                     t = 1 < arguments.length && void 0 !== t ? t : {};
                     if (!Hn()) return null;
                     var n = t.csp,
                         r = t.prepend,
                         o = document.createElement("style"),
-                        i = (o.setAttribute("data-rc-order", "queue" === (i = r) ? "prependQueue" : i ? "prepend" : "append"), null != n && n.nonce && (o.nonce = null == n ? void 0 : n.nonce), o.innerHTML = e, k_(t)),
+                        i = (o.setAttribute("data-rc-order", "queue" === (i = r) ? "prependQueue" : i ? "prepend" : "append"), null != n && n.nonce && (o.nonce = null == n ? void 0 : n.nonce), o.innerHTML = e, z_(t)),
                         n = i.firstChild;
                     if (r) {
                         if ("queue" === r) {
-                            e = C_(i).filter(function(e) {
+                            e = P_(i).filter(function(e) {
                                 return ["prepend", "prependQueue"].includes(e.getAttribute("data-rc-order"))
                             });
                             if (e.length) return i.insertBefore(o, e[e.length - 1].nextSibling), o
                         }
                         i.insertBefore(o, n)
                     } else i.appendChild(o);
                     return o
                 }
 
-                function P_(e, t, n) {
+                function M_(e, t, n) {
                     var n = 2 < arguments.length && void 0 !== n ? n : {},
-                        r = k_(n),
-                        o = (r = r, o = n, (i = S_.get(r)) && function(e, t) {
+                        r = z_(n),
+                        o = (r = r, o = n, (i = k_.get(r)) && function(e, t) {
                             if (e) {
                                 if (e.contains) return e.contains(t);
                                 for (var n = t; n;) {
                                     if (n === e) return 1;
                                     n = n.parentNode
                                 }
                             }
-                        }(document, i) || (o = (i = z_("", o)).parentNode, S_.set(r, o), r.removeChild(i)), function(t, e) {
+                        }(document, i) || (o = (i = T_("", o)).parentNode, k_.set(r, o), r.removeChild(i)), function(t, e) {
                             var n = 1 < arguments.length && void 0 !== e ? e : {};
-                            return C_(k_(n)).find(function(e) {
-                                return e.getAttribute(j_(n)) === t
+                            return P_(z_(n)).find(function(e) {
+                                return e.getAttribute(C_(n)) === t
                             })
                         }(t, n));
                     if (o) return null != (r = n.csp) && r.nonce && o.nonce !== (null == (i = n.csp) ? void 0 : i.nonce) && (o.nonce = null == (r = n.csp) ? void 0 : r.nonce), o.innerHTML !== e && (o.innerHTML = e);
-                    var i = z_(e, n);
-                    i.setAttribute(j_(n), t)
+                    var i = T_(e, n);
+                    i.setAttribute(C_(n), t)
                 }
 
-                function T_(e) {
+                function A_(e) {
                     return "object" === Kt(e) && "string" == typeof e.name && "string" == typeof e.theme && ("object" === Kt(e.icon) || "function" == typeof e.icon)
                 }
 
-                function M_(e) {
+                function R_(e) {
                     var r = 0 < arguments.length && void 0 !== e ? e : {};
                     return Object.keys(r).reduce(function(e, t) {
                         var n = r[t];
                         return "class" === t ? (e.className = n, delete e.class) : e[t] = n, e
                     }, {})
                 }
 
-                function A_(e) {
-                    return __(e)[0]
+                function D_(e) {
+                    return O_(e)[0]
                 }
 
-                function R_(e) {
+                function I_(e) {
                     return e ? Array.isArray(e) ? e : [e] : []
                 }
 
-                function D_(e) {
+                function L_(e) {
                     var t = e.icon,
                         n = e.className,
                         r = e.onClick,
                         o = e.style,
                         i = e.primaryColor,
                         a = e.secondaryColor,
-                        e = en(e, I_),
-                        s = L_;
+                        e = en(e, N_),
+                        s = U_;
                     return i && (s = {
                             primaryColor: i,
-                            secondaryColor: a || A_(i)
+                            secondaryColor: a || D_(i)
                         }),
                         function(e) {
                             var t = 0 < arguments.length && void 0 !== e ? e : "\n.anticon {\n  display: inline-block;\n  color: inherit;\n  font-style: normal;\n  line-height: 0;\n  text-align: center;\n  text-transform: none;\n  vertical-align: -0.125em;\n  text-rendering: optimizeLegibility;\n  -webkit-font-smoothing: antialiased;\n  -moz-osx-font-smoothing: grayscale;\n}\n\n.anticon > * {\n  line-height: 1;\n}\n\n.anticon svg {\n  display: inline-block;\n}\n\n.anticon::before {\n  display: none;\n}\n\n.anticon .anticon-icon {\n  display: block;\n}\n\n.anticon[tabindex] {\n  cursor: pointer;\n}\n\n.anticon-spin::before,\n.anticon-spin {\n  display: inline-block;\n  -webkit-animation: loadingCircle 1s infinite linear;\n  animation: loadingCircle 1s infinite linear;\n}\n\n@-webkit-keyframes loadingCircle {\n  100% {\n    -webkit-transform: rotate(360deg);\n    transform: rotate(360deg);\n  }\n}\n\n@keyframes loadingCircle {\n  100% {\n    -webkit-transform: rotate(360deg);\n    transform: rotate(360deg);\n  }\n}\n",
-                                n = Object(ze.useContext)(o_).csp;
+                                n = Object(ze.useContext)(a_).csp;
                             Object(ze.useEffect)(function() {
-                                P_(t, "@ant-design-icons", {
+                                M_(t, "@ant-design-icons", {
                                     prepend: !0,
                                     csp: n
                                 })
                             }, [])
-                        }(), a = T_(t), i = "icon should be icon definiton, but got ".concat(t), on(a, "[@ant-design/icons] ".concat(i)), T_(t) ? function n(r, o, e) {
+                        }(), a = A_(t), i = "icon should be icon definiton, but got ".concat(t), on(a, "[@ant-design/icons] ".concat(i)), A_(t) ? function n(r, o, e) {
                             return e ? xe.a.createElement(r.tag, Pe(Pe({
                                 key: o
-                            }, M_(r.attrs)), e), (r.children || []).map(function(e, t) {
+                            }, R_(r.attrs)), e), (r.children || []).map(function(e, t) {
                                 return n(e, "".concat(o, "-").concat(r.tag, "-").concat(t))
                             })) : xe.a.createElement(r.tag, Pe({
                                 key: o
-                            }, M_(r.attrs)), (r.children || []).map(function(e, t) {
+                            }, R_(r.attrs)), (r.children || []).map(function(e, t) {
                                 return n(e, "".concat(o, "-").concat(r.tag, "-").concat(t))
                             }))
                         }((a = (a = t) && "function" == typeof a.icon ? Pe(Pe({}, a), {}, {
                             icon: a.icon(s.primaryColor, s.secondaryColor)
                         }) : a).icon, "svg-".concat(a.name), Pe({
                             className: n,
                             onClick: r,
@@ -54306,102 +54351,102 @@
                             "data-icon": a.name,
                             width: "1em",
                             height: "1em",
                             fill: "currentColor",
                             "aria-hidden": "true"
                         }, e)) : null
                 }
-                var I_ = ["icon", "className", "onClick", "style", "primaryColor", "secondaryColor"],
-                    L_ = {
+                var N_ = ["icon", "className", "onClick", "style", "primaryColor", "secondaryColor"],
+                    U_ = {
                         primaryColor: "#333",
                         secondaryColor: "#E6E6E6",
                         calculated: !1
                     },
-                    N_ = (D_.displayName = "IconReact", D_.getTwoToneColors = function() {
-                        return Pe({}, L_)
-                    }, D_.setTwoToneColors = function(e) {
+                    B_ = (L_.displayName = "IconReact", L_.getTwoToneColors = function() {
+                        return Pe({}, U_)
+                    }, L_.setTwoToneColors = function(e) {
                         var t = e.primaryColor,
                             e = e.secondaryColor;
-                        L_.primaryColor = t, L_.secondaryColor = e || A_(t), L_.calculated = !!e
-                    }, D_);
+                        U_.primaryColor = t, U_.secondaryColor = e || D_(t), U_.calculated = !!e
+                    }, L_);
 
-                function U_(e) {
-                    var e = Qt(R_(e), 2),
+                function F_(e) {
+                    var e = Qt(I_(e), 2),
                         t = e[0],
                         e = e[1];
-                    return N_.setTwoToneColors({
+                    return B_.setTwoToneColors({
                         primaryColor: t,
                         secondaryColor: e
                     })
                 }
 
-                function B_(e, t) {
-                    return ze.createElement(V_, Pe(Pe({}, e), {}, {
+                function W_(e, t) {
+                    return ze.createElement(q_, Pe(Pe({}, e), {}, {
                         ref: t,
-                        icon: r_
+                        icon: i_
                     }))
                 }
 
-                function F_(e, t) {
-                    return ze.createElement(V_, Pe(Pe({}, e), {}, {
+                function H_(e, t) {
+                    return ze.createElement(q_, Pe(Pe({}, e), {}, {
                         ref: t,
-                        icon: $_
+                        icon: Y_
                     }))
                 }
 
-                function W_(e, t) {
-                    return ze.createElement(V_, Pe(Pe({}, e), {}, {
+                function V_(e, t) {
+                    return ze.createElement(q_, Pe(Pe({}, e), {}, {
                         ref: t,
-                        icon: q_
+                        icon: K_
                     }))
                 }
-                var H_ = ["className", "icon", "spin", "rotate", "tabIndex", "onClick", "twoToneColor"],
-                    f = (U_("#1890ff"), ze.forwardRef(function(e, t) {
+                var $_ = ["className", "icon", "spin", "rotate", "tabIndex", "onClick", "twoToneColor"],
+                    f = (F_("#1890ff"), ze.forwardRef(function(e, t) {
                         var n = e.className,
                             r = e.icon,
                             o = e.spin,
                             i = e.rotate,
                             a = e.tabIndex,
                             s = e.onClick,
                             l = e.twoToneColor,
-                            e = en(e, H_),
-                            c = ze.useContext(o_),
+                            e = en(e, $_),
+                            c = ze.useContext(a_),
                             u = c.prefixCls,
                             u = void 0 === u ? "anticon" : u,
                             c = c.rootClassName,
                             u = Te()(c, u, (Gt(c = {}, "".concat(u, "-").concat(r.name), !!r.name), Gt(c, "".concat(u, "-spin"), !!o || "loading" === r.name), c), n),
                             o = a,
                             c = (void 0 === a && s && (o = -1), i ? {
                                 msTransform: "rotate(".concat(i, "deg)"),
                                 transform: "rotate(".concat(i, "deg)")
                             } : void 0),
-                            n = Qt(R_(l), 2),
+                            n = Qt(I_(l), 2),
                             a = n[0],
                             i = n[1];
                         return ze.createElement("span", Pe(Pe({
                             role: "img",
                             "aria-label": r.name
                         }, e), {}, {
                             ref: t,
                             tabIndex: o,
                             onClick: s,
                             className: u
-                        }), ze.createElement(N_, {
+                        }), ze.createElement(B_, {
                             icon: r,
                             primaryColor: a,
                             secondaryColor: i,
                             style: c
                         }))
                     })),
-                    V_ = (f.displayName = "AntdIcon", f.getTwoToneColor = function() {
-                        var e = N_.getTwoToneColors();
+                    q_ = (f.displayName = "AntdIcon", f.getTwoToneColor = function() {
+                        var e = B_.getTwoToneColors();
                         return e.calculated ? [e.primaryColor, e.secondaryColor] : e.primaryColor
-                    }, f.setTwoToneColor = U_, f),
-                    i = (B_.displayName = "HolderOutlined", ze.forwardRef(B_)),
-                    $_ = {
+                    }, f.setTwoToneColor = F_, f),
+                    i = (W_.displayName = "HolderOutlined", ze.forwardRef(W_)),
+                    Y_ = {
                         icon: {
                             tag: "svg",
                             attrs: {
                                 viewBox: "64 64 896 896",
                                 focusable: "false"
                             },
                             children: [{
@@ -54410,16 +54455,16 @@
                                     d: "M904 160H120c-4.4 0-8 3.6-8 8v64c0 4.4 3.6 8 8 8h784c4.4 0 8-3.6 8-8v-64c0-4.4-3.6-8-8-8zm0 624H120c-4.4 0-8 3.6-8 8v64c0 4.4 3.6 8 8 8h784c4.4 0 8-3.6 8-8v-64c0-4.4-3.6-8-8-8zm0-312H120c-4.4 0-8 3.6-8 8v64c0 4.4 3.6 8 8 8h784c4.4 0 8-3.6 8-8v-64c0-4.4-3.6-8-8-8z"
                                 }
                             }]
                         },
                         name: "menu",
                         theme: "outlined"
                     },
-                    d = (F_.displayName = "MenuOutlined", ze.forwardRef(F_)),
-                    q_ = {
+                    d = (H_.displayName = "MenuOutlined", ze.forwardRef(H_)),
+                    K_ = {
                         icon: {
                             tag: "svg",
                             attrs: {
                                 viewBox: "64 64 896 896",
                                 focusable: "false"
                             },
                             children: [{
@@ -54429,257 +54474,302 @@
                                 }
                             }]
                         },
                         name: "drag",
                         theme: "outlined"
                     };
 
-                function Y_(e) {
-                    return (Y_ = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                function X_(e) {
+                    return (X_ = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                     })(e)
                 }
 
-                function K_(e, t) {
+                function G_(e, t) {
                     (null == t || t > e.length) && (t = e.length);
                     for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
                     return r
                 }
 
-                function X_() {
-                    return (X_ = Object.assign ? Object.assign.bind() : function(e) {
+                function J_() {
+                    return (J_ = Object.assign ? Object.assign.bind() : function(e) {
                         for (var t = 1; t < arguments.length; t++) {
                             var n, r = arguments[t];
                             for (n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
                         }
                         return e
                     }).apply(this, arguments)
                 }
 
-                function G_(t, e) {
+                function Z_(t, e) {
                     var n, r = Object.keys(t);
                     return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(t), e && (n = n.filter(function(e) {
                         return Object.getOwnPropertyDescriptor(t, e).enumerable
                     })), r.push.apply(r, n)), r
                 }
 
-                function Z_(r) {
+                function Q_(r) {
                     for (var e = 1; e < arguments.length; e++) {
                         var o = null != arguments[e] ? arguments[e] : {};
-                        e % 2 ? G_(Object(o), !0).forEach(function(e) {
+                        e % 2 ? Z_(Object(o), !0).forEach(function(e) {
                             var t, n;
                             t = r, e = o[n = e], (n = function() {
                                 var e = function(e) {
-                                    if ("object" !== Y_(e) || null === e) return e;
+                                    if ("object" !== X_(e) || null === e) return e;
                                     var t = e[Symbol.toPrimitive];
                                     if (void 0 === t) return String(e);
                                     t = t.call(e, "string");
-                                    if ("object" !== Y_(t)) return t;
+                                    if ("object" !== X_(t)) return t;
                                     throw new TypeError("@@toPrimitive must return a primitive value.")
                                 }(n);
-                                return "symbol" === Y_(e) ? e : String(e)
+                                return "symbol" === X_(e) ? e : String(e)
                             }()) in t ? Object.defineProperty(t, n, {
                                 value: e,
                                 enumerable: !0,
                                 configurable: !0,
                                 writable: !0
                             }) : t[n] = e
-                        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(r, Object.getOwnPropertyDescriptors(o)) : G_(Object(o)).forEach(function(e) {
+                        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(r, Object.getOwnPropertyDescriptors(o)) : Z_(Object(o)).forEach(function(e) {
                             Object.defineProperty(r, e, Object.getOwnPropertyDescriptor(o, e))
                         })
                     }
                     return r
                 }
-                W_.displayName = "DragOutlined";
+                V_.displayName = "DragOutlined";
 
-                function J_(e) {
+                function ex(e) {
                     var t = e.id,
                         n = e.style,
                         r = e.draggingStyle,
                         o = e.className,
                         i = e.draggingClassName,
                         a = e.children,
                         s = e.handleStyle,
                         l = e.handleClassName,
                         c = e.handlePosition,
                         u = e.handleType,
                         e = e.itemDraggingScale,
-                        f = (t = n_({
+                        f = (t = o_({
                             id: t
                         })).attributes,
                         d = t.listeners,
                         p = t.setNodeRef,
                         h = t.transform,
                         g = t.transition,
                         b = t.setActivatorNodeRef,
                         t = t.isDragging,
-                        h = Z_(Z_({
-                            transform: S1.Transform.toString(h && Z_(Z_({}, h), {}, {
+                        h = Q_(Q_({
+                            transform: S1.Transform.toString(h && Q_(Q_({}, h), {}, {
                                 scaleY: 1
                             }, t ? {
                                 scaleX: e,
                                 scaleY: e
                             } : {})),
                             transition: g,
                             display: "flex",
                             alignItems: "center"
-                        }, n), t ? Z_({
+                        }, n), t ? Q_({
                             position: "relative",
                             zIndex: 999
                         }, r) : {});
-                    return xe.a.createElement("div", X_({
+                    return xe.a.createElement("div", J_({
                         ref: p
                     }, f, {
                         style: h,
                         className: t ? Object(D.isString)(o) ? o : o ? Bu(o) : void 0 : Object(D.isString)(i) ? i : i ? Bu(i) : void 0
                     }), "end" === c ? xe.a.createElement("div", {
                         style: {
                             flex: "auto"
                         }
-                    }, a) : null, xe.a.createElement(ex.get(u), Z_({
-                        style: Z_({
+                    }, a) : null, xe.a.createElement(rx.get(u), Q_({
+                        style: Q_({
                             color: "#737373",
                             touchAction: "none",
                             cursor: t ? "grabbing" : "grab",
                             flex: "none"
                         }, s),
                         className: Object(D.isString)(l) ? l : l ? Bu(l) : void 0,
                         ref: b
                     }, d)), "start" === c ? xe.a.createElement("div", {
                         style: {
                             flex: "auto"
                         }
                     }, a) : null)
                 }
 
-                function Q_(e) {
+                function tx(e) {
                     var t = e.id,
                         n = e.style,
                         r = e.handleStyle,
                         o = e.className,
                         i = e.handleClassName,
                         a = e.items,
-                        s = e.itemDraggingScale,
-                        l = e.handlePosition,
-                        c = e.handleType,
-                        u = e.setProps,
+                        s = e.direction,
+                        l = e.itemDraggingScale,
+                        c = e.handlePosition,
+                        u = e.handleType,
+                        f = e.setProps,
                         e = e.loading_state;
                     Object(ze.useEffect)(function() {
-                        u({
+                        f({
                             currentOrder: a.map(function(e) {
                                 return e.key
                             })
                         })
                     }, [a]);
-                    var f, d = function() {
+                    var d, p = function() {
                         for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
                         return Object(ze.useMemo)(() => [...t].filter(e => null != e), [...t])
-                    }((f = gw, Object(ze.useMemo)(() => ({
-                        sensor: f,
+                    }((d = gw, Object(ze.useMemo)(() => ({
+                        sensor: d,
                         options: {}
-                    }), [f, void 0])));
+                    }), [d, void 0])));
                     return xe.a.createElement(Fw, {
-                        sensors: d,
+                        sensors: p,
                         collisionDetection: B1,
                         onDragEnd: function(e) {
                             var t, n, r = e.active,
                                 o = e.over;
                             (null == r ? void 0 : r.id) !== (null == o ? void 0 : o.id) && (e = a.findIndex(function(e) {
                                 return e.key === (null == r ? void 0 : r.id)
                             }), t = a.findIndex(function(e) {
                                 return e.key === (null == o ? void 0 : o.id)
-                            }), u({
+                            }), f({
                                 items: Vw(function(e) {
-                                    if (Array.isArray(e)) return K_(e)
+                                    if (Array.isArray(e)) return G_(e)
                                 }(n = a) || function() {
                                     if ("undefined" != typeof Symbol && null != n[Symbol.iterator] || null != n["@@iterator"]) return Array.from(n)
                                 }() || function(e) {
                                     var t;
-                                    if (e) return "string" == typeof e ? K_(e, void 0) : "Map" === (t = "Object" === (t = Object.prototype.toString.call(e).slice(8, -1)) && e.constructor ? e.constructor.name : t) || "Set" === t ? Array.from(e) : "Arguments" === t || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(t) ? K_(e, void 0) : void 0
+                                    if (e) return "string" == typeof e ? G_(e, void 0) : "Map" === (t = "Object" === (t = Object.prototype.toString.call(e).slice(8, -1)) && e.constructor ? e.constructor.name : t) || "Set" === t ? Array.from(e) : "Arguments" === t || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(t) ? G_(e, void 0) : void 0
                                 }(n) || function() {
                                     throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                                 }(), e, t)
                             }))
                         }
-                    }, xe.a.createElement(Gw, {
+                    }, xe.a.createElement(Zw, {
                         items: a.map(function(e) {
-                            return Z_(Z_({}, e), {}, {
+                            return Q_(Q_({}, e), {}, {
                                 id: e.key
                             })
                         }),
-                        strategy: Kw
+                        strategy: "horizontal" === s ? Yw : Gw
                     }, xe.a.createElement("ul", {
                         id: t,
-                        style: Z_({
+                        style: Q_({
                             paddingLeft: 0
                         }, n),
                         className: Object(D.isString)(o) ? o : o ? Bu(o) : void 0,
                         "data-dash-is-loading": e && e.is_loading || void 0
                     }, a.map(function(e) {
-                        return xe.a.createElement(J_, {
+                        return xe.a.createElement(ex, {
                             id: e.key,
                             key: e.key,
                             style: e.style,
                             draggingStyle: e.draggingStyle,
                             className: e.className,
                             draggingClassName: e.draggingClassName,
                             children: e.content,
                             handleStyle: r,
                             handleClassName: i,
-                            handlePosition: l,
-                            handleType: c,
-                            itemDraggingScale: s
+                            handlePosition: c,
+                            handleType: u,
+                            itemDraggingScale: l
                         })
                     }))))
                 }
-                var ex = new Map([
+
+                function nx(e) {
+                    var t = e.id,
+                        n = e.data,
+                        r = e.initialSync,
+                        o = e.setProps,
+                        e = e.loading_state;
+                    return Object(ze.useEffect)(function() {
+                        function e(e) {
+                            e.triggerKey === t && (e = localStorage.getItem(t)) && o({
+                                data: JSON.parse(e)
+                            })
+                        }
+                        return window.addEventListener("localStorageSetItem", e),
+                            function() {
+                                window.removeEventListener("localStorageSetItem", e)
+                            }
+                    }, []), Object(ze.useEffect)(function() {
+                        var e;
+                        r && (e = localStorage.getItem(t)) && o({
+                            data: JSON.parse(e)
+                        })
+                    }, []), Object(ze.useEffect)(function() {
+                        Object(D.isUndefined)(n) || localStorage.setItem(t, JSON.stringify(n))
+                    }, [n]), xe.a.createElement("div", {
+                        id: t,
+                        "data-dash-is-loading": e && e.is_loading || void 0
+                    })
+                }
+                var rx = new Map([
                         ["holder", i],
                         ["menu", d],
-                        ["drag", ze.forwardRef(W_)]
+                        ["drag", ze.forwardRef(V_)]
                     ]),
-                    tx = (Q_.propTypes = {
+                    ox = (tx.propTypes = {
                         id: t.a.string,
                         style: t.a.object,
                         handleStyle: t.a.object,
                         handleClassName: t.a.oneOfType([t.a.string, t.a.object]),
                         className: t.a.oneOfType([t.a.string, t.a.object]),
                         key: t.a.string,
                         items: t.a.arrayOf(t.a.exact({
                             key: t.a.oneOfType([t.a.number, t.a.string]).isRequired,
                             content: t.a.node,
                             style: t.a.object,
                             className: t.a.oneOfType([t.a.string, t.a.object]),
                             draggingStyle: t.a.object,
                             draggingClassName: t.a.oneOfType([t.a.string, t.a.object])
                         })).isRequired,
+                        direction: t.a.oneOf(["vertical", "horizontal"]),
                         itemDraggingScale: t.a.number,
                         handlePosition: t.a.oneOf(["start", "end"]),
                         handleType: t.a.oneOf(["holder", "menu", "drag"]),
                         currentOrder: t.a.arrayOf(t.a.oneOfType([t.a.number, t.a.string])),
                         loading_state: t.a.shape({
                             is_loading: t.a.bool,
                             prop_name: t.a.string,
                             component_name: t.a.string
                         }),
                         setProps: t.a.func
-                    }, Q_.defaultProps = {
+                    }, tx.defaultProps = {
+                        direction: "vertical",
                         itemDraggingScale: 1,
                         handlePosition: "end",
                         handleType: "holder"
-                    }, xe.a.memo(Q_)),
-                    nx = (o.d(e, "FefferyCaptcha", function() {
+                    }, xe.a.memo(tx)),
+                    ix = (nx.propTypes = {
+                        id: t.a.string.isRequired,
+                        data: t.a.any,
+                        initialSync: t.a.bool,
+                        loading_state: t.a.shape({
+                            is_loading: t.a.bool,
+                            prop_name: t.a.string,
+                            component_name: t.a.string
+                        }),
+                        setProps: t.a.func
+                    }, nx.defaultProps = {
+                        initialSync: !1
+                    }, nx),
+                    ax = (o.d(e, "FefferyCaptcha", function() {
                         return A
                     }), o.d(e, "FefferyTopProgress", function() {
                         return G
                     }), o.d(e, "FefferyShortcutPanel", function() {
-                        return Z.a
-                    }), o.d(e, "FefferyGuide", function() {
                         return J.a
+                    }), o.d(e, "FefferyGuide", function() {
+                        return Z.a
                     }), o.d(e, "FefferySplit", function() {
                         return me
                     }), o.d(e, "FefferySplitPane", function() {
                         return je
                     }), o.d(e, "FefferyExecuteJs", function() {
                         return ke.a
                     }), o.d(e, "FefferyScroll", function() {
@@ -54719,27 +54809,27 @@
                     }), o.d(e, "FefferySetTitle", function() {
                         return Al
                     }), o.d(e, "FefferyResponsive", function() {
                         return Wl
                     }), o.d(e, "FefferyGeolocation", function() {
                         return Hl
                     }), o.d(e, "FefferyIdle", function() {
-                        return Jl
+                        return Zl
                     }), o.d(e, "FefferyWindowSize", function() {
                         return ec
                     }), o.d(e, "FefferyKeyPress", function() {
                         return uc
                     }), o.d(e, "FefferyTimeout", function() {
                         return dc
                     }), o.d(e, "FefferyCountDown", function() {
                         return yc
                     }), o.d(e, "FefferyRawHTML", function() {
                         return _c
                     }), o.d(e, "FefferyFancyNotification", function() {
-                        return Jc
+                        return Zc
                     }), o.d(e, "FefferyQRCode", function() {
                         return ku
                     }), o.d(e, "FefferyFancyMessage", function() {
                         return Pu
                     }), o.d(e, "FefferyStyle", function() {
                         return B.a
                     }), o.d(e, "FefferyDiv", function() {
@@ -54791,19 +54881,26 @@
                     }), o.d(e, "FefferyCookie", function() {
                         return Sy
                     }), o.d(e, "FefferyResizable", function() {
                         return Uy
                     }), o.d(e, "FefferyCompareSlider", function() {
                         return o1
                     }), o.d(e, "FefferySortableList", function() {
-                        return tx
-                    }), sessionStorage.setItem);
-                sessionStorage.setItem = function(e, t) {
-                    nx.apply(this, [e, t]);
-                    var n = new Event("sessionStorageSetItem");
+                        return ox
+                    }), o.d(e, "FefferyLocalStorage", function() {
+                        return ix
+                    }), sessionStorage.setItem),
+                    sx = (sessionStorage.setItem = function(e, t) {
+                        ax.apply(this, [e, t]);
+                        var n = new Event("sessionStorageSetItem");
+                        n.triggerKey = e, n[e] = t, window.dispatchEvent(n)
+                    }, localStorage.setItem);
+                localStorage.setItem = function(e, t) {
+                    sx.apply(this, [e, t]);
+                    var n = new Event("localStorageSetItem");
                     n.triggerKey = e, n[e] = t, window.dispatchEvent(n)
                 }
             }, function(I, L, e) {
                 "use strict";
                 const o = window,
                     N = o.ShadowRoot && (void 0 === o.ShadyCSS || o.ShadyCSS.nativeShadow) && "adoptedStyleSheets" in Document.prototype && "replace" in CSSStyleSheet.prototype,
                     U = Symbol(),
@@ -55059,17 +55156,17 @@
                     firstUpdated(e) {}
                 }
                 t.finalized = !0, t.elementProperties = new Map, t.elementStyles = [], t.shadowRootOptions = {
                     mode: "open"
                 }, null != Y && Y({
                     ReactiveElement: t
                 }), (null != (n = V.reactiveElementVersions) ? n : V.reactiveElementVersions = []).push("1.6.1");
-                const Z = window,
-                    c = Z.trustedTypes,
-                    J = c ? c.createPolicy("lit-html", {
+                const J = window,
+                    c = J.trustedTypes,
+                    Z = c ? c.createPolicy("lit-html", {
                         createHTML: e => e
                     }) : void 0,
                     d = `lit$${(Math.random()+"").slice(9)}$`,
                     Q = "?" + d,
                     ee = `<${Q}>`,
                     l = document,
                     u = () => l.createComment(""),
@@ -55103,15 +55200,15 @@
                             let e, t, n = -1,
                                 r = 0;
                             for (; r < a.length && (u.lastIndex = r, null !== (t = u.exec(a)));) r = u.lastIndex, u === p ? "!--" === t[1] ? u = re : void 0 !== t[1] ? u = oe : void 0 !== t[2] ? (se.test(t[2]) && (l = RegExp("</" + t[2], "g")), u = h) : void 0 !== t[3] && (u = h) : u === h ? ">" === t[0] ? (u = null != l ? l : p, n = -1) : void 0 === t[1] ? n = -2 : (n = u.lastIndex - t[2].length, e = t[1], u = void 0 === t[3] ? h : '"' === t[3] ? ae : ie) : u === ae || u === ie ? u = h : u === re || u === oe ? u = p : (u = h, l = void 0);
                             var f = u === h && i[o + 1].startsWith("/>") ? " " : "";
                             c += u === p ? a + ee : 0 <= n ? (s.push(e), a.slice(0, n) + "$lit$" + a.slice(n) + d + f) : a + d + (-2 === n ? (s.push(void 0), o) : f)
                         }
                         e = c + (i[a] || "<?>") + (2 === e ? "</svg>" : "");
-                        if (Array.isArray(i) && i.hasOwnProperty("raw")) return [void 0 !== J ? J.createHTML(e) : e, s];
+                        if (Array.isArray(i) && i.hasOwnProperty("raw")) return [void 0 !== Z ? Z.createHTML(e) : e, s];
                         throw Error("invalid template strings array")
                     };
                 class fe {
                     constructor({
                         strings: t,
                         _$litType$: n
                     }, e) {
@@ -55372,16 +55469,16 @@
                         I: y,
                         H: w,
                         N: ge,
                         U: be,
                         F: pe,
                         B: me
                     },
-                    r = Z.litHtmlPolyfillSupport;
-                null != r && r(fe, y), (null != (r = Z.litHtmlVersions) ? r : Z.litHtmlVersions = []).push("2.7.0");
+                    r = J.litHtmlPolyfillSupport;
+                null != r && r(fe, y), (null != (r = J.litHtmlVersions) ? r : J.litHtmlVersions = []).push("2.7.0");
                 class a extends t {
                     constructor() {
                         super(...arguments), this.renderOptions = {
                             host: this
                         }, this._$Do = void 0
                     }
                     createRenderRoot() {
@@ -55850,15 +55947,15 @@
                     var r;
                     if (t.scope === n || "all" === t.scope) {
                         for (var o in r = 0 < t.mods.length, C) Object.prototype.hasOwnProperty.call(C, o) && (!C[o] && -1 < t.mods.indexOf(+o) || C[o] && -1 === t.mods.indexOf(+o)) && (r = !1);
                         (0 !== t.mods.length || C[16] || C[18] || C[17] || C[91]) && !r && "*" !== t.shortcut || !1 === t.method(e, t) && (e.preventDefault ? e.preventDefault() : e.returnValue = !1, e.stopPropagation && e.stopPropagation(), e.cancelBubble) && (e.cancelBubble = !0)
                     }
                 }
 
-                function Ze(n) {
+                function Je(n) {
                     var e = z["*"],
                         t = n.keyCode || n.which || n.charCode;
                     if (M.filter.call(this, n)) {
                         if (-1 === P.indexOf(t = 93 !== t && 224 !== t ? t : 91) && 229 !== t && P.push(t), ["ctrlKey", "altKey", "shiftKey", "metaKey"].forEach(function(e) {
                                 var t = He[e];
                                 n[e] && -1 === P.indexOf(t) ? P.push(t) : !n[e] && -1 < P.indexOf(t) ? P.splice(P.indexOf(t), 1) : "metaKey" !== e || !n[e] || 3 !== P.length || n.ctrlKey || n.shiftKey || n.altKey || (P = P.slice(P.indexOf(t)))
                             }), t in C) {
@@ -55896,26 +55993,26 @@
                         mods: o,
                         shortcut: r[s],
                         method: n,
                         key: r[s],
                         splitKey: u
                     });
                     void 0 === a || (t = a, -1 < qe.indexOf(t)) || !window || (qe.push(a), Ue(a, "keydown", function(e) {
-                        Ze(e)
+                        Je(e)
                     }), Ue(window, "focus", function() {
                         P = []
                     }), Ue(a, "keyup", function(e) {
-                        Ze(e);
+                        Je(e);
                         var t = e.keyCode || e.which || e.charCode,
                             n = P.indexOf(t);
                         if (0 <= n && P.splice(n, 1), e.key && "meta" === e.key.toLowerCase() && P.splice(0, P.length), (t = 93 !== t && 224 !== t ? t : 91) in C)
                             for (var r in C[t] = !1, k) k[r] === t && (M[r] = !1)
                     }))
                 }
-                var Je, Qe, et = {
+                var Ze, Qe, et = {
                     setScope: Ke,
                     getScope: T,
                     deleteScope: function(e, t) {
                         var n, r, o;
                         for (o in e = e || T(), z)
                             if (Object.prototype.hasOwnProperty.call(z, o))
                                 for (n = z[o], r = 0; r < n.length;) n[r].scope === e ? n.splice(r, 1) : r++;
@@ -55951,15 +56048,15 @@
                                 })
                             }
                         } else Object.keys(z).forEach(function(e) {
                             return delete z[e]
                         })
                     }
                 };
-                for (Je in et) Object.prototype.hasOwnProperty.call(et, Je) && (M[Je] = et[Je]);
+                for (Ze in et) Object.prototype.hasOwnProperty.call(et, Ze) && (M[Ze] = et[Ze]);
                 "undefined" != typeof window && (Qe = window.hotkeys, M.noConflict = function(e) {
                     return e && window.hotkeys === M && (window.hotkeys = Qe), M
                 }, window.hotkeys = M);
 
                 function A(e, t, n, r) {
                     var o, i = arguments.length,
                         a = i < 3 ? t : null === r ? r = Object.getOwnPropertyDescriptor(t, n) : r;
```

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/metadata.json` & `feffery_utils_components-0.2.0a4/feffery_utils_components/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9843543956043955%*

 * *Differences: {"'src/lib/components/sortable/FefferySortableList.react.js'": "{'props': {'direction': "*

 * *                                                               "OrderedDict([('type', "*

 * *                                                               "OrderedDict([('name', 'enum'), "*

 * *                                                               "('value', [OrderedDict([('value', "*

 * *                                                               '"\'vertical\'"), (\'computed\', '*

 * *                                        […]*

```diff
@@ -7669,14 +7669,35 @@
                             {
                                 "name": "string"
                             }
                         ]
                     }
                 }
             },
+            "direction": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "'vertical'"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "'vertical'"
+                        },
+                        {
+                            "computed": false,
+                            "value": "'horizontal'"
+                        }
+                    ]
+                }
+            },
             "handleClassName": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "union",
                     "value": [
                         {
@@ -8184,14 +8205,77 @@
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             }
         }
     },
+    "src/lib/components/store/FefferyLocalStorage.js": {
+        "description": "",
+        "displayName": "FefferyLocalStorage",
+        "methods": [],
+        "props": {
+            "data": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "any"
+                }
+            },
+            "id": {
+                "description": "",
+                "required": true,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "initialSync": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "false"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
+            "loading_state": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "shape",
+                    "value": {
+                        "component_name": {
+                            "description": "Holds the name of the component that is loading",
+                            "name": "string",
+                            "required": false
+                        },
+                        "is_loading": {
+                            "description": "Determines if the component is loading or not",
+                            "name": "bool",
+                            "required": false
+                        },
+                        "prop_name": {
+                            "description": "Holds which property is loading",
+                            "name": "string",
+                            "required": false
+                        }
+                    }
+                }
+            },
+            "setProps": {
+                "description": "Dash-assigned callback that should be called to report property changes\r\nto Dash, to make them available for callbacks.",
+                "required": false,
+                "type": {
+                    "name": "func"
+                }
+            }
+        }
+    },
     "src/lib/components/store/FefferySessionStorage.js": {
         "description": "",
         "displayName": "FefferySessionStorage",
         "methods": [],
         "props": {
             "data": {
                 "description": "",
@@ -8203,14 +8287,25 @@
             "id": {
                 "description": "",
                 "required": true,
                 "type": {
                     "name": "string"
                 }
             },
+            "initialSync": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "false"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
             "loading_state": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "shape",
                     "value": {
                         "component_name": {
```

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components/package-info.json` & `feffery_utils_components-0.2.0a4/feffery_utils_components/package-info.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9652482269503546%*

 * *Differences: {"'dependencies'": "{'react-popout': '^3.0.0', 'react-popout-v2': '^0.0.8'}",*

 * * "'version'": "'0.2.0-a4'"}*

```diff
@@ -42,14 +42,16 @@
         "react-countup": "^6.4.2",
         "react-device-detect": "^2.2.2",
         "react-flip-numbers": "^3.0.7",
         "react-grid-layout": "^1.3.4",
         "react-highlight-words": "^0.18.0",
         "react-hot-toast": "^2.4.0",
         "react-lazy-load": "^3.1.14",
+        "react-popout": "^3.0.0",
+        "react-popout-v2": "^0.0.8",
         "react-resize-detector": "^7.1.2",
         "react-scroll": "^1.8.6",
         "react-shadow": "^19.0.3",
         "react-spinners-kit": "^1.9.1",
         "react-split": "^2.0.14",
         "react-stickynode": "^4.1.0",
         "react-syntax-highlighter": "^15.4.4",
@@ -113,9 +115,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_utils_components -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.0-a3"
+    "version": "0.2.0-a4"
 }
```

### Comparing `feffery_utils_components-0.2.0a3/feffery_utils_components.egg-info/SOURCES.txt` & `feffery_utils_components-0.2.0a4/feffery_utils_components.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,19 @@
 feffery_utils_components/FefferyInViewport.py
 feffery_utils_components/FefferyJsonViewer.py
 feffery_utils_components/FefferyKeyPress.py
 feffery_utils_components/FefferyLazyLoad.py
 feffery_utils_components/FefferyListenPaste.py
 feffery_utils_components/FefferyListenScroll.py
 feffery_utils_components/FefferyListenUnload.py
+feffery_utils_components/FefferyLocalStorage.py
 feffery_utils_components/FefferyLocation.py
 feffery_utils_components/FefferyMotion.py
 feffery_utils_components/FefferyMousePosition.py
+feffery_utils_components/FefferyPopout.py
 feffery_utils_components/FefferyQRCode.py
 feffery_utils_components/FefferyRawHTML.py
 feffery_utils_components/FefferyReload.py
 feffery_utils_components/FefferyResizable.py
 feffery_utils_components/FefferyResponsive.py
 feffery_utils_components/FefferyRgbColorPicker.py
 feffery_utils_components/FefferyScroll.py
```

### Comparing `feffery_utils_components-0.2.0a3/package.json` & `feffery_utils_components-0.2.0a4/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9652482269503546%*

 * *Differences: {"'dependencies'": "{'react-popout': '^3.0.0', 'react-popout-v2': '^0.0.8'}",*

 * * "'version'": "'0.2.0-a4'"}*

```diff
@@ -42,14 +42,16 @@
         "react-countup": "^6.4.2",
         "react-device-detect": "^2.2.2",
         "react-flip-numbers": "^3.0.7",
         "react-grid-layout": "^1.3.4",
         "react-highlight-words": "^0.18.0",
         "react-hot-toast": "^2.4.0",
         "react-lazy-load": "^3.1.14",
+        "react-popout": "^3.0.0",
+        "react-popout-v2": "^0.0.8",
         "react-resize-detector": "^7.1.2",
         "react-scroll": "^1.8.6",
         "react-shadow": "^19.0.3",
         "react-spinners-kit": "^1.9.1",
         "react-split": "^2.0.14",
         "react-stickynode": "^4.1.0",
         "react-syntax-highlighter": "^15.4.4",
@@ -113,9 +115,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_utils_components -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.0-a3"
+    "version": "0.2.0-a4"
 }
```

### Comparing `feffery_utils_components-0.2.0a3/setup.py` & `feffery_utils_components-0.2.0a4/setup.py`

 * *Files identical despite different names*

