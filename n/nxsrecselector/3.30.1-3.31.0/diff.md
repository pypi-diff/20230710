# Comparing `tmp/nxsrecselector-3.30.1.tar.gz` & `tmp/nxsrecselector-3.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxsrecselector-3.30.1.tar", last modified: Tue Jul  4 05:22:52 2023, max compression
+gzip compressed data, was "nxsrecselector-3.31.0.tar", last modified: Mon Jul 10 14:41:45 2023, max compression
```

## Comparing `nxsrecselector-3.30.1.tar` & `nxsrecselector-3.31.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-07-04 05:22:52.185659 nxsrecselector-3.30.1/
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-10-10 09:18:56.000000 nxsrecselector-3.30.1/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)       93 2016-05-11 08:07:11.000000 nxsrecselector-3.30.1/MANIFEST.in
--rwxr-xr-x   0 jkotan   (15949) irc         (39)      941 2023-06-27 15:45:03.000000 nxsrecselector-3.30.1/NXSRecSelector
--rw-r--r--   0 jkotan   (15949) irc         (39)     7119 2023-07-04 05:22:52.185659 nxsrecselector-3.30.1/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     4313 2023-06-23 12:04:33.000000 nxsrecselector-3.30.1/README.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-07-04 05:22:52.181659 nxsrecselector-3.30.1/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)      938 2017-03-18 22:59:30.000000 nxsrecselector-3.30.1/man/NXSRecSelector.1
--rw-r--r--   0 jkotan   (15949) irc         (39)   109341 2023-03-10 08:35:11.000000 nxsrecselector-3.30.1/man/nxsrecconfig.1
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-07-04 05:22:52.181659 nxsrecselector-3.30.1/nxsrecconfig/
--rw-r--r--   0 jkotan   (15949) irc         (39)     6669 2023-06-07 08:45:59.000000 nxsrecselector-3.30.1/nxsrecconfig/CheckerThread.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10979 2020-01-31 13:48:24.000000 nxsrecselector-3.30.1/nxsrecconfig/Converter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    23789 2023-02-01 13:37:17.000000 nxsrecselector-3.30.1/nxsrecconfig/Describer.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    22847 2023-02-01 13:37:17.000000 nxsrecselector-3.30.1/nxsrecconfig/DynamicComponent.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    19957 2023-06-07 08:45:59.000000 nxsrecselector-3.30.1/nxsrecconfig/MacroServerPools.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    75699 2023-06-29 12:48:10.000000 nxsrecselector-3.30.1/nxsrecconfig/NXSConfig.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    59851 2023-07-04 05:22:18.000000 nxsrecselector-3.30.1/nxsrecconfig/ProfileManager.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      930 2023-07-04 05:22:18.000000 nxsrecselector-3.30.1/nxsrecconfig/Release.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     9075 2020-01-31 13:48:24.000000 nxsrecselector-3.30.1/nxsrecconfig/Selection.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    16157 2023-02-01 13:37:17.000000 nxsrecselector-3.30.1/nxsrecconfig/Selector.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    45630 2023-06-29 12:48:10.000000 nxsrecselector-3.30.1/nxsrecconfig/Settings.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5795 2023-03-09 16:17:52.000000 nxsrecselector-3.30.1/nxsrecconfig/StreamSet.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    29259 2023-05-26 09:16:32.000000 nxsrecselector-3.30.1/nxsrecconfig/Utils.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1683 2023-02-01 13:37:17.000000 nxsrecselector-3.30.1/nxsrecconfig/__init__.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-07-04 05:22:52.185659 nxsrecselector-3.30.1/nxsrecselector.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)     7119 2023-07-04 05:22:52.000000 nxsrecselector-3.30.1/nxsrecselector.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)      710 2023-07-04 05:22:52.000000 nxsrecselector-3.30.1/nxsrecselector.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-07-04 05:22:52.000000 nxsrecselector-3.30.1/nxsrecselector.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-12-01 13:43:40.000000 nxsrecselector-3.30.1/nxsrecselector.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)       17 2023-07-04 05:22:52.000000 nxsrecselector-3.30.1/nxsrecselector.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)       13 2023-07-04 05:22:52.000000 nxsrecselector-3.30.1/nxsrecselector.egg-info/top_level.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)      213 2023-07-04 05:22:52.185659 nxsrecselector-3.30.1/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     4035 2023-06-29 15:14:01.000000 nxsrecselector-3.30.1/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-07-10 14:41:45.502677 nxsrecselector-3.31.0/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-10-10 09:18:56.000000 nxsrecselector-3.31.0/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)       93 2016-05-11 08:07:11.000000 nxsrecselector-3.31.0/MANIFEST.in
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)      941 2023-06-27 15:45:03.000000 nxsrecselector-3.31.0/NXSRecSelector
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7119 2023-07-10 14:41:45.502677 nxsrecselector-3.31.0/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4313 2023-06-23 12:04:33.000000 nxsrecselector-3.31.0/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-07-10 14:41:45.498677 nxsrecselector-3.31.0/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      938 2017-03-18 22:59:30.000000 nxsrecselector-3.31.0/man/NXSRecSelector.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)   109341 2023-03-10 08:35:11.000000 nxsrecselector-3.31.0/man/nxsrecconfig.1
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-07-10 14:41:45.498677 nxsrecselector-3.31.0/nxsrecconfig/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6669 2023-06-07 08:45:59.000000 nxsrecselector-3.31.0/nxsrecconfig/CheckerThread.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10979 2020-01-31 13:48:24.000000 nxsrecselector-3.31.0/nxsrecconfig/Converter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    25288 2023-07-10 14:41:35.000000 nxsrecselector-3.31.0/nxsrecconfig/Describer.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    22847 2023-02-01 13:37:17.000000 nxsrecselector-3.31.0/nxsrecconfig/DynamicComponent.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    19957 2023-06-07 08:45:59.000000 nxsrecselector-3.31.0/nxsrecconfig/MacroServerPools.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    75699 2023-06-29 12:48:10.000000 nxsrecselector-3.31.0/nxsrecconfig/NXSConfig.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    59851 2023-07-04 05:22:18.000000 nxsrecselector-3.31.0/nxsrecconfig/ProfileManager.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      930 2023-07-10 14:41:35.000000 nxsrecselector-3.31.0/nxsrecconfig/Release.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9075 2020-01-31 13:48:24.000000 nxsrecselector-3.31.0/nxsrecconfig/Selection.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    16157 2023-02-01 13:37:17.000000 nxsrecselector-3.31.0/nxsrecconfig/Selector.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    45630 2023-07-07 12:05:27.000000 nxsrecselector-3.31.0/nxsrecconfig/Settings.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5795 2023-03-09 16:17:52.000000 nxsrecselector-3.31.0/nxsrecconfig/StreamSet.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    29259 2023-05-26 09:16:32.000000 nxsrecselector-3.31.0/nxsrecconfig/Utils.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1683 2023-02-01 13:37:17.000000 nxsrecselector-3.31.0/nxsrecconfig/__init__.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-07-10 14:41:45.502677 nxsrecselector-3.31.0/nxsrecselector.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7119 2023-07-10 14:41:45.000000 nxsrecselector-3.31.0/nxsrecselector.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)      710 2023-07-10 14:41:45.000000 nxsrecselector-3.31.0/nxsrecselector.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-07-10 14:41:45.000000 nxsrecselector-3.31.0/nxsrecselector.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-12-01 13:43:40.000000 nxsrecselector-3.31.0/nxsrecselector.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       17 2023-07-10 14:41:45.000000 nxsrecselector-3.31.0/nxsrecselector.egg-info/requires.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)       13 2023-07-10 14:41:45.000000 nxsrecselector-3.31.0/nxsrecselector.egg-info/top_level.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)      213 2023-07-10 14:41:45.502677 nxsrecselector-3.31.0/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4035 2023-06-29 15:14:01.000000 nxsrecselector-3.31.0/setup.py
```

### Comparing `nxsrecselector-3.30.1/COPYRIGHT` & `nxsrecselector-3.31.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/NXSRecSelector` & `nxsrecselector-3.31.0/NXSRecSelector`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/PKG-INFO` & `nxsrecselector-3.31.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxsrecselector
-Version: 3.30.1
+Version: 3.31.0
 Summary: Selector Server for NeXus Sardana recorder
 Home-page: https://github.com/jkotan/nexdatas/
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: ========================================
         Welcome to nxsrecconfig's documentation!
```

