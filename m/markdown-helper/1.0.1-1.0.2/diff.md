# Comparing `tmp/markdown_helper-1.0.1.tar.gz` & `tmp/markdown_helper-1.0.2.tar.gz`

## Comparing `markdown_helper-1.0.1.tar` & `markdown_helper-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/.coveragerc
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/EXAMPLE.md
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/SECURITY.md
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/.vscode/settings.json
--rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/src/markdown_helper/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0    10116 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/tests/test_markdown.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/LICENSE
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/README.md
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 markdown_helper-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 markdown_helper-1.0.2/.coveragerc
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 markdown_helper-1.0.2/EXAMPLE.md
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 markdown_helper-1.0.2/SECURITY.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 markdown_helper-1.0.2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 markdown_helper-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 markdown_helper-1.0.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 markdown_helper-1.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0    15716 2020-02-02 00:00:00.000000 markdown_helper-1.0.2/src/markdown_helper/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_helper-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0    17734 2020-02-02 00:00:00.000000 markdown_helper-1.0.2/tests/test_markdown.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 markdown_helper-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 markdown_helper-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 markdown_helper-1.0.2/README.md
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 markdown_helper-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 markdown_helper-1.0.2/PKG-INFO
```

### Comparing `markdown_helper-1.0.1/.github/workflows/pylint.yml` & `markdown_helper-1.0.2/.github/workflows/pylint.yml`

 * *Files 3% similar despite different names*

```diff
@@ -14,10 +14,11 @@
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install pylint
+        pip install pytest
     - name: Analysing the code with pylint
       run: |
         pylint $(git ls-files '*.py')
```

### Comparing `markdown_helper-1.0.1/.github/workflows/python-publish.yml` & `markdown_helper-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `markdown_helper-1.0.1/.github/workflows/tests.yml` & `markdown_helper-1.0.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `markdown_helper-1.0.1/.vscode/settings.json` & `markdown_helper-1.0.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `markdown_helper-1.0.1/src/markdown_helper/__init__.py` & `markdown_helper-1.0.2/src/markdown_helper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,43 +68,60 @@
         
         Args:
             rows (list[dict[str, str | int | float | bool]]): List of rows to add
         """
         for row in rows:
             self.add_row(row)
 
-    def add_row(self, row: dict[str, str | int | float | bool]):
+    def add_row(self, row: dict[str, str | int | float | bool] | list[str]):
         """Add a row to the table.
         
         Args:
-            row (dict[str, str | int | float | bool]): Row to add
+            row (dict[str, str | int | float | bool], list[str]): Row to add
         """
 
-        # Check that all the keys in the row are in the headers
-        for key in row.keys():
-            if key not in self.headers:
-                if self.flexible_headers:
-                    self.headers.append(key)
-                else:
-                    raise ValueError(
-                        f"Key {key} not in headers and flexible_headers is False"
-                    )
+        # If row is a list, convert it to a dict, using the headers as keys
+        if isinstance(row, list):
+            if len(row) != len(self.headers):
+                raise ValueError(
+                    f"Row length ({len(row)}) does not match header length ({len(self.headers)})"
+                )
+            row = dict(zip(self.headers, row))
+        # If row is a dict, check that all the keys are in the headers, if not, raise error
+        elif isinstance(row, dict):
+            for key in row.keys():
+                if key not in self.headers:
+                    if self.flexible_headers:
+                        self.headers.append(key)
+                    else:
+                        raise ValueError(
+                            f"Key {key} not in headers and flexible_headers is False"
+                        )
         # Check that all the headers are in the row
         for header in self.headers:
             if header not in row.keys():
                 row[header] = ""
 
         self.rows.append(row)
 
-    def sort_table(self):
+    def sort_table(self, disable_convert: bool = False):
         """Sort the table by the sort_key."""
         if self.sort_key:
             # If multiple sort keys are provided, prioritize the first one, then the second, etc.
             sort_keys = self.sort_key.split(",")
             for sort_key in sort_keys:
+                if sort_key not in self.headers:
+                    raise ValueError(f"sort_key {sort_key} not in headers")
+                if disable_convert:
+                    self.rows = sorted(
+                        self.rows,
+                        key=lambda row: row.get(sort_key, ""), # pylint: disable=cell-var-from-loop
+                        reverse=self.sort_reverse,
+                    )
+                    break
                 if all( # pylint: disable=use-a-generator
                     [
                         row.get(sort_key, "")
                         in [1, 0, False, True, "False", "True", "false", "true"]
                         for row in self.rows
                     ]
                 ):
@@ -224,16 +241,18 @@
             image += f"_{self.caption}_\n"
         return image
     def __str__(self):
         if any([self.width, self.height, self.align]):
             return self.html()
         return self.markdown()
     def __repr__(self):
-        return f"""Image(url={self.url}, title={self.title}, alt={self.alt},
-          width={self.width}, height={self.height}, align={self.align}, caption={self.caption})"""
+        return_string = f"Image(url={self.url}, title={self.title}, alt={self.alt}"
+        return_string += f", width={self.width}, height={self.height}, align={self.align},"
+        return_string +=f"caption={self.caption})"
+        return return_string
 
 
 class Link:
     """Link object for markdown."""
     def __init__(self, url: str, text: str = "", **kwargs):
         """Create a link object.
 
@@ -318,15 +337,15 @@
             content (str, optional): Content of the section.
         """
         if isinstance(title, str):
             title = Header(title, **kwargs)
         self.title = title
         self.content = kwargs.get("content", "")
 
-    def add(self, content: str | Table | List | Image | Link):
+    def add(self, content: str | Table | List | Image | Link | Header):
         """Add content to the section.
 
         Args:
             content (str | Table | List | Image | Link): Content to add to the section.
         """
         if self.content:
             self.content += "\n"
```

