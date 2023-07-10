# Comparing `tmp/sphinx-readme-0.0.1b5.tar.gz` & `tmp/sphinx-readme-0.0.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-readme-0.0.1b5.tar", last modified: Fri Jul  7 11:54:23 2023, max compression
+gzip compressed data, was "sphinx-readme-0.0.1b6.tar", last modified: Mon Jul 10 13:25:29 2023, max compression
```

## Comparing `sphinx-readme-0.0.1b5.tar` & `sphinx-readme-0.0.1b6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 11:54:23.555747 sphinx-readme-0.0.1b5/
--rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.0.1b5/LICENSE
--rw-rw-rw-   0        0        0     8624 2023-07-07 11:54:23.555747 sphinx-readme-0.0.1b5/PKG-INFO
--rw-rw-rw-   0        0        0     7833 2023-07-07 11:54:04.000000 sphinx-readme-0.0.1b5/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-07 11:54:23.555747 sphinx-readme-0.0.1b5/setup.cfg
--rw-rw-rw-   0        0        0     1454 2023-07-07 11:49:24.000000 sphinx-readme-0.0.1b5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 11:54:23.524503 sphinx-readme-0.0.1b5/sphinx_readme/
--rw-rw-rw-   0        0        0     1598 2023-07-07 11:50:39.000000 sphinx-readme-0.0.1b5/sphinx_readme/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 11:54:23.555747 sphinx-readme-0.0.1b5/sphinx_readme/config/
--rw-rw-rw-   0        0        0      136 2023-07-07 10:19:59.000000 sphinx-readme-0.0.1b5/sphinx_readme/config/__init__.py
--rw-rw-rw-   0        0        0     6890 2023-07-07 10:19:59.000000 sphinx-readme-0.0.1b5/sphinx_readme/config/linkcode.py
--rw-rw-rw-   0        0        0     8198 2023-07-07 10:50:47.000000 sphinx-readme-0.0.1b5/sphinx_readme/config/main.py
--rw-rw-rw-   0        0        0    21021 2023-07-07 11:49:24.000000 sphinx-readme-0.0.1b5/sphinx_readme/parser.py
--rw-rw-rw-   0        0        0     4878 2023-07-07 10:50:47.000000 sphinx-readme-0.0.1b5/sphinx_readme/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 11:54:23.555747 sphinx-readme-0.0.1b5/sphinx_readme.egg-info/
--rw-rw-rw-   0        0        0     8624 2023-07-07 11:54:23.000000 sphinx-readme-0.0.1b5/sphinx_readme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-07-07 11:54:23.000000 sphinx-readme-0.0.1b5/sphinx_readme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 11:54:23.000000 sphinx-readme-0.0.1b5/sphinx_readme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-07 11:54:23.000000 sphinx-readme-0.0.1b5/sphinx_readme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-07 11:54:23.000000 sphinx-readme-0.0.1b5/sphinx_readme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 13:25:29.443000 sphinx-readme-0.0.1b6/
+-rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.0.1b6/LICENSE
+-rw-rw-rw-   0        0        0     9372 2023-07-10 13:25:29.443000 sphinx-readme-0.0.1b6/PKG-INFO
+-rw-rw-rw-   0        0        0     8581 2023-07-10 13:24:24.000000 sphinx-readme-0.0.1b6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-10 13:25:29.443000 sphinx-readme-0.0.1b6/setup.cfg
+-rw-rw-rw-   0        0        0     1454 2023-07-07 16:12:34.000000 sphinx-readme-0.0.1b6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:25:29.396136 sphinx-readme-0.0.1b6/sphinx_readme/
+-rw-rw-rw-   0        0        0     1712 2023-07-10 13:12:35.000000 sphinx-readme-0.0.1b6/sphinx_readme/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:25:29.443000 sphinx-readme-0.0.1b6/sphinx_readme/config/
+-rw-rw-rw-   0        0        0       57 2023-07-10 13:08:55.000000 sphinx-readme-0.0.1b6/sphinx_readme/config/__init__.py
+-rw-rw-rw-   0        0        0     7156 2023-07-10 13:08:55.000000 sphinx-readme-0.0.1b6/sphinx_readme/config/linkcode.py
+-rw-rw-rw-   0        0        0     9080 2023-07-10 13:08:55.000000 sphinx-readme-0.0.1b6/sphinx_readme/config/main.py
+-rw-rw-rw-   0        0        0    20713 2023-07-10 13:08:55.000000 sphinx-readme-0.0.1b6/sphinx_readme/parser.py
+-rw-rw-rw-   0        0        0     4878 2023-07-07 16:12:34.000000 sphinx-readme-0.0.1b6/sphinx_readme/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:25:29.427382 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/
+-rw-rw-rw-   0        0        0     9372 2023-07-10 13:25:29.000000 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-07-10 13:25:29.000000 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 13:25:29.000000 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-10 13:25:29.000000 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-10 13:25:29.000000 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/top_level.txt
```

### Comparing `sphinx-readme-0.0.1b5/LICENSE` & `sphinx-readme-0.0.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b5/PKG-INFO` & `sphinx-readme-0.0.1b6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-readme
-Version: 0.0.1b5
+Version: 0.0.1b6
 Summary: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 Home-page: https://github.com/tdkorn/sphinx-readme
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-readme/tarball/main
 Keywords: sphinx,docutils,sphinx-extension,sphinx-contrib,reStructuredText,rst,reST,parser,rst-parser,README.rst,README,autodoc,linkcode
@@ -14,101 +14,96 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
 .. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
 .. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
-.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b5/sphinx_readme/parser.py#L124-L134
-.. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
-.. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
 .. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
 .. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |attention| replace:: ⚠
-.. |caution| replace:: ⚠
-.. |danger| replace:: ☢
-.. |error| replace:: ❌
+.. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
+.. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
+.. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
+.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b6/sphinx_readme/parser.py#L124-L134
+.. |attention| replace:: 🔔️
+.. |caution| replace:: ⚠️
+.. |danger| replace:: ☢️
+.. |error| replace:: ⛔
 .. |hint| replace:: 🧠
-.. |important| replace:: ‼
+.. |important| replace:: 📢
 .. |note| replace:: 📝
 .. |tip| replace:: 💡
