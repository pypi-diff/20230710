# Comparing `tmp/plyfile-0.9.tar.gz` & `tmp/plyfile-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plyfile-0.9.tar", last modified: Thu Apr 13 06:51:39 2023, max compression
+gzip compressed data, was "plyfile-1.0.tar", last modified: Mon Jul 10 06:45:14 2023, max compression
```

## Comparing `plyfile-0.9.tar` & `plyfile-1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35147 2019-08-03 21:55:54.506719 plyfile-0.9/COPYING
--rw-r--r--   0        0        0    20787 2023-04-13 05:53:27.177994 plyfile-0.9/README.md
--rw-r--r--   0        0        0    42475 2023-04-13 06:18:18.158979 plyfile-0.9/plyfile.py
--rw-r--r--   0        0        0      934 2023-04-13 06:47:02.102832 plyfile-0.9/pyproject.toml
--rw-r--r--   0        0        0    21538 1970-01-01 00:00:00.000000 plyfile-0.9/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-07-02 02:49:51.243322 plyfile-1.0/COPYING
+-rw-r--r--   0        0        0     1144 2023-07-02 02:49:51.243322 plyfile-1.0/README.md
+-rw-r--r--   0        0        0    42554 2023-07-02 02:49:51.243322 plyfile-1.0/plyfile.py
+-rw-r--r--   0        0        0     1538 2023-07-10 06:41:40.695934 plyfile-1.0/pyproject.toml
+-rw-r--r--   0        0        0     2029 1970-01-01 00:00:00.000000 plyfile-1.0/PKG-INFO
```

### Comparing `plyfile-0.9/COPYING` & `plyfile-1.0/COPYING`

 * *Files identical despite different names*

### Comparing `plyfile-0.9/plyfile.py` & `plyfile-1.0/plyfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright 2014-2020 Darsh Ranjan
+#   Copyright 2014-2023 Darsh Ranjan and plyfile authors.
 #
 #   This file is part of python-plyfile.
 #
 #   python-plyfile is free software: you can redistribute it and/or
 #   modify it under the terms of the GNU General Public License as
 #   published by the Free Software Foundation, either version 3 of the
 #   License, or (at your option) any later version.
@@ -11,365 +11,25 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #   General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with python-plyfile.  If not, see
 #       <http://www.gnu.org/licenses/>.
+"""
+NumPy-based PLY format input and output for Python.
+"""
 
 import io as _io
 from itertools import islice as _islice
 
 import numpy as _np
 from sys import byteorder as _byteorder
 
 