### Comparing `markdown_helper-1.0.1/tests/test_markdown.py` & `markdown_helper-1.0.2/tests/test_markdown.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 """
 This file contains the pytest tests for the markdown_helper.py file.
 """
+import pytest
 try:
     from src import markdown_helper as markdown
 except ModuleNotFoundError:
     try:
         import markdown_helper as markdown
     except ModuleNotFoundError:
-        from ..src import markdown_helper as markdown # pylint: disable=import-error, relative-beyond-top-level
+        from ..src import (  # pylint: disable=relative-beyond-top-level
+            markdown_helper as markdown,  # pylint: disable=import-error
+        )  # pylint: disable=relative-beyond-top-level
+
+
 def test_ordered_list():
     """
     This function tests the markdown.List class.
     """
     list_1: markdown.List = markdown.List(["item 1", "item 2", "item 3"], ordered=True)
     assert (
         str(list_1) == "1. item 1\n2. item 2\n3. item 3\n"
     ), "String representation of ordered list is incorrect."
     assert list_1.items == ["item 1", "item 2", "item 3"], "List items are incorrect."
 
+def test_empty_list():
+    """
+    This function tests the markdown.List class.
+    """
+    list_1: markdown.List = markdown.List([], ordered=True)
+    assert (
+        str(list_1) == ""
+    ), "String representation of ordered list is incorrect."
+    assert list_1.items == [], "List items are incorrect."
+    assert repr(list_1) == "List(title=False, items=[], ordered=True)", "List items are incorrect."
 
 def test_modify_list():
     """
     This function tests the markdown.List class.
     """
     list_1 = markdown.List(["item 1", "item 2", "item 3"], ordered=True)
     list_1.add("item 4")
@@ -65,14 +80,17 @@
     """
     link_1 = markdown.Link("http://www.google.com", "Google")
     assert (
         str(link_1) == "[Google](http://www.google.com)\n"
     ), "String representation of link is incorrect."
     assert link_1.url == "http://www.google.com", "Link URL is incorrect."
     assert link_1.text == "Google", "Link text is incorrect."
+    assert (
+        repr(link_1) == "Link(url=http://www.google.com, text=Google, title=False, new_tab=False)"
+    )
 
 
 def test_link_no_trailing():
     """
     This function tests the markdown.Link class.
     """
     link_1 = markdown.Link("http://www.google.com", "Google", trailing=False)
@@ -115,14 +133,30 @@
     assert (
         str(image_1) == "![Google](http://www.google.com)\n"
     ), "String representation of image is incorrect."
     assert image_1.url == "http://www.google.com", "Image URL is incorrect."
     assert image_1.alt == "Google", "Image text is incorrect."
 
 
