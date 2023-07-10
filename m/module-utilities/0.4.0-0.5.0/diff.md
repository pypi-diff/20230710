# Comparing `tmp/module-utilities-0.4.0.tar.gz` & `tmp/module-utilities-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "module-utilities-0.4.0.tar", last modified: Wed Jun 14 21:22:11 2023, max compression
+gzip compressed data, was "module-utilities-0.5.0.tar", last modified: Mon Jul 10 16:25:34 2023, max compression
```

## Comparing `module-utilities-0.4.0.tar` & `module-utilities-0.5.0.tar`

### file list

```diff
@@ -1,122 +1,135 @@
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.774150 module-utilities-0.4.0/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1367 2023-06-14 21:18:50.000000 module-utilities-0.4.0/.cruft.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-02 03:09:02.000000 module-utilities-0.4.0/.editorconfig
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.733679 module-utilities-0.4.0/.github/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      368 2023-05-02 03:09:02.000000 module-utilities-0.4.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1371 2023-06-14 21:18:50.000000 module-utilities-0.4.0/.gitignore
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-04-27 23:45:36.000000 module-utilities-0.4.0/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3644 2023-06-14 21:18:50.000000 module-utilities-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-04-27 23:45:36.000000 module-utilities-0.4.0/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      527 2023-06-14 20:02:14.000000 module-utilities-0.4.0/.recipe-append.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-27 23:45:36.000000 module-utilities-0.4.0/AUTHORS.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      645 2023-06-14 21:18:50.000000 module-utilities-0.4.0/CHANGELOG.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9874 2023-06-14 21:18:50.000000 module-utilities-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1789 2023-06-14 21:18:50.000000 module-utilities-0.4.0/LICENSE
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-04-27 23:45:36.000000 module-utilities-0.4.0/MANIFEST.in
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9401 2023-06-14 21:18:50.000000 module-utilities-0.4.0/Makefile
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9286 2023-06-14 21:22:11.773665 module-utilities-0.4.0/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5615 2023-06-14 21:18:50.000000 module-utilities-0.4.0/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.734596 module-utilities-0.4.0/changelog.d/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-04-27 23:45:36.000000 module-utilities-0.4.0/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.735025 module-utilities-0.4.0/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.736026 module-utilities-0.4.0/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-04-27 23:45:36.000000 module-utilities-0.4.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-04-27 23:45:36.000000 module-utilities-0.4.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-04-27 23:45:36.000000 module-utilities-0.4.0/changelog.d/templates/new_fragment.md.j2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      204 2023-04-27 23:45:36.000000 module-utilities-0.4.0/conftest.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.740769 module-utilities-0.4.0/docs/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1401 2023-05-03 02:36:13.000000 module-utilities-0.4.0/docs/Makefile
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.718685 module-utilities-0.4.0/docs/_static/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.741128 module-utilities-0.4.0/docs/_static/css/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.742006 module-utilities-0.4.0/docs/_static/js/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.744842 module-utilities-0.4.0/docs/_templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.746778 module-utilities-0.4.0/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.747912 module-utilities-0.4.0/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/class-single-page.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1186 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/custom-module-template.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1212 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/module-custom-imported.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/authors.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/changelog.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14851 2023-06-14 20:02:42.000000 module-utilities-0.4.0/docs/conf.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/contributing.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.748343 module-utilities-0.4.0/docs/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       75 2023-06-14 21:18:50.000000 module-utilities-0.4.0/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.749447 module-utilities-0.4.0/docs/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.4.0/docs/examples/usage/cached.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.4.0/docs/examples/usage/docfiller.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      224 2023-06-14 20:02:45.000000 module-utilities-0.4.0/docs/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      940 2023-06-14 21:18:50.000000 module-utilities-0.4.0/docs/installation.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/license.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/make.bat
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.750032 module-utilities-0.4.0/docs/reference/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      192 2023-06-14 20:02:51.000000 module-utilities-0.4.0/docs/reference/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.754775 module-utilities-0.4.0/environment/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      227 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/base.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      419 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/dev.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      225 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      418 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/docs.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      136 2023-05-02 03:09:02.000000 module-utilities-0.4.0/environment/lint.yaml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.756369 module-utilities-0.4.0/environment/lock/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/lock/py310.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/lock/py311.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       63 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/lock/py38.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       63 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/lock/py39.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      193 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/test-extras.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      265 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      287 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/test.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      296 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/typing.yaml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.756790 module-utilities-0.4.0/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-04-27 23:45:36.000000 module-utilities-0.4.0/examples/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.758142 module-utilities-0.4.0/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.4.0/examples/usage/cached.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.4.0/examples/usage/docfiller.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    29603 2023-06-14 21:18:50.000000 module-utilities-0.4.0/noxfile.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     7469 2023-06-14 21:18:50.000000 module-utilities-0.4.0/pyproject.toml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-06-14 21:22:11.774261 module-utilities-0.4.0/setup.cfg
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.723004 module-utilities-0.4.0/src/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.763036 module-utilities-0.4.0/src/module_utilities/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      546 2023-06-14 21:18:50.000000 module-utilities-0.4.0/src/module_utilities/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2646 2023-05-02 03:09:02.000000 module-utilities-0.4.0/src/module_utilities/_doc.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      382 2023-05-02 03:09:02.000000 module-utilities-0.4.0/src/module_utilities/_typing.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5930 2023-05-03 20:28:18.000000 module-utilities-0.4.0/src/module_utilities/attributedict.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9991 2023-05-03 20:28:18.000000 module-utilities-0.4.0/src/module_utilities/cached.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    21035 2023-06-14 21:18:50.000000 module-utilities-0.4.0/src/module_utilities/docfiller.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-02 03:09:02.000000 module-utilities-0.4.0/src/module_utilities/py.typed
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.770461 module-utilities-0.4.0/src/module_utilities/vendored/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1298 2023-06-14 21:18:50.000000 module-utilities-0.4.0/src/module_utilities/vendored/LICENSE.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       93 2023-06-14 21:18:50.000000 module-utilities-0.4.0/src/module_utilities/vendored/README.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       24 2023-06-14 21:18:50.000000 module-utilities-0.4.0/src/module_utilities/vendored/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23449 2023-06-14 21:18:50.000000 module-utilities-0.4.0/src/module_utilities/vendored/docscrape.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.766773 module-utilities-0.4.0/src/module_utilities.egg-info/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9286 2023-06-14 21:22:11.000000 module-utilities-0.4.0/src/module_utilities.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2659 2023-06-14 21:22:11.000000 module-utilities-0.4.0/src/module_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-06-14 21:22:11.000000 module-utilities-0.4.0/src/module_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      719 2023-06-14 21:22:11.000000 module-utilities-0.4.0/src/module_utilities.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       17 2023-06-14 21:22:11.000000 module-utilities-0.4.0/src/module_utilities.egg-info/top_level.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:05:27.000000 module-utilities-0.4.0/src/module_utilities.egg-info/zip-safe
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.772576 module-utilities-0.4.0/tests/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       46 2023-04-27 23:45:36.000000 module-utilities-0.4.0/tests/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.4.0/tests/conftest.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10864 2023-05-02 03:09:02.000000 module-utilities-0.4.0/tests/test_cached.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     8959 2023-05-03 20:28:18.000000 module-utilities-0.4.0/tests/test_docfiller.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-06-14 20:04:01.000000 module-utilities-0.4.0/tests/test_module_utilities.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.772964 module-utilities-0.4.0/tools/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    20805 2023-06-14 21:18:50.000000 module-utilities-0.4.0/tools/noxtools.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.441504 module-utilities-0.5.0/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1367 2023-07-10 16:24:53.000000 module-utilities-0.5.0/.cruft.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-02 03:09:02.000000 module-utilities-0.5.0/.editorconfig
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.374016 module-utilities-0.5.0/.github/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      368 2023-05-02 03:09:02.000000 module-utilities-0.5.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1409 2023-07-10 16:24:53.000000 module-utilities-0.5.0/.gitignore
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-04-27 23:45:36.000000 module-utilities-0.5.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3635 2023-07-10 16:24:53.000000 module-utilities-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-04-27 23:45:36.000000 module-utilities-0.5.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      527 2023-06-29 17:23:57.000000 module-utilities-0.5.0/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-27 23:45:36.000000 module-utilities-0.5.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      789 2023-07-10 16:24:53.000000 module-utilities-0.5.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11143 2023-07-10 16:24:53.000000 module-utilities-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1789 2023-06-29 17:24:09.000000 module-utilities-0.5.0/LICENSE
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-04-27 23:45:36.000000 module-utilities-0.5.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9644 2023-07-10 16:24:53.000000 module-utilities-0.5.0/Makefile
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9430 2023-07-10 16:25:34.440140 module-utilities-0.5.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5615 2023-06-29 17:24:16.000000 module-utilities-0.5.0/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.375119 module-utilities-0.5.0/changelog.d/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-04-27 23:45:36.000000 module-utilities-0.5.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.375818 module-utilities-0.5.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.377562 module-utilities-0.5.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-04-27 23:45:36.000000 module-utilities-0.5.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-04-27 23:45:36.000000 module-utilities-0.5.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-04-27 23:45:36.000000 module-utilities-0.5.0/changelog.d/templates/new_fragment.md.j2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      204 2023-04-27 23:45:36.000000 module-utilities-0.5.0/conftest.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.384057 module-utilities-0.5.0/docs/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1401 2023-05-03 02:36:13.000000 module-utilities-0.5.0/docs/Makefile
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.357670 module-utilities-0.5.0/docs/_static/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.384807 module-utilities-0.5.0/docs/_static/css/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.386361 module-utilities-0.5.0/docs/_static/js/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.391048 module-utilities-0.5.0/docs/_templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.394871 module-utilities-0.5.0/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.397029 module-utilities-0.5.0/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/class-single-page.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1186 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1212 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/module-custom-imported.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/authors.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/changelog.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    15101 2023-07-10 16:24:53.000000 module-utilities-0.5.0/docs/conf.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/contributing.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.397779 module-utilities-0.5.0/docs/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       75 2023-06-29 17:24:43.000000 module-utilities-0.5.0/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.399407 module-utilities-0.5.0/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.5.0/docs/examples/usage/cached.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.5.0/docs/examples/usage/docfiller.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      224 2023-06-29 17:24:47.000000 module-utilities-0.5.0/docs/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      940 2023-06-29 17:24:47.000000 module-utilities-0.5.0/docs/installation.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/license.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/make.bat
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.400196 module-utilities-0.5.0/docs/reference/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      192 2023-06-29 17:24:47.000000 module-utilities-0.5.0/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.409736 module-utilities-0.5.0/environment/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      227 2023-07-10 16:25:24.000000 module-utilities-0.5.0/environment/base.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      419 2023-07-10 16:25:25.000000 module-utilities-0.5.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      280 2023-07-10 16:25:26.000000 module-utilities-0.5.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-07-10 16:25:26.000000 module-utilities-0.5.0/environment/dist-pypi.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      225 2023-07-10 16:25:25.000000 module-utilities-0.5.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      406 2023-07-10 16:25:25.000000 module-utilities-0.5.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      136 2023-05-02 03:09:02.000000 module-utilities-0.5.0/environment/lint.yaml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.420925 module-utilities-0.5.0/environment/lock/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    37993 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py310-dev-conda-lock.yml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    73122 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py310-dist-conda-conda-lock.yml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23235 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py310-dist-pypi-conda-lock.yml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13842 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py310-test-conda-lock.yml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    15181 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py310-typing-conda-lock.yml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-06-14 21:18:50.000000 module-utilities-0.5.0/environment/lock/py310.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14231 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py311-test-conda-lock.yml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    15570 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py311-typing-conda-lock.yml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-06-14 21:18:50.000000 module-utilities-0.5.0/environment/lock/py311.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13457 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py38-test-conda-lock.yml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14788 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py38-typing-conda-lock.yml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       63 2023-06-14 21:18:50.000000 module-utilities-0.5.0/environment/lock/py38.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13831 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py39-test-conda-lock.yml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    15164 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py39-typing-conda-lock.yml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       63 2023-06-14 21:18:50.000000 module-utilities-0.5.0/environment/lock/py39.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      193 2023-07-10 16:25:26.000000 module-utilities-0.5.0/environment/test-extras.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      265 2023-07-10 16:25:26.000000 module-utilities-0.5.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      287 2023-07-10 16:25:24.000000 module-utilities-0.5.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      296 2023-07-10 16:25:24.000000 module-utilities-0.5.0/environment/typing.yaml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.421911 module-utilities-0.5.0/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-04-27 23:45:36.000000 module-utilities-0.5.0/examples/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.423762 module-utilities-0.5.0/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.5.0/examples/usage/cached.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.5.0/examples/usage/docfiller.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    32098 2023-07-10 16:24:53.000000 module-utilities-0.5.0/noxfile.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     7499 2023-07-10 16:24:53.000000 module-utilities-0.5.0/pyproject.toml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-07-10 16:25:34.441887 module-utilities-0.5.0/setup.cfg
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.360910 module-utilities-0.5.0/src/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.428319 module-utilities-0.5.0/src/module_utilities/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      340 2023-07-10 16:24:53.000000 module-utilities-0.5.0/src/module_utilities/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3199 2023-07-10 16:24:53.000000 module-utilities-0.5.0/src/module_utilities/_doc.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      382 2023-05-02 03:09:02.000000 module-utilities-0.5.0/src/module_utilities/_typing.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      160 2023-07-10 16:25:34.000000 module-utilities-0.5.0/src/module_utilities/_version.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5930 2023-05-03 20:28:18.000000 module-utilities-0.5.0/src/module_utilities/attributedict.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9991 2023-05-03 20:28:18.000000 module-utilities-0.5.0/src/module_utilities/cached.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    21356 2023-07-10 16:24:53.000000 module-utilities-0.5.0/src/module_utilities/docfiller.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-02 03:09:02.000000 module-utilities-0.5.0/src/module_utilities/py.typed
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.434895 module-utilities-0.5.0/src/module_utilities/vendored/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1298 2023-06-14 21:18:50.000000 module-utilities-0.5.0/src/module_utilities/vendored/LICENSE.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       93 2023-06-14 21:18:50.000000 module-utilities-0.5.0/src/module_utilities/vendored/README.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       24 2023-06-14 21:18:50.000000 module-utilities-0.5.0/src/module_utilities/vendored/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23449 2023-06-14 21:18:50.000000 module-utilities-0.5.0/src/module_utilities/vendored/docscrape.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.431587 module-utilities-0.5.0/src/module_utilities.egg-info/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9430 2023-07-10 16:25:34.000000 module-utilities-0.5.0/src/module_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3205 2023-07-10 16:25:34.000000 module-utilities-0.5.0/src/module_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-07-10 16:25:34.000000 module-utilities-0.5.0/src/module_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      696 2023-07-10 16:25:34.000000 module-utilities-0.5.0/src/module_utilities.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       17 2023-07-10 16:25:34.000000 module-utilities-0.5.0/src/module_utilities.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:05:27.000000 module-utilities-0.5.0/src/module_utilities.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.438091 module-utilities-0.5.0/tests/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       46 2023-04-27 23:45:36.000000 module-utilities-0.5.0/tests/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.5.0/tests/conftest.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10864 2023-05-02 03:09:02.000000 module-utilities-0.5.0/tests/test_cached.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10075 2023-07-10 16:24:53.000000 module-utilities-0.5.0/tests/test_docfiller.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-06-29 17:27:13.000000 module-utilities-0.5.0/tests/test_module_utilities.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.438794 module-utilities-0.5.0/tools/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    24175 2023-07-10 16:24:53.000000 module-utilities-0.5.0/tools/noxtools.py
```

### Comparing `module-utilities-0.4.0/.cruft.json` & `module-utilities-0.5.0/.cruft.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'c205c8acb0c3f69df17cbdfc00c03f806e0eef9b'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": "feature/nox",
-    "commit": "8b671d07d854bd6f5bd566267cc39118c8d76ba7",
+    "commit": "c205c8acb0c3f69df17cbdfc00c03f806e0eef9b",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
                 "docs/_templates/autosummary/*.rst",
                 "docs/_templates/autodocsumm/*.rst",