-# Many-many relation
-_data_type_relation = [
-    ('int8', 'i1'),
-    ('char', 'i1'),
-    ('uint8', 'u1'),
-    ('uchar', 'b1'),
-    ('uchar', 'u1'),
-    ('int16', 'i2'),
-    ('short', 'i2'),
-    ('uint16', 'u2'),
-    ('ushort', 'u2'),
-    ('int32', 'i4'),
-    ('int', 'i4'),
-    ('uint32', 'u4'),
-    ('uint', 'u4'),
-    ('float32', 'f4'),
-    ('float', 'f4'),
-    ('float64', 'f8'),
-    ('double', 'f8')
-]
-
-_data_types = dict(_data_type_relation)
-_data_type_reverse = dict((b, a) for (a, b) in _data_type_relation)
-
-_types_list = []
-_types_set = set()
-for (_a, _b) in _data_type_relation:
-    if _a not in _types_set:
-        _types_list.append(_a)
-        _types_set.add(_a)
-    if _b not in _types_set:
-        _types_list.append(_b)
-        _types_set.add(_b)
-
-
-_byte_order_map = {
-    'ascii': '=',
-    'binary_little_endian': '<',
-    'binary_big_endian': '>'
-}
-
-_byte_order_reverse = {
-    '<': 'binary_little_endian',
-    '>': 'binary_big_endian'
-}
-
-_native_byte_order = {'little': '<', 'big': '>'}[_byteorder]
-
-
-def _lookup_type(type_str):
-    if type_str not in _data_type_reverse:
-        try:
-            type_str = _data_types[type_str]
-        except KeyError:
-            raise ValueError("field type %r not in %r" %
-                             (type_str, _types_list))
-
-    return _data_type_reverse[type_str]
-
-
-class _PlyHeaderLines(object):
-    """
-    Generator over lines in the PLY header.
-
-    LF, CR, and CRLF line endings are supported.
-    """
-
-    def __init__(self, stream):
-        """
-        Parameters
-        ----------
-        stream : text or binary stream.
-
-        Raises
-        ------
-        PlyHeaderParseError
-        """
-        s = self._decode(stream.read(4))
-        self.chars = []
-        if s[:3] != 'ply':
-            raise PlyHeaderParseError("expected 'ply'", 1)
-        self.nl = s[3:]
-        if s[3:] =='\r':
-            c = self._decode(stream.read(1))
-            if c == '\n':
-                self.nl += c
-            else:
-                self.chars.append(c)
-        elif s[3:] != '\n':
-            raise PlyHeaderParseError(
-                "unexpected characters after 'ply'", 1)
-        self.stream = stream
-        self.len_nl = len(self.nl)
-        self.done = False
-        self.lines = 1
-
-    @staticmethod
-    def _decode(s):
-        """
-        Convert input `str` or `bytes` instance to `str`, decoding
-        as ASCII if necessary.
-        """
-        if isinstance(s, str):
-            return s
-        return s.decode('ascii')
-
-    def __iter__(self):
-        """
-        Yields
-        ------
-        line : str
-            Decoded line with newline removed.
-        """
-        while not self.done:
-            self.lines += 1
-            while ''.join(self.chars[-self.len_nl:]) != self.nl:
-                char = self._decode(self.stream.read(1))
-                if not char:
-                    raise PlyHeaderParseError("early end-of-file",
-                                              self.lines)
-                self.chars.append(char)
-            line = ''.join(self.chars[:-self.len_nl])
-            self.chars = []
-            if line == 'end_header':
-                self.done = True
-            yield line
-
-
-class _PlyHeaderParser(object):
-    """
-    Parser for PLY format header.
-
-    Attributes
-    ----------
-    format : str
-        "ascii", "binary_little_endian", or "binary_big_endian"
-    elements : list of (name, comments, count, properties)
-    comments : list of str
-    obj_info : list of str
-    lines : int
-    """
-
-    def __init__(self, lines):
-        """
-        Parameters
-        ----------
-        lines : iterable of str
-            Header lines, starting *after* the "ply" line.
-
-        Raises
-        ------
-        PlyHeaderParseError
-        """
-        self.format = None
-        self.elements = []
-        self.comments = []
-        self.obj_info = []
-        self.lines = 1
-        self._allowed = ['format', 'comment', 'obj_info']
-        for line in lines:
-            self.consume(line)
-        if self._allowed:
-            self._error("early end-of-file")
-
-    def consume(self, raw_line):
-        """
-        Parse and internalize one line of input.
-        """
-        self.lines += 1
-        if not raw_line:
-            self._error("early end-of-file")
-
-        line = raw_line.strip()
-        try:
-            keyword = line.split(None, 1)[0]
-        except IndexError:
-            self._error()
-
-        if keyword not in self._allowed:
-            self._error("expected one of {%s}" %
-                        ", ".join(self._allowed))
-
-        # This dynamic method lookup pattern is somewhat questionable,
-        # but it's probably not worth replacing it with something more
-        # principled but also more complex.
-        getattr(self, 'parse_' + keyword)(line[len(keyword)+1:])
-        return self._allowed
-
-    def _error(self, message="parse error"):
-        raise PlyHeaderParseError(message, self.lines)
-
-    # The parse_* methods below are used to parse all the different
-    # types of PLY header lines. (See `consume` above for the call site,
-    # which uses dynamic lookup.) Each method accepts a single argument,
-    # which is the remainder of the header line after the first word,
-    # and the method does two things:
-    # - internalize the semantic content of the string into the
-    #   instance's attributes, and
-    # - set self._allowed to a list of the line types that can come
-    #   next.
-
-    def parse_format(self, data):
-        fields = data.strip().split()
-        if len(fields) != 2:
-            self._error("expected \"format {format} 1.0\"")
-
-        self.format = fields[0]
-        if self.format not in _byte_order_map:
-            self._error("don't understand format %r" % self.format)
-
-        if fields[1] != '1.0':
-            self._error("expected version '1.0'")
-
-        self._allowed = ['element', 'comment', 'obj_info', 'end_header']
-
-    def parse_comment(self, data):
-        if not self.elements:
-            self.comments.append(data)
-        else:
-            self.elements[-1][3].append(data)
-
-    def parse_obj_info(self, data):
-        self.obj_info.append(data)
-
-    def parse_element(self, data):
-        fields = data.strip().split()
-        if len(fields) != 2:
-            self._error("expected \"element {name} {count}\"")
-
-        name = fields[0]
-        try:
-            count = int(fields[1])
-        except ValueError:
-            self._error("expected integer count")
-
-        self.elements.append((name, [], count, []))
-        self._allowed = ['element', 'comment', 'property', 'end_header']
-
-    def parse_property(self, data):
-        properties = self.elements[-1][1]
-        fields = data.strip().split()
-        if len(fields) < 2:
-            self._error("bad 'property' line")
-
-        if fields[0] == 'list':
-            if len(fields) != 4:
-                self._error("expected \"property list "
-                            "{len_type} {val_type} {name}\"")
-
-            try:
-                properties.append(
-                    PlyListProperty(fields[3], fields[1], fields[2])
-                )
-            except ValueError as e:
-                self._error(str(e))
-
-        else:
-            if len(fields) != 2:
-                self._error("expected \"property {type} {name}\"")
-
-            try:
-                properties.append(
-                    PlyProperty(fields[1], fields[0])
-                )
-            except ValueError as e:
-                self._error(str(e))
-
-    def parse_end_header(self, data):
-        if data:
-            self._error("unexpected data after 'end_header'")
-        self._allowed = []
-
-
-class PlyParseError(Exception):
-    """
-    Base class for PLY parsing errors.
-    """
-
-    pass
-
-
-class PlyElementParseError(PlyParseError):
-    """
-    Raised when a PLY element cannot be parsed.
-
-    Attributes
-    ----------
-    message : str
-    element : PlyElement
-    row : int
-    prop : PlyProperty
-    """
-
-    def __init__(self, message, element=None, row=None, prop=None):
-        self.message = message
-        self.element = element
-        self.row = row
-        self.prop = prop
-
-        s = ''
-        if self.element:
-            s += 'element %r: ' % self.element.name
-        if self.row is not None:
-            s += 'row %d: ' % self.row
-        if self.prop:
-            s += 'property %r: ' % self.prop.name
-        s += self.message
-
-        Exception.__init__(self, s)
-
-    def __repr__(self):
-        return ('%s(%r, element=%r, row=%r, prop=%r)' %
-                (self.__class__.__name__,
-                 self.message, self.element, self.row, self.prop))
-
-
-class PlyHeaderParseError(PlyParseError):
-    """
-    Raised when a PLY header cannot be parsed.
-
-    Attributes
-    ----------
-    line : str
-        Which header line the error occurred on.
-    """
-
-    def __init__(self, message, line=None):
-        self.message = message
-        self.line = line
-
-        s = ''
-        if self.line:
-            s += 'line %r: ' % self.line
-        s += self.message
-
-        Exception.__init__(self, s)
-
-    def __repr__(self):
-        return ('%s(%r, line=%r)' %
-                (self.__class__.__name__,
-                 self.message, self.line))
-
-
 class PlyData(object):
     """
     PLY file header and data.
 
     A `PlyData` instance is created in one of two ways: by the static
     method `PlyData.read` (to read a PLY file), or directly from
     `__init__` given a sequence of elements (which can then be written
@@ -623,46 +283,14 @@
     def __repr__(self):
         return ('PlyData(%r, text=%r, byte_order=%r, '
                 'comments=%r, obj_info=%r)' %
                 (self.elements, self.text, self.byte_order,
                  self.comments, self.obj_info))
 
 
-def _open_stream(stream, read_or_write):
-    """
-    Normalizing function: given a filename or open stream,
-    return an open stream.
-
-    Parameters
-    ----------
-    stream : str or open file-like object
-    read_or_write : str
-        `"read"` or `"write"`, the method to be used on the stream.
-
-    Returns
-    -------
-    must_close : bool
-        Whether `.close` needs to be called on the file object
-        by the caller (i.e., it wasn't already open).
-    file : file-like object
-
-    Raises
-    ------
-    TypeError
-        If `stream` is neither a string nor has the
-        `read_or_write`-indicated method.
-    """
-    if hasattr(stream, read_or_write):
-        return (False, stream)
-    try:
-        return (True, open(stream, read_or_write[0] + 'b'))
-    except TypeError:
-        raise TypeError("expected open file or filename")
-
-
 class PlyElement(object):
     """
     PLY file element.
 
     Creating a `PlyElement` instance is generally done in one of two
     ways: as a byproduct of `PlyData.read` (when reading a PLY file) and
     by `PlyElement.describe` (before writing a PLY file).
@@ -769,18 +397,18 @@
 
     @property
     def name(self):
         return self._name
 
     def dtype(self, byte_order='='):
         """
-        Return the `numpy` `dtype` of the in-memory representation of the
-        data.  (If there are no list properties, and the PLY format is
-        binary, then this also accurately describes the on-disk
-        representation of the element.)
+        Return the `numpy.dtype` description of the in-memory
+        representation of the data.  (If there are no list properties,
+        and the PLY format is binary, then this also accurately
+        describes the on-disk representation of the element.)
 
         Parameters
         ----------
         byte_order : {'<', '>', '='}
 
         Returns
         -------
@@ -802,20 +430,21 @@
         len_types : dict, optional
             Mapping from list property names to type strings
             (`numpy`-style like `'u1'`, `'f4'`, etc., or PLY-style like
             `'int8'`, `'float32'`, etc.), which will be used to encode
             the length of the list in binary-format PLY files.  Defaults
             to `'u1'` (8-bit integer) for all list properties.
         val_types : dict, optional
-            Mapping from list property names to type strings as for `len_types`,
-            but is used to encode the list elements in binary-format PLY files.
-            Defaults to `'i4'` (32-bit integer) for all list properties.
+            Mapping from list property names to type strings as for
+            `len_types`, but is used to encode the list elements in
+            binary-format PLY files.  Defaults to `'i4'` (32-bit
+            integer) for all list properties.
         comments : list of str
-            Comments between the "element" line and first property definition
-            in the header.
+            Comments between the "element" line and first property
+            definition in the header.
 
         Returns
         -------
         PlyElement
 
         Raises
         ------
@@ -931,28 +560,23 @@
         known_list_len : dict
         """
         list_len_props = {}
         # update the dtype to include the list length and list dtype
         new_dtype = []
         for p in self.properties:
             if isinstance(p, PlyListProperty):
+                len_dtype, val_dtype = p.list_dtype(byte_order)
                 # create new dtype for the list length
-                new_dtype.append(
-                    (p.name + "\nlen", byte_order + p.len_dtype)
-                )
+                new_dtype.append((p.name + "\nlen", len_dtype))
                 # a new dtype with size for the list values themselves
-                new_dtype.append(
-                    (p.name, byte_order + p.val_dtype,
-                     (known_list_len[p.name],))
-                )
+                new_dtype.append((p.name, val_dtype,
+                                  (known_list_len[p.name],)))
                 list_len_props[p.name] = p.name + "\nlen"
             else:
-                new_dtype.append(
-                    (p.name, p.dtype(byte_order))
-                )
+                new_dtype.append((p.name, p.dtype(byte_order)))
         dtype = _np.dtype(new_dtype)
         num_bytes = self.count * dtype.itemsize
         offset = stream.tell()
         stream.seek(0, 2)
         max_bytes = stream.tell() - offset
         if max_bytes < num_bytes:
             raise PlyElementParseError("early end-of-file", self,
@@ -1101,47 +725,26 @@
 
     def __repr__(self):
         return ('PlyElement(%r, %r, count=%d, comments=%r)' %
                 (self.name, self.properties, self.count,
                  self.comments))
 
 
-def _check_comments(comments):
-    """
-    Check that the given comments can be safely used in a PLY header.
-
-    Parameters
-    ----------
-    comments : list of str
-
-    Raises
-    ------
-    ValueError
-        If the check fails.
-    """
-    for comment in comments:
-        for char in comment:
-            if not 0 <= ord(char) < 128:
-                raise ValueError("non-ASCII character in comment")
-            if char == '\n':
-                raise ValueError("embedded newline in comment")
-
-
 class PlyProperty(object):
     """
     PLY property description.
 
     This class is pure metadata. The data itself is contained in
     `PlyElement` instances.
 
     Attributes
     ----------
     name : str
     val_dtype : str
-        `numpy` `dtype` string for the property's data.
+        `numpy.dtype` description for the property's data.
     """
 
     def __init__(self, name, val_dtype):
         """
         Parameters
         ----------
         name : str
@@ -1161,15 +764,15 @@
 
     @property
     def name(self):
         return self._name
 
     def dtype(self, byte_order='='):
         """
-        Return the `numpy` `dtype` description for this property.
+        Return the `numpy.dtype` description for this property.
 
         Parameters
         ----------
         byte_order : {'<', '>', '='}, default='='
 
         Returns
         -------
@@ -1257,15 +860,15 @@
     PLY list property description.
 
     Attributes
     ----------
     name
     val_dtype
     len_dtype : str
-        `numpy` `dtype` for the property's length field.
+        `numpy.dtype` description for the property's length field.
     """
 
     def __init__(self, name, len_dtype, val_dtype):
         """
         Parameters
         ----------
         name : str
@@ -1282,25 +885,26 @@
     def _set_len_dtype(self, len_dtype):
         self._len_dtype = _data_types[_lookup_type(len_dtype)]
 
     len_dtype = property(_get_len_dtype, _set_len_dtype)
 
     def dtype(self, byte_order='='):
         """
-        `dtype` name for the property's field in the element.
+        `numpy.dtype` name for the property's field in the element.
 
         List properties always have a numpy dtype of "object".
 
         Parameters
         ----------
         byte_order : {'<', '>', '='}
 
         Returns
         -------
-        '|O'
+        dtype : str
+            Always `'|O'`.
         """
         return '|O'
 
     def list_dtype(self, byte_order='='):
         """
         Return the pair `(len_dtype, val_dtype)` (both numpy-friendly
         strings).
@@ -1424,14 +1028,329 @@
     def __repr__(self):
         return ('PlyListProperty(%r, %r, %r)' %
                 (self.name,
                  _lookup_type(self.len_dtype),
                  _lookup_type(self.val_dtype)))
 
 
+class PlyParseError(Exception):
+    """
+    Base class for PLY parsing errors.
+    """
+
+    pass
+
+
+class PlyElementParseError(PlyParseError):
+    """
+    Raised when a PLY element cannot be parsed.
+
+    Attributes
+    ----------
+    message : str
+    element : PlyElement
+    row : int
+    prop : PlyProperty
+    """
+
+    def __init__(self, message, element=None, row=None, prop=None):
+        self.message = message
+        self.element = element
+        self.row = row
+        self.prop = prop
+
+        s = ''
+        if self.element:
+            s += 'element %r: ' % self.element.name
+        if self.row is not None:
+            s += 'row %d: ' % self.row
+        if self.prop:
+            s += 'property %r: ' % self.prop.name
+        s += self.message
+
+        Exception.__init__(self, s)
+
+    def __repr__(self):
+        return ('%s(%r, element=%r, row=%r, prop=%r)' %
+                (self.__class__.__name__,
+                 self.message, self.element, self.row, self.prop))
+
+
+class PlyHeaderParseError(PlyParseError):
+    """
+    Raised when a PLY header cannot be parsed.
+
+    Attributes
+    ----------
+    line : str
+        Which header line the error occurred on.
+    """
+
+    def __init__(self, message, line=None):
+        self.message = message
+        self.line = line
+
+        s = ''
+        if self.line:
+            s += 'line %r: ' % self.line
+        s += self.message
+
+        Exception.__init__(self, s)
+
+    def __repr__(self):
+        return ('%s(%r, line=%r)' %
+                (self.__class__.__name__,
+                 self.message, self.line))
+
+
+class _PlyHeaderParser(object):
+    """
+    Parser for PLY format header.
+
+    Attributes
+    ----------
+    format : str
+        "ascii", "binary_little_endian", or "binary_big_endian"
+    elements : list of (name, comments, count, properties)
+    comments : list of str
+    obj_info : list of str
+    lines : int
+    """
+
+    def __init__(self, lines):
+        """
+        Parameters
+        ----------
+        lines : iterable of str
+            Header lines, starting *after* the "ply" line.
+
+        Raises
+        ------
+        PlyHeaderParseError
+        """
+        self.format = None
+        self.elements = []
+        self.comments = []
+        self.obj_info = []
+        self.lines = 1
+        self._allowed = ['format', 'comment', 'obj_info']
+        for line in lines:
+            self.consume(line)
+        if self._allowed:
+            self._error("early end-of-file")
+
+    def consume(self, raw_line):
+        """
+        Parse and internalize one line of input.
+        """
+        self.lines += 1
+        if not raw_line:
+            self._error("early end-of-file")
+
+        line = raw_line.strip()
+        try:
+            keyword = line.split(None, 1)[0]
+        except IndexError:
+            self._error()
+
+        if keyword not in self._allowed:
+            self._error("expected one of {%s}" %
+                        ", ".join(self._allowed))
+
+        # This dynamic method lookup pattern is somewhat questionable,
+        # but it's probably not worth replacing it with something more
+        # principled but also more complex.
+        getattr(self, 'parse_' + keyword)(line[len(keyword)+1:])
+        return self._allowed
+
+    def _error(self, message="parse error"):
+        raise PlyHeaderParseError(message, self.lines)
+
+    # The parse_* methods below are used to parse all the different
+    # types of PLY header lines. (See `consume` above for the call site,
+    # which uses dynamic lookup.) Each method accepts a single argument,
+    # which is the remainder of the header line after the first word,
+    # and the method does two things:
+    # - internalize the semantic content of the string into the
+    #   instance's attributes, and
+    # - set self._allowed to a list of the line types that can come
+    #   next.
+
+    def parse_format(self, data):
+        fields = data.strip().split()
+        if len(fields) != 2:
+            self._error("expected \"format {format} 1.0\"")
+
+        self.format = fields[0]
+        if self.format not in _byte_order_map:
+            self._error("don't understand format %r" % self.format)
+
+        if fields[1] != '1.0':
+            self._error("expected version '1.0'")
+
+        self._allowed = ['element', 'comment', 'obj_info', 'end_header']
+
+    def parse_comment(self, data):
+        if not self.elements:
+            self.comments.append(data)
+        else:
+            self.elements[-1][3].append(data)
+
+    def parse_obj_info(self, data):
+        self.obj_info.append(data)
+
+    def parse_element(self, data):
+        fields = data.strip().split()
+        if len(fields) != 2:
+            self._error("expected \"element {name} {count}\"")
+
+        name = fields[0]
+        try:
+            count = int(fields[1])
+        except ValueError:
+            self._error("expected integer count")
+
+        self.elements.append((name, [], count, []))
+        self._allowed = ['element', 'comment', 'property', 'end_header']
+
+    def parse_property(self, data):
+        properties = self.elements[-1][1]
+        fields = data.strip().split()
+        if len(fields) < 2:
+            self._error("bad 'property' line")
+
+        if fields[0] == 'list':
+            if len(fields) != 4:
+                self._error("expected \"property list "
+                            "{len_type} {val_type} {name}\"")
+
+            try:
+                properties.append(
+                    PlyListProperty(fields[3], fields[1], fields[2])
+                )
+            except ValueError as e:
+                self._error(str(e))
+
+        else:
+            if len(fields) != 2:
+                self._error("expected \"property {type} {name}\"")
+
+            try:
+                properties.append(
+                    PlyProperty(fields[1], fields[0])
+                )
+            except ValueError as e:
+                self._error(str(e))
+
+    def parse_end_header(self, data):
+        if data:
+            self._error("unexpected data after 'end_header'")
+        self._allowed = []
+
+
+class _PlyHeaderLines(object):
+    """
+    Generator over lines in the PLY header.
+
+    LF, CR, and CRLF line endings are supported.
+    """
+
+    def __init__(self, stream):
+        """
+        Parameters
+        ----------
+        stream : text or binary stream.
+
+        Raises
+        ------
+        PlyHeaderParseError
+        """
+        s = self._decode(stream.read(4))
+        self.chars = []
+        if s[:3] != 'ply':
+            raise PlyHeaderParseError("expected 'ply'", 1)
+        self.nl = s[3:]
+        if s[3:] == '\r':
+            c = self._decode(stream.read(1))
+            if c == '\n':
+                self.nl += c
+            else:
+                self.chars.append(c)
+        elif s[3:] != '\n':
+            raise PlyHeaderParseError(
+                "unexpected characters after 'ply'", 1)
+        self.stream = stream
+        self.len_nl = len(self.nl)
+        self.done = False
+        self.lines = 1
+
+    @staticmethod
+    def _decode(s):
+        """
+        Convert input `str` or `bytes` instance to `str`, decoding
+        as ASCII if necessary.
+        """
+        if isinstance(s, str):
+            return s
+        return s.decode('ascii')
+
+    def __iter__(self):
+        """
+        Yields
+        ------
+        line : str
+            Decoded line with newline removed.
+        """
+        while not self.done:
+            self.lines += 1
+            while ''.join(self.chars[-self.len_nl:]) != self.nl:
+                char = self._decode(self.stream.read(1))
+                if not char:
+                    raise PlyHeaderParseError("early end-of-file",
+                                              self.lines)
+                self.chars.append(char)
+            line = ''.join(self.chars[:-self.len_nl])
+            self.chars = []
+            if line == 'end_header':
+                self.done = True
+            yield line
+
+
+def _open_stream(stream, read_or_write):
+    """
+    Normalizing function: given a filename or open stream,
+    return an open stream.
+
+    Parameters
+    ----------
+    stream : str or open file-like object
+    read_or_write : str
+        `"read"` or `"write"`, the method to be used on the stream.
+
+    Returns
+    -------
+    must_close : bool
+        Whether `.close` needs to be called on the file object
+        by the caller (i.e., it wasn't already open).
+    file : file-like object
+
+    Raises
+    ------
+    TypeError
+        If `stream` is neither a string nor has the
+        `read_or_write`-indicated method.
+    """
+    if hasattr(stream, read_or_write):
+        return (False, stream)
+    try:
+        return (True, open(stream, read_or_write[0] + 'b'))
+    except TypeError:
+        raise TypeError("expected open file or filename")
+
+
 def _check_name(name):
     """
     Check that a string can be safely be used as the name of an element
     or property in a PLY file.
 
     Parameters
     ----------
@@ -1445,14 +1364,35 @@
     for char in name:
         if not 0 <= ord(char) < 128:
             raise ValueError("non-ASCII character in name %r" % name)
         if char.isspace():
             raise ValueError("space character(s) in name %r" % name)
 
 
+def _check_comments(comments):
+    """
+    Check that the given comments can be safely used in a PLY header.
+
+    Parameters
+    ----------
+    comments : list of str
+
+    Raises
+    ------
+    ValueError
+        If the check fails.
+    """
+    for comment in comments:
+        for char in comment:
+            if not 0 <= ord(char) < 128:
+                raise ValueError("non-ASCII character in comment")
+            if char == '\n':
+                raise ValueError("embedded newline in comment")
+
+
 def _read_array(stream, dtype, n):
     """
     Read `n` elements of type `dtype` from an open stream.
 
     Parameters
     ----------
     stream : readable open binary file
@@ -1502,12 +1442,72 @@
     """
     try:
         pos = stream.tell()
         try:
             _np.memmap(stream, 'u1', 'c')
             stream.seek(pos)
             return True
-        except Exception as e:
+        except Exception:
             stream.seek(pos)
             return False
-    except Exception as e:
+    except Exception:
         return False
+
+
+def _lookup_type(type_str):
+    if type_str not in _data_type_reverse:
+        try:
+            type_str = _data_types[type_str]
+        except KeyError:
+            raise ValueError("field type %r not in %r" %
+                             (type_str, _types_list))
+
+    return _data_type_reverse[type_str]
+
+
+# Many-many relation
+_data_type_relation = [
+    ('int8', 'i1'),
+    ('char', 'i1'),
+    ('uint8', 'u1'),
+    ('uchar', 'b1'),
+    ('uchar', 'u1'),
+    ('int16', 'i2'),
+    ('short', 'i2'),
+    ('uint16', 'u2'),
+    ('ushort', 'u2'),
+    ('int32', 'i4'),
+    ('int', 'i4'),
+    ('uint32', 'u4'),
+    ('uint', 'u4'),
+    ('float32', 'f4'),
+    ('float', 'f4'),
+    ('float64', 'f8'),
+    ('double', 'f8')
+]
+
+_data_types = dict(_data_type_relation)
+_data_type_reverse = dict((b, a) for (a, b) in _data_type_relation)
+
+_types_list = []
+_types_set = set()
+for (_a, _b) in _data_type_relation:
+    if _a not in _types_set:
+        _types_list.append(_a)
+        _types_set.add(_a)
+    if _b not in _types_set:
+        _types_list.append(_b)
+        _types_set.add(_b)
+
+
+_byte_order_map = {
+    'ascii': '=',
+    'binary_little_endian': '<',
+    'binary_big_endian': '>'
+}
+
+_byte_order_reverse = {
+    '<': 'binary_little_endian',
+    '>': 'binary_big_endian'
+}
+
+_native_byte_order = {'little': '<', 'big': '>'}[_byteorder]
```

### Comparing `plyfile-0.9/pyproject.toml` & `plyfile-1.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,64 @@
-[tool.pdm]
+[tool.pdm.dev-dependencies]
+test = [
+    "tox>=4.4.8",
+    "pytest>=7.2.2",
+    "tox-gh-actions>=3.1.0",
+]
+doc = [
+    "sphinx>=5.3.0",
+    "numpydoc>=1.5.0",
+    "myst-parser>=1.0.0",
+    "sphinx-rtd-theme>=1.2.0",
+]
+lint = [
+    "flake8>=3.9.2",
+]
+
+[tool.pdm.scripts]
+test-quick = "pytest test -v"
+test-matrix = "tox -v --skip-missing-interpreters=true"
+test-all = "tox -v --skip-missing-interpreters=false"
+doc = "sphinx-build doc doc/build -b html"
+lint = "flake8 plyfile.py test/test_plyfile.py"
 
 [project]
 name = "plyfile"
-version = "0.9"
+version = "1.0"
 description = "PLY file reader/writer"
 authors = [
     { name = "Darsh Ranjan", email = "dranjan@berkeley.edu" },
 ]
 dependencies = [
     "numpy>=1.17",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "ply",
     "numpy",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 
 [project.license]
 file = "COPYING"
 
 [project.urls]
 Homepage = "https://github.com/dranjan/python-plyfile"
+Documentation = "https://python-plyfile.readthedocs.io"
+Repository = "https://github.com/dranjan/python-plyfile"
 
 [build-system]
 requires = [
     "pdm-pep517>=1.0.0",
 ]
 build-backend = "pdm.pep517.api"
```