+def test_image_texts():
+    """
+    This function tests the markdown.Image class.
+    """
+    image_1 = markdown.Image(
+        "http://www.google.com", alt="Google", title="Title", caption="Caption"
+    )
+    assert (
+        image_1.markdown() == "### Title\n![Google](http://www.google.com)\n_Caption_\n"
+    ), "Markdown string representation of image is incorrect."
+    assert (
+        repr(image_1)
+        == "Image(url=http://www.google.com, title=Title, alt=Google, width=False, height=False, align=False,caption=Caption)"  # pylint: disable=line-too-long
+    ), "String representation of image is incorrect."
+
+
 def test_image_size():
     """
     This function tests the markdown.Image class.
     """
     image_1 = markdown.Image(
         "http://www.google.com", alt="Google", width=100, height=100
     )
@@ -179,57 +213,181 @@
         "col 3",
     ], "Table columns are incorrect."
     assert table_1.rows == [
         {"col 1": "item 1", "col 2": "item 2", "col 3": "item 3"}
     ], "Table rows are incorrect."
 
 
+def test_table_add_row_no_headers():
+    """
+    This function tests the table.add_row function with a list input.
+    """
+    table_1 = markdown.Table(["col 1", "col 2", "col 3"])
+    table_1.add_row(["item 1", "item 2", "item 3"])
+    assert (
+        str(table_1)
+        == "| col 1 | col 2 | col 3 |\n| --- | --- | --- |\n| item 1 | item 2 | item 3 |\n"
+    ), "String representation of table is incorrect."
+    assert table_1.headers == [
+        "col 1",
+        "col 2",
+        "col 3",
+    ], "Table columns are incorrect."
+    assert table_1.rows == [
+        {"col 1": "item 1", "col 2": "item 2", "col 3": "item 3"}
+    ], "Table rows are incorrect."
+
+
+def test_table_title():
+    """
+    This function tests the markdown.Table class.
+    """
+    table_1 = markdown.Table(["col 1", "col 2", "col 3"], title="My Table")
+    table_1.add_row({"col 1": "value 1", "col 2": "value 2", "col 3": "value 3"})
+    assert (
+        str(table_1)
+        == "### My Table\n| col 1 | col 2 | col 3 |\n| --- | --- | --- |\n| value 1 | value 2 | value 3 |\n" # pylint: disable=line-too-long
+    ), "String representation of table is incorrect."
+    assert table_1.headers == [
+        "col 1",
+        "col 2",
+        "col 3",
+    ], "Table columns are incorrect."
+    assert table_1.title == "My Table", "Table title is incorrect."
+
+
 def test_table_sort():
     """
     This function tests the markdown.Table class.
     """
     table_1 = markdown.Table(["Name", "Value"], sort_key="Value")
     table_1.add_row({"Name": "First", "Value": 1})
     table_1.add_row({"Name": "Second", "Value": 2})
     table_1.add_row({"Name": "Fourth", "Value": 4})
     table_1.add_row({"Name": "Third", "Value": 3})
     assert (
         str(table_1)
-        == "| Name | Value |\n| --- | --- |\n| First | 1 |\n| Second | 2 |\n| Third | 3 |\n| Fourth | 4 |\n" # pylint: disable=line-too-long
+        == "| Name | Value |\n| --- | --- |\n| First | 1 |\n| Second | 2 |\n| Third | 3 |\n| Fourth | 4 |\n"  # pylint: disable=line-too-long
     ), "Sorted Table is incorrect."
     assert table_1.headers == ["Name", "Value"], "Table columns are incorrect."
     table_1.sort_reverse = True
     assert (
         str(table_1)
-        == "| Name | Value |\n| --- | --- |\n| Fourth | 4 |\n| Third | 3 |\n| Second | 2 |\n| First | 1 |\n" # pylint: disable=line-too-long
+        == "| Name | Value |\n| --- | --- |\n| Fourth | 4 |\n| Third | 3 |\n| Second | 2 |\n| First | 1 |\n"  # pylint: disable=line-too-long
     ), "Reverse sorted Table is incorrect."
     table_1.sort_reverse = False
     table_1.sort_key = "Name"
     assert (
         str(table_1)
-        == "| Name | Value |\n| --- | --- |\n| First | 1 |\n| Fourth | 4 |\n| Second | 2 |\n| Third | 3 |\n" # pylint: disable=line-too-long
+        == "| Name | Value |\n| --- | --- |\n| First | 1 |\n| Fourth | 4 |\n| Second | 2 |\n| Third | 3 |\n"  # pylint: disable=line-too-long
     ), "Second sorted Table is incorrect."
 