-.. |warning| replace:: ❗
+.. |warning| replace:: 🚩
 .. |default| replace:: 📄
-.. |client| replace:: 💻
+.. |about| replace:: 📚
 
 .. meta::
    :author: Adam Korn
    :title: Sphinx README
-   :description: Sphinx extension to generate reStructuredText README.rst files that render beautifully on GitHub, PyPi, GitLab, BitBucket
-
-
-.. |RTD| replace:: **Explore the docs »**
-.. _RTD: https://sphinx-readme.readthedocs.io/en/latest/
+   :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b5/docs/source/_static/logo.png?raw=True
-   :alt: Sphinx README: Generate reStructuredText files that render beautifully on GitHub, PyPi, GitLab, BitBucket
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/logo_readme.png
+   :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
 
 A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
+.. |RTD| replace:: **Explore the docs »**
+.. _RTD: https://sphinx-readme.readthedocs.io/en/latest/
+
 |RTD|_
 
-|
 
 .. image:: https://img.shields.io/pypi/v/sphinx-readme?color=eb5202
-   :target: https://pypi.org/project/sphinx-readme/
-   :alt: PyPI Version
+   :target: https://pypi.org/project/sphinx-readme
+   :alt: PyPI Project for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 .. image:: https://img.shields.io/badge/GitHub-sphinx--readme-4f1abc
    :target: https://github.com/tdkorn/sphinx-readme
-   :alt: GitHub Repository
+   :alt: GitHub Repository for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 .. image:: https://static.pepy.tech/personalized-badge/sphinx-readme?period=total&units=none&left_color=grey&right_color=blue&left_text=Downloads
-    :target: https://pepy.tech/project/sphinx-readme
+   :target: https://pepy.tech/project/sphinx-readme
+   :alt: Downloads for Sphinx README
 
 .. image:: https://readthedocs.org/projects/sphinx-readme/badge/?version=latest
-    :target: https://sphinx-readme.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
-
+   :target: https://sphinx-readme.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 
 |
 
 About Sphinx README
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
 .. csv-table::
-   :header: |default| What's Sphinx README?
+   :header: |about| What's Sphinx README?
 
    "``sphinx_readme`` is a ``reStructuredText`` parser that uses Sphinx
    to generate ``rst`` files that render beautifully on
    GitHub, PyPi, GitLab, and BitBucket."
 
 
 
 With ``sphinx_readme``, there's no need to rewrite your ``README.rst`` as a ``README.md`` file
 ==============================================================================================
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
 
-
-
-
-.. image:: https://github.com/TDKorn/sphinx-readme/raw/v0.0.1b5/docs/source/_static/demo/demo.gif?raw=True
-   :alt: Demonstration of sphinx-readme extension output on GitHub, PyPi, GitLab, BitBucket
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/demo/demo.gif
+   :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 Features
 ~~~~~~~~~~
 
 ``sphinx_readme`` adds support for the following ``sphinx`` and ``docutils`` directives and features:
@@ -121,61 +116,61 @@
 * Rubrics
 * Images
 
 
 Installation
 ~~~~~~~~~~~~~
 
-To install with pip:
-
-.. code-block:: terminal
+Install using pip::
 
    pip install sphinx-readme
 
 
-Add the following to your ``conf.py``:
+Add the extension to your ``conf.py``:
 
 .. code-block:: python
 
    extensions = [
       'sphinx_readme',
    ]
 
 
+
 Configuration
 ~~~~~~~~~~~~~~~
 
-The behaviour and output of ``sphinx_readme`` can be customized by setting
-configuration variables in your ``conf.py``
 
-Please see `Extension Configuration <https://sphinx-readme.readthedocs.io/en/latest/configuring.html>`_ for documentation on all possible configuration variables
 
 
-Mandatory Configuration Values
-==================================
 
+Please see `Extension Configuration <https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html>`_ for full documentation on configuration variables
 
 
-.. Use substitutions for README until confval directive parsing is implemented
+Mandatory ``conf.py`` Values
+==================================
 
 |html_context|_
  A dictionary containing info about your repository
 
+  Type: ``dict``
+
  * At minimum, the username and repository name must be specified
  * Please see `HTML Context Settings <https://docs.readthedocs.io/en/stable/guides/edit-source-links-sphinx.html>`_
    to determine the correct dictionary keys for your hosting platform
 
 .. |html_context| replace:: ``html_context``
 .. _html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
 
 ...
 
 |html_baseurl|_
  The base URL which points to the root of the HTML documentation
 
+  Type: ``str``
+
 .. |html_baseurl| replace:: ``html_baseurl``
 .. _html_baseurl: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_baseurl
 
 ...
 
 |readme_src_files|_
  An individual or list of ``rst`` files to parse
@@ -186,49 +181,52 @@
 .. csv-table::
    :header: |important| Important
 
    "Filepaths should be specified relative to the source directory"
 
 
 .. |readme_src_files| replace:: ``readme_src_files``
-.. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuring.html#confval-readme_src_files
+.. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
 
 ...
 
 |readme_docs_url_type|_
  The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
+  Type: ``str``
+
  Must be either ``"code"`` or ``"html"``
 
  * ``"code"``: uses |.`sphinx.ext.linkcode`|_ to replace references with links to highlighted source code
 
-   *Example*: |.`~.parse_intersphinx_node`|_
+   **Example**: |.`~.parse_intersphinx_node`|_
+
 
  * ``"html"``: replaces references with links to HTML documentation entries
 
-   *Example*: |parse_intersphinx_node_html|_
+   **Example**: |parse_intersphinx_node_html|_
 
 
 .. csv-table::
    :header: |note| Note
 
    "If set to ``code``, then :code:`:attr:` cross-references will not be replaced with links
 
    * Instead, they'll be replaced with ``inline literals`` or left as is
    * Please see |readme_replace_attrs|_ and |readme_inline_markup|_"
 
 
 .. |readme_docs_url_type| replace:: ``readme_docs_url_type``
