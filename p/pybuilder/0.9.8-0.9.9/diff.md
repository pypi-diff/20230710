# Comparing `tmp/pybuilder-0.9.8.tar.gz` & `tmp/pybuilder-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybuilder-0.9.8.tar", last modified: Mon Mar 11 12:16:38 2013, max compression
+gzip compressed data, was "dist/pybuilder-0.9.9.tar", last modified: Fri Aug 16 07:33:49 2013, max compression
```

## Comparing `pybuilder-0.9.8.tar` & `pybuilder-0.9.9.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxr-x   0 mgruber  (40169) admins    (1000)        0 2013-03-11 12:16:38.000000 pybuilder-0.9.8/
--rwxrwxr-x   0 mgruber  (40169) admins    (1000)      761 2013-03-11 11:56:35.000000 pybuilder-0.9.8/pyb
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     1130 2013-03-11 12:16:38.000000 pybuilder-0.9.8/PKG-INFO
-drwxrwxr-x   0 mgruber  (40169) admins    (1000)        0 2013-03-11 12:16:38.000000 pybuilder-0.9.8/pybuilder/
--rw-rw-r--   0 mgruber  (40169) admins    (1000)      652 2013-03-11 11:56:35.000000 pybuilder-0.9.8/pybuilder/__init__.py
-drwxrwxr-x   0 mgruber  (40169) admins    (1000)        0 2013-03-11 12:16:38.000000 pybuilder-0.9.8/pybuilder/plugins/
-drwxrwxr-x   0 mgruber  (40169) admins    (1000)        0 2013-03-11 12:16:38.000000 pybuilder-0.9.8/pybuilder/plugins/python/
--rw-rw-r--   0 mgruber  (40169) admins    (1000)      629 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/__init__.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     3285 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/flake8_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     5722 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/coverage_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     4466 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/pychecker_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)      891 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/setuptools_plugin_helper.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     3646 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/pydev_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     1995 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/python_plugin_helper.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     4820 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/install_dependencies_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     1454 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/pylint_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     1477 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/pep8_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     7260 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/distutils_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     3541 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/unittest_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     4768 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/integrationtest_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     1751 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/pymetrics_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     1266 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/pyfix_unittest_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     2983 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/pyfix_plugin_impl.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     1724 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/django_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     4344 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/python/core_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)      639 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/__init__.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)      827 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/analysis_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     2091 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/filter_resources_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     1828 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/copy_resources_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     1816 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/source_distribution_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     2563 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/plugins/core_plugin.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)    10835 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/cli.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)    12131 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/core.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     5959 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/utils.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     9906 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/reactor.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     9911 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/execution.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     1806 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/pluginloader.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     3123 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/terminal.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     3359 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pybuilder/errors.py
-drwxrwxr-x   0 mgruber  (40169) admins    (1000)        0 2013-03-11 12:16:38.000000 pybuilder-0.9.8/pythonbuilder/
--rw-rw-r--   0 mgruber  (40169) admins    (1000)      756 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pythonbuilder/__init__.py
--rw-rw-r--   0 mgruber  (40169) admins    (1000)       29 2013-03-11 09:30:53.000000 pybuilder-0.9.8/pythonbuilder/core.py
-drwxrwxr-x   0 mgruber  (40169) admins    (1000)        0 2013-03-11 12:16:38.000000 pybuilder-0.9.8/pybuilder.egg-info/
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     1130 2013-03-11 12:16:38.000000 pybuilder-0.9.8/pybuilder.egg-info/PKG-INFO
--rw-rw-r--   0 mgruber  (40169) admins    (1000)        1 2013-03-11 11:56:37.000000 pybuilder-0.9.8/pybuilder.egg-info/zip-safe
--rw-rw-r--   0 mgruber  (40169) admins    (1000)       24 2013-03-11 12:16:38.000000 pybuilder-0.9.8/pybuilder.egg-info/top_level.txt
--rw-rw-r--   0 mgruber  (40169) admins    (1000)     1456 2013-03-11 12:16:38.000000 pybuilder-0.9.8/pybuilder.egg-info/SOURCES.txt
--rw-rw-r--   0 mgruber  (40169) admins    (1000)        1 2013-03-11 12:16:38.000000 pybuilder-0.9.8/pybuilder.egg-info/dependency_links.txt
--rw-rw-r--   0 mgruber  (40169) admins    (1000)       59 2013-03-11 12:16:38.000000 pybuilder-0.9.8/setup.cfg
--rwxr-xr-x   0 mgruber  (40169) admins    (1000)     1403 2013-03-11 11:56:35.000000 pybuilder-0.9.8/setup.py
+drwxrwxr-x   0 max       (9999) max       (9999)        0 2013-08-16 07:33:49.000000 pybuilder-0.9.9/
+-rw-rw-r--   0 max       (9999) max       (9999)       59 2013-08-16 07:33:49.000000 pybuilder-0.9.9/setup.cfg
+drwxrwxr-x   0 max       (9999) max       (9999)        0 2013-08-16 07:33:49.000000 pybuilder-0.9.9/pybuilder/
+-rw-rw-r--   0 max       (9999) max       (9999)    10250 2013-08-15 12:20:43.000000 pybuilder-0.9.9/pybuilder/execution.py
+-rw-rw-r--   0 max       (9999) max       (9999)     3123 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/terminal.py
+-rw-rw-r--   0 max       (9999) max       (9999)     3359 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/errors.py
+-rw-rw-r--   0 max       (9999) max       (9999)    12131 2013-08-15 11:53:22.000000 pybuilder-0.9.9/pybuilder/core.py
+-rw-rw-r--   0 max       (9999) max       (9999)      652 2013-08-16 07:33:21.000000 pybuilder-0.9.9/pybuilder/__init__.py
+drwxrwxr-x   0 max       (9999) max       (9999)        0 2013-08-16 07:33:49.000000 pybuilder-0.9.9/pybuilder/plugins/
+drwxrwxr-x   0 max       (9999) max       (9999)        0 2013-08-16 07:33:49.000000 pybuilder-0.9.9/pybuilder/plugins/python/
+-rw-rw-r--   0 max       (9999) max       (9999)     4819 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/python/install_dependencies_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     1266 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/python/pyfix_unittest_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     3541 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/python/unittest_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)      629 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/python/__init__.py
+-rw-rw-r--   0 max       (9999) max       (9999)     5722 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/python/coverage_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     4344 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/python/core_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     3285 2013-08-15 13:39:44.000000 pybuilder-0.9.9/pybuilder/plugins/python/flake8_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     1751 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/python/pymetrics_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     1995 2013-08-15 13:15:45.000000 pybuilder-0.9.9/pybuilder/plugins/python/python_plugin_helper.py
+-rw-rw-r--   0 max       (9999) max       (9999)     4768 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/python/integrationtest_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)      891 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/python/setuptools_plugin_helper.py
+-rw-rw-r--   0 max       (9999) max       (9999)     1724 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/python/django_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     2983 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/python/pyfix_plugin_impl.py
+-rw-rw-r--   0 max       (9999) max       (9999)     3638 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/python/pydev_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     1493 2013-07-22 07:21:40.000000 pybuilder-0.9.9/pybuilder/plugins/python/pylint_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     7260 2013-08-15 11:52:40.000000 pybuilder-0.9.9/pybuilder/plugins/python/distutils_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     4466 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/python/pychecker_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     1477 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/python/pep8_plugin.py
+-rw-rw-rw-   0 max       (9999) max       (9999)     2877 2013-08-15 15:11:36.000000 pybuilder-0.9.9/pybuilder/plugins/ronn_manpage_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     2091 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/filter_resources_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)      639 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/__init__.py
+-rw-rw-r--   0 max       (9999) max       (9999)      827 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/analysis_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     2563 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/core_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     1816 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/source_distribution_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     1828 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/plugins/copy_resources_plugin.py
+-rw-rw-r--   0 max       (9999) max       (9999)     5975 2013-08-15 13:29:44.000000 pybuilder-0.9.9/pybuilder/utils.py
+-rw-rw-r--   0 max       (9999) max       (9999)    10835 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/cli.py
+-rw-rw-r--   0 max       (9999) max       (9999)     1806 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/pluginloader.py
+-rw-rw-r--   0 max       (9999) max       (9999)     9906 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pybuilder/reactor.py
+-rw-rw-r--   0 max       (9999) max       (9999)     1516 2013-08-16 07:33:49.000000 pybuilder-0.9.9/PKG-INFO
+-rwxr-xr-x   0 max       (9999) max       (9999)     1726 2013-08-16 07:33:21.000000 pybuilder-0.9.9/setup.py
+drwxrwxr-x   0 max       (9999) max       (9999)        0 2013-08-16 07:33:49.000000 pybuilder-0.9.9/pybuilder.egg-info/
+-rw-rw-r--   0 max       (9999) max       (9999)     1497 2013-08-16 07:33:49.000000 pybuilder-0.9.9/pybuilder.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (9999) max       (9999)     1516 2013-08-16 07:33:49.000000 pybuilder-0.9.9/pybuilder.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (9999) max       (9999)       24 2013-08-16 07:33:49.000000 pybuilder-0.9.9/pybuilder.egg-info/top_level.txt
+-rw-rw-r--   0 max       (9999) max       (9999)        1 2013-08-16 07:33:22.000000 pybuilder-0.9.9/pybuilder.egg-info/zip-safe
+-rw-rw-r--   0 max       (9999) max       (9999)        1 2013-08-16 07:33:49.000000 pybuilder-0.9.9/pybuilder.egg-info/dependency_links.txt
+drwxrwxr-x   0 max       (9999) max       (9999)        0 2013-08-16 07:33:49.000000 pybuilder-0.9.9/pythonbuilder/
+-rw-rw-r--   0 max       (9999) max       (9999)       29 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pythonbuilder/core.py
+-rw-rw-r--   0 max       (9999) max       (9999)      756 2013-07-03 14:01:31.000000 pybuilder-0.9.9/pythonbuilder/__init__.py
+-rwxrwxr-x   0 max       (9999) max       (9999)      761 2013-08-16 07:33:21.000000 pybuilder-0.9.9/pyb
```

### Comparing `pybuilder-0.9.8/pyb` & `pybuilder-0.9.9/pyb`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/PKG-INFO` & `pybuilder-0.9.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-Metadata-Version: 1.1
-Name: pybuilder
-Version: 0.9.8
-Summary: An extensible, easy to use continuous build tool for Python
-Home-page: http://pybuilder.github.com
-Author: Alexander Metzner, Michael Gruber, Udo Juettner
-Author-email: alexander.metzner@gmail.com, aelgru@gmail.com, udo.juettner@gmail.com
-License: Apache License
-Description: PyBuilder is a continuous build tool for multiple languages.
-        
-        PyBuilder primarily targets Python projects but due to its extensible
-        nature it can be used for other languages as well.
-        
-        PyBuilder features a powerful yet easy to use plugin mechanism which 
-        allows programmers to extend the tool in an unlimited way.  
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Testing
+#!/usr/bin/env python
+
+from setuptools import setup
+
+if __name__ == '__main__':
+    setup(
+          name = 'pybuilder',
+          version = '0.9.9',
+          description = 'An extensible, easy to use continuous build tool for Python',
+          long_description = '''PyBuilder is a continuous build tool for multiple languages.
+
+PyBuilder primarily targets Python projects but due to its extensible
+nature it can be used for other languages as well.
+
+PyBuilder features a powerful yet easy to use plugin mechanism which
+allows programmers to extend the tool in an unlimited way.
+''',
+          author = "Alexander Metzner, Michael Gruber, Udo Juettner",
+          author_email = "alexander.metzner@gmail.com, aelgru@gmail.com, udo.juettner@gmail.com",
+          license = 'Apache License',
+          url = 'http://pybuilder.github.com',
+          scripts = ['pyb'],
+          packages = ['pybuilder', 'pythonbuilder', 'pybuilder.plugins', 'pybuilder.plugins.python'],
+          classifiers = ['Programming Language :: Python', 'Programming Language :: Python :: Implementation :: CPython', 'Programming Language :: Python :: Implementation :: PyPy', 'Programming Language :: Python :: 2.6', 'Programming Language :: Python :: 2.7', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.2', 'Programming Language :: Python :: 3.3', 'Development Status :: 3 - Alpha', 'Environment :: Console', 'Intended Audience :: Developers', 'License :: OSI Approved :: Apache Software License', 'Topic :: Software Development :: Build Tools', 'Topic :: Software Development :: Quality Assurance', 'Topic :: Software Development :: Testing'],
+          
+          
+          
+          
+          zip_safe=True
+    )
```

