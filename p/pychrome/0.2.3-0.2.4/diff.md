# Comparing `tmp/pychrome-0.2.3.tar.gz` & `tmp/pychrome-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pychrome-0.2.3.tar", last modified: Tue May  7 14:43:01 2019, max compression
+gzip compressed data, was "pychrome-0.2.4.tar", last modified: Mon Jul 10 14:08:10 2023, max compression
```

## Comparing `pychrome-0.2.3.tar` & `pychrome-0.2.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 fate0      (501) staff       (20)        0 2019-05-07 14:43:01.000000 pychrome-0.2.3/
--rw-r--r--   0 fate0      (501) staff       (20)     1495 2019-05-07 14:17:36.000000 pychrome-0.2.3/LICENSE
--rw-r--r--   0 fate0      (501) staff       (20)      138 2019-05-07 14:17:36.000000 pychrome-0.2.3/MANIFEST.in
--rw-r--r--   0 fate0      (501) staff       (20)     5330 2019-05-07 14:43:01.000000 pychrome-0.2.3/PKG-INFO
--rw-r--r--   0 fate0      (501) staff       (20)     3358 2019-05-07 14:17:36.000000 pychrome-0.2.3/README.md
-drwxr-xr-x   0 fate0      (501) staff       (20)        0 2019-05-07 14:43:01.000000 pychrome-0.2.3/examples/
--rw-r--r--   0 fate0      (501) staff       (20)      637 2019-05-07 14:17:37.000000 pychrome-0.2.3/examples/demo1.py
--rw-r--r--   0 fate0      (501) staff       (20)      445 2019-05-07 14:17:37.000000 pychrome-0.2.3/examples/demo2.py
--rw-r--r--   0 fate0      (501) staff       (20)     2537 2019-05-07 14:17:37.000000 pychrome-0.2.3/examples/multi_tabs_navigate.py
--rw-r--r--   0 fate0      (501) staff       (20)     2034 2019-05-07 14:17:37.000000 pychrome-0.2.3/examples/multi_tabs_pdf.py
--rw-r--r--   0 fate0      (501) staff       (20)     2042 2019-05-07 14:17:37.000000 pychrome-0.2.3/examples/multi_tabs_screenshot.py
-drwxr-xr-x   0 fate0      (501) staff       (20)        0 2019-05-07 14:43:01.000000 pychrome-0.2.3/pychrome/
--rw-r--r--   0 fate0      (501) staff       (20)      180 2019-05-07 14:41:45.000000 pychrome-0.2.3/pychrome/__init__.py
--rw-r--r--   0 fate0      (501) staff       (20)     2133 2019-05-07 14:17:37.000000 pychrome-0.2.3/pychrome/browser.py
--rw-r--r--   0 fate0      (501) staff       (20)     2940 2019-05-07 14:17:37.000000 pychrome-0.2.3/pychrome/cli.py
--rw-r--r--   0 fate0      (501) staff       (20)      416 2019-05-07 14:17:37.000000 pychrome-0.2.3/pychrome/exceptions.py
--rw-r--r--   0 fate0      (501) staff       (20)     7121 2019-05-07 14:17:37.000000 pychrome-0.2.3/pychrome/tab.py
-drwxr-xr-x   0 fate0      (501) staff       (20)        0 2019-05-07 14:43:01.000000 pychrome-0.2.3/pychrome.egg-info/
--rw-r--r--   0 fate0      (501) staff       (20)     5330 2019-05-07 14:43:01.000000 pychrome-0.2.3/pychrome.egg-info/PKG-INFO
--rw-r--r--   0 fate0      (501) staff       (20)      570 2019-05-07 14:43:01.000000 pychrome-0.2.3/pychrome.egg-info/SOURCES.txt
--rw-r--r--   0 fate0      (501) staff       (20)        1 2019-05-07 14:43:01.000000 pychrome-0.2.3/pychrome.egg-info/dependency_links.txt
--rw-r--r--   0 fate0      (501) staff       (20)       48 2019-05-07 14:43:01.000000 pychrome-0.2.3/pychrome.egg-info/entry_points.txt
--rw-r--r--   0 fate0      (501) staff       (20)        1 2019-05-07 14:43:01.000000 pychrome-0.2.3/pychrome.egg-info/not-zip-safe
--rw-r--r--   0 fate0      (501) staff       (20)       53 2019-05-07 14:43:01.000000 pychrome-0.2.3/pychrome.egg-info/requires.txt
--rw-r--r--   0 fate0      (501) staff       (20)        9 2019-05-07 14:43:01.000000 pychrome-0.2.3/pychrome.egg-info/top_level.txt
--rw-r--r--   0 fate0      (501) staff       (20)       67 2019-05-07 14:43:01.000000 pychrome-0.2.3/setup.cfg
--rw-r--r--   0 fate0      (501) staff       (20)     1533 2019-05-07 14:17:37.000000 pychrome-0.2.3/setup.py
-drwxr-xr-x   0 fate0      (501) staff       (20)        0 2019-05-07 14:43:01.000000 pychrome-0.2.3/tests/
--rw-r--r--   0 fate0      (501) staff       (20)     1982 2019-05-07 14:17:37.000000 pychrome-0.2.3/tests/test_browser.py
--rw-r--r--   0 fate0      (501) staff       (20)     1802 2019-05-07 14:17:37.000000 pychrome-0.2.3/tests/test_multi_tabs.py
--rw-r--r--   0 fate0      (501) staff       (20)     7095 2019-05-07 14:17:37.000000 pychrome-0.2.3/tests/test_single_tab.py
+drwxr-xr-x   0 fate0      (501) staff       (20)        0 2023-07-10 14:08:10.849187 pychrome-0.2.4/
+-rw-r--r--   0 fate0      (501) staff       (20)     1495 2023-07-10 13:49:53.000000 pychrome-0.2.4/LICENSE
+-rw-r--r--   0 fate0      (501) staff       (20)      138 2023-07-10 13:49:53.000000 pychrome-0.2.4/MANIFEST.in
+-rw-r--r--   0 fate0      (501) staff       (20)     4153 2023-07-10 14:08:10.849242 pychrome-0.2.4/PKG-INFO
+-rw-r--r--   0 fate0      (501) staff       (20)     3358 2023-07-10 13:49:53.000000 pychrome-0.2.4/README.md
+drwxr-xr-x   0 fate0      (501) staff       (20)        0 2023-07-10 14:08:10.847452 pychrome-0.2.4/examples/
+-rw-r--r--   0 fate0      (501) staff       (20)      637 2023-07-10 13:49:53.000000 pychrome-0.2.4/examples/demo1.py
+-rw-r--r--   0 fate0      (501) staff       (20)      445 2023-07-10 13:49:53.000000 pychrome-0.2.4/examples/demo2.py
+-rw-r--r--   0 fate0      (501) staff       (20)     2537 2023-07-10 13:49:53.000000 pychrome-0.2.4/examples/multi_tabs_navigate.py
+-rw-r--r--   0 fate0      (501) staff       (20)     2034 2023-07-10 13:49:53.000000 pychrome-0.2.4/examples/multi_tabs_pdf.py
+-rw-r--r--   0 fate0      (501) staff       (20)     2042 2023-07-10 13:49:53.000000 pychrome-0.2.4/examples/multi_tabs_screenshot.py
+-rw-r--r--   0 fate0      (501) staff       (20)     2196 2023-07-10 13:49:53.000000 pychrome-0.2.4/examples/post_request.py
+drwxr-xr-x   0 fate0      (501) staff       (20)        0 2023-07-10 14:08:10.847997 pychrome-0.2.4/pychrome/
+-rw-r--r--   0 fate0      (501) staff       (20)      180 2023-07-10 13:50:28.000000 pychrome-0.2.4/pychrome/__init__.py
+-rw-r--r--   0 fate0      (501) staff       (20)     2133 2023-07-10 13:49:53.000000 pychrome-0.2.4/pychrome/browser.py
+-rw-r--r--   0 fate0      (501) staff       (20)     2940 2023-07-10 13:49:53.000000 pychrome-0.2.4/pychrome/cli.py
+-rw-r--r--   0 fate0      (501) staff       (20)      416 2023-07-10 13:49:53.000000 pychrome-0.2.4/pychrome/exceptions.py
+-rw-r--r--   0 fate0      (501) staff       (20)     7143 2023-07-10 13:49:53.000000 pychrome-0.2.4/pychrome/tab.py
+drwxr-xr-x   0 fate0      (501) staff       (20)        0 2023-07-10 14:08:10.848775 pychrome-0.2.4/pychrome.egg-info/
+-rw-r--r--   0 fate0      (501) staff       (20)     4153 2023-07-10 14:08:10.000000 pychrome-0.2.4/pychrome.egg-info/PKG-INFO
+-rw-r--r--   0 fate0      (501) staff       (20)      595 2023-07-10 14:08:10.000000 pychrome-0.2.4/pychrome.egg-info/SOURCES.txt
+-rw-r--r--   0 fate0      (501) staff       (20)        1 2023-07-10 14:08:10.000000 pychrome-0.2.4/pychrome.egg-info/dependency_links.txt
+-rw-r--r--   0 fate0      (501) staff       (20)       47 2023-07-10 14:08:10.000000 pychrome-0.2.4/pychrome.egg-info/entry_points.txt
+-rw-r--r--   0 fate0      (501) staff       (20)        1 2023-07-10 13:52:00.000000 pychrome-0.2.4/pychrome.egg-info/not-zip-safe
+-rw-r--r--   0 fate0      (501) staff       (20)       53 2023-07-10 14:08:10.000000 pychrome-0.2.4/pychrome.egg-info/requires.txt
+-rw-r--r--   0 fate0      (501) staff       (20)        9 2023-07-10 14:08:10.000000 pychrome-0.2.4/pychrome.egg-info/top_level.txt
+-rw-r--r--   0 fate0      (501) staff       (20)       67 2023-07-10 14:08:10.849456 pychrome-0.2.4/setup.cfg
+-rw-r--r--   0 fate0      (501) staff       (20)     1584 2023-07-10 14:07:34.000000 pychrome-0.2.4/setup.py
+drwxr-xr-x   0 fate0      (501) staff       (20)        0 2023-07-10 14:08:10.849091 pychrome-0.2.4/tests/
+-rw-r--r--   0 fate0      (501) staff       (20)     1982 2023-07-10 13:49:53.000000 pychrome-0.2.4/tests/test_browser.py
+-rw-r--r--   0 fate0      (501) staff       (20)     1802 2023-07-10 13:49:53.000000 pychrome-0.2.4/tests/test_multi_tabs.py
+-rw-r--r--   0 fate0      (501) staff       (20)     7095 2023-07-10 13:49:53.000000 pychrome-0.2.4/tests/test_single_tab.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pychrome-0.2.3/LICENSE` & `pychrome-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pychrome-0.2.3/README.md` & `pychrome-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pychrome-0.2.3/examples/demo1.py` & `pychrome-0.2.4/examples/demo1.py`

 * *Files identical despite different names*

### Comparing `pychrome-0.2.3/examples/multi_tabs_navigate.py` & `pychrome-0.2.4/examples/multi_tabs_navigate.py`

 * *Files identical despite different names*

### Comparing `pychrome-0.2.3/examples/multi_tabs_pdf.py` & `pychrome-0.2.4/examples/multi_tabs_pdf.py`

 * *Files identical despite different names*

### Comparing `pychrome-0.2.3/examples/multi_tabs_screenshot.py` & `pychrome-0.2.4/examples/multi_tabs_screenshot.py`

 * *Files identical despite different names*

### Comparing `pychrome-0.2.3/pychrome/browser.py` & `pychrome-0.2.4/pychrome/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         if self.dev_url not in self._all_tabs:
             self._tabs = self._all_tabs[self.dev_url] = {}
         else:
             self._tabs = self._all_tabs[self.dev_url]
 
     def new_tab(self, url=None, timeout=None):
         url = url or ''