-.. _readme_docs_url_type: https://sphinx-readme.readthedocs.io/en/latest/configuring.html#confval-readme_docs_url_type
+.. _readme_docs_url_type: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_docs_url_type
 .. |parse_intersphinx_node_html| replace:: ``parse_intersphinx_node()``
 .. _parse_intersphinx_node_html: http://sphinx-readme.readthedocs.io/en/latest/parser.html#sphinx_readme.parser.READMEParser.parse_intersphinx_node
 .. |readme_replace_attrs| replace:: ``readme_replace_attrs``
-.. _readme_replace_attrs: https://sphinx-readme.readthedocs.io/en/latest/configuring.html#confval-readme_replace_attrs
+.. _readme_replace_attrs: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_replace_attrs
 .. |readme_inline_markup| replace:: ``readme_inline_markup``
-.. _readme_inline_markup: https://sphinx-readme.readthedocs.io/en/latest/configuring.html#confval-readme_inline_markup
+.. _readme_inline_markup: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_inline_markup
 
 
 Sample ``conf.py``
 ~~~~~~~~~~~~~~~~~~~
 
 .. code-block:: python
 
@@ -245,14 +243,33 @@
    html_baseurl = "https://sphinx-readme.readthedocs.io/en/latest"
 
    readme_src_files = "README.rst"
 
    readme_docs_url_type = "code"
 
 
+.. |readme_raw_directive| replace:: ``readme_raw_directive``
+.. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
+
+
+
+.. csv-table::
+   :header: |important| Important
+
+   "If generating a ``README`` for a platform that doesn't support ``raw``
+   directives (PyPi, GitLab, and BitBucket), be sure to disable |readme_raw_directive|_:
+
+   .. code-block:: python
+
+      readme_raw_directive = False"
+
+
+
+
+
 Documentation
 ~~~~~~~~~~~~~~~~
 
 Full documentation can be found on |docs|_
 
 
 .. |docs| replace:: ``ReadTheDocs``
```

### Comparing `sphinx-readme-0.0.1b5/README.rst` & `sphinx-readme-0.0.1b6/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,96 +1,91 @@
 .. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
 .. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
-.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b5/sphinx_readme/parser.py#L124-L134
-.. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
-.. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
 .. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
 .. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |attention| replace:: ⚠
-.. |caution| replace:: ⚠
-.. |danger| replace:: ☢
-.. |error| replace:: ❌
+.. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
+.. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
+.. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
+.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b6/sphinx_readme/parser.py#L124-L134
+.. |attention| replace:: 🔔️
+.. |caution| replace:: ⚠️
+.. |danger| replace:: ☢️
+.. |error| replace:: ⛔
 .. |hint| replace:: 🧠
-.. |important| replace:: ‼
+.. |important| replace:: 📢
 .. |note| replace:: 📝
 .. |tip| replace:: 💡
-.. |warning| replace:: ❗
+.. |warning| replace:: 🚩
 .. |default| replace:: 📄
-.. |client| replace:: 💻
+.. |about| replace:: 📚
 
 .. meta::
    :author: Adam Korn
    :title: Sphinx README
-   :description: Sphinx extension to generate reStructuredText README.rst files that render beautifully on GitHub, PyPi, GitLab, BitBucket
-
-
-.. |RTD| replace:: **Explore the docs »**
-.. _RTD: https://sphinx-readme.readthedocs.io/en/latest/
+   :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b5/docs/source/_static/logo.png?raw=True
-   :alt: Sphinx README: Generate reStructuredText files that render beautifully on GitHub, PyPi, GitLab, BitBucket
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/logo_readme.png
+   :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
 
 A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
+.. |RTD| replace:: **Explore the docs »**
+.. _RTD: https://sphinx-readme.readthedocs.io/en/latest/
+
 |RTD|_
 
-|
 
 .. image:: https://img.shields.io/pypi/v/sphinx-readme?color=eb5202
-   :target: https://pypi.org/project/sphinx-readme/
-   :alt: PyPI Version
+   :target: https://pypi.org/project/sphinx-readme
+   :alt: PyPI Project for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 .. image:: https://img.shields.io/badge/GitHub-sphinx--readme-4f1abc
    :target: https://github.com/tdkorn/sphinx-readme
-   :alt: GitHub Repository
+   :alt: GitHub Repository for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 .. image:: https://static.pepy.tech/personalized-badge/sphinx-readme?period=total&units=none&left_color=grey&right_color=blue&left_text=Downloads
-    :target: https://pepy.tech/project/sphinx-readme
+   :target: https://pepy.tech/project/sphinx-readme
+   :alt: Downloads for Sphinx README
 
 .. image:: https://readthedocs.org/projects/sphinx-readme/badge/?version=latest
-    :target: https://sphinx-readme.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
-
+   :target: https://sphinx-readme.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 
 |
 
 About Sphinx README
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
 .. csv-table::
-   :header: |default| What's Sphinx README?
+   :header: |about| What's Sphinx README?
 
    "``sphinx_readme`` is a ``reStructuredText`` parser that uses Sphinx
    to generate ``rst`` files that render beautifully on
    GitHub, PyPi, GitLab, and BitBucket."
 
 
 
 With ``sphinx_readme``, there's no need to rewrite your ``README.rst`` as a ``README.md`` file
 ==============================================================================================
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
 
-
-
-
-.. image:: https://github.com/TDKorn/sphinx-readme/raw/v0.0.1b5/docs/source/_static/demo/demo.gif?raw=True
-   :alt: Demonstration of sphinx-readme extension output on GitHub, PyPi, GitLab, BitBucket
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/demo/demo.gif
+   :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 Features
 ~~~~~~~~~~
 
 ``sphinx_readme`` adds support for the following ``sphinx`` and ``docutils`` directives and features:
@@ -103,61 +98,61 @@
 * Rubrics
 * Images
 
 
 Installation
 ~~~~~~~~~~~~~
 
-To install with pip:
-
-.. code-block:: terminal
+Install using pip::
 
    pip install sphinx-readme
 
 
-Add the following to your ``conf.py``:
+Add the extension to your ``conf.py``:
 
 .. code-block:: python
 
    extensions = [
       'sphinx_readme',
    ]
 
 
+
 Configuration
 ~~~~~~~~~~~~~~~
 
-The behaviour and output of ``sphinx_readme`` can be customized by setting
-configuration variables in your ``conf.py``
 