### Comparing `pybuilder-0.9.8/pybuilder/__init__.py` & `pybuilder-0.9.9/pybuilder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
```

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/__init__.py` & `pybuilder-0.9.9/pybuilder/plugins/python/__init__.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/flake8_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/python/flake8_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/coverage_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/python/coverage_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/pychecker_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/python/pychecker_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/setuptools_plugin_helper.py` & `pybuilder-0.9.9/pybuilder/plugins/python/setuptools_plugin_helper.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/pydev_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/python/pydev_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import os
 import string
 
 from pybuilder.core import init, task, description
 
 _DOT_PROJECT_TEMPLATE = string.Template("""<?xml version="1.0" encoding="UTF-8"?>
 
-<!-- This file has been generated by the Pythonbuilder Pydev Plugin -->
+<!-- This file has been generated by the PyBuilder Pydev Plugin -->
 
 <projectDescription>
     <name>${project_name}</name>
     <comment></comment>
     <projects>
     </projects>
     <buildSpec>
@@ -42,15 +42,15 @@
 """)
 
 _DOT_PYDEVPROJECT_PATH_LINE_TEMPLATE = string.Template("\t\t<path>/$project_name/$path</path>\n")
 
 _DOT_PYDEVPROJECT_TEMPLATE = string.Template("""<?xml version="1.0" encoding="UTF-8" standalone="no"?>
 <?eclipse-pydev version="1.0"?>
 
-<!-- This file has been generated by the Pythonbuilder Pydev Plugin -->
+<!-- This file has been generated by the PyBuilder Pydev Plugin -->
 
 <pydev_project>
     <pydev_property name="org.python.pydev.PYTHON_PROJECT_INTERPRETER">${interpreter}</pydev_property>
     <pydev_property name="org.python.pydev.PYTHON_PROJECT_VERSION">${version}</pydev_property>
     <pydev_pathproperty name="org.python.pydev.PROJECT_SOURCE_PATH">
 $paths
     </pydev_pathproperty>
```

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/python_plugin_helper.py` & `pybuilder-0.9.9/pybuilder/plugins/python/python_plugin_helper.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/install_dependencies_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/python/install_dependencies_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     project.set_property_if_unset("install_dependencies_extra_index_url", None)
     project.set_property_if_unset("install_dependencies_use_mirrors", True)
     project.set_property_if_unset("install_dependencies_upgrade", False)
 
 
 @after("prepare")
 def check_pip_available(logger):