```

### Comparing `module-utilities-0.4.0/.editorconfig` & `module-utilities-0.5.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/.gitignore` & `module-utilities-0.5.0/.gitignore`

 * *Files 23% similar despite different names*

```diff
@@ -110,7 +110,9 @@
 .noxconfig.toml
 cruft.patch
 /docs/**/generated/
 /monkeytype.sqlite3
 /dist-conda/
 /tmp/
 /module-utilities-feedstock*/
+/src/**/_version.py
+tuna-loadtime.log
```

### Comparing `module-utilities-0.4.0/.pre-commit-config.yaml` & `module-utilities-0.5.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -17,41 +17,41 @@
       - id: check-yaml
       - id: check-json
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-toml
   #* Formatting
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.6"
+    rev: "v3.0.0"
     hooks:
       - id: prettier
         stages: [commit]
         additional_dependencies:
           - prettier-plugin-toml
   #** markdown
   - repo: https://github.com/DavidAnson/markdownlint-cli2
-    rev: v0.6.0
+    rev: v0.8.1
     hooks:
       - id: markdownlint-cli2
         args: ["--style prettier"]
   #* Linting
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
-    rev: "v0.0.261"
+    rev: "v0.0.277"
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       # - id: black-jupyter
       # Move to just black.  use nbqa for notebook formatting
       - id: black
         exclude: ^src/module-utilities/vendored/docscrape.py
   - repo: https://github.com/adamchainz/blacken-docs
-    rev: "1.13.0"
+    rev: "1.15.0"
     hooks:
       - id: blacken-docs
         additional_dependencies:
           - black==23.3.0
         # exclude: ^README.md
   - repo: https://github.com/nbQA-dev/nbQA
     rev: 1.7.0
@@ -59,15 +59,15 @@
       - id: nbqa-ruff
         additional_dependencies: [ruff]
       - id: nbqa-black
         additional_dependencies: [black]
 
   #* Commit message
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: v3.0.1
+    rev: 3.5.2
     hooks:
       - id: commitizen
         stages: [commit-msg]
 
   #* Manual Linting
   - repo: local
     hooks:
@@ -94,15 +94,15 @@
   # isort, pyupgrade, flake8 defer to ruff
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
         stages: [manual]
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.9.0
     hooks:
       - id: pyupgrade
         stages: [manual]
         args: [--py38-plus]
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
@@ -122,14 +122,14 @@
         stages: [manual]
         args: [--py38-plus]
       - id: nbqa-isort
         additional_dependencies: [isort]
         stages: [manual]
   #** spelling
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
+    rev: v2.2.5
     hooks:
       - id: codespell
         types_or: [python, rst, markdown, cython, c]
         additional_dependencies: [tomli]
         args: [-I, docs/spelling_wordlist.txt]
         stages: [manual]