-Please see `Extension Configuration <https://sphinx-readme.readthedocs.io/en/latest/configuring.html>`_ for documentation on all possible configuration variables
 
 
-Mandatory Configuration Values
-==================================
 
+Please see `Extension Configuration <https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html>`_ for full documentation on configuration variables
 
 
-.. Use substitutions for README until confval directive parsing is implemented
+Mandatory ``conf.py`` Values
+==================================
 
 |html_context|_
  A dictionary containing info about your repository
 
+  Type: ``dict``
+
  * At minimum, the username and repository name must be specified
  * Please see `HTML Context Settings <https://docs.readthedocs.io/en/stable/guides/edit-source-links-sphinx.html>`_
    to determine the correct dictionary keys for your hosting platform
 
 .. |html_context| replace:: ``html_context``
 .. _html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
 
 ...
 
 |html_baseurl|_
  The base URL which points to the root of the HTML documentation
 
+  Type: ``str``
+
 .. |html_baseurl| replace:: ``html_baseurl``
 .. _html_baseurl: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_baseurl
 
 ...
 
 |readme_src_files|_
  An individual or list of ``rst`` files to parse
@@ -168,49 +163,52 @@
 .. csv-table::
    :header: |important| Important
 
    "Filepaths should be specified relative to the source directory"
 
 
 .. |readme_src_files| replace:: ``readme_src_files``
-.. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuring.html#confval-readme_src_files
+.. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
 
 ...
 
 |readme_docs_url_type|_
  The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
+  Type: ``str``
+
  Must be either ``"code"`` or ``"html"``
 
  * ``"code"``: uses |.`sphinx.ext.linkcode`|_ to replace references with links to highlighted source code
 
-   *Example*: |.`~.parse_intersphinx_node`|_
+   **Example**: |.`~.parse_intersphinx_node`|_
+
 
  * ``"html"``: replaces references with links to HTML documentation entries
 
-   *Example*: |parse_intersphinx_node_html|_
+   **Example**: |parse_intersphinx_node_html|_
 
 
 .. csv-table::
    :header: |note| Note
 
    "If set to ``code``, then :code:`:attr:` cross-references will not be replaced with links
 
    * Instead, they'll be replaced with ``inline literals`` or left as is
    * Please see |readme_replace_attrs|_ and |readme_inline_markup|_"
 
 
 .. |readme_docs_url_type| replace:: ``readme_docs_url_type``
-.. _readme_docs_url_type: https://sphinx-readme.readthedocs.io/en/latest/configuring.html#confval-readme_docs_url_type
+.. _readme_docs_url_type: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_docs_url_type
 .. |parse_intersphinx_node_html| replace:: ``parse_intersphinx_node()``
 .. _parse_intersphinx_node_html: http://sphinx-readme.readthedocs.io/en/latest/parser.html#sphinx_readme.parser.READMEParser.parse_intersphinx_node
 .. |readme_replace_attrs| replace:: ``readme_replace_attrs``
-.. _readme_replace_attrs: https://sphinx-readme.readthedocs.io/en/latest/configuring.html#confval-readme_replace_attrs
+.. _readme_replace_attrs: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_replace_attrs
 .. |readme_inline_markup| replace:: ``readme_inline_markup``
-.. _readme_inline_markup: https://sphinx-readme.readthedocs.io/en/latest/configuring.html#confval-readme_inline_markup
+.. _readme_inline_markup: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_inline_markup
 
 
 Sample ``conf.py``
 ~~~~~~~~~~~~~~~~~~~
 
 .. code-block:: python
 
@@ -227,14 +225,33 @@
    html_baseurl = "https://sphinx-readme.readthedocs.io/en/latest"
 
    readme_src_files = "README.rst"
 
    readme_docs_url_type = "code"
 
 
+.. |readme_raw_directive| replace:: ``readme_raw_directive``
+.. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
+
+
+
+.. csv-table::
+   :header: |important| Important
+
+   "If generating a ``README`` for a platform that doesn't support ``raw``
+   directives (PyPi, GitLab, and BitBucket), be sure to disable |readme_raw_directive|_:
+
+   .. code-block:: python
+
+      readme_raw_directive = False"
+
+
+
+
+
 Documentation
 ~~~~~~~~~~~~~~~~
 
 Full documentation can be found on |docs|_
 
 
 .. |docs| replace:: ``ReadTheDocs``
```

### Comparing `sphinx-readme-0.0.1b5/setup.py` & `sphinx-readme-0.0.1b6/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b5/sphinx_readme/__init__.py` & `sphinx-readme-0.0.1b6/sphinx_readme/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import os
 import sphinx
-from pathlib import Path
 from typing import Dict, Any
 from docutils.nodes import document
 from sphinx.application import Sphinx
 from sphinx.environment import BuildEnvironment
 from sphinx_readme.utils import get_conf_val, set_conf_val
 from sphinx_readme.config import get_repo_dir
 from sphinx_readme.parser import READMEParser
 
 
-__version__ = "v0.0.1b5"
+__version__ = "v0.0.1b6"
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
+    # Avoid setting up extension if building on ReadTheDocs
+    if os.environ.get("READTHEDOCS") == "True":
+        return {}
+
     app.connect('env-check-consistency', parse_titles)
     app.connect('doctree-resolved', parse_references)
     app.connect('build-finished', resolve_readme)
 
     app.add_config_value("readme_inline_markup", True, True)
     app.add_config_value("readme_raw_directive", True, True)
     app.add_config_value("readme_include_directive", True, True)
@@ -25,15 +29,14 @@
     app.add_config_value("readme_blob", 'head', True)
     app.add_config_value("readme_default_admonition_icon", "📄", True)
 
     set_conf_val(app, 'READMEParser', READMEParser(app))
 
     return {'version': sphinx.__display_version__, 'parallel_read_safe': True}
 
-
 def parse_titles(app: Sphinx, env: BuildEnvironment):
     readme = get_conf_val(app, 'READMEParser')
     readme.parse_titles(env)
 
 
 def parse_references(app: Sphinx, doctree: document, docname: str):
     readme = get_conf_val(app, 'READMEParser')