-    logger.debug("Chechking if pip is available")
+    logger.debug("Checking if pip is available")
     assert_can_execute("pip", "pip", "plugin python.install_dependencies")
 
 
 @task
 @description("Installs all (both runtime and build) dependencies specified in the build descriptor")
 def install_dependencies(logger, project):
     logger.info("Installing all dependencies")
```

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/pylint_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/python/pylint_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 use_plugin("analysis")
 
 DEFAULT_PYLINT_OPTIONS = ["--max-line-length=100", "--no-docstring-rgx=.*"]
 
 
 @init
 def init_pylint(project):
+    project.build_depends_on("pylint")
     project.set_property_if_unset("pylint_options", DEFAULT_PYLINT_OPTIONS)
 
 
 @after("prepare")
 def check_pylint_availability(logger):
     logger.debug("Checking availability of pychecker")
     assert_can_execute(("pylint", ), "pylint", "plugin python.pylint")
```

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/pep8_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/python/pep8_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/distutils_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/python/distutils_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/unittest_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/python/unittest_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/integrationtest_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/python/integrationtest_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/pymetrics_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/python/pymetrics_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/pyfix_unittest_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/python/pyfix_unittest_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/pyfix_plugin_impl.py` & `pybuilder-0.9.9/pybuilder/plugins/python/pyfix_plugin_impl.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/django_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/python/django_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/python/core_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/python/core_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/__init__.py` & `pybuilder-0.9.9/pybuilder/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/analysis_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/analysis_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/filter_resources_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/filter_resources_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/copy_resources_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/copy_resources_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/source_distribution_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/source_distribution_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/plugins/core_plugin.py` & `pybuilder-0.9.9/pybuilder/plugins/core_plugin.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/cli.py` & `pybuilder-0.9.9/pybuilder/cli.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/core.py` & `pybuilder-0.9.9/pybuilder/core.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/utils.py` & `pybuilder-0.9.9/pybuilder/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import tempfile
 import time
 
 from pybuilder.errors import MissingPrerequisiteException, PythonbuilderException
 
 
 def render_report(report_dict):