```

### Comparing `module-utilities-0.4.0/.recipe-append.yaml` & `module-utilities-0.5.0/.recipe-append.yaml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/CHANGELOG.md` & `module-utilities-0.5.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 ## Unreleased
 
 See the fragment files in
 [changelog.d](https://github.com/usnistgov/module-utilities)
 
 <!-- scriv-insert-here -->
 
+## v0.5.0 — 2023-07-10
+
+### Added
+
+- Add `_prepend` option to docfiller. Default behavior is now to append current
+  docstring to templates.
+
 ## v0.4.0 — 2023-06-14
 
 ### Added
 
 - Package now available on conda-forge
 
 ### Changed
```

### Comparing `module-utilities-0.4.0/CONTRIBUTING.md` & `module-utilities-0.5.0/CONTRIBUTING.md`

 * *Files 12% similar despite different names*

```diff
@@ -381,21 +381,59 @@
 
 [setuptools_scm]: https://github.com/pypa/setuptools_scm
 
 Versioning is handled with [setuptools_scm].The package version is set by the
 git tag. For convenience, you can override the version with nox setting
 `--version ...`. This is useful for updating the docs, etc.
 
+We use the `write_to` option to [setuptools_scm]. This stores the current
+version in `_version.py`. Note that if you build the package (or, build docs
+with the `--version` flag), this will overwrite information in `_version.py` in
+the `src` directory. To refresh the version, run:
+
+```bash
+make version-scm
+```
+
+This scheme avoids having to install `setuptools-scm` (and `setuptools`) in each
+environment.
+
 ## Notes on [nox]
 
 One downside of using [tox] with this particular workflow is the need for
 multiple scripts/makefiles, while with [nox], most everything is self contained
 in the file `noxfile.py`. [nox] also is allows for a mix of conda and virtualenv
 environments.
 
+We use a mix of conda environments and virtualenv with nox. For example, for
+building the distribution, we use virtualenv, while for development, the default
+is to create a conda environment. To facilitate this, we need to let virtualenv
+know where different python interpreters are. I've had trouble mixing pyenv with
+conda. Instead, I use conda to create multiple invironments to hold different
+python version:
+
+```bash
+$ for version in 3.8 3.9 3.10 3.11; do
+    conda create -n test-3.8 python=3.8
+  done
+```
+
+To tell nox where these environments live, create the file `.noxconfig.toml`
+with the following:
+
+```toml
+[nox.python]
+paths = ["~/.conda/envs/test-3.*/bin"]
+
+```
+
+where `~/.conda/envs` should be replaced by whatever prefix you have setup on
+your machine. The noxfile will add this to the search path for python versions
+when creating virtualenvs.
+
 ## Serving the documentation
 
 To view to documentation with js headers/footers, you'll need to serve them:
 
 ```bash
 python -m http.server -d docs/_build/html
 ```
```

### Comparing `module-utilities-0.4.0/LICENSE` & `module-utilities-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/Makefile` & `module-utilities-0.5.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -129,19 +129,20 @@
 	$(BROWSER) htmlcov/index.html
 
 
 ################################################################################
 # versioning
 ################################################################################
 .PHONY: version-scm version-import version
-version-scm: ## check version of package
+
+version-scm: ## check/update version of package with setuptools-scm
 	python -m setuptools_scm
 
 version-import: ## check version from python import
-	python -c 'import module_utilities; print(module_utilities.__version__)'
+	-python -c 'import module_utilities; print(module_utilities.__version__)'
 
 version: version-scm version-import
 
 ################################################################################
 # Environment files
 ################################################################################
 .PHONY: environment-files-clean
@@ -186,15 +187,15 @@
 	$(NOX) -s docs -- -d build
 docs-clean: ## clean docs
 	rm -rf docs/_build/*
 	rm -rf docs/generated/*
 	rm -rf docs/reference/generated/*
 docs-clean-build: docs-clean docs-build ## clean and build
 docs-release: ## release docs.
-	$(NOX) -s docs -- release
+	$(NOX) -s docs -- -d release
 docs-command: ## run arbitrary command with command=...
 	$(NOX) -s docs -- --docs-run $(command)
 
 .PHONY: .docs-spelling docs-nist-pages docs-open docs-livehtml docs-clean-build docs-linkcheck
 docs-spelling: ## run spell check with sphinx
 	$(NOX) -s docs -- -d spelling
 docs-livehtml: ## use autobuild for docs
@@ -266,7 +267,14 @@
 
 # Note that this requires `auto-changelog`, which can be installed with pip(x)
 auto-changelog: ## autogenerate changelog and print to stdout
 	auto-changelog -u -r usnistgov -v unreleased --tag-prefix v --stdout --template changelog.d/templates/auto-changelog/template.jinja2
 
 commitizen-changelog:
 	cz changelog --unreleased-version unreleased --dry-run --incremental
+
+# tuna analyze load time:
+.PHONY: tuna-analyze
+tuna-import: ## Analyze load time for module
+	python -X importtime -c 'import module_utilities' 2> tuna-loadtime.log
+	tuna tuna-loadtime.log
+	rm tuna-loadtime.log
```

### Comparing `module-utilities-0.4.0/PKG-INFO` & `module-utilities-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-utilities
-Version: 0.4.0
+Version: 0.5.0
 Summary: Collection of utilities to aid working with python modules.
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/module-utilities
 Project-URL: documentation, https://pages.nist.gov/module-utilities/
 Keywords: module-utilities
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -301,14 +301,21 @@
 ## Unreleased
 
 See the fragment files in
 [changelog.d](https://github.com/usnistgov/module-utilities)
 
 <!-- scriv-insert-here -->
 
+## v0.5.0 — 2023-07-10
+
+### Added
+
+- Add `_prepend` option to docfiller. Default behavior is now to append current
+  docstring to templates.
+
 ## v0.4.0 — 2023-06-14
 
 ### Added
 
 - Package now available on conda-forge
 
 ### Changed
```

### Comparing `module-utilities-0.4.0/README.md` & `module-utilities-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/changelog.d/templates/auto-changelog/template.jinja2` & `module-utilities-0.5.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/Makefile` & `module-utilities-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/_static/css/nist-combined.css` & `module-utilities-0.5.0/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/_static/js/leave_notice.js` & `module-utilities-0.5.0/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/_static/js/nist-header-footer.js` & `module-utilities-0.5.0/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/_templates/autosummary/class.rst` & `module-utilities-0.5.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/_templates/autosummary/module.rst` & `module-utilities-0.5.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/_templates/class-individual-pages.rst` & `module-utilities-0.5.0/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/_templates/class-single-page.rst` & `module-utilities-0.5.0/docs/_templates/class-single-page.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/_templates/custom-module-template.rst` & `module-utilities-0.5.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/_templates/module-custom-imported.rst` & `module-utilities-0.5.0/docs/_templates/module-custom-imported.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/_templates/module-custom.rst` & `module-utilities-0.5.0/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/_templates/module-single.rst` & `module-utilities-0.5.0/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/_templates/module-template.rst` & `module-utilities-0.5.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/conf.py` & `module-utilities-0.5.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,23 +233,36 @@
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 # versioning with scm with editable install has issues.
 # instead, try to use scm if available.
-try:
-    from setuptools_scm import get_version
+# try:
+#     from setuptools_scm import get_version
+
+#     version = get_version(root="..", relative_to=__file__)
+#     release = version
+# except ImportError:
+#     version = module_utilities.__version__
+#     # The full version, including alpha/beta/rc tags.
+#     release = module_utilities.__version__
+
+
+def _get_version():
+    import os
+
+    version = os.environ.get("SETUPTOOLS_SCM_PRETEND_VERSION", None)
+    if version is None:
+        version = module_utilities.__version__
+    return version
+
+
+release = version = _get_version()
 
-    version = get_version(root="..", relative_to=__file__)
-    release = version
-except ImportError:
-    version = module_utilities.__version__
-    # The full version, including alpha/beta/rc tags.
-    release = module_utilities.__version__
 
 # if always want to print "latest"
 # release = "latest"
 # version = "latest"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
```

### Comparing `module-utilities-0.4.0/docs/examples/usage/cached.ipynb` & `module-utilities-0.5.0/docs/examples/usage/cached.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/examples/usage/docfiller.ipynb` & `module-utilities-0.5.0/docs/examples/usage/docfiller.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/installation.md` & `module-utilities-0.5.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/docs/make.bat` & `module-utilities-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/examples/usage/cached.ipynb` & `module-utilities-0.5.0/examples/usage/cached.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/examples/usage/docfiller.ipynb` & `module-utilities-0.5.0/examples/usage/docfiller.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/noxfile.py` & `module-utilities-0.5.0/noxfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,117 +1,78 @@
 """Config file for nox"""
 from __future__ import annotations
 
 import shutil
 from dataclasses import replace  # noqa
 from pathlib import Path
 from textwrap import dedent
-from typing import Annotated, Any, Callable, Collection, Literal, TypeVar, cast
+from typing import Annotated, Any, Callable, Collection, TypeVar, cast
 
 import nox
 from noxopt import NoxOpt, Option, Session
 
 from tools.noxtools import (
     combine_list_str,
+    load_nox_config,
+    open_webpage,
     prepend_flag,
     session_install_envs,
     session_install_envs_lock,
     # session_install_package,
     session_install_pip,
     session_run_commands,
-    # session_skip_install,
     sort_like,
     update_target,
 )
 
-# --- nox options ----------------------------------------------------------------------
+# * nox options ------------------------------------------------------------------------
 ROOT = Path(__file__).parent
 
 nox.options.reuse_existing_virtualenvs = True
 nox.options.sessions = ["test"]
 
-# --- Options --------------------------------------------------------------------------
+# * Options ----------------------------------------------------------------------------
 
 PACKAGE_NAME = "module-utilities"
 IMPORT_NAME = "module_utilities"
 KERNEL_BASE = "module_utilities"
 
 PYTHON_ALL_VERSIONS = ["3.8", "3.9", "3.10", "3.11"]
 PYTHON_DEFAULT_VERSION = "3.10"
 
 # conda/mamba
 if shutil.which("mamba"):
     CONDA_BACKEND = "mamba"
 elif shutil.which("conda"):
     CONDA_BACKEND = "conda"
 else:
-    raise ValueError("neigher conda or mamba found")
+    raise ValueError("neither conda or mamba found")
 
 SESSION_DEFAULT_KWS = {"python": PYTHON_DEFAULT_VERSION, "venv_backend": CONDA_BACKEND}
 SESSION_ALL_KWS = {"python": PYTHON_ALL_VERSIONS, "venv_backend": CONDA_BACKEND}
 
 
-# --- Set PATH to find all python versions ---------------------------------------------
+# * User config ------------------------------------------------------------------------
 
-DEFAULTS: dict[str, Any] = {}
+CONFIG = load_nox_config()
 
-
-def load_nox_config():
-    path = Path(".") / ".noxconfig.toml"
-    if not path.exists():
-        return
-
-    import os
-    from glob import glob
-
-    import tomli
-
-    with path.open("rb") as f:
-        data = tomli.load(f)
-
-    # python paths
-    try:
-        paths = []
-        for p in data["nox"]["python"]["paths"]:
-            paths.extend(glob(os.path.expanduser(p)))
-
-        paths_str = ":".join(map(str, paths))
-        os.environ["PATH"] = paths_str + ":" + os.environ["PATH"]
-    except KeyError:
-        pass
-
-    # extras:
-    extras = {"dev": ["nox", "dev"]}
-    try:
-        for k, v in data["nox"]["extras"].items():
-            extras[k] = v
-    except KeyError:
-        pass
-
-    DEFAULTS["environment-extras"] = extras
-
-    # for py in PYTHON_ALL_VERSIONS:
-    #     print(f"which python{py}", shutil.which(f"python{py}"))
-
-    return
-
-
-load_nox_config()
-
-
-# --- noxopt ---------------------------------------------------------------------------
+# * noxopt -----------------------------------------------------------------------------
 group = NoxOpt(auto_tag=True)
 
 F = TypeVar("F", bound=Callable[..., Any])
+C = Callable[[F], F]
+
+DEFAULT_SESSION = cast(C, group.session(**SESSION_DEFAULT_KWS))  # type: ignore
+ALL_SESSION = cast(C, group.session(**SESSION_ALL_KWS))  # type: ignore
 
-DEFAULT_SESSION = cast(Callable[[F], F], group.session(**SESSION_DEFAULT_KWS))  # type: ignore
-ALL_SESSION = cast(Callable[[F], F], group.session(**SESSION_ALL_KWS))  # type: ignore
+DEFAULT_SESSION_VENV = cast(C, group.session(python=PYTHON_DEFAULT_VERSION))  # type: ignore
+ALL_SESSION_VENV = cast(C, group.session(python=PYTHON_ALL_VERSIONS))  # type: ignore
 
 OPTS_OPT = Option(nargs="*", type=str)
-SET_KERNEL_OPT = Option(type=bool, help="If True, try to set the kernel name")
+# SET_KERNEL_OPT = Option(type=bool, help="If True, try to set the kernel name")
 RUN_OPT = Option(
     nargs="*",
     type=str,
     action="append",
     help="run passed command_demo using `external=True` flag",
 )
 
@@ -135,91 +96,106 @@
 RUN_CLI = Annotated[list[list[str]], RUN_OPT]
 TEST_OPTS_CLI = opts_annotated(help="extra arguments/flags to pytest")
 
 # CMD_CLI = Annotated[list[str], CMD_OPT]
 
 FORCE_REINSTALL_CLI = Annotated[
     bool,
-    Option(type=bool, help="If True, force reinstall even if environment unchanged"),
+    Option(
+        type=bool,
+        help="If True, force reinstall requirements and package even if environment unchanged",
+    ),
 ]
 
 VERSION_CLI = Annotated[
     str, Option(type=str, help="Version to substitute or check against")
 ]
 
 LOG_SESSION_CLI = Annotated[
     bool,
     Option(
         type=bool,
         help="If flag included, log python and package (if installed) version",
     ),
 ]
 
-# --- installer ------------------------------------------------------------------------
 
-
-def install_requirements(
+# * Installation command ---------------------------------------------------------------
+def pkg_install_condaenv(
     session: nox.Session,
     name: str,
-    style: Literal["conda", "conda-lock", "pip"] | None = None,
     lock: bool = False,
     display_name: str | None = None,
-    set_kernel: bool = True,
     install_package: bool = True,
     force_reinstall: bool = False,
     log_session: bool = False,
     deps: Collection[str] | None = None,
     reqs: Collection[str] | None = None,
-    extras: str | Collection[str] | None = None,
     channels: Collection[str] | None = None,
     **kwargs,
 ):
     """Install requirements.  If need fine control, do it in calling func"""
 
-    if display_name is None and set_kernel:
-        display_name = f"{KERNEL_BASE}-{name}"
-
-    style = style or ("conda-lock" if lock else "conda")
-
-    if style == "pip":
-        session_install_pip(
-            session=session,
-            extras=extras,
-            display_name=display_name,
-            force_reinstall=force_reinstall,
-            reqs=reqs,
-            install_package=install_package,
-            **kwargs,
-        )
-
-    elif style == "conda-lock":
+    if lock:
         py = session.python.replace(".", "")  # type: ignore
         session_install_envs_lock(
             session=session,
             lockfile=f"./environment/lock/py{py}-{name}-conda-lock.yml",
             display_name=display_name,
             force_reinstall=force_reinstall,
             install_package=install_package,
             **kwargs,
         )
 
-    elif style == "conda":
+    else:
         session_install_envs(
             session,
             f"./environment/{name}.yaml",
             display_name=display_name,
             force_reinstall=force_reinstall,
             deps=deps,
             reqs=reqs,
             channels=channels,
             install_package=install_package,
             **kwargs,
         )
+
+    if log_session:
+        session_log_session(session, install_package)
+
+
+def pkg_install_venv(
+    session: nox.Session,
+    name: str,
+    lock: bool = False,
+    requirement_paths: Collection[str] | None = None,
+    constraint_paths: Collection[str] | None = None,
+    extras: str | Collection[str] | None = None,
+    reqs: Collection[str] | None = None,
+    display_name: str | None = None,
+    force_reinstall: bool = False,
+    install_package: bool = False,
+    no_deps: bool = False,
+    log_session: bool = False,
+):
+    if lock:
+        raise ValueError("lock not yet supported for install_pip")
+
     else:
-        raise ValueError(f"style={style} not recognized")
+        session_install_pip(
+            session=session,
+            requirement_paths=requirement_paths,
+            constraint_paths=constraint_paths,
+            extras=extras,
+            reqs=reqs,
+            display_name=display_name,
+            force_reinstall=force_reinstall,
+            install_package=install_package,
+            no_deps=no_deps,
+        )
 
     if log_session:
         session_log_session(session, install_package)
 
 
 def session_log_session(session, has_package=False):
     session.run("python", "--version")
@@ -232,47 +208,74 @@
         import {IMPORT_NAME}
         print({IMPORT_NAME}.__version__)
         """
             ),
         )
 
 
+# * Environments------------------------------------------------------------------------
+# ** Development (conda)
 @DEFAULT_SESSION
 def dev(
     session: Session,
-    # set_kernel: SET_KERNEL_CLI = True,
     dev_run: RUN_CLI = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
 ):
     """Create dev env"""
     # using conda
 
-    install_requirements(
+    pkg_install_condaenv(
         session=session,
         name="dev",
         lock=lock,
-        set_kernel=True,
+        display_name=f"{PACKAGE_NAME}-dev",
         install_package=True,
         force_reinstall=force_reinstall,
         log_session=log_session,
     )
     session_run_commands(session, dev_run)
 
 
-@group.session(python=PYTHON_DEFAULT_VERSION)  # type: ignore
+@DEFAULT_SESSION_VENV
+def dev_venv(
+    session: Session,
+    dev_run: RUN_CLI = [],  # noqa
+    lock: LOCK_CLI = False,
+    force_reinstall: FORCE_REINSTALL_CLI = False,
+    log_session: bool = False,
+):
+    """Create dev env"""
+    # using conda
+
+    pkg_install_venv(
+        session=session,
+        name="dev-venv",
+        lock=lock,
+        extras=["dev"],
+        display_name=f"{PACKAGE_NAME}-dev-venv",
+        install_package=True,
+        force_reinstall=force_reinstall,
+        log_session=log_session,
+    )
+    session_run_commands(session, dev_run)
+
+
+# ** pyproject2conda (create environment.yaml and requirement.txt files)
+@DEFAULT_SESSION_VENV
 def pyproject2conda(
     session: Session,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     pyproject2conda_force: bool = False,
 ):
     """Create environment.yaml files from pyproject.toml using pyproject2conda."""
-    session_install_envs(
-        session,
+    pkg_install_venv(
+        session=session,
+        name="pyporject2conda",
         reqs=["pyproject2conda>=0.4.0"],
         force_reinstall=force_reinstall,
     )
 
     def create_env(output, extras=None, python="get", base=True, cmd="yaml"):
         def _to_args(flag, val):
             if val is None:
@@ -295,30 +298,33 @@
             session.log(
                 f"{output} up to data.  Pass --pyproject2conda-force to force recreation"
             )
 
     # create root environment
     create_env("environment/base.yaml")
 
-    extras = DEFAULTS["environment-extras"]
+    extras = CONFIG["environment-extras"]
     for k in ["test", "typing", "docs", "dev"]:
         create_env(f"environment/{k}.yaml", extras=extras.get(k, k), base=True)
 
     # isolated
     for k in ["dist-pypi", "dist-conda"]:
         create_env(f"environment/{k}.yaml", extras=k, base=False)
+        if k == "dist-pypi":
+            create_env(f"environment/{k}.txt", extras=k, base=False, cmd="requirements")
 
     # need an isolated set of test requirements
     create_env("environment/test-extras.yaml", extras="test", base=False)
     create_env(
         "environment/test-extras.txt", extras="test", base=False, cmd="requirements"
     )
 
 
-@DEFAULT_SESSION
+# ** conda-lock
+@DEFAULT_SESSION_VENV
 def conda_lock(
     session: Session,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     conda_lock_channel: cmd_annotated(help="conda channels to use") = (),  # type: ignore
     conda_lock_platform: cmd_annotated(  # type: ignore
         help="platforms to build lock files for",
         choices=["osx-64", "linux-64", "win-64", "all"],
@@ -329,17 +335,17 @@
     ) = (),
     conda_lock_run: RUN_CLI = [],  # noqa
     conda_lock_mamba: bool = False,
     conda_lock_force: bool = False,
 ):
     """Create lock files using conda-lock"""
 
-    session_install_envs(
+    pkg_install_venv(
         session,
-        # reqs=["git+https://github.com/conda/conda-lock.git"],
+        name="conda-lock",
         reqs=["conda-lock>=2.0.0"],
         force_reinstall=force_reinstall,
     )
 
     session.run("conda-lock", "--version")
 
     platform = conda_lock_platform
@@ -407,122 +413,160 @@
         elif c == "dist-conda":
             create_lock(
                 PYTHON_DEFAULT_VERSION,
                 "dist-conda",
             )
 
 
+# ** testing
+def _test(session, run, test_no_pytest, test_opts, no_cov):
+    session_run_commands(session, run)
+    if not test_no_pytest:
+        opts = combine_list_str(test_opts)
+        if not no_cov:
+            session.env["COVERAGE_FILE"] = str(Path(session.create_tmp()) / ".coverage")
+            if "--cov" not in opts:
+                opts.append("--cov")
+        session.run("pytest", *opts)
+
+
 @ALL_SESSION
 def test(
     session: Session,
     test_no_pytest: bool = False,
     test_opts: TEST_OPTS_CLI = (),  # type: ignore
     test_run: RUN_CLI = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
     no_cov: bool = False,
 ):
     """Test environments with conda installs"""
 
-    install_requirements(
+    pkg_install_condaenv(
         session=session,
         name="test",
         lock=lock,
-        set_kernel=False,
         install_package=True,
         force_reinstall=force_reinstall,
         log_session=log_session,
     )
 
-    run = test_run
-    session_run_commands(session, run)
-
-    if not test_no_pytest:
-        opts = combine_list_str(test_opts)
-
-        if not no_cov:
-            session.env["COVERAGE_FILE"] = str(Path(session.create_tmp()) / ".coverage")
-            if "--cov" not in opts:
-                opts.append("--cov")
-        session.run("pytest", *opts)
+    _test(
+        session=session,
+        run=test_run,
+        test_no_pytest=test_no_pytest,
+        test_opts=test_opts,
+        no_cov=no_cov,
+    )
 
 
-@group.session(python=PYTHON_ALL_VERSIONS)  # type: ignore
+@ALL_SESSION_VENV
 def test_venv(
     session: Session,
     test_no_pytest: bool = False,
     test_opts: TEST_OPTS_CLI = (),  # type: ignore
     test_run: RUN_CLI = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
     no_cov: bool = False,
 ):
     """Test environments virtualenv and pip installs"""
 
-    install_requirements(
+    pkg_install_venv(
         session=session,
         name="test-pip",
         extras="test",
         install_package=True,
         force_reinstall=force_reinstall,
         log_session=log_session,
-        style="pip",
     )
 
-    run = test_run
+    _test(
+        session=session,
+        run=test_run,
+        test_no_pytest=test_no_pytest,
+        test_opts=test_opts,
+        no_cov=no_cov,
+    )
+
+
+# ** coverage
+def _coverage(session, run, cmd, run_internal):
     session_run_commands(session, run)
 
-    if not test_no_pytest:
-        opts = combine_list_str(test_opts)
+    if not cmd and not run and not run_internal:
+        cmd = ["combine", "report"]
 
-        if not no_cov:
-            session.env["COVERAGE_FILE"] = str(Path(session.create_tmp()) / ".coverage")
-            if "--cov" not in opts:
-                opts.append("--cov")
-        session.run("pytest", *opts)
+    session.log(f"{cmd}")
+
+    for c in cmd:
+        if c == "combine":
+            paths = list(Path(".nox").glob("test*/tmp/.coverage"))
+            if update_target(".coverage", *paths):
+                session.run("coverage", "combine", "--keep", "-a", *map(str, paths))
+        elif c == "open":
+            open_webpage(path="htmlcov/index.html")
+        else:
+            session.run("coverage", c)
 
+    session_run_commands(session, run_internal, external=False)
 
-@group.session(python=PYTHON_DEFAULT_VERSION)  # type: ignore
+
+@DEFAULT_SESSION_VENV
 def coverage(
     session: Session,
     coverage_cmd: cmd_annotated(  # type: ignore
         choices=["erase", "combine", "report", "html", "open"]
     ) = (),
     coverage_run: RUN_CLI = [],  # noqa
     coverage_run_internal: run_annotated(  # type: ignore
         help="Arbitrary commands to run within the session"
     ) = [],  # noqa
     force_reinstall: FORCE_REINSTALL_CLI = False,
 ):
-    session_install_envs(
+    pkg_install_venv(
         session,
+        name="coverage",
         reqs=["coverage[toml]"],
         force_reinstall=force_reinstall,
     )
-    session_run_commands(session, coverage_run)
 
-    if not coverage_cmd and not coverage_run and not coverage_run_internal:
-        coverage_cmd = ["combine", "report"]
+    _coverage(
+        session=session,
+        run=coverage_run,
+        cmd=coverage_cmd,
+        run_internal=coverage_run_internal,
+    )
 
-    session.log(f"{coverage_cmd}")
 
-    for cmd in coverage_cmd:
-        if cmd == "combine":
-            paths = list(Path(".nox").glob("test*/tmp/.coverage"))
-            if update_target(".coverage", *paths):
-                session.run("coverage", "combine", "--keep", "-a", *map(str, paths))
-        elif cmd == "open":
-            _open_webpage(path="htmlcov/index.html")
+# ** Docs
+def _docs(session, run, cmd, version):
+    if version:
+        session.env["SETUPTOOLS_SCM_PRETEND_VERSION"] = version
 
-        else:
-            session.run("coverage", cmd)
+    session_run_commands(session, run)
 
-    session_run_commands(session, coverage_run_internal, external=False)
+    if not run and not cmd:
+        cmd = ["html"]
+
+    if "symlink" in cmd:
+        cmd.remove("symlink")
+        _create_doc_examples_symlinks(session)
+
+    if open_page := "open" in cmd:
+        cmd.remove("open")
+
+    if cmd:
+        args = ["make", "-C", "docs"] + combine_list_str(cmd)
+        session.run(*args, external=True)
+
+    if open_page:
+        open_webpage(path="./docs/_build/html/index.html")
 
 
 @DEFAULT_SESSION
 def docs(
     session: nox.Session,
     docs_cmd: cmd_annotated(  # type: ignore
         choices=[
@@ -542,87 +586,73 @@
     docs_run: RUN_CLI = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     version: VERSION_CLI = "",
     log_session: bool = False,
 ):
     """Runs make in docs directory. For example, 'nox -s docs -- --docs-cmd html' -> 'make -C docs html'. With 'release' option, you can set the message with 'message=...' in posargs."""
-    install_requirements(
+    pkg_install_condaenv(
         session=session,
         name="docs",
         lock=lock,
-        set_kernel=True,
+        display_name=f"{PACKAGE_NAME}-docs",
         install_package=True,
         force_reinstall=force_reinstall,
         log_session=log_session,
     )
 
-    if version:
-        session.env["SETUPTOOLS_SCM_PRETEND_VERSION"] = version
-
-    cmd = docs_cmd
-    run = docs_run
-
-    session_run_commands(session, run)
-
-    if not run and not cmd:
-        cmd = ["html"]
-
-    if "symlink" in cmd:
-        cmd.remove("symlink")
-        _create_doc_examples_symlinks(session)
-
-    if open_page := "open" in cmd:
-        cmd.remove("open")
-
-    if cmd:
-        args = ["make", "-C", "docs"] + combine_list_str(cmd)
-        # if version:
-        #     args.append( f"SETUPTOOLS_SCM_PRETEND_VERSION={version}" )
-        session.run(*args, external=True)
-
-    if open_page:
-        _open_webpage(path="./docs/_build/html/index.html")
+    _docs(session=session, cmd=docs_cmd, run=docs_run, version=version)
 
 
-@DEFAULT_SESSION
-def dist_pypi(
+@DEFAULT_SESSION_VENV
+def docs_venv(
     session: nox.Session,
-    dist_pypi_run: RUN_CLI = [],  # noqa
-    dist_pypi_cmd: cmd_annotated(  # type: ignore
-        choices=["clean", "build", "testrelease", "release"],
-        flags=("--dist-pypi-cmd", "-p"),
+    docs_cmd: cmd_annotated(  # type: ignore
+        choices=[
+            "html",
+            "build",
+            "symlink",
+            "clean",
+            "livehtml",
+            "linkcheck",
+            "spelling",
+            "showlinks",
+            "release",
+            "open",
+        ],
+        flags=("--docs-cmd", "-d"),
     ) = (),
+    docs_run: RUN_CLI = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     version: VERSION_CLI = "",
     log_session: bool = False,
 ):
-    """Run 'nox -s dist_pypi -- {clean, build, testrelease, release}'"""
-    # conda
-
-    install_requirements(
+    """Runs make in docs directory. For example, 'nox -s docs -- --docs-cmd html' -> 'make -C docs html'. With 'release' option, you can set the message with 'message=...' in posargs."""
+    pkg_install_venv(
         session=session,
-        name="dist-pypi",
-        set_kernel=False,
-        install_package=False,
+        name="docs-venv",
+        lock=lock,
+        display_name=f"{PACKAGE_NAME}-docs-venv",
+        install_package=True,
         force_reinstall=force_reinstall,
         log_session=log_session,
+        extras="docs",
     )
 
-    if version:
-        session.env["SETUPTOOLS_SCM_PRETEND_VERSION"] = version
+    _docs(session=session, cmd=docs_cmd, run=docs_run, version=version)
 
-    run, cmd = dist_pypi_run, dist_pypi_cmd
 
+# ** Dist pypi
+def _dist_pypi(session, run, cmd, version):
+    if version:
+        session.env["SETUPTOOLS_SCM_PRETEND_VERSION"] = version
     session_run_commands(session, run)
-
     if not run and not cmd:
         cmd = ["build"]
-
     if cmd:
         if "build" in cmd:
             cmd.append("clean")
         cmd = sort_like(cmd, ["clean", "build", "testrelease", "release"])
 
         session.log(f"cmd={cmd}")
 
@@ -635,14 +665,78 @@
             elif command == "testrelease":
                 session.run("twine", "upload", "--repository", "testpypi", "dist/*")
 
             elif command == "release":
                 session.run("twine", "upload", "dist/*")
 
 
+@DEFAULT_SESSION_VENV
+def dist_pypi(
+    session: nox.Session,
+    dist_pypi_run: RUN_CLI = [],  # noqa
+    dist_pypi_cmd: cmd_annotated(  # type: ignore
+        choices=["clean", "build", "testrelease", "release"],
+        flags=("--dist-pypi-cmd", "-p"),
+    ) = (),
+    lock: LOCK_CLI = False,
+    force_reinstall: FORCE_REINSTALL_CLI = False,
+    version: VERSION_CLI = "",
+    log_session: bool = False,
+):
+    """Run 'nox -s dist-pypi -- {clean, build, testrelease, release}'"""
+
+    pkg_install_venv(
+        session=session,
+        name="dist-pypi",
+        requirement_paths=["environment/dist-pypi.txt"],
+        force_reinstall=force_reinstall,
+        install_package=False,
+    )
+
+    _dist_pypi(
+        session=session,
+        run=dist_pypi_run,
+        cmd=dist_pypi_cmd,
+        version=version,
+    )
+
+
+@DEFAULT_SESSION
+def dist_pypi_condaenv(
+    session: nox.Session,
+    dist_pypi_run: RUN_CLI = [],  # noqa
+    dist_pypi_cmd: cmd_annotated(  # type: ignore
+        choices=["clean", "build", "testrelease", "release"],
+        flags=("--dist-pypi-cmd", "-p"),
+    ) = (),
+    lock: LOCK_CLI = False,
+    force_reinstall: FORCE_REINSTALL_CLI = False,
+    version: VERSION_CLI = "",
+    log_session: bool = False,
+):
+    """Run 'nox -s dist_pypi -- {clean, build, testrelease, release}'"""
+    # conda
+
+    pkg_install_condaenv(
+        session=session,
+        name="dist-pypi",
+        install_package=False,
+        force_reinstall=force_reinstall,
+        log_session=log_session,
+    )
+
+    _dist_pypi(
+        session=session,
+        run=dist_pypi_run,
+        cmd=dist_pypi_cmd,
+        version=version,
+    )
+
+
+# ** Dist conda
 @DEFAULT_SESSION
 def dist_conda(
     session: nox.Session,
     dist_conda_run: RUN_CLI = [],  # noqa
     dist_conda_cmd: cmd_annotated(  # type: ignore
         choices=[
             "recipe",
@@ -650,25 +744,24 @@
             "clean",
             "clean-recipe",
             "clean-build",
             "recipe-cat-full",
         ],
         flags=("--dist-conda-cmd", "-c"),
     ) = (),
-    lock: LOCK_CLI = False,
+    # lock: LOCK_CLI = False,
     sdist_path: str = "",
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
     version: VERSION_CLI = "",
 ):
     """Runs make -C dist-conda posargs"""
-    install_requirements(
+    pkg_install_condaenv(
         session=session,
         name="dist-conda",
-        set_kernel=False,
         install_package=False,
         force_reinstall=force_reinstall,
         log_session=log_session,
     )
 
     run, cmd = dist_conda_run, dist_conda_cmd
     session_run_commands(session, run)
@@ -749,14 +842,29 @@
     with open(append_path) as f:
         append = f.readlines()
 
     with open(recipe_path, "w") as f:
         f.writelines(recipe + ["\n"] + append)
 
 
+# type checking
+def _typing(session, run, cmd, run_internal):
+    session_run_commands(session, run)
+    if not run and not run_internal and not cmd:
+        cmd = ["mypy"]
+    for c in cmd:
+        if c == "mypy":
+            session.run("mypy", "--color-output")
+        elif c == "pyright":
+            session.run("pyright", external=True)
+        elif c == "pytype":
+            session.run("pytype")
+    session_run_commands(session, run_internal, external=False)
+
+
 @ALL_SESSION
 def typing(
     session: nox.Session,
     typing_cmd: cmd_annotated(  # type: ignore
         choices=["mypy", "pyright", "pytype"],
         flags=("--typing-cmd", "-m"),
     ) = (),
@@ -766,42 +874,67 @@
     ) = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
 ):
     """Run type checkers (mypy, pyright, pytype)"""
 
-    install_requirements(
+    pkg_install_condaenv(
         session=session,
         name="typing",
         lock=lock,
-        set_kernel=False,
         install_package=True,
         force_reinstall=force_reinstall,
         log_session=log_session,
     )
 
-    run, cmd = typing_run, typing_cmd
+    _typing(
+        session=session,
+        run=typing_run,
+        cmd=typing_cmd,
+        run_internal=typing_run_internal,
+    )
 
-    session_run_commands(session, run)
 
-    if not run and not typing_run_internal and not cmd:
-        cmd = ["mypy"]
+@ALL_SESSION_VENV
+def typing_venv(
+    session: nox.Session,
+    typing_cmd: cmd_annotated(  # type: ignore
+        choices=["mypy", "pyright", "pytype"],
+        flags=("--typing-cmd", "-m"),
+    ) = (),
+    typing_run: RUN_CLI = [],  # noqa
+    typing_run_internal: run_annotated(  # type: ignore
+        help="run arbitrary (internal) commands.  For example, --typing-run-internal 'mypy --some-option'",
+    ) = [],  # noqa
+    lock: LOCK_CLI = False,
+    force_reinstall: FORCE_REINSTALL_CLI = False,
+    log_session: bool = False,
+):
+    """Run type checkers (mypy, pyright, pytype)"""
 
-    for c in cmd:
-        if c == "mypy":
-            session.run("mypy", "--color-output")
-        elif c == "pyright":
-            session.run("pyright", external=True)
-        elif c == "pytype":
-            session.run("pytype")
+    pkg_install_venv(
+        session=session,
+        name="typing",
+        lock=lock,
+        install_package=True,
+        force_reinstall=force_reinstall,
+        log_session=log_session,
+        extras="typing",
+    )
 
-    session_run_commands(session, typing_run_internal, external=False)
+    _typing(
+        session=session,
+        run=typing_run,
+        cmd=typing_cmd,
+        run_internal=typing_run_internal,
+    )
 
 
+# ** testdist conda
 @ALL_SESSION
 def testdist_conda(
     session: Session,
     test_no_pytest: bool = False,
     test_opts: TEST_OPTS_CLI = (),  # type: ignore
     testdist_conda_run: RUN_CLI = [],  # noqa
     force_reinstall: FORCE_REINSTALL_CLI = False,
@@ -816,27 +949,29 @@
 
     session_install_envs(
         session,
         "environment/test-extras.yaml",
         deps=[install_str],
         channels=["conda-forge"],
         force_reinstall=force_reinstall,
+        install_package=False,
     )
 
     if log_session:
         session_log_session(session, False)
 
     session_run_commands(session, testdist_conda_run)
 
     if not test_no_pytest:
         opts = combine_list_str(test_opts)
         session.run("pytest", *opts)
 
 
-@ALL_SESSION
+# ** testdist pypi
+@ALL_SESSION_VENV
 def testdist_pypi(
     session: Session,
     test_no_pytest: bool = False,
     test_opts: TEST_OPTS_CLI = (),  # type: ignore
     testdist_pypi_run: RUN_CLI = [],  # noqa
     testdist_pypi_extras: cmd_annotated(help="extras to install") = (),  # type: ignore
     force_reinstall: FORCE_REINSTALL_CLI = False,
@@ -849,33 +984,37 @@
 
     if extras:
         install_str = "{}[{}]".format(install_str, ",".join(extras))
 
     if version:
         install_str = f"{install_str}=={version}"
 
-    session_install_envs(
-        session,
-        "environment/test-extras.yaml",
+    pkg_install_venv(
+        session=session,
+        name="testdist-pypi",
+        requirement_paths=["environment/test-extras.txt"],
         reqs=[install_str],
-        channels=["conda-forge"],
         force_reinstall=force_reinstall,
+        install_package=False,
     )
 
     if log_session:
         session_log_session(session, False)
 
-    session_run_commands(session, testdist_pypi_run)
-    if not test_no_pytest:
-        opts = combine_list_str(test_opts)
-        session.run("pytest", *opts)
+    _test(
+        session=session,
+        run=testdist_pypi_run,
+        test_no_pytest=test_no_pytest,
+        test_opts=test_opts,
+        no_cov=True,
+    )
 
 
-@group.session(python=PYTHON_ALL_VERSIONS)  # type: ignore
-def testdist_pypi_venv(
+@ALL_SESSION
+def testdist_pypi_condaenv(
     session: Session,
     test_no_pytest: bool = False,
     test_opts: TEST_OPTS_CLI = (),  # type: ignore
     testdist_pypi_run: RUN_CLI = [],  # noqa
     testdist_pypi_extras: cmd_annotated(help="extras to install") = (),  # type: ignore
     force_reinstall: FORCE_REINSTALL_CLI = False,
     version: VERSION_CLI = "",
@@ -887,34 +1026,35 @@
 
     if extras:
         install_str = "{}[{}]".format(install_str, ",".join(extras))
 
     if version:
         install_str = f"{install_str}=={version}"
 
-    install_requirements(
-        session=session,
-        name="testdist-pypi-venv",
-        set_kernel=False,
-        install_package=False,
+    session_install_envs(
+        session,
+        "environment/test-extras.yaml",
+        reqs=[install_str],
+        channels=["conda-forge"],
         force_reinstall=force_reinstall,
-        style="pip",
-        reqs=["-r", "environment/test-extras.txt", install_str],
+        install_package=False,
     )
-
     if log_session:
         session_log_session(session, False)
 
-    session_run_commands(session, testdist_pypi_run)
-    if not test_no_pytest:
-        opts = combine_list_str(test_opts)
-        session.run("pytest", *opts)
+    _test(
+        session=session,
+        run=testdist_pypi_run,
+        test_no_pytest=test_no_pytest,
+        test_opts=test_opts,
+        no_cov=True,
+    )
 
 
-# --- Utilities ------------------------------------------------------------------------
+# * Utilities --------------------------------------------------------------------------
 def _create_doc_examples_symlinks(session, clean=True):
     """Create symlinks from docs/examples/*.md files to /examples/usage/..."""
 
     import os
 
     def usage_paths(path):
         with path.open("r") as f:
@@ -957,71 +1097,37 @@
 
             target_rel = os.path.relpath(target, start=link.parent)
             session.log(f"linking {target_rel} -> {link}")
 
             os.symlink(target_rel, link)
 
 
-def _open_webpage(path=None, url=None):
-    import webbrowser
-    from urllib.request import pathname2url
-
-    if path:
-        url = "file://" + pathname2url(str(Path(path).absolute()))
-    if url:
-        webbrowser.open(url)
-
-
-# @group.session(python=PYTHON_DEFAULT_VERSION)
-# def conda_merge(
+# # If want seperate env for updating/reporting version with setuptools-scm
+# # We do this from dev environment.
+# # ** version report/update
+# @DEFAULT_SESSION_VENV
+# def version_scm(
 #     session: Session,
-#     conda_merge_force: bool = False,
+#     version: VERSION_CLI = "",
 #     force_reinstall: FORCE_REINSTALL_CLI = False,
 # ):
-#     """Merge environments using conda-merge."""
-#     import tempfile
-#     session_install_envs(
-#         session,
-#         reqs=["conda-merge", "ruamel.yaml"],
+#     """
+#     Get current version from setuptools-scm
+
+#     Note that the version of editable installs can get stale.
+#     This will show the actual current version.
+#     Avoids need to include setuptools-scm in develop/docs/etc.
+#     """
+
+#     pkg_install_venv(
+#         session=session,
+#         name="version-scm",
+#         install_package=True,
+#         reqs=["setuptools_scm"],
 #         force_reinstall=force_reinstall,
+#         no_deps=True,
 #     )
 
-#     env_base = ROOT / "environment.yaml"
-#     env_dir = ROOT / "environment"
-
-#     def create_env(*extras, others=None, name=None, base=True):
-#         if name is None:
-#             name = extras[0]
-#         env = env_dir / f"{name}.yaml"
-
-#         deps = []
-#         if base:
-#             deps.append(str(env_base))
-#         for extra in extras:
-#             deps.append(str(env_dir / f"{extra}-extras.yaml"))
-
-#         if conda_merge_force or update_target(env, *deps):
-#             session.log(f"creating {env}")
-
-#             args = ["conda-merge"] + deps
-#             with tempfile.TemporaryDirectory() as d:
-#                 tmp_path = Path(d) / "tmp_env.yaml"
-
-#                 with tmp_path.open("w") as f:
-#                     session.run(*args, stdout=f)
-
-#                 run_str = dedent(
-#                     f"""
-#                 from ruamel.yaml import YAML; from pathlib import Path;
-#                 pin, pout = Path("{tmp_path}"), Path("{env}")
-#                 y = YAML(); y.indent(mapping=2, sequence=4, offset=2)
-#                 y.dump(y.load(pin.open("r")), pout.open("w"))
-#                 """
-#                 )
-
-#                 session.run("python", "-c", run_str, silent=True)
-
-#     for extra in ["test", "docs"]:
-#         create_env(extra, base=True)
+#     if version:
+#         session.env["SETUPTOOLS_SCM_PRETEND_VERSION"] = version
 
-#     create_env("test", "typing", name="typing", base=True)
-#     create_env("dev", "test", "typing", "nox", name="dev", base=True)
+#     session.run("python", "-m", "setuptools_scm")
```

### Comparing `module-utilities-0.4.0/pyproject.toml` & `module-utilities-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 test = [
     "pytest", #
     "pytest-xdist",
     "pytest-cov",
     "pytest-sugar",
 ]
 dev-extras = [
+    "setuptools-scm", #
     "pytest-accept", # p2c: -p
-    "setuptools-scm",
     "ipython",
     "ipykernel",
 ]
 typing-extras = [
     # "pytype; python_version < '3.11'",
     "mypy",
 ]
@@ -69,19 +69,18 @@
 ]
 dev-complete = [
     "module-utilities[dev]", #
     "module-utilities[tools]",
     "module-utilities[nox]",
 ]
 docs = [
-    "setuptools-scm", #
-    "ipython",
+    "ipython", #
     "pyenchant",
     "ghp-import",
-    "sphinx",
+    "sphinx>=5.3.0",
     "sphinx-copybutton",
     "sphinxcontrib-spelling",
     "sphinx-autobuild",
     "myst-nb",
     "sphinx-book-theme",
     "autodocsumm",
 ]
@@ -89,15 +88,14 @@
 dist-pypi = ["twine", "build"]
 dist-conda = [
     "anaconda-client", #
     "grayskull",
     "conda-build",
     "conda-verify",
     "boa",
-    "setuptools-scm",
 ]
 
 [tool.pyproject2conda]
 channels = ["conda-forge"]
 
 ## grayskull still messes some things up, but use scripts/recipe-append.sh for this
 [tool.setuptools]
@@ -116,32 +114,32 @@
     "README.md",
     "CHANGELOG.md",
     "LICENSE"
 ], content-type = "text/markdown" }
 
 [tool.setuptools_scm]
 fallback_version = "999"
+write_to = "src/module_utilities/_version.py"
 
 [tool.aliases]
 test = "pytest"
 
 [tool.pytest.ini_options]
-addopts = "--doctest-modules --doctest-glob='*.md'"
+addopts = "-n 4 --doctest-modules --doctest-glob='*.md'"
 # testpaths = ["src/module_utilities", "tests", "./README.md"]
 testpaths = ["src", "tests", "README.md"]
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 known_first_party = ["module_utilities"]
 
 [tool.ruff]
 fix = true
 line-length = 88
-update-check = false
 target-version = "py38"
 select = [
     # pyflakes
     "F",
     # pycodestyle
     "E",
     "W",
@@ -150,19 +148,21 @@
     # pyupgrade
     "UP",
     # pydocstyle
     "D",
     # # flake8-2020
     "YTT",
     # # flake8-bugbear
-    # "B",
+    "B",
     # flake8-quotes
     "Q",
     # # pylint
     # "PLE", "PLR", "PLW",
+    "PLE",
+    "PLW",
     # # misc lints
     "PIE",
     # # tidy imports
     "TID",
     # # implicit string concatenation
     # "ISC",
     # # type-checking imports
@@ -303,16 +303,17 @@
 module = ["module_utilities.vendored.docscrape"]
 
 [tool.pyright]
 include = ["src", "tests"]
 exclude = [
     "**/__pycache__",
     ".tox/**",
+    ".nox/**",
     "**/.mypy_cache",
-    "src/module-utilities/vendored"
+    "src/module_utilities/vendored"
 ]
 pythonVersion = "3.10"
 typeCheckingMode = "basic"
 # enable subset of "strict"
 reportDuplicateImport = true
 reportInvalidStubStatement = true
 reportOverlappingOverload = true
```

### Comparing `module-utilities-0.4.0/src/module_utilities/_doc.py` & `module-utilities-0.5.0/src/module_utilities/_doc.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,48 +10,63 @@
 from textwrap import dedent
 from typing import TYPE_CHECKING, Callable
 
 if TYPE_CHECKING:
     from ._typing import F
 
 
-def doc(*docstrings: None | str | Callable, **params) -> Callable[[F], F]:
+def doc(
+    *docstrings: None | str | Callable, _prepend: bool = False, **params
+) -> Callable[[F], F]:
     """
     A decorator to take docstring templates, concatenate them and perform string
     substitution on them.
     This decorator will add a variable "_docstring_components" to the wrapped
     callable to keep track the original docstring template for potential usage.
     If it should be consider as a template, it will be saved as a string.
     Otherwise, it will be saved as callable, and later user __doc__ and dedent
     to get docstring.
 
     Parameters
     ----------
     *docstrings : None, str, or callable
         The string / docstring / docstring template to be appended in order
         after default docstring under callable.
+    _prepend : bool, default=False
+        If True, prepend decorated function docstring.  Otherwise, append to end.
     **params
         The string which would be used to format docstring template.
+
     """
 
     def decorator(decorated: F) -> F:
         # collecting docstring and docstring templates
         docstring_components: list[str | Callable] = []
-        if decorated.__doc__:
-            docstring_components.append(dedent(decorated.__doc__))
+        # if decorated.__doc__:
+        #     docstring_components.append(dedent(decorated.__doc__))
 
         for docstring in docstrings:
             if docstring is None:
                 continue
             if hasattr(docstring, "_docstring_components"):
                 docstring_components.extend(
                     docstring._docstring_components  # pyright: ignore[reportGeneralTypeIssues] # noqa: E501
                 )
-            elif isinstance(docstring, str) or docstring.__doc__:
+            elif isinstance(docstring, str):
                 docstring_components.append(docstring)
+            elif docstring.__doc__:
+                # docstring_components.append(docstring)
+                docstring_components.append(dedent(docstring.__doc__ or ""))
+
+        # make default to append
+        if decorated.__doc__:
+            if _prepend:
+                docstring_components.insert(0, dedent(decorated.__doc__))
+            else:
+                docstring_components.append(dedent(decorated.__doc__))
 
         params_applied = [
             # component.format(**params)
             component.format_map(params)
             if isinstance(component, str) and len(params) > 0
             else component
             for component in docstring_components
```

### Comparing `module-utilities-0.4.0/src/module_utilities/attributedict.py` & `module-utilities-0.5.0/src/module_utilities/attributedict.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/src/module_utilities/cached.py` & `module-utilities-0.5.0/src/module_utilities/cached.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/src/module_utilities/docfiller.py` & `module-utilities-0.5.0/src/module_utilities/docfiller.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,17 @@
         "false",
     )
 except KeyError:
     DOC_SUB = True
 
 
 # Factory method to create doc_decorate
-def doc_decorate(*docstrings: str | Callable, **params) -> Callable[[F], F]:
+def doc_decorate(
+    *docstrings: str | Callable, _prepend: bool = False, **params
+) -> Callable[[F], F]:
     """
     A decorator take docstring templates, concatenate them and perform string
     substitution on it.
 
     This decorator will add a variable "_docstring_components" to the wrapped
     callable to keep track the original docstring template for potential usage.
     If it should be consider as a template, it will be saved as a string.
@@ -45,25 +47,27 @@
     to get docstring
 
     Parameters
     ----------
     *docstrings : str or callable
         The string / docstring / docstring template to be appended in order
         after default docstring under callable.
+    _prepend : bool, default=False
+        If True, prepend decorated function docstring.  Otherwise, append to end.
     **params
         The string which would be used to format docstring template.
 
     Notes
     -----
     Doc filling can be turned off by setting the environment variable
     ``DOCFILLER_SUB`` to one of ``0, f, false``.
     """
 
     if DOC_SUB:
-        return _pd_doc(*docstrings, **params)
+        return _pd_doc(*docstrings, _prepend=_prepend, **params)
     else:
 
         def decorated(func):
             return func
 
         return decorated
 
@@ -387,15 +391,15 @@
 
         return new
 
     def assign_param(
         self,
         name: str,
         ptype: str = "",
-        desc: str | list[str] = [],
+        desc: str | list[str] | None = None,
         key: str | None = None,
     ):
         """
         Add in a new parameter
 
         Parameters
         ----------
@@ -428,16 +432,18 @@
         x : float
             A parameter
             with multiple levels
         """
 
         new = self.new_like()
 
-        # cleanup desc
-        if isinstance(desc, str):
+        if desc is None:
+            desc = []
+        elif isinstance(desc, str):
+            # cleanup desc
             desc = dedent(desc).strip().split("\n")
 
         key = name if key is None else key
 
         new.data[key] = _build_param_docstring(name=name, ptype=ptype, desc=desc)
 
         return new
@@ -562,15 +568,17 @@
         """
         Default decorator.
 
         This uses `self.params` and the decorated funciton docstring as a template.
         """
         return self._default_decorator(func)  # type: ignore
 
-    def __call__(self, *templates: Callable | str, **params) -> Callable[[F], F]:
+    def __call__(
+        self, *templates: Callable | str, _prepend: bool = False, **params
+    ) -> Callable[[F], F]:
         """
         General decorator.
 
         This should always be used in a callable manner.
 
         If want to call without any parameter use decorate()
 
@@ -579,20 +587,20 @@
         *templates : callable
             docstrings to be used as templates.
         **params
             Extra parameters to be substituted.
         """
         ntemplates, nparams = len(templates), len(params)
 
-        if ntemplates == nparams == 0:
+        if ntemplates == nparams == 0 and not _prepend:
             return self.decorate
         elif nparams == 0:
-            return doc_decorate(*templates, **self.params)
+            return doc_decorate(*templates, _prepend=_prepend, **self.params)
         else:
-            return self.update(params)(*templates)
+            return self.update(params)(*templates, _prepend=_prepend)
 
     # NOTE: This is dangerous.
     # if you pass a function as a template, but forget to explicitly pass it,
     # you overwrite the docstring for that function.  Just really confusing
     # def dec(self, *funcs, docstrings=None, **params) -> Callable[[F], F]:
     #     """
     #     General decorator.
```

### Comparing `module-utilities-0.4.0/src/module_utilities/vendored/LICENSE.txt` & `module-utilities-0.5.0/src/module_utilities/vendored/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/src/module_utilities/vendored/docscrape.py` & `module-utilities-0.5.0/src/module_utilities/vendored/docscrape.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/src/module_utilities.egg-info/PKG-INFO` & `module-utilities-0.5.0/src/module_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-utilities
-Version: 0.4.0
+Version: 0.5.0
 Summary: Collection of utilities to aid working with python modules.
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/module-utilities
 Project-URL: documentation, https://pages.nist.gov/module-utilities/
 Keywords: module-utilities
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -301,14 +301,21 @@
 ## Unreleased
 
 See the fragment files in
 [changelog.d](https://github.com/usnistgov/module-utilities)
 
 <!-- scriv-insert-here -->
 
+## v0.5.0 — 2023-07-10
+
+### Added
+
+- Add `_prepend` option to docfiller. Default behavior is now to append current
+  docstring to templates.
+
 ## v0.4.0 — 2023-06-14
 
 ### Added
 
 - Package now available on conda-forge
 
 ### Changed
```

### Comparing `module-utilities-0.4.0/src/module_utilities.egg-info/SOURCES.txt` & `module-utilities-0.5.0/src/module_utilities.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -52,31 +52,44 @@
 docs/examples/index.md
 docs/examples/usage/cached.ipynb
 docs/examples/usage/docfiller.ipynb
 docs/reference/index.md
 environment/base.yaml
 environment/dev.yaml
 environment/dist-conda.yaml
+environment/dist-pypi.txt
 environment/dist-pypi.yaml
 environment/docs.yaml
 environment/lint.yaml
 environment/test-extras.txt
 environment/test-extras.yaml
 environment/test.yaml
 environment/typing.yaml
+environment/lock/py310-dev-conda-lock.yml
+environment/lock/py310-dist-conda-conda-lock.yml
+environment/lock/py310-dist-pypi-conda-lock.yml
+environment/lock/py310-test-conda-lock.yml
+environment/lock/py310-typing-conda-lock.yml
 environment/lock/py310.yaml
+environment/lock/py311-test-conda-lock.yml
+environment/lock/py311-typing-conda-lock.yml
 environment/lock/py311.yaml
+environment/lock/py38-test-conda-lock.yml
+environment/lock/py38-typing-conda-lock.yml
 environment/lock/py38.yaml
+environment/lock/py39-test-conda-lock.yml
+environment/lock/py39-typing-conda-lock.yml
 environment/lock/py39.yaml
 examples/README.md
 examples/usage/cached.ipynb
 examples/usage/docfiller.ipynb
 src/module_utilities/__init__.py
 src/module_utilities/_doc.py
 src/module_utilities/_typing.py
+src/module_utilities/_version.py
 src/module_utilities/attributedict.py
 src/module_utilities/cached.py
 src/module_utilities/docfiller.py
 src/module_utilities/py.typed
 src/module_utilities.egg-info/PKG-INFO
 src/module_utilities.egg-info/SOURCES.txt
 src/module_utilities.egg-info/dependency_links.txt
```

### Comparing `module-utilities-0.4.0/src/module_utilities.egg-info/requires.txt` & `module-utilities-0.5.0/src/module_utilities.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -7,37 +7,35 @@
 
 [dev-complete]
 module-utilities[dev]
 module-utilities[tools]
 module-utilities[nox]
 
 [dev-extras]
-pytest-accept
 setuptools-scm
+pytest-accept
 ipython
 ipykernel
 
 [dist-conda]
 anaconda-client
 grayskull
 conda-build
 conda-verify
 boa
-setuptools-scm
 
 [dist-pypi]
 twine
 build
 
 [docs]
-setuptools-scm
 ipython
 pyenchant
 ghp-import
-sphinx
+sphinx>=5.3.0
 sphinx-copybutton
 sphinxcontrib-spelling
 sphinx-autobuild
 myst-nb
 sphinx-book-theme
 autodocsumm
```

### Comparing `module-utilities-0.4.0/tests/test_cached.py` & `module-utilities-0.5.0/tests/test_cached.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.4.0/tests/test_docfiller.py` & `module-utilities-0.5.0/tests/test_docfiller.py`

 * *Files 11% similar despite different names*

```diff
@@ -545,7 +545,86 @@
     assert hello.__doc__ == expected
 
     @d(hello)
     class hello2(hello):
         pass
 
     assert hello.__doc__ == expected
+
+
+def test_prepend():
+    expected = """
+    A summary
+
+    A longer summary
+
+    Parameters
+    ----------
+    x : float
+        x param
+        some other stuff
+    y : float
+        y param
+
+    Returns
+    -------
+    out : float
+        output
+    """
+
+    expected = dedent(expected)
+
+    d = DocFiller.from_docstring(expected, combine_keys="parameters")
+
+    def template():
+        """
+        {summary}
+
+        {extended_summary}
+
+        Parameters
+        ----------
+        {x}
+        {y}
+        """
+
+    @d(template)
+    def hello():
+        """
+        Returns
+        -------
+        {returns.out}
+        """
+        pass
+
+    assert hello.__doc__ == expected
+
+    # prepend
+    @d(template, _prepend=True)
+    def there():
+        """
+        Returns
+        -------
+        {returns.out}
+        """
+        pass
+
+    expected = """
+    Returns
+    -------
+    out : float
+        output
+
+    A summary
+
+    A longer summary
+
+    Parameters
+    ----------
+    x : float
+        x param
+        some other stuff
+    y : float
+        y param
+    """
+
+    assert dedent(expected) == there.__doc__
```

### Comparing `module-utilities-0.4.0/tools/noxtools.py` & `module-utilities-0.5.0/tools/noxtools.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Utilities to work with nox"""
 
 from __future__ import annotations
 
 import shlex
-import tempfile
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Iterable, Literal, cast
 
 from ruamel.yaml import safe_load
 
 if TYPE_CHECKING:
     from collections.abc import Collection, Sequence
@@ -32,17 +31,15 @@
     # only unique
     sorter = {k: i for i, k in enumerate(like)}
     return sorted(set(values), key=lambda k: sorter[k])
 
 
 def update_target(target: str | Path, *deps: str | Path) -> bool:
     """Check if target is older than deps:"""
-
     target_path = Path(target)
-
     deps_path = tuple(map(Path, deps))
 
     for d in deps_path:
         if not d.exists():
             raise ValueError(f"dependency {d} does not exist")
 
     if not target_path.exists():
@@ -66,14 +63,87 @@
 
     if len(args) == 1 and not isinstance(args[0], str):
         args = args[0]
 
     return sum([[flag, _] for _ in args], [])
 
 
+def open_webpage(path: str | Path | None = None, url: str | None = None):
+    """
+    Open webpage from path or url.
+
+    Useful if want to view webpage with javascript, etc., as well as static html.
+    """
+    import webbrowser
+    from urllib.request import pathname2url
+
+    if path:
+        url = "file://" + pathname2url(str(Path(path).absolute()))
+    if url:
+        webbrowser.open(url)
+
+
+# --- Load user configuration ----------------------------------------------------------
+def load_nox_config(path: str | Path = "./.noxconfig.toml") -> dict[str, Any]:
+    """
+    Load user toml config file.
+
+    File should look something like:
+
+    [nox.python]
+    paths = ["~/.conda/envs/test-3.*/bin"]
+
+    # Extras for environments
+    # for example, could have
+    # dev = ["dev", "nox", "tools"]
+    [nox.extras]
+    dev = ["dev", "nox"]
+
+    """
+    import os
+    from glob import glob
+
+    import tomli
+
+    config = {}
+
+    path = Path(path)
+    if not path.exists():
+        return config
+
+    with path.open("rb") as f:
+        data = tomli.load(f)
+
+    # Python paths
+    try:
+        paths = []
+        for p in data["nox"]["python"]["paths"]:
+            paths.extend(glob(os.path.expanduser(p)))
+
+        paths_str = ":".join(map(str, paths))
+        os.environ["PATH"] = paths_str + ":" + os.environ["PATH"]
+    except KeyError:
+        pass
+
+    # extras:
+    extras = {"dev": ["nox", "dev"]}
+    try:
+        for k, v in data["nox"]["extras"].items():
+            extras[k] = v
+    except KeyError:
+        pass
+
+    config["environment-extras"] = extras
+
+    # for py in PYTHON_ALL_VERSIONS:
+    #     print(f"which python{py}", shutil.which(f"python{py}"))
+
+    return config
+
+
 # --- Nox session utilities ------------------------------------------------------------
 def session_skip_install(session: nox.Session) -> bool:
     """
     Utility to check if we're skipping install and reusing existing venv
     This is a hack and may need to change if upstream changes.
     """
     return session._runner.global_config.no_install and session._runner.venv._reused  # type: ignore
@@ -125,16 +195,14 @@
     if no_deps:
         command.append("--no-deps")
 
     session.install(*command, *args, **kwargs)
 
 
 # --- Create env from lock -------------------------------------------------------------
-
-
 def session_install_envs_lock(
     session: nox.Session,
     lockfile: str | Path,
     extras: str | list[str] | None = None,
     display_name: str | None = None,
     force_reinstall: bool = False,
     install_package: bool = False,
@@ -176,16 +244,14 @@
 
     write_hashfile(hashes, session=session, prefix="lock")
 
     return unchanged
 
 
 # --- create env from yaml -------------------------------------------------------------
-
-
 def parse_envs(
     *paths: str | Path,
     remove_python: bool = True,
     deps: Collection[str] | None = None,
     reqs: Collection[str] | None = None,
     channels: Collection[str] | None = None,
 ) -> tuple[set[str], set[str], set[str], str | None]:
@@ -246,33 +312,35 @@
     install_package: bool = False,
 ) -> bool:
     """Parse and install everything. Pass an already merged yaml file."""
 
     if session_skip_install(session):
         return True
 
+    channels, deps, reqs, name = parse_envs(
+        *paths,
+        remove_python=remove_python,
+        deps=deps,
+        reqs=reqs,
+        channels=channels,
+    )
+
     unchanged, hashes = env_unchanged(
         session,
-        *paths,
         prefix="env",
         other=dict(
-            deps=deps, reqs=reqs, channels=channels, install_package=install_package
+            deps=deps,
+            reqs=reqs,
+            channels=channels,
+            install_package=install_package,
         ),
     )
     if unchanged and not force_reinstall:
         return unchanged
 
-    channels, deps, reqs, name = parse_envs(
-        *paths,
-        remove_python=remove_python,
-        deps=deps,
-        reqs=reqs,
-        channels=channels,
-    )
-
     if not channels:
         channels = ""
     if deps:
         conda_install_kws = conda_install_kws or {}
         conda_install_kws.update(channel=channels)
         session.conda_install(*deps, **(conda_install_kws or {}))
 
@@ -287,41 +355,49 @@
     write_hashfile(hashes, session=session, prefix="env")
 
     return unchanged
 
 
 def session_install_pip(
     session: nox.Session,
-    requirement_paths: Collection[str] | None = None,
-    constraint_paths: Collection[str] | None = None,
+    requirement_paths: str | Collection[str] | None = None,
+    constraint_paths: str | Collection[str] | None = None,
     extras: str | Collection[str] | None = None,
-    reqs: Collection[str] | None = None,
+    reqs: str | Collection[str] | None = None,
     display_name: str | None = None,
     force_reinstall: bool = False,
     install_package: bool = False,
     no_deps: bool = False,
 ):
     if session_skip_install(session):
         return True
 
+    def _check_param(x):
+        if x is None:
+            return []
+        elif isinstance(x, str):
+            return [x]
+        else:
+            return x
+
+    extras = _check_param(extras)
     if extras:
         install_package = True
-        if not isinstance(extras, str):
-            extras = ",".join(extras)
+        extras = ",".join(extras)
         install_package_args = ["-e", f".[{extras}]"]
     elif install_package:
         install_package_args = ["-e", "."]
 
     if install_package and no_deps:
         install_package_args.append("--no-deps")
 
-    requirement_paths = requirement_paths or ()
-    constraint_paths = constraint_paths or ()
-    reqs = reqs or ()
-    paths = requirement_paths + constraint_paths
+    requirement_paths = _check_param(requirement_paths)
+    constraint_paths = _check_param(constraint_paths)
+    reqs = _check_param(reqs)
+    paths = list(requirement_paths) + list(constraint_paths)
 
     unchanged, hashes = env_unchanged(
         session,
         *paths,
         prefix="pip",
         other=dict(
             reqs=reqs, extras=extras, install_package=install_package, no_deps=no_deps
@@ -340,82 +416,29 @@
     if install_args:
         session.install(*install_args)
 
     if install_package:
         session.install(*install_package_args)
 
     session_set_ipykernel_display_name(session, display_name)
-
     write_hashfile(hashes, session=session, prefix="pip")
 
 
-def session_install_envs_merge(
-    session,
-    *paths,
-    remove_python=True,
-    deps=None,
-    reqs=None,
-    channels=None,
-    conda_install_kws=None,
-    install_kws=None,
-    display_name=None,
-    force_reinstall=False,
-) -> bool:
-    """Merge files (using conda-merge) and then create env"""
-
-    if session_skip_install(session):
-        return True
-
-    unchanged, hashes = env_unchanged(
-        session, *paths, prefix="env", other=dict(deps=deps, reqs=reqs)
-    )
-    if unchanged and not force_reinstall:
-        return unchanged
-
-    # first create a temporary file for the environment
-    with tempfile.TemporaryDirectory() as d:
-        yaml = Path(d) / "tmp_env.yaml"
-        with yaml.open("w") as f:
-            session.run("conda-merge", *paths, stdout=f, external=True)
-        session.run("cat", str(yaml), external=True, silent=True)
-
-        channels, deps, reqs, _ = parse_envs(
-            yaml, remove_python=remove_python, deps=deps, reqs=reqs, channels=channels
-        )
-
-    if deps:
-        if conda_install_kws is None:
-            conda_install_kws = {}
-        conda_install_kws.update(channel=channels)
-        session.conda_install(*deps, **conda_install_kws)
-
-    if reqs:
-        if install_kws is None:
-            install_kws = {}
-        session.install(*reqs, **install_kws)
-
-    session_set_ipykernel_display_name(session, display_name)
-
-    write_hashfile(hashes, session=session, prefix="env")
-
-    return unchanged
-
-
 # --- Hash environment -----------------------------------------------------------------
 
 PREFIX_HASH_EXTS = Literal["env", "lock", "pip"]
 
 
 def env_unchanged(
     session: nox.Session,
     *paths: str | Path,
     prefix: PREFIX_HASH_EXTS,
     verbose: bool = True,
     hashes: dict[str, str] | None = None,
-    other: Any | None = None,
+    other: dict[str, Any] | None = None,
 ) -> tuple[bool, dict[str, str]]:
     hashfile = hashfile_path(session, prefix)
 
     if hashes is None:
         hashes = get_hashes(*paths, other=other)
 
     if hashfile.exists():
@@ -431,23 +454,36 @@
         session.log(f"session {session.name} changed")
 
     return unchanged, hashes
 
 
 def get_hashes(
     *paths: str | Path,
-    other: str | None = None,
+    other: dict[str, Any] | None = None,
 ) -> dict[str, str]:
     """Get md5 hashes for paths"""
-    out = {str(path): _get_file_hash(path) for path in paths}
+
+    out = {"path": {str(path): _get_file_hash(path) for path in paths}}
 
     if other:
         import hashlib
 
-        out["other"] = hashlib.md5(str(other).encode("utf-8")).hexdigest()
+        other_hashes = {}
+        for k, v in other.items():
+            if isinstance(v, str):
+                s = v
+            else:
+                try:
+                    s = str(sorted(v))
+                except Exception:
+                    s = str(v)
+            other_hashes[k] = hashlib.md5(s.encode("utf-8")).hexdigest()
+
+        out["other"] = other_hashes
+
     return out
 
 
 def hashfile_path(session: nox.Session, prefix: PREFIX_HASH_EXTS) -> Path:
     """Path for hashfile for this session"""
     return Path(session.create_tmp()) / f"{prefix}.json"
 
@@ -484,40 +520,65 @@
             data = f.read(buff_size)
             if not data:
                 break
             md5.update(data)
     return md5.hexdigest()
 
 
-# from contextlib import contextmanager
-# @contextmanager
-# def check_hashed_env(
-#         session: nox.Session,
-#         *paths: str | Path,
-#         prefix: Literal["env", "lock"],
-#         verbose: bool=True,
-#         recreate_session=False,
-# ):
+# --- Old stuff ------------------------------------------------------------------------
+# def session_install_envs_merge(
+#     session,
+#     *paths,
+#     remove_python=True,
+#     deps=None,
+#     reqs=None,
+#     channels=None,
+#     conda_install_kws=None,
+#     install_kws=None,
+#     display_name=None,
+#     force_reinstall=False,
+# ) -> bool:
+#     """Merge files (using conda-merge) and then create env"""
+
+#     if session_skip_install(session):
+#         return True
+
+#     unchanged, hashes = env_unchanged(
+#         session, *paths, prefix="env", other=dict(deps=deps, reqs=reqs)
+#     )
+#     if unchanged and not force_reinstall:
+#         return unchanged
 
-#     changed, hashes = env_hashes_changed(session, *paths, prefix, verbose=verbose, return_hashes=True)
+#     # first create a temporary file for the environment
+#     with tempfile.TemporaryDirectory() as d:
+#         yaml = Path(d) / "tmp_env.yaml"
+#         with yaml.open("w") as f:
+#             session.run("conda-merge", *paths, stdout=f, external=True)
+#         session.run("cat", str(yaml), external=True, silent=True)
 
+#         channels, deps, reqs, _ = parse_envs(
+#             yaml, remove_python=remove_python, deps=deps, reqs=reqs, channels=channels
+#         )
 
-#     if changed and recreate_session:
-#         if verbose:
-#             session.log("env changed.  Recreating {session.virtualenv.location_name}")
-#             _reuse_original = session.virtualenv.reuse_existing
-#             _no_install_original = session._runner.global_config.no_install
+#     if deps:
+#         if conda_install_kws is None:
+#             conda_install_kws = {}
+#         conda_install_kws.update(channel=channels)
+#         session.conda_install(*deps, **conda_install_kws)
+
+#     if reqs:
+#         if install_kws is None:
+#             install_kws = {}
+#         session.install(*reqs, **install_kws)
 
-#             session.virtualenv.reuse_existing = False
-#             session._runner.global_config.no_install = False
+#     session_set_ipykernel_display_name(session, display_name)
 
-#             session.virtualenv.create()
-#             env_hashes_changed(session, *paths, prefix, verbose=verbose, hashes=hashes)
+#     write_hashfile(hashes, session=session, prefix="env")
 
-#             session.virtualenv.reuse_existing = _reuse_original
+#     return unchanged
 
 
 # def _remove_python_from_yaml(path):
 #     from yaml import safe_dump
 
 #     path = Path(path)
 
@@ -766,7 +827,65 @@
 #         external = False
 
 #     args = check_args_with_default(args, default=default)
 
 # #     session.log(f"args {args}")
 # #     session.log(f"external {external}")
 # #     session.run(*args, external=external, **kws)
+
+
+## This should actually go in the noxfile.  Keeping here
+## incase want it again in the future.
+# @group.session(python=PYTHON_DEFAULT_VERSION)
+# def conda_merge(
+#     session: Session,
+#     conda_merge_force: bool = False,
+#     force_reinstall: FORCE_REINSTALL_CLI = False,
+# ):
+#     """Merge environments using conda-merge."""
+#     import tempfile
+#     session_install_envs(
+#         session,
+#         reqs=["conda-merge", "ruamel.yaml"],
+#         force_reinstall=force_reinstall,
+#     )
+
+#     env_base = ROOT / "environment.yaml"
+#     env_dir = ROOT / "environment"
+
+#     def create_env(*extras, others=None, name=None, base=True):
+#         if name is None:
+#             name = extras[0]
+#         env = env_dir / f"{name}.yaml"
+
+#         deps = []
+#         if base:
+#             deps.append(str(env_base))
+#         for extra in extras:
+#             deps.append(str(env_dir / f"{extra}-extras.yaml"))
+
+#         if conda_merge_force or update_target(env, *deps):
+#             session.log(f"creating {env}")
+
+#             args = ["conda-merge"] + deps
+#             with tempfile.TemporaryDirectory() as d:
+#                 tmp_path = Path(d) / "tmp_env.yaml"
+
+#                 with tmp_path.open("w") as f:
+#                     session.run(*args, stdout=f)
+
+#                 run_str = dedent(
+#                     f"""
+#                 from ruamel.yaml import YAML; from pathlib import Path;
+#                 pin, pout = Path("{tmp_path}"), Path("{env}")
+#                 y = YAML(); y.indent(mapping=2, sequence=4, offset=2)
+#                 y.dump(y.load(pin.open("r")), pout.open("w"))
+#                 """
+#                 )
+
+#                 session.run("python", "-c", run_str, silent=True)
+
+#     for extra in ["test", "docs"]:
+#         create_env(extra, base=True)
+
+#     create_env("test", "typing", name="typing", base=True)
+#     create_env("dev", "test", "typing", "nox", name="dev", base=True)
```