```

### Comparing `sphinx-readme-0.0.1b5/sphinx_readme/config/linkcode.py` & `sphinx-readme-0.0.1b6/sphinx_readme/config/linkcode.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,40 +37,42 @@
     for host in ('github', 'gitlab', 'bitbucket'):
         user = context.get(f"{host}_user")
         repo = context.get(f"{host}_repo")
 
         if not all((user, repo)):
             continue
 
-        tld = "org" if host == "bitbucket" else "com"
+        if host == "bitbucket":
+            tld = "org"
+        else:
+            tld = "com"
+
         return f"https://{host}.{tld}/{user}/{repo}"
 
-    logger.error("``sphinx_readme``: unable to determine repo url")
-    return None
+    raise ExtensionError(
+        "``sphinx_readme``: unable to determine repo url")
 
 
 def get_blob_url(repo_url: str, blob: Optional[str] = None, context: Optional[Dict] = None) -> str:
     """Generate the url for a specific blob of a repository
 
     If ``blob`` and ``context`` are not provided, the most recent commit hash will be used
     """
-    host = get_repo_host(repo_url)
-
     if context:
+        host = get_repo_host(repo_url)
         blob = context.get(f"{host}_version")
 
-    if blob:
+    if blob is not None:
         # Use blob from kwarg/html_context
         blob = get_linkcode_revision(blob)
-
     else:
         # Use hash of the most recent commit
         blob = get_linkcode_revision('head')
 
-    if host == "bitbucket":
+    if "bitbucket" in repo_url:
         return repo_url.strip('/') + f"/src/{blob}"
     else:
         return repo_url.strip("/") + f"/blob/{blob}"
 
 
 def get_repo_host(url: str):
     if match := re.match(r"https?://(\w+)\.(?:com|org)", url):
@@ -139,19 +141,25 @@
 def get_repo_dir() -> Path:
     """Get the root directory of the repository
 
     :raises RuntimeError: if the directory can't be determined
     """
     try:
         cmd = "git rev-parse --show-toplevel"
-        return Path(subprocess.check_output(cmd.split(" ")).strip().decode('utf-8'))
+        repo_dir = Path(subprocess.check_output(cmd.split(" ")).strip().decode('utf-8'))
 
     except subprocess.CalledProcessError as e:
         raise RuntimeError("Unable to determine the repository directory") from e
 
+    # For ReadTheDocs, repo is cloned to /path/to/<repo_dir>/checkouts/<version>/
+    if repo_dir.parent == "checkouts":
+        return repo_dir.parent.parent
+    else:
+        return repo_dir
+
 
 def get_linkcode_resolve(linkcode_url: str) -> Callable:
     """Defines and returns a ``linkcode_resolve`` function for your package
 
     Used by default if ``linkcode_resolve`` isn't defined in ``conf.py``
     """
```

### Comparing `sphinx-readme-0.0.1b5/sphinx_readme/config/main.py` & `sphinx-readme-0.0.1b6/sphinx_readme/config/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Union, List, Dict
 from functools import cached_property
 
 from sphinx.application import Sphinx
 from sphinx.errors import ExtensionError
 
 from sphinx_readme.utils import get_conf_val, set_conf_val, logger, replace_only_directives, remove_raw_directives
-from sphinx_readme.config import get_repo_dir, get_blob_url, get_repo_url, get_linkcode_url, get_linkcode_resolve
+from sphinx_readme.config import get_repo_dir, get_repo_host, get_blob_url, get_repo_url, get_linkcode_url, get_linkcode_resolve
 
 
 class READMEConfig:
 
     REFERENCE_MAPPING = {
         "replace": None,
         "target": None,
@@ -34,61 +34,68 @@
         self.raw_directive = get_conf_val(app, 'readme_raw_directive')
         self.rubric_heading = get_conf_val(app, 'readme_rubric_heading')
         self.admonition_icons = get_conf_val(app, 'readme_admonition_icons')
         self.include_directive = get_conf_val(app, 'readme_include_directive')
         self.default_admonition_icon = get_conf_val(app, 'readme_default_admonition_icon')
 
         self.repo_blob = get_conf_val(app, "readme_blob")
-        self.repo_url = self.get_repo_url(app)
+        self.repo_url = self.get_repo_url()
         self.blob_url = get_blob_url(
             repo_url=self.repo_url,
             blob=self.repo_blob
         )
-        self.docs_url = self.get_docs_url(app)
+        self.docs_url = self.get_docs_url()
         self.ref_map = self.get_ref_map()
         self.source_files = self.read_source_files()
 
         if self.docs_url_type == "code":
             self.setup_linkcode_resolve(app)
 
-    def get_repo_url(self, app: Sphinx):
-        if repo_url := get_conf_val(app, "readme_repo_url"):
-            return repo_url.rstrip("/")
-
-        if self.html_context:
-            return get_repo_url(self.html_context)
-
-        raise ExtensionError(
-            "sphinx_readme: conf.py value must be set for "
-            "``readme_repo_url`` or ``html_context``"
-        )
+    def get_repo_url(self) -> str:
+        """Generates the repository URL from the :external+sphinx:confval:`html_context` dict
 
-    def get_docs_url(self, app: Sphinx) -> str:
-        if docs_url := get_conf_val(app, "readme_docs_url") is None:
-            # Generate docs URL from other conf.py values
-            if self.docs_url_type == "html":
-                if self.html_baseurl:
-                    docs_url = self.html_baseurl
-                else:
-                    raise ExtensionError(
-                        "sphinx_readme: conf.py value must be set for "
-                        "``readme_docs_url`` or ``html_baseurl``"
-                    )
-            else:  # ``docs_url_type`` is "code"
-                docs_url = self.blob_url
+        :raises ExtensionError: if ``html_context`` is not set or missing values
+        """
+        if not self.html_context:
+            raise ExtensionError(
+                "``sphinx_readme``: conf.py value "
+                "must be set for ``html_context``"
+            )
+        return get_repo_url(self.html_context)
+
+    def get_docs_url(self) -> str:
+        """Returns the base URL of the documentation source to use
+        when resolving :mod:`~.sphinx.ext.autodoc` cross-references
+
+         If :attr:`docs_url_type` is
+
+         * ``"code"``: uses the :attr:`blob_url`
+         * ``"html"``: uses the :confval:`html_baseurl`
+
+        :raises ExtensionError: if ``html_baseurl`` is missing
+        """
+        if self.docs_url_type == "html":
+            if self.html_baseurl:
+                docs_url = self.html_baseurl
+            else:
+                raise ExtensionError(
+                    "``sphinx_readme``: conf.py value "
+                    "must be set for ``html_baseurl``"
+                )
+        else:  # ``docs_url_type`` is "code"
+            docs_url = self.blob_url
 
         return docs_url.rstrip("/")
 
     def setup_linkcode_resolve(self, app: Sphinx) -> None:
         linkcode_func = get_conf_val(app, "linkcode_resolve")
 
         if not callable(linkcode_func):
             self.logger.info(
-                "``sphinx_readme:`` Function `linkcode_resolve` not found in ``conf.py``; "
-                "using default function from ``sphinx_readme``"
+                "``sphinx_readme:`` using default ``linkcode_resolve``"
             )
             # Get the template for linking to source code
             linkcode_url = get_linkcode_url(self.blob_url)
             linkcode_func = get_linkcode_resolve(linkcode_url)
 
         set_conf_val(app, 'linkcode_resolve', linkcode_func)
         app.setup_extension("sphinx.ext.linkcode")
@@ -121,26 +128,24 @@
                 pattern=include_pattern,
                 string=rst,
                 flags=re.M
             )
             for include in included:
                 # Determine abs path of included file
                 if include.startswith("/"):