+def test_table_sort_error():
+    """
+    This function tests the markdown.Table class.
+    """
+    table_1 = markdown.Table(["Name", "Value"], sort_key="Value")
+    table_1.add_row({"Name": "First", "Value": 1})
+    table_1.add_row({"Name": "Second", "Value": False})
+    table_1.add_row({"Name": "Fourth", "Value": 4})
+    table_1.add_row({"Name": "Third", "Value": "String"})
+    with pytest.raises(ValueError):
+        table_1.sort_key = "invalid"
+        table_1.sort_table()
+
+def test_table_disable_convert():
+    """
+    This function tests the markdown.Table class.
+    """
+    table_1 = markdown.Table(["Name", "Value"], sort_key="Value")
+    table_1.add_row({"Name": "First", "Value": 1})
+    table_1.add_row({"Name": "Second", "Value": 0})
+    table_1.add_row({"Name": "Fourth", "Value": 1})
+    table_1.add_row({"Name": "Third", "Value": 0})
+    table_1.sort_table(True)
+    assert (
+        table_1.rows == [{'Name': 'Second', 'Value': 0}, {'Name': 'Third', 'Value': 0},
+                        {'Name': 'First', 'Value': 1}, {'Name': 'Fourth', 'Value': 1}]
+    ), "Sorted Table is incorrect."
+
+def test_table_sort_convert():
+    """
+    This function tests the markdown.Table class.
+    """
+    table_1 = markdown.Table(["Name", "Value"], sort_key="Value")
+    table_1.add_row({"Name": "First", "Value": 1})
+    table_1.add_row({"Name": "Second", "Value": 0})
+    table_1.add_row({"Name": "Fourth", "Value": 1})
+    table_1.add_row({"Name": "Third", "Value": 0})
+    table_1.sort_table()
+    assert (
+        table_1.rows == [{'Name': 'Second', 'Value': False}, {'Name': 'Third', 'Value': False},
+                        {'Name': 'First', 'Value': True}, {'Name': 'Fourth', 'Value': True}]
+    ), "Sorted Table is incorrect."
 
 def test_table_flexible():
     """
     This function tests the markdown.Table class.
     """
     table_1 = markdown.Table(["Name", "Value"], flexible_headers=True)
     table_1.add_row({"Name": "First", "Value": 1})
     table_1.add_row({"Name": "Second", "Value": 2})
     table_1.add_row({"Name": "Third", "Value": 3, "Extra": "Extra Value"})
     table_1.add_row({"Name": "Fourth", "Value": 4})
     assert (
         str(table_1)
-        == "| Name | Value | Extra |\n| --- | --- | --- |\n| First | 1 |  |\n| Second | 2 |  |\n| Third | 3 | Extra Value |\n| Fourth | 4 |  |\n" # pylint: disable=line-too-long
+        == "| Name | Value | Extra |\n| --- | --- | --- |\n| First | 1 |  |\n| Second | 2 |  |\n| Third | 3 | Extra Value |\n| Fourth | 4 |  |\n"  # pylint: disable=line-too-long
     ), "Flexible Table is incorrect."
     assert table_1.headers == ["Name", "Value", "Extra"], "Table columns are incorrect."
 
+def test_table_add_rows():
+    """
+    This function tests the markdown.Table class.
+    """
+    table_1 = markdown.Table(["Name", "Value"])
+    table_1.add_rows([{"Name": "First", "Value": 1}, {"Name": "Second", "Value": 2}])
+    assert (
+        str(table_1)
+        == "| Name | Value |\n| --- | --- |\n| First | 1 |\n| Second | 2 |\n"
+    ), "Table is incorrect."
+    assert table_1.headers == ["Name", "Value"], "Table columns are incorrect."
+
+def test_table_remap():
+    """
+    This function tests the markdown.Table class.
+    """
+    table_1 = markdown.Table(["Name", "Value"], custom_map={"Name":{"First":"1st","Second":"2nd"}})
+    table_1.add_row({"Name": "First", "Value": 1})
+    table_1.add_row({"Name": "Second", "Value": 2})
+    assert (
+        str(table_1.get_table())
+        == "| Name | Value |\n| --- | --- |\n| 1st | 1 |\n| 2nd | 2 |\n"  # pylint: disable=line-too-long
+    ), "Remapped Table is incorrect."
+    assert table_1.headers == ["Name", "Value"], "Table columns are incorrect."
+    table_2 = markdown.Table(["Name", "Value"], custom_map={"Name":{"First":"1st","Second":"2nd"}})
+    table_2.add_row({"Name": "First", "Value": 1})
+    table_2.remap()
+    assert (
+        str(table_2)
+        == "| Name | Value |\n| --- | --- |\n| 1st | 1 |\n"  # pylint: disable=line-too-long
+    ), "Remapped Table is incorrect."
 