-    return json.dumps(report_dict, indent=2)
+    return json.dumps(report_dict, indent=2, sort_keys=True)
 
 
 def format_timestamp(timestamp):
     return timestamp.strftime("%Y-%m-%d %H:%M:%S")
 
 
 def timedelta_in_millis(timedelta):
```

### Comparing `pybuilder-0.9.8/pybuilder/reactor.py` & `pybuilder-0.9.9/pybuilder/reactor.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/execution.py` & `pybuilder-0.9.9/pybuilder/execution.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,14 +82,27 @@
 class Task(object):
     def __init__(self, name, callable, dependencies=None, description=""):
         self.name = name
         self.executables = [Executable(name, callable, description)]
         self.dependencies = as_task_name_list(dependencies)
         self.description = [description]
 
+    def __eq__(self, other):
+        if isinstance(other, Task):
+            return self.name == other.name
+        return False
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
+    def __lt__(self, other):
+        if isinstance(other, Task):
+            return self.name < other.name
+        return self.name < other
+
     def extend(self, task):
         self.executables += task.executables
         self.dependencies += task.dependencies
         self.description += task.description
 
     def execute(self, logger, argument_dict):
         for executable in self.executables:
```

### Comparing `pybuilder-0.9.8/pybuilder/pluginloader.py` & `pybuilder-0.9.9/pybuilder/pluginloader.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/terminal.py` & `pybuilder-0.9.9/pybuilder/terminal.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder/errors.py` & `pybuilder-0.9.9/pybuilder/errors.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pythonbuilder/__init__.py` & `pybuilder-0.9.9/pythonbuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `pybuilder-0.9.8/pybuilder.egg-info/SOURCES.txt` & `pybuilder-0.9.9/pybuilder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 pybuilder.egg-info/top_level.txt
 pybuilder.egg-info/zip-safe
 pybuilder/plugins/__init__.py
 pybuilder/plugins/analysis_plugin.py
 pybuilder/plugins/copy_resources_plugin.py
 pybuilder/plugins/core_plugin.py
 pybuilder/plugins/filter_resources_plugin.py
+pybuilder/plugins/ronn_manpage_plugin.py
 pybuilder/plugins/source_distribution_plugin.py
 pybuilder/plugins/python/__init__.py
 pybuilder/plugins/python/core_plugin.py
 pybuilder/plugins/python/coverage_plugin.py
 pybuilder/plugins/python/distutils_plugin.py
 pybuilder/plugins/python/django_plugin.py
 pybuilder/plugins/python/flake8_plugin.py
```