-
                     # These paths are relative to source dir
-                    file = Path(f"{self.src_dir}/{include}").resolve()
-
+                    file = Path(f"{self.src_dir}{include}").resolve()
                 else:
                     # These paths are relative to rst_file dir
                     file = (Path(rst_file).parent / Path(include)).resolve()
 
                 # Sub in the file content
                 rst = re.sub(
                     pattern=rf".. include:: {include}",
-                    repl=self.read_rst(file).replace(r'\n', r'\\n'),
+                    repl=self.read_rst(file, replace_only).replace(r'\n', r'\\n'),
                     string=rst
                 )
         else:
             # Remove all include directives from the text
             rst = re.sub(include_pattern, '', rst, flags=re.M)
 
         if self.raw_directive is False:
@@ -191,17 +196,36 @@
         if docs_url_type == "code" and not self.html_baseurl:
             raise ExtensionError(  # HTML url is needed for non-source code xrefs
                 "``sphinx_readme``: conf.py value missing for ``html_baseurl``"
             )
         self._docs_url_type = docs_url_type
 
     @cached_property
+    def repo_host(self):
+        return get_repo_host(self.repo_url)
+
+    @cached_property
+    def image_baseurl(self):
+        if self.repo_host == "github":
+            # Ex. https://raw.githubusercontent.com/TDKorn/sphinx-readme/main
+            return self.blob_url.replace("github.com", "raw.githubusercontent.com").replace('blob/', '')
+
+        elif self.repo_host == "gitlab":
+            # Ex. https://gitlab.com/TDKorn/sphinx-readme/raw/main
+            return self.blob_url.replace("/blob/", "/raw/")
+
+        else:
+            # Ex. https://bitbucket.org/TDKorn/sphinx-readme/raw/main
+            return self.blob_url.replace("/src/", "/raw/")
+
+
+    @cached_property
     def icon_map(self):
         types = ("attention", "caution", "danger", "error", "hint", "important", "note", "tip", "warning", "default")
-        icons = ("⚠", "⚠", "☢", "❌", "🧠", "‼", "📝", "💡", "❗", self.default_admonition_icon)
+        icons = ("🔔️", "⚠️", "☢️", '⛔', "🧠", "📢", "📝", "💡", "🚩", self.default_admonition_icon)
         icon_map = dict(zip(types, icons))
 
         # Update/add custom admonition icons from conf.py
         if self.admonition_icons:
             if isinstance(self.admonition_icons, Dict):
                 icon_map.update(self.admonition_icons)
```

### Comparing `sphinx-readme-0.0.1b5/sphinx_readme/parser.py` & `sphinx-readme-0.0.1b6/sphinx_readme/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,17 +125,17 @@
         pattern = r":(mod|class|meth|func|attr):`~?\.?[.\w]+`"
         match = re.match(pattern, node.rawsource)
         target = node.parent.get('refuri')
 
         if not all((match, target)):
             return
 
-        is_method = match.group(1) == "meth"
+        is_callable = match.group(1) in ("meth", "func")
         qualified_name = target.split("#")[-1].split("-")[-1]
-        self.add_variants(qualified_name, target, is_method)
+        self.add_variants(qualified_name, target, is_callable)
 
     def parse_module_node(self, node: Node, docname: str):
         qualified_name = node.parent.get("reftitle", "")
 
         if self.config.docs_url_type == 'code':
             # Ex. sphinx_readme.parser -> sphinx_readme/parser.py
             refuri = qualified_name.replace('.', '/') + '.py'
@@ -151,17 +151,17 @@
     def parse_autodoc_node(self, node: nodes.literal, docname: str):
         qualified_name = node.parent.get("reftitle")
         refuri = self._parse_refuri(node, docname)
 
         if not all((refuri, qualified_name)):
             return
 
-        is_method = 'py-meth' in node['classes']
+        is_callable = bool(re.match(r":(meth|func):", node.rawsource))
         target = f"{self.config.docs_url}/{refuri}"
-        self.add_variants(qualified_name, target, is_method)
+        self.add_variants(qualified_name, target, is_callable)
 
     def _parse_refuri(self, node: Node, docname: str):
         if 'refuri' in node.parent:
             # Ex. ../parser.html#sphinx_readme.parser.READMEParser
             return node.parent["refuri"].lstrip("./")
 
         elif 'refid' in node.parent:
@@ -173,38 +173,38 @@
             if 'viewcode-link' in node['classes'] or 'linkcode-link' in node['classes']:
                 if node.parent.get('internal') is False:
                     # Only parse links to external source code
                     self.parse_linkcode_node(node)
 
     def parse_linkcode_node(self, node: nodes.inline):
         grandparent = node.parent.parent