### Comparing `nxsrecselector-3.30.1/README.rst` & `nxsrecselector-3.31.0/README.rst`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/man/NXSRecSelector.1` & `nxsrecselector-3.31.0/man/NXSRecSelector.1`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/man/nxsrecconfig.1` & `nxsrecselector-3.31.0/man/nxsrecconfig.1`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/nxsrecconfig/CheckerThread.py` & `nxsrecselector-3.31.0/nxsrecconfig/CheckerThread.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/nxsrecconfig/Converter.py` & `nxsrecselector-3.31.0/nxsrecconfig/Converter.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/nxsrecconfig/Describer.py` & `nxsrecselector-3.31.0/nxsrecconfig/Describer.py`

 * *Files 20% similar despite different names*

```diff
@@ -38,40 +38,47 @@
     unicode = str
 
 
 class DSItem(object):
 
     """ Basic DataSource item
     """
-    __slots__ = 'name', 'dstype', 'record'
+    __slots__ = 'name', 'dstype', 'record', 'parentobj'
 
     #
-    def __init__(self, name=None, dstype=None, record=None, dsitem=None):
+    def __init__(self, name=None, dstype=None, record=None, dsitem=None,
+                 parentobj=None):
         """ constructor
 
         :param name: datasource name
         :type name: :obj:`str`
         :param dstype: datasource type
         :type dstype: :obj:`str`
         :param record: datasource record
         :type record: :obj:`str`
         :param dsitem: datasource item
         :type dsitem: :class:`DSItem`
+        :param parentobj: datasource parent object
+        :type parentobj: :obj:`str`
         """
         if dsitem:
             #: (:obj:`str`) datasource name
             self.name = dsitem.name
             #: (:obj:`str`) datasource type
             self.dstype = dsitem.dstype
             #: (:obj:`str`) datasource record
             self.record = dsitem.record
+            #: (:obj:`str`) datasource parentobj
+            self.parentobj = dsitem.parentobj
         else:
             self.name = Utils.tostr(name) if name is not None else None
             self.dstype = Utils.tostr(dstype) if dstype is not None else None
             self.record = Utils.tostr(record) if record is not None else None
+            self.parentobj = Utils.tostr(parentobj) \
+                if parentobj is not None else None
 
 
 class ExDSItem(DSItem):
 
     """ Extended DataSource item
     """
     __slots__ = 'mode', 'nxtype', 'shape'
@@ -259,14 +266,15 @@
                 for vds in dss[ds]:
                     if (not strategy or vds.mode == strategy) and \
                        (not dstype or vds.dstype == dstype):
                         elem = {}
                         elem["dsname"] = ds
                         elem["strategy"] = vds.mode
                         elem["dstype"] = vds.dstype
+                        elem["parentobj"] = vds.parentobj
                         elem["record"] = vds.record
                         elem["nxtype"] = vds.nxtype
                         elem["shape"] = vds.shape
                         elem["cpname"] = cp
                         result.append(elem)
         return result
 
@@ -291,15 +299,15 @@
             for ds in dss.keys():
                 for vds in dss[ds]:
                     if (not strategy or vds.mode == strategy) and \
                             (not dstype or vds.dstype == dstype):
                         if ds not in tr:
                             tr[ds] = []
                         tr[ds].append((vds.mode, vds.dstype, vds.record,
-                                       vds.nxtype, vds.shape))
+                                       vds.nxtype, vds.shape, vds.parentobj))
             result[cp] = tr
         return result
 
     def __getDSFromNode(self, parent, dsl=None):
         """ provides datasource item from XML node
 
         :param node: xml node
@@ -317,23 +325,32 @@
         dsxmls = None
 
         nodes = parent.findall("datasource")
         for node in nodes:
             dstype = node.get("type")
             name = node.get("name")
             record = Utils.getRecord(node)
-            dslist.append(DSItem(name, dstype, record))
+            parentobj = (parent.tag
+                         if hasattr(parent, "tag") else None)
+            dslist.append(
+                DSItem(name, dstype, record,
+                       parentobj=parentobj))
             if name and Utils.tostr(dstype) == 'PYEVAL':
                 if dsxmls and self.__pyevalfromscript:
-                    dslist.extend(self.__findsubdatasources(dsxmls[0]))
+                    if node not in parent:
+                        parentobj = "datasource"
+                    dslist.extend(
+                        self.__findsubdatasources(dsxmls[0]), parentobj)
                 else:
                     self.__getDSFromNode(node, dslist)
         if not name and not dslist:
             dstxt = Utils.getText(parent)
-            dsitem = DSItem()
+            dsitem = DSItem(
+                parentobj=(parent.tag
+                           if hasattr(parent, "tag") else None))
             index = dstxt.find("$%s." % label)
             while index != -1:
                 try:
                     if sys.version_info > (3,):
                         subc = re.finditer(
                             r"[\w]+",
                             dstxt[(index + len(label) + 2):]
@@ -347,35 +364,49 @@
                 name = subc.strip() if subc else ""
                 if Utils.tostr(name) in self.__availableDataSources:
                     dsxmls = TangoUtils.command(
                         self.__nexusconfig_device,
                         "dataSources", [Utils.tostr(name)])
                 else:
                     dsxmls = None
-                    dsitem = DSItem(name, "__ERROR__", "__ERROR__")
+                    dsitem = DSItem(
+                        name, "__ERROR__", "__ERROR__",
+                        parentobj=(parent.tag
+                                   if hasattr(parent, "tag") else None))
                 if dsxmls:
                     dsitem = self.__describeDataSource(name, dsxmls[0])
+                    dsitem.parentobj = (
+                        parent.tag
+                        if hasattr(parent, "tag") else None)
                     if dsitem.dstype:
                         dstype = dsitem.dstype
                         break
                 else:
-                    dsitem = DSItem(name, None, None)
+                    dsitem = DSItem(
+                        name, None, None,
+                        parentobj=(parent.tag
+                                   if hasattr(parent, "tag") else None)
+                    )
                 index = dstxt.find("$%s." % label, index + 1)
             dslist.append(dsitem)
             if name and Utils.tostr(dstype) == 'PYEVAL':
                 if dsxmls and self.__pyevalfromscript:
-                    dslist.extend(self.__findsubdatasources(dsxmls[0]))
+                    dslist.extend(
+                        self.__findsubdatasources(
+                            dsxmls[0], "datasource"))
 
         return dslist
 
-    def __findsubdatasources(self, dsxml):
+    def __findsubdatasources(self, dsxml, parentobj="datasource"):
         """ finds datasources in pyeval scripts
 
         :param dsxml: pyeval xml
         :type dsxml: :obj:`str`
+        :param parentobj: parentobj
+        :type parentobj: :obj:`str`
         :returns: list with datasource items (DSItem)
         :rtype: :obj:`list` <:class:`DSItem`>
         """
         dslist = []
         result = ""
         label = 'datasources'
         if sys.version_info > (3,):
@@ -406,18 +437,20 @@
             name = subc.strip() if subc else ""
             if name in result:
                 chdsxml = TangoUtils.command(
                     self.__nexusconfig_device,
                     "dataSources", [Utils.tostr(name)])
                 if chdsxml:
                     dsitem = self.__describeDataSource(name, chdsxml[0])
+                    dsitem.parentobj = parentobj
                     if dsitem.dstype:
                         dslist.append(dsitem)
                 else:
-                    dslist.append(DSItem(name, None, None))
+                    dslist.append(
+                        DSItem(name, None, None, parentobj=parentobj))
             index = dsxml.find("$%s." % label, index + 1)
         return dslist
 
     @classmethod
     def __getShape(cls, node):
         """ provides shape from node
 
@@ -527,15 +560,14 @@
                         nxtype = None
                         dset = parent
                         nxtype = dset.get("type")
                         shape = None
                         dimensions = parent.findall("dimensions")
                         if dimensions:
                             shape = self.__getShape(dimensions[0])
-
                         name = dss.appendDSList(self.__getDSFromNode(parent),
                                                 mode, nxtype, shape)
                         if name:
                             break
         return dss
 
     def dataSources(self, names=None, dstype=''):
```