+
+def test_header():
+    """
+    This function tests the markdown.Header class.
+    """
+    header_1 = markdown.Header("Header 1", 2)
+    assert (
+        str(header_1) == "## Header 1"
+    ), "String representation of header is incorrect."
+    assert header_1.text == "Header 1", "Header text is incorrect."
+    assert (
+        repr(header_1) == "## Header 1"
+    )
 def test_section():
     """
     This function tests the markdown.Section class.
     """
     section_1 = markdown.Section("Section 1")
     assert (
         str(section_1) == "# Section 1\n\n"
@@ -242,14 +400,31 @@
     This function tests the markdown.Section class.
     """
     section_1 = markdown.Section("Section 1")
     section_1.add("This is a paragraph.")
     assert (
         str(section_1) == "# Section 1\nThis is a paragraph.  \n"
     ), "String representation of section is incorrect."
+    assert section_1.title.text == "Section 1", "Section title is incorrect."
+    assert (
+        repr(section_1) == "Section(title=# Section 1, content=This is a paragraph.  )"
+    ), "Section representation is incorrect."
+
+
+def test_section_add_nonempty():
+    """
+    This function tests the markdown.Section class.
+    """
+    section_1 = markdown.Section("Section 1")
+    section_1.add("This is a paragraph.")
+    section_1.add("This is another paragraph.")
+    assert (
+        str(section_1) == "# Section 1\nThis is a paragraph.  \nThis is another paragraph.  \n"
+    ), "String representation of section is incorrect."
+    assert section_1.title.text == "Section 1", "Section title is incorrect."
 
 
 def test_document():
     """
     This function tests the markdown.Document class.
     """
     document_1 = markdown.Document("Document 1", filename="document_1.md")
@@ -259,14 +434,34 @@
     ), "Section title is incorrect."
     section = document_1.sections["Section 1"]
     section.add("This is a paragraph.")
     assert (
         str(document_1) == "# Document 1\n## Section 1\nThis is a paragraph.  \n"
     ), "String representation of document is incorrect."
 
+def test_add_section():
+    """
+    This function tests the markdown.Document class.
+    """
+    document_1 = markdown.Document("Document 1", filename="document_1.md")
+    document_1.add_section("RAW SECTION")
+    assert (
+        str(document_1) == "# Document 1\n# RAW SECTION\n\n"
+    ), "String representation of document is incorrect."
+
+def test_document_toc():
+    """
+    This function tests the markdown.Document class.
+    """
+    document_1 = markdown.Document("Document 1", filename="document_1.md", table_of_contents=True) # pylint: disable=line-too-long
+    document_1.add_section(markdown.Section(markdown.Header("Section 1", 2)))
+    assert (
+        document_1.get_document() == "# Document 1\n## Table of Contents\n* [Section 1](#section-1)\n## Section 1\n\n" # pylint: disable=line-too-long
+    ), "String representation of document is incorrect."
+
 
 def test_document_save(tmp_path):
     """
     This function tests the markdown.Document class.
     """
     filename = tmp_path / "document_1.md"
     document_1 = markdown.Document("Document 1", filename=str(filename))
```

### Comparing `markdown_helper-1.0.1/.gitignore` & `markdown_helper-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `markdown_helper-1.0.1/LICENSE` & `markdown_helper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_helper-1.0.1/README.md` & `markdown_helper-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `markdown_helper-1.0.1/pyproject.toml` & `markdown_helper-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "markdown_helper"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name="Arttu Mahlakaarto", email="arttu.mahlakaarto@gmail.com" },
 ]
 description = "A simple markdown helper"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.10"
```

### Comparing `markdown_helper-1.0.1/PKG-INFO` & `markdown_helper-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown_helper
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple markdown helper
 Project-URL: homepage, https://github.com/amahlaka/python-markdown-helper
 Project-URL: bug-tracker, https://github.com/amahlaka/python-markdown-helper/issues
 Author-email: Arttu Mahlakaarto <arttu.mahlakaarto@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