-        is_method = grandparent.get("_toc_name", "").endswith("()")
+        is_callable = grandparent.get("_toc_name", "").endswith("()")
 
         try:
             qualified_name = grandparent.get("ids")[0]
         except IndexError:
             qualified_name = grandparent.get("module", "") + grandparent.get("fullname", "")
 
         target = node.parent.get("refuri")
-        self.add_variants(qualified_name, target, is_method)
+        self.add_variants(qualified_name, target, is_callable)
 
-    def add_variants(self, qualified_name, target, is_method: bool = False):
+    def add_variants(self, qualified_name, target, is_callable: bool = False):
         short_ref = qualified_name.split('.')[-1]
         variants = get_all_variants(qualified_name)
 
         for variant in variants:
             if variant in self.ref_map:
                 continue
 
             if variant.startswith("~"):
                 replace = short_ref
             else:
                 replace = variant.lstrip('.')
 
-            if is_method:
+            if is_callable:
                 replace += "()"
 
             if self.config.inline_markup:
                 replace = f"``{replace}``"
 
             self.ref_map[variant].update({
                 'target': target,
@@ -367,44 +367,37 @@
            value of :confval:`readme_docs_url_type`
 
         :param rst_src: absolute path of the rst file being parsed
         :param rst: the content of the rst file being parsed
         """
         src_dir = self.config.src_dir
         repo_dir = self.config.repo_dir
-        relpath_to_src_dir = src_dir.relative_to(repo_dir)
         rst_src_dir = Path(rst_src).parent
-        blob_url = self.config.blob_url
+        relpath_to_src_dir = src_dir.relative_to(repo_dir)
 
         # Find the targets of all image directives
         img_pattern = r"\.\. image:: ([./\w-]+\.\w{3,4})"
         img_paths = re.findall(img_pattern, rst)
 
         for img_path in img_paths:
             if img_path.startswith("/"):
-                # These image paths are "absolute" (relative to src_dir)
-                # .. image:: /path/to/image.ext
-                path_to_img = (relpath_to_src_dir / Path(img_path)).as_posix()
+                # These paths are relative to source dir
+                path_to_img = Path(f"{relpath_to_src_dir}{img_path}").as_posix()
 
             else:
-                # These image paths are relative to the rst source file
-                # .. image:: image.png || .. image:: images/image.png || .. image:: ../images/image.png
+                # These paths are relative to rst_file dir
                 abs_img_path = (rst_src_dir / Path(img_path)).resolve()
 
                 # Find path of image relative to the repo directory
                 path_to_img = abs_img_path.relative_to(repo_dir).as_posix()
 
-            # Use raw url for gifs
-            if img_path.endswith("gif"):
-                blob_url = blob_url.replace("blob", "raw")
-
             # Sub that hoe in!!!
             rst = re.sub(
                 pattern=rf"\.\. image:: {img_path}",
-                repl=fr".. image:: {blob_url}/{path_to_img}?raw=True",
+                repl=fr".. image:: {self.config.image_baseurl}/{path_to_img}",
                 string=rst
             )
         return rst
 
     def replace_rst_rubrics(self, rst: str):
         heading_chars = '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~'
         rubric_pattern = r'\.\. rubric:: (.+?)(?=\n)'
```

### Comparing `sphinx-readme-0.0.1b5/sphinx_readme/utils.py` & `sphinx-readme-0.0.1b6/sphinx_readme/utils.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b5/sphinx_readme.egg-info/PKG-INFO` & `sphinx-readme-0.0.1b6/sphinx_readme.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-readme
-Version: 0.0.1b5
+Version: 0.0.1b6
 Summary: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 Home-page: https://github.com/tdkorn/sphinx-readme
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-readme/tarball/main
 Keywords: sphinx,docutils,sphinx-extension,sphinx-contrib,reStructuredText,rst,reST,parser,rst-parser,README.rst,README,autodoc,linkcode
@@ -14,101 +14,96 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
 .. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
 .. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
-.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b5/sphinx_readme/parser.py#L124-L134
-.. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
-.. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
 .. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
 .. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |attention| replace:: ⚠
-.. |caution| replace:: ⚠
-.. |danger| replace:: ☢
-.. |error| replace:: ❌
+.. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
+.. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
+.. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
+.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b6/sphinx_readme/parser.py#L124-L134
+.. |attention| replace:: 🔔️
+.. |caution| replace:: ⚠️
+.. |danger| replace:: ☢️
+.. |error| replace:: ⛔
 .. |hint| replace:: 🧠
-.. |important| replace:: ‼
+.. |important| replace:: 📢
 .. |note| replace:: 📝
 .. |tip| replace:: 💡
-.. |warning| replace:: ❗
+.. |warning| replace:: 🚩
 .. |default| replace:: 📄
-.. |client| replace:: 💻
+.. |about| replace:: 📚
 
 .. meta::
    :author: Adam Korn
    :title: Sphinx README
-   :description: Sphinx extension to generate reStructuredText README.rst files that render beautifully on GitHub, PyPi, GitLab, BitBucket
-
-
-.. |RTD| replace:: **Explore the docs »**
-.. _RTD: https://sphinx-readme.readthedocs.io/en/latest/
+   :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b5/docs/source/_static/logo.png?raw=True
-   :alt: Sphinx README: Generate reStructuredText files that render beautifully on GitHub, PyPi, GitLab, BitBucket
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/logo_readme.png
+   :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
 
 A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
+.. |RTD| replace:: **Explore the docs »**
+.. _RTD: https://sphinx-readme.readthedocs.io/en/latest/
+
 |RTD|_
 
-|
 
 .. image:: https://img.shields.io/pypi/v/sphinx-readme?color=eb5202
-   :target: https://pypi.org/project/sphinx-readme/
-   :alt: PyPI Version
+   :target: https://pypi.org/project/sphinx-readme
+   :alt: PyPI Project for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 .. image:: https://img.shields.io/badge/GitHub-sphinx--readme-4f1abc
    :target: https://github.com/tdkorn/sphinx-readme
-   :alt: GitHub Repository
+   :alt: GitHub Repository for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 .. image:: https://static.pepy.tech/personalized-badge/sphinx-readme?period=total&units=none&left_color=grey&right_color=blue&left_text=Downloads
-    :target: https://pepy.tech/project/sphinx-readme
+   :target: https://pepy.tech/project/sphinx-readme
+   :alt: Downloads for Sphinx README
 
 .. image:: https://readthedocs.org/projects/sphinx-readme/badge/?version=latest
-    :target: https://sphinx-readme.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
-
+   :target: https://sphinx-readme.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 
 |
 
 About Sphinx README
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
 .. csv-table::
-   :header: |default| What's Sphinx README?
+   :header: |about| What's Sphinx README?
 
    "``sphinx_readme`` is a ``reStructuredText`` parser that uses Sphinx
    to generate ``rst`` files that render beautifully on
    GitHub, PyPi, GitLab, and BitBucket."
 
 
 
 With ``sphinx_readme``, there's no need to rewrite your ``README.rst`` as a ``README.md`` file
 ==============================================================================================
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
 
-
-
-
-.. image:: https://github.com/TDKorn/sphinx-readme/raw/v0.0.1b5/docs/source/_static/demo/demo.gif?raw=True
-   :alt: Demonstration of sphinx-readme extension output on GitHub, PyPi, GitLab, BitBucket
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/demo/demo.gif
+   :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 Features
 ~~~~~~~~~~
 
 ``sphinx_readme`` adds support for the following ``sphinx`` and ``docutils`` directives and features:
@@ -121,61 +116,61 @@
 * Rubrics
 * Images
 
 
 Installation
 ~~~~~~~~~~~~~
 
-To install with pip:
-
-.. code-block:: terminal
+Install using pip::
 
    pip install sphinx-readme
 
 
-Add the following to your ``conf.py``:
+Add the extension to your ``conf.py``:
 
 .. code-block:: python
 
    extensions = [
       'sphinx_readme',
    ]
 
 
+
 Configuration
 ~~~~~~~~~~~~~~~
 
-The behaviour and output of ``sphinx_readme`` can be customized by setting
-configuration variables in your ``conf.py``
 
-Please see `Extension Configuration <https://sphinx-readme.readthedocs.io/en/latest/configuring.html>`_ for documentation on all possible configuration variables
 
 
-Mandatory Configuration Values
-==================================
 
+Please see `Extension Configuration <https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html>`_ for full documentation on configuration variables
 
 
-.. Use substitutions for README until confval directive parsing is implemented
+Mandatory ``conf.py`` Values
+==================================
 
 |html_context|_
  A dictionary containing info about your repository
 
+  Type: ``dict``
+
  * At minimum, the username and repository name must be specified
  * Please see `HTML Context Settings <https://docs.readthedocs.io/en/stable/guides/edit-source-links-sphinx.html>`_
    to determine the correct dictionary keys for your hosting platform
 
 .. |html_context| replace:: ``html_context``
 .. _html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
 
 ...
 
 |html_baseurl|_
  The base URL which points to the root of the HTML documentation
 
+  Type: ``str``
+
 .. |html_baseurl| replace:: ``html_baseurl``
 .. _html_baseurl: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_baseurl
 
 ...
 
 |readme_src_files|_
  An individual or list of ``rst`` files to parse
@@ -186,49 +181,52 @@
 .. csv-table::
    :header: |important| Important
 
    "Filepaths should be specified relative to the source directory"
 
 
 .. |readme_src_files| replace:: ``readme_src_files``
-.. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuring.html#confval-readme_src_files
+.. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
 
 ...
 
 |readme_docs_url_type|_
  The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
+  Type: ``str``
+
  Must be either ``"code"`` or ``"html"``
 
  * ``"code"``: uses |.`sphinx.ext.linkcode`|_ to replace references with links to highlighted source code
 
-   *Example*: |.`~.parse_intersphinx_node`|_
+   **Example**: |.`~.parse_intersphinx_node`|_
+
 
  * ``"html"``: replaces references with links to HTML documentation entries
 
-   *Example*: |parse_intersphinx_node_html|_
+   **Example**: |parse_intersphinx_node_html|_
 
 
 .. csv-table::
    :header: |note| Note
 
    "If set to ``code``, then :code:`:attr:` cross-references will not be replaced with links
 
    * Instead, they'll be replaced with ``inline literals`` or left as is
    * Please see |readme_replace_attrs|_ and |readme_inline_markup|_"
 
 
 .. |readme_docs_url_type| replace:: ``readme_docs_url_type``
-.. _readme_docs_url_type: https://sphinx-readme.readthedocs.io/en/latest/configuring.html#confval-readme_docs_url_type
+.. _readme_docs_url_type: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_docs_url_type
 .. |parse_intersphinx_node_html| replace:: ``parse_intersphinx_node()``
 .. _parse_intersphinx_node_html: http://sphinx-readme.readthedocs.io/en/latest/parser.html#sphinx_readme.parser.READMEParser.parse_intersphinx_node
 .. |readme_replace_attrs| replace:: ``readme_replace_attrs``
-.. _readme_replace_attrs: https://sphinx-readme.readthedocs.io/en/latest/configuring.html#confval-readme_replace_attrs
+.. _readme_replace_attrs: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_replace_attrs
 .. |readme_inline_markup| replace:: ``readme_inline_markup``
-.. _readme_inline_markup: https://sphinx-readme.readthedocs.io/en/latest/configuring.html#confval-readme_inline_markup
+.. _readme_inline_markup: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_inline_markup
 
 
 Sample ``conf.py``
 ~~~~~~~~~~~~~~~~~~~
 
 .. code-block:: python
 
@@ -245,14 +243,33 @@
    html_baseurl = "https://sphinx-readme.readthedocs.io/en/latest"
 
    readme_src_files = "README.rst"
 
    readme_docs_url_type = "code"
 
 
+.. |readme_raw_directive| replace:: ``readme_raw_directive``
+.. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
+
+
+
+.. csv-table::
+   :header: |important| Important
+
+   "If generating a ``README`` for a platform that doesn't support ``raw``
+   directives (PyPi, GitLab, and BitBucket), be sure to disable |readme_raw_directive|_:
+
+   .. code-block:: python
+
+      readme_raw_directive = False"
+
+
+
+
+
 Documentation
 ~~~~~~~~~~~~~~~~
 
 Full documentation can be found on |docs|_
 
 
 .. |docs| replace:: ``ReadTheDocs``
```