-        rp = requests.get("%s/json/new?%s" % (self.dev_url, url), json=True, timeout=timeout)
+        rp = requests.put("%s/json/new?%s" % (self.dev_url, url), json=True, timeout=timeout)
         tab = Tab(**rp.json())
         self._tabs[tab.id] = tab
         return tab
 
     def list_tab(self, timeout=None):
         rp = requests.get("%s/json" % self.dev_url, json=True, timeout=timeout)
         tabs_map = {}
```

### Comparing `pychrome-0.2.3/pychrome/cli.py` & `pychrome-0.2.4/pychrome/cli.py`

 * *Files identical despite different names*

### Comparing `pychrome-0.2.3/pychrome/tab.py` & `pychrome-0.2.4/pychrome/tab.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 
         if not self._websocket_url:
             raise RuntimeException("Already has another client connect to this tab")
 
         self._started = True
         self.status = self.status_started
         self._stopped.clear()
-        self._ws = websocket.create_connection(self._websocket_url, enable_multithread=True)
+        self._ws = websocket.create_connection(self._websocket_url, enable_multithread=True, suppress_origin=True)
         self._recv_th.start()
         self._handle_event_th.start()
         return True
 
     def stop(self):
         if self._stopped.is_set():
             return False
```

### Comparing `pychrome-0.2.3/pychrome.egg-info/SOURCES.txt` & `pychrome-0.2.4/pychrome.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 setup.py
 examples/demo1.py
 examples/demo2.py
 examples/multi_tabs_navigate.py
 examples/multi_tabs_pdf.py
 examples/multi_tabs_screenshot.py
+examples/post_request.py
 pychrome/__init__.py
 pychrome/browser.py
 pychrome/cli.py
 pychrome/exceptions.py
 pychrome/tab.py
 pychrome.egg-info/PKG-INFO
 pychrome.egg-info/SOURCES.txt
```

### Comparing `pychrome-0.2.3/setup.py` & `pychrome-0.2.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 ]
 
 setup(
     name='pychrome',
     version=version,
     description="A Python Package for the Google Chrome Dev Protocol",
     long_description=readme,
+    long_description_content_type="text/markdown",
     author="fate0",
     author_email='fate0@fatezero.org',
     url='https://github.com/fate0/pychrome',
     packages=find_packages(),
     package_dir={},
     entry_points={
         'console_scripts': [
```

### Comparing `pychrome-0.2.3/tests/test_browser.py` & `pychrome-0.2.4/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `pychrome-0.2.3/tests/test_multi_tabs.py` & `pychrome-0.2.4/tests/test_multi_tabs.py`

 * *Files identical despite different names*

### Comparing `pychrome-0.2.3/tests/test_single_tab.py` & `pychrome-0.2.4/tests/test_single_tab.py`

 * *Files identical despite different names*

