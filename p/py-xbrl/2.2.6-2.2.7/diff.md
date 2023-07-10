# Comparing `tmp/py-xbrl-2.2.6.tar.gz` & `tmp/py-xbrl-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-xbrl-2.2.6.tar", last modified: Thu Feb  2 22:23:12 2023, max compression
+gzip compressed data, was "py-xbrl-2.2.7.tar", last modified: Mon Jul 10 10:18:32 2023, max compression
```

## Comparing `py-xbrl-2.2.6.tar` & `py-xbrl-2.2.7.tar`

### file list

```diff
@@ -1,27 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-02-02 22:23:12.423355 py-xbrl-2.2.6/
--rw-rw-rw-   0        0        0    35821 2021-01-27 14:34:43.000000 py-xbrl-2.2.6/LICENSE
--rw-rw-rw-   0        0        0     4006 2023-02-02 22:23:12.423355 py-xbrl-2.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     2941 2022-07-27 12:07:48.000000 py-xbrl-2.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-02-02 22:23:12.315486 py-xbrl-2.2.6/py_xbrl.egg-info/
--rw-rw-rw-   0        0        0     4006 2023-02-02 22:23:12.000000 py-xbrl-2.2.6/py_xbrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-02-02 22:23:12.000000 py-xbrl-2.2.6/py_xbrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-02 22:23:12.000000 py-xbrl-2.2.6/py_xbrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-02-02 22:23:12.000000 py-xbrl-2.2.6/py_xbrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-02-02 22:23:12.000000 py-xbrl-2.2.6/py_xbrl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-02 22:23:12.424321 py-xbrl-2.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1733 2023-02-02 22:21:23.000000 py-xbrl-2.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-02 22:23:12.385811 py-xbrl-2.2.6/xbrl/
--rw-rw-rw-   0        0        0     2701 2023-02-02 22:21:23.000000 py-xbrl-2.2.6/xbrl/__init__.py
--rw-rw-rw-   0        0        0     7475 2022-10-27 18:35:46.000000 py-xbrl-2.2.6/xbrl/cache.py
-drwxrwxrwx   0        0        0        0 2023-02-02 22:23:12.419311 py-xbrl-2.2.6/xbrl/helper/
--rw-rw-rw-   0        0        0        0 2021-01-21 10:29:50.000000 py-xbrl-2.2.6/xbrl/helper/__init__.py
--rw-rw-rw-   0        0        0     2929 2022-07-27 12:03:56.000000 py-xbrl-2.2.6/xbrl/helper/connection_manager.py
--rw-rw-rw-   0        0        0     2976 2022-02-18 08:57:21.000000 py-xbrl-2.2.6/xbrl/helper/text2num.py
--rw-rw-rw-   0        0        0     2785 2022-10-11 17:49:32.000000 py-xbrl-2.2.6/xbrl/helper/uri_helper.py
--rw-rw-rw-   0        0        0      986 2022-06-04 09:52:47.000000 py-xbrl-2.2.6/xbrl/helper/xml_parser.py
--rw-rw-rw-   0        0        0    33142 2023-01-11 21:29:32.000000 py-xbrl-2.2.6/xbrl/instance.py
--rw-rw-rw-   0        0        0    27789 2022-12-09 09:47:43.000000 py-xbrl-2.2.6/xbrl/linkbase.py
--rw-rw-rw-   0        0        0    53060 2022-10-11 17:49:32.000000 py-xbrl-2.2.6/xbrl/taxonomy.py
-drwxrwxrwx   0        0        0        0 2023-02-02 22:23:12.422321 py-xbrl-2.2.6/xbrl/transformations/
--rw-rw-rw-   0        0        0    21966 2023-02-02 22:08:52.000000 py-xbrl-2.2.6/xbrl/transformations/__init__.py
--rw-rw-rw-   0        0        0     3497 2022-02-17 21:04:36.000000 py-xbrl-2.2.6/xbrl/transformations/text2num.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:18:32.406223 py-xbrl-2.2.7/
+-rw-rw-rw-   0        0        0    35821 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/LICENSE
+-rw-rw-rw-   0        0        0     4006 2023-07-10 10:18:32.406223 py-xbrl-2.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2941 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 10:18:32.326031 py-xbrl-2.2.7/py_xbrl.egg-info/
+-rw-rw-rw-   0        0        0     4006 2023-07-10 10:18:32.000000 py-xbrl-2.2.7/py_xbrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-07-10 10:18:32.000000 py-xbrl-2.2.7/py_xbrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 10:18:32.000000 py-xbrl-2.2.7/py_xbrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-10 10:18:32.000000 py-xbrl-2.2.7/py_xbrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-10 10:18:32.000000 py-xbrl-2.2.7/py_xbrl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 10:18:32.406223 py-xbrl-2.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1733 2023-07-10 09:02:28.000000 py-xbrl-2.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:18:32.362889 py-xbrl-2.2.7/tests/
+-rw-rw-rw-   0        0        0     2504 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_cache.py
+-rw-rw-rw-   0        0        0     1436 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_local_instance.py
+-rw-rw-rw-   0        0        0     1670 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_local_linkbase.py
+-rw-rw-rw-   0        0        0     1157 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_local_taxonomy.py
+-rw-rw-rw-   0        0        0     2616 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_remote_instance.py
+-rw-rw-rw-   0        0        0     2238 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_remote_linkbase.py
+-rw-rw-rw-   0        0        0     2193 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_remote_taxonomy.py
+-rw-rw-rw-   0        0        0    16117 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_transformation.py
+-rw-rw-rw-   0        0        0     4603 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_uri_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:18:32.385845 py-xbrl-2.2.7/xbrl/
+-rw-rw-rw-   0        0        0     2701 2023-07-10 09:02:28.000000 py-xbrl-2.2.7/xbrl/__init__.py
+-rw-rw-rw-   0        0        0     7475 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/cache.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:18:32.400066 py-xbrl-2.2.7/xbrl/helper/
+-rw-rw-rw-   0        0        0        0 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/helper/__init__.py
+-rw-rw-rw-   0        0        0     2929 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/helper/connection_manager.py
+-rw-rw-rw-   0        0        0     2976 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/helper/text2num.py
+-rw-rw-rw-   0        0        0     2785 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/helper/uri_helper.py
+-rw-rw-rw-   0        0        0      986 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/helper/xml_parser.py
+-rw-rw-rw-   0        0        0    33142 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/instance.py
+-rw-rw-rw-   0        0        0    27789 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/linkbase.py
+-rw-rw-rw-   0        0        0    53683 2023-07-10 08:50:01.000000 py-xbrl-2.2.7/xbrl/taxonomy.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:18:32.405216 py-xbrl-2.2.7/xbrl/transformations/
+-rw-rw-rw-   0        0        0    21966 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/transformations/__init__.py
+-rw-rw-rw-   0        0        0     3497 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/transformations/text2num.py
```

### Comparing `py-xbrl-2.2.6/LICENSE` & `py-xbrl-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.6/PKG-INFO` & `py-xbrl-2.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-xbrl
-Version: 2.2.6
+Version: 2.2.7
 Summary: Parser for parsing XBRL and iXBRL files (instance documents, taxonomy schemas, taxonomy linkbases).
 Home-page: https://github.com/manusimidt/xbrl_parser
 Author: Manuel Schmidt
 Author-email: hello@schmidt-manuel.de
 License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-xbrl-2.2.6/README.md` & `py-xbrl-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.6/py_xbrl.egg-info/PKG-INFO` & `py-xbrl-2.2.7/py_xbrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-xbrl