### Comparing `nxsrecselector-3.30.1/nxsrecconfig/DynamicComponent.py` & `nxsrecselector-3.31.0/nxsrecconfig/DynamicComponent.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/nxsrecconfig/MacroServerPools.py` & `nxsrecselector-3.31.0/nxsrecconfig/MacroServerPools.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/nxsrecconfig/NXSConfig.py` & `nxsrecselector-3.31.0/nxsrecconfig/NXSConfig.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/nxsrecconfig/ProfileManager.py` & `nxsrecselector-3.31.0/nxsrecconfig/ProfileManager.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/nxsrecconfig/Release.py` & `nxsrecselector-3.31.0/nxsrecconfig/Release.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """  NeXus Sardana Recorder Settings - Release """
 
 #: (:obj:`str`) package version
-__version__ = "3.30.1"
+__version__ = "3.31.0"
```

### Comparing `nxsrecselector-3.30.1/nxsrecconfig/Selection.py` & `nxsrecselector-3.31.0/nxsrecconfig/Selection.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/nxsrecconfig/Selector.py` & `nxsrecselector-3.31.0/nxsrecconfig/Selector.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/nxsrecconfig/Settings.py` & `nxsrecselector-3.31.0/nxsrecconfig/Settings.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/nxsrecconfig/StreamSet.py` & `nxsrecselector-3.31.0/nxsrecconfig/StreamSet.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/nxsrecconfig/Utils.py` & `nxsrecselector-3.31.0/nxsrecconfig/Utils.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/nxsrecconfig/__init__.py` & `nxsrecselector-3.31.0/nxsrecconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/nxsrecselector.egg-info/PKG-INFO` & `nxsrecselector-3.31.0/nxsrecselector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxsrecselector
-Version: 3.30.1
+Version: 3.31.0
 Summary: Selector Server for NeXus Sardana recorder
 Home-page: https://github.com/jkotan/nexdatas/
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: ========================================
         Welcome to nxsrecconfig's documentation!
```

### Comparing `nxsrecselector-3.30.1/nxsrecselector.egg-info/SOURCES.txt` & `nxsrecselector-3.31.0/nxsrecselector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.1/setup.py` & `nxsrecselector-3.31.0/setup.py`

 * *Files identical despite different names*