-Version: 2.2.6
+Version: 2.2.7
 Summary: Parser for parsing XBRL and iXBRL files (instance documents, taxonomy schemas, taxonomy linkbases).
 Home-page: https://github.com/manusimidt/xbrl_parser
 Author: Manuel Schmidt
 Author-email: hello@schmidt-manuel.de
 License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-xbrl-2.2.6/setup.py` & `py-xbrl-2.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding='utf-8') as fd:
         return re.sub(text_type(r':[a-z]+:`~?(.*?)`'), text_type(r'``\1``'), fd.read())
 
 
 setup(
     name="py-xbrl",
-    version="2.2.6",
+    version="2.2.7",
     url="https://github.com/manusimidt/xbrl_parser",
     license='GNU General Public License v3 (GPLv3)',
     author="Manuel Schmidt",
     author_email="hello@schmidt-manuel.de",
 
     description="Parser for parsing XBRL and iXBRL files (instance documents, taxonomy schemas, taxonomy linkbases).",
     long_description_content_type="text/markdown",
```

### Comparing `py-xbrl-2.2.6/xbrl/__init__.py` & `py-xbrl-2.2.7/xbrl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 class ContextParseException(InstanceParseException):
     """
     Exception thrown when a Context could not be parsed
     """
     pass
 
 
-__version__ = '2.2.6'
+__version__ = '2.2.7'
 __author__ = 'Manuel Schmidt <hello@schmidt-manuel.de>'
 __all__ = [
     XbrlParseException,
     TaxonomyParseException,
     TaxonomyNotFound,
     InstanceParseException,
     ContextParseException,
```

### Comparing `py-xbrl-2.2.6/xbrl/cache.py` & `py-xbrl-2.2.7/xbrl/cache.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.6/xbrl/helper/connection_manager.py` & `py-xbrl-2.2.7/xbrl/helper/connection_manager.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.6/xbrl/helper/text2num.py` & `py-xbrl-2.2.7/xbrl/helper/text2num.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.6/xbrl/helper/uri_helper.py` & `py-xbrl-2.2.7/xbrl/helper/uri_helper.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.6/xbrl/helper/xml_parser.py` & `py-xbrl-2.2.7/xbrl/helper/xml_parser.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.6/xbrl/instance.py` & `py-xbrl-2.2.7/xbrl/instance.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.6/xbrl/linkbase.py` & `py-xbrl-2.2.7/xbrl/linkbase.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.6/xbrl/taxonomy.py` & `py-xbrl-2.2.7/xbrl/taxonomy.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,15 @@
     "http://fasb.org/dis/rcctmp05/2018-01-31": "http://xbrl.fasb.org/us-gaap/2018/dis/us-gaap-dis-rcctmp05-2018-01-31.xsd",
     "http://fasb.org/dis/rcctmp05/2019-01-31": "http://xbrl.fasb.org/us-gaap/2019/dis/us-gaap-dis-rcctmp05-2019-01-31.xsd",
     "http://fasb.org/srt/2018-01-31": "http://xbrl.fasb.org/srt/2018/elts/srt-2018-01-31.xsd",
     "http://fasb.org/srt/2019-01-31": "http://xbrl.fasb.org/srt/2019/elts/srt-2019-01-31.xsd",
     "http://fasb.org/srt/2020-01-31": "http://xbrl.fasb.org/srt/2020/elts/srt-2020-01-31.xsd",
     "http://fasb.org/srt/2021-01-31": "http://xbrl.fasb.org/srt/2021/elts/srt-2021-01-31.xsd",
     "http://fasb.org/srt/2022": "https://xbrl.fasb.org/srt/2022/elts/srt-2022.xsd",
+    "http://fasb.org/srt/2023": "https://xbrl.fasb.org/srt/2023/elts/srt-2023.xsd",
     "http://fasb.org/srt-roles/2018-01-31": "http://xbrl.fasb.org/srt/2018/elts/srt-roles-2018-01-31.xsd",
     "http://fasb.org/srt-roles/2019-01-31": "http://xbrl.fasb.org/srt/2019/elts/srt-roles-2019-01-31.xsd",
     "http://fasb.org/srt-roles/2020-01-31": "http://xbrl.fasb.org/srt/2020/elts/srt-roles-2020-01-31.xsd",
     "http://fasb.org/srt-roles/2021-01-31": "http://xbrl.fasb.org/srt/2021/elts/srt-roles-2021-01-31.xsd",
     "http://fasb.org/srt-types/2018-01-31": "http://xbrl.fasb.org/srt/2018/elts/srt-types-2018-01-31.xsd",
     "http://fasb.org/srt-types/2019-01-31": "http://xbrl.fasb.org/srt/2019/elts/srt-types-2019-01-31.xsd",
     "http://fasb.org/srt-types/2020-01-31": "http://xbrl.fasb.org/srt/2020/elts/srt-types-2020-01-31.xsd",
@@ -183,14 +184,16 @@
     "http://fasb.org/us-gaap/2016-01-31": "http://xbrl.fasb.org/us-gaap/2016/elts/us-gaap-2016-01-31.xsd",
     "http://fasb.org/us-gaap/2017-01-31": "http://xbrl.fasb.org/us-gaap/2017/elts/us-gaap-2017-01-31.xsd",
     "http://fasb.org/us-gaap/2018-01-31": "http://xbrl.fasb.org/us-gaap/2018/elts/us-gaap-2018-01-31.xsd",
     "http://fasb.org/us-gaap/2019-01-31": "http://xbrl.fasb.org/us-gaap/2019/elts/us-gaap-2019-01-31.xsd",
     "http://fasb.org/us-gaap/2020-01-31": "http://xbrl.fasb.org/us-gaap/2020/elts/us-gaap-2020-01-31.xsd",
     "http://fasb.org/us-gaap/2021-01-31": "http://xbrl.fasb.org/us-gaap/2021/elts/us-gaap-2021-01-31.xsd",
     "http://fasb.org/us-gaap/2022-01-31": "https://xbrl.fasb.org/us-gaap/2022/elts/us-gaap-2022.xsd",
+    "http://fasb.org/us-gaap/2022": "https://xbrl.fasb.org/us-gaap/2022/elts/us-gaap-2022.xsd",
+    "http://fasb.org/us-gaap/2023": "https://xbrl.fasb.org/us-gaap/2023/elts/us-gaap-2023.xsd",
 
     "http://fasb.org/us-roles/2011-01-31": "http://xbrl.fasb.org/us-gaap/2011/elts/us-roles-2011-01-31.xsd",
     "http://fasb.org/us-roles/2012-01-31": "http://xbrl.fasb.org/us-gaap/2012/elts/us-roles-2012-01-31.xsd",
     "http://fasb.org/us-roles/2013-01-31": "http://xbrl.fasb.org/us-gaap/2013/elts/us-roles-2013-01-31.xsd",
     "http://fasb.org/us-roles/2014-01-31": "http://xbrl.fasb.org/us-gaap/2014/elts/us-roles-2014-01-31.xsd",
     "http://fasb.org/us-roles/2015-01-31": "http://xbrl.fasb.org/us-gaap/2015/elts/us-roles-2015-01-31.xsd",
     "http://fasb.org/us-roles/2016-01-31": "http://xbrl.fasb.org/us-gaap/2016/elts/us-roles-2016-01-31.xsd",
@@ -271,14 +274,15 @@
     "http://xbrl.sec.gov/dei/2013-01-31": "https://xbrl.sec.gov/dei/2013/dei-2013-01-31.xsd",
     "http://xbrl.sec.gov/dei/2014-01-31": "https://xbrl.sec.gov/dei/2014/dei-2014-01-31.xsd",
     "http://xbrl.sec.gov/dei/2018-01-31": "https://xbrl.sec.gov/dei/2018/dei-2018-01-31.xsd",
     "http://xbrl.sec.gov/dei/2019-01-31": "https://xbrl.sec.gov/dei/2019/dei-2019-01-31.xsd",
     "http://xbrl.sec.gov/dei/2020-01-31": "https://xbrl.sec.gov/dei/2020/dei-2020-01-31.xsd",
     "http://xbrl.sec.gov/dei/2021": "https://xbrl.sec.gov/dei/2021/dei-2021.xsd",
     "http://xbrl.sec.gov/dei/2022": "https://xbrl.sec.gov/dei/2022/dei-2022.xsd",
+    "http://xbrl.sec.gov/dei/2023": "https://xbrl.sec.gov/dei/2023/dei-2023.xsd",
     "http://xbrl.sec.gov/dei/2021q4": "https://xbrl.sec.gov/dei/2021q4/dei-2021q4.xsd",
     "http://xbrl.sec.gov/dei-def/2021": "https://xbrl.sec.gov/dei/2021/dei-2021_def.xsd",
     "http://xbrl.sec.gov/dei-entire/2021": "https://xbrl.sec.gov/dei/2021/dei-entire-2021.xsd",
     "http://xbrl.sec.gov/dei-ent-std/2019-01-31": "https://xbrl.sec.gov/dei/2019/dei-ent-std-2019-01-31.xsd",
     "http://xbrl.sec.gov/dei-ent-std/2020-01-31": "https://xbrl.sec.gov/dei/2020/dei-ent-std-2020-01-31.xsd",
     "http://xbrl.sec.gov/dei-lab/2021": "https://xbrl.sec.gov/dei/2021/dei-2021_lab.xsd",
     "http://xbrl.sec.gov/dei-pre/2021": "https://xbrl.sec.gov/dei/2021/dei-2021_pre.xsd",
@@ -291,24 +295,27 @@
     "http://xbrl.sec.gov/exch/2015-01-31": "https://xbrl.sec.gov/exch/2015/exch-2015-01-31.xsd",
     "http://xbrl.sec.gov/exch/2016-01-31": "https://xbrl.sec.gov/exch/2016/exch-2016-01-31.xsd",
     "http://xbrl.sec.gov/exch/2017-01-31": "https://xbrl.sec.gov/exch/2017/exch-2017-01-31.xsd",
     "http://xbrl.sec.gov/exch/2018-01-31": "https://xbrl.sec.gov/exch/2018/exch-2018-01-31.xsd",
     "http://xbrl.sec.gov/exch/2019-01-31": "https://xbrl.sec.gov/exch/2019/exch-2019-01-31.xsd",
     "http://xbrl.sec.gov/exch/2020-01-31": "https://xbrl.sec.gov/exch/2020/exch-2020-01-31.xsd",
     "http://xbrl.sec.gov/exch/2021": "https://xbrl.sec.gov/exch/2021/exch-2021.xsd",
+    "http://xbrl.sec.gov/exch/2022": "https://xbrl.sec.gov/exch/2022/exch-2022.xsd",
+    "http://xbrl.sec.gov/exch/2023": "https://xbrl.sec.gov/exch/2023/exch-2023.xsd",
     "http://xbrl.sec.gov/exch-def/2021": "https://xbrl.sec.gov/exch/2021/exch-2021_def.xsd",
     "http://xbrl.sec.gov/exch-lab/2021": "https://xbrl.sec.gov/exch/2021/exch-2021_lab.xsd",
     "http://xbrl.sec.gov/exch-pre/2021": "https://xbrl.sec.gov/exch/2021/exch-2021_pre.xsd",
     "http://xbrl.sec.gov/invest/2011-01-31": "https://xbrl.sec.gov/invest/2011/invest-2011-01-31.xsd",
     "http://xbrl.sec.gov/invest/2012-01-31": "https://xbrl.sec.gov/invest/2012/invest-2012-01-31.xsd",
     "http://xbrl.sec.gov/invest/2013-01-31": "https://xbrl.sec.gov/invest/2013/invest-2013-01-31.xsd",
     "http://xbrl.sec.gov/naics/2011-01-31": "https://xbrl.sec.gov/naics/2011/naics-2011-01-31.xsd",
     "http://xbrl.sec.gov/naics/2017-01-31": "https://xbrl.sec.gov/naics/2017/naics-2017-01-31.xsd",
     "http://xbrl.sec.gov/naics/2021": "https://xbrl.sec.gov/naics/2021/naics-2021.xsd",
     "http://xbrl.sec.gov/naics/2022": "https://xbrl.sec.gov/naics/2022/naics-2022.xsd",
+    "http://xbrl.sec.gov/naics/2023": "https://xbrl.sec.gov/naics/2023/naics-2023.xsd",
     "http://xbrl.sec.gov/rr/2010-02-28": "https://xbrl.sec.gov/rr/2010/rr-2010-02-28.xsd",
     "http://xbrl.sec.gov/rr/2012-01-31": "https://xbrl.sec.gov/rr/2012/rr-2012-01-31.xsd",
     "http://xbrl.sec.gov/rr/2018-01-31": "https://xbrl.sec.gov/rr/2018/rr-2018-01-31.xsd",
     "http://xbrl.sec.gov/rr/2021": "https://xbrl.sec.gov/rr/2021/rr-2021.xsd",
     "http://xbrl.sec.gov/rr-cal/2010-02-28": "https://xbrl.sec.gov/rr/2010/rr-cal-2010-02-28.xsd",
     "http://xbrl.sec.gov/rr-cal/2012-01-31": "https://xbrl.sec.gov/rr/2012/rr-cal-2012-01-31.xsd",
     "http://xbrl.sec.gov/rr-cal/2018-01-31": "https://xbrl.sec.gov/rr/2018/rr-cal-2018-01-31.xsd",
```

### Comparing `py-xbrl-2.2.6/xbrl/transformations/__init__.py` & `py-xbrl-2.2.7/xbrl/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.6/xbrl/transformations/text2num.py` & `py-xbrl-2.2.7/xbrl/transformations/text2num.py`

 * *Files identical despite different names*

