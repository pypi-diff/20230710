# Comparing `tmp/bowtie_json_schema-2023.7.2.tar.gz` & `tmp/bowtie_json_schema-2023.7.3.tar.gz`

## Comparing `bowtie_json_schema-2023.7.2.tar` & `bowtie_json_schema-2023.7.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.flake8
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.readthedocs.yml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/action.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/io-schema.json -> bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/noxfile.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/test-requirements.in
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/test-requirements.txt
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/SECURITY.md
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/release.yml
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/workflows/build-frontend.yml
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/workflows/dependabot-merge.yml
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/workflows/deploy-frontend.yml
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/workflows/images.yml
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.github/workflows/report.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/__main__.py
--rw-r--r--   0        0        0    31499 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/_cli.py
--rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/_commands.py
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/_core.py
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/_report.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/schemas/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/Makefile
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/cli.rst
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/conf.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/contributing.rst
--rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/implementers.rst
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/index.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/requirements.in
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/requirements.txt
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/docs/_static/dreamed.png
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/.eslintrc.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/index.html
--rw-r--r--   0        0        0   126070 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/package-lock.json
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/package.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/vite.config.js
--rw-r--r--   0        0        0   130217 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/public/favicon.ico
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/MainContainer.jsx
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/ReportDataHandler.jsx
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/ReportView.jsx
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/index.jsx
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/CopyToClipboard.jsx
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/LoadingAnimation.jsx
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/NavBar.jsx
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Cases/AccordionItem.jsx
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Cases/AccordionSvg.jsx
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Cases/CasesSection.jsx
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Cases/SchemaDisplay.jsx
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/DragAndDrop/DragAndDrop.css
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/DragAndDrop/DragAndDrop.jsx
--rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Modals/DetailsButtonModal.jsx
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Modals/RunTimeInfoModal.jsx
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/RunInfo/RunInfoSection.jsx
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Summary/ImplementationRow.jsx
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Summary/SummarySection.jsx
--rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/components/Summary/SummaryTable.jsx
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/context/BowtieVersionContext.jsx
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/context/ThemeContext.jsx
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/data/runInfo.js
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/frontend/src/data/summary.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/conftest.py
--rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/test_integration.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/fauxmplementations/badsonschema/Dockerfile
--rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/fauxmplementations/badsonschema/badsonschema
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/fauxmplementations/lintsonschema/Dockerfile
--rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/fauxmplementations/lintsonschema/io-schema.json
--rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/templates/report.html.j2
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/LICENSE
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/README.rst
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/pyproject.toml
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.2/PKG-INFO
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/.flake8
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/.readthedocs.yml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/action.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/io-schema.json -> bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/noxfile.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/test-requirements.in
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/test-requirements.txt
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/.github/SECURITY.md
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/.github/release.yml
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/.github/workflows/build-frontend.yml
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/.github/workflows/dependabot-merge.yml
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/.github/workflows/deploy-frontend.yml
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/.github/workflows/images.yml
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/.github/workflows/report.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/bowtie/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/bowtie/__main__.py
+-rw-r--r--   0        0        0    31602 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/bowtie/_cli.py
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/bowtie/_commands.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/bowtie/_core.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/bowtie/_report.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/bowtie/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/bowtie/schemas/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/docs/Makefile
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/docs/cli.rst
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/docs/conf.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/docs/contributing.rst
+-rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/docs/implementers.rst
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/docs/index.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/docs/requirements.in
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/docs/requirements.txt
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/docs/_static/dreamed.png
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/.eslintrc.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/index.html
+-rw-r--r--   0        0        0   164653 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/package-lock.json
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/package.json
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/tsconfig.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/vite.config.js
+-rw-r--r--   0        0        0   130217 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/public/favicon.ico
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/MainContainer.jsx
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/ReportDataHandler.jsx
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/ReportView.jsx
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/index.jsx
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/CopyToClipboard.jsx
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/LoadingAnimation.jsx
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/NavBar.jsx
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/Cases/AccordionItem.jsx
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/Cases/AccordionSvg.jsx
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/Cases/CasesSection.jsx
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/Cases/SchemaDisplay.jsx
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/DragAndDrop/DragAndDrop.css
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/DragAndDrop/DragAndDrop.jsx
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/Modals/DetailsButtonModal.jsx
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/Modals/RunTimeInfoModal.jsx
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/RunInfo/RunInfoSection.jsx
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/Summary/ImplementationRow.jsx
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/Summary/SummarySection.jsx
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/components/Summary/SummaryTable.jsx
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/context/BowtieVersionContext.jsx
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/context/ThemeContext.jsx
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/tests/conftest.py
+-rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/tests/test_integration.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/tests/fauxmplementations/badsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/tests/fauxmplementations/badsonschema/badsonschema
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/tests/fauxmplementations/lintsonschema/Dockerfile
+-rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/tests/fauxmplementations/lintsonschema/io-schema.json
+-rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/bowtie/templates/report.html.j2
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/LICENSE
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/README.rst
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/pyproject.toml
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.3/PKG-INFO
```

### Comparing `bowtie_json_schema-2023.7.2/.flake8` & `bowtie_json_schema-2023.7.3/.flake8`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/.pre-commit-config.yaml` & `bowtie_json_schema-2023.7.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/noxfile.py` & `bowtie_json_schema-2023.7.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/test-requirements.txt` & `bowtie_json_schema-2023.7.3/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/.github/SECURITY.md` & `bowtie_json_schema-2023.7.3/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/.github/dependabot.yml` & `bowtie_json_schema-2023.7.3/.github/dependabot.yml`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,19 @@
       interval: "daily"
 
   - package-ecosystem: "gradle"
     directory: "implementations/java-json-schema"
     schedule:
       interval: "daily"
 
+  - package-ecosystem: "gradle"
+    directory: "implementations/java-json-schema-validator"
+    schedule:
+      interval: "daily"
+
   # Dependabot for Dockerfiles
   # --------------------------
 
   # See dependabot/dependabot-core#1015 or dependabot/dependabot-core#2178,
   # this doesn't happen automatically, so hooray, manual list.
 
   - package-ecosystem: "docker"
@@ -146,14 +151,19 @@
 
   - package-ecosystem: "docker"
     directory: "/implementations/java-json-schema"
     schedule:
       interval: "daily"
 
   - package-ecosystem: "docker"
+    directory: "/implementations/java-json-schema-validator"
+    schedule:
+      interval: "daily"
+
+  - package-ecosystem: "docker"
     directory: "/tests/fauxmplementations/badsonschema"
     schedule:
       interval: "daily"
 
   - package-ecosystem: "docker"
     directory: "/tests/fauxmplementations/envsonschema"
     schedule:
```

### Comparing `bowtie_json_schema-2023.7.2/.github/workflows/build-frontend.yml` & `bowtie_json_schema-2023.7.3/.github/workflows/build-frontend.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/.github/workflows/ci.yml` & `bowtie_json_schema-2023.7.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/.github/workflows/dependabot-merge.yml` & `bowtie_json_schema-2023.7.3/.github/workflows/dependabot-merge.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/.github/workflows/deploy-frontend.yml` & `bowtie_json_schema-2023.7.3/.github/workflows/deploy-frontend.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/.github/workflows/images.yml` & `bowtie_json_schema-2023.7.3/.github/workflows/images.yml`

 * *Files 0% similar despite different names*

```diff
@@ -83,13 +83,13 @@
           tags: ${{ steps.build_image.outputs.tags }}
           registry: ghcr.io/${{ github.repository_owner }}
           username: ${{ github.actor }}
           password: ${{ github.token }}
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
 
       - name: Install Bowtie
-        uses: bowtie-json-schema/bowtie@v2023.06.4
+        uses: bowtie-json-schema/bowtie@v2023.07.2
         if: steps.changes.outputs.impl == 'true' || (github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags'))
 
       - name: Smoke Test
         run: bowtie smoke -i "${{ steps.build_image.outputs.image-with-tag }}"
         if: steps.changes.outputs.impl == 'true' || (github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags'))
```

### Comparing `bowtie_json_schema-2023.7.2/.github/workflows/report.yml` & `bowtie_json_schema-2023.7.3/.github/workflows/report.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/bowtie/_cli.py` & `bowtie_json_schema-2023.7.3/bowtie/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,16 @@
     default=lambda: "pretty" if sys.stdout.isatty() else "json",
     show_default="pretty if stdout is a tty, otherwise JSON",
     type=click.Choice(["json", "pretty"]),
 )
 _F = Literal["json", "pretty"]
 
 
-@tui()
-@click.group(context_settings=dict(help_option_names=["--help", "-h"]))
+@tui()  # type: ignore[reportGeneralTypeIssues]
+@click.group(context_settings=dict(help_option_names=["--help", "-h"]))  # type: ignore[reportUntypedFunctionDecorator]  # noqa: E501
 @click.version_option(prog_name="bowtie", package_name="bowtie-json-schema")
 def main():
     """
     A meta-validator for the JSON Schema specifications.
     """
     redirect_structlog()
```

### Comparing `bowtie_json_schema-2023.7.2/bowtie/_commands.py` & `bowtie_json_schema-2023.7.3/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/bowtie/_core.py` & `bowtie_json_schema-2023.7.3/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/bowtie/_report.py` & `bowtie_json_schema-2023.7.3/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/bowtie/exceptions.py` & `bowtie_json_schema-2023.7.3/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/docs/Makefile` & `bowtie_json_schema-2023.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/docs/cli.rst` & `bowtie_json_schema-2023.7.3/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/docs/conf.py` & `bowtie_json_schema-2023.7.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/docs/contributing.rst` & `bowtie_json_schema-2023.7.3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/docs/implementers.rst` & `bowtie_json_schema-2023.7.3/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/docs/index.rst` & `bowtie_json_schema-2023.7.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/docs/requirements.txt` & `bowtie_json_schema-2023.7.3/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/docs/_static/dreamed.png` & `bowtie_json_schema-2023.7.3/docs/_static/dreamed.png`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/frontend/package-lock.json` & `bowtie_json_schema-2023.7.3/frontend/package-lock.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745413750436072%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'react-bootstrap': '^2.8.0'}, 'devDependencies': {'eslint': "*

 * *               "'8.43.0', 'eslint-plugin-react': '7.32.2', 'eslint-plugin-react-hooks': '4.6.0', "*

 * *               "'@types/react': '^18.2.14', '@types/react-dom': '^18.2.6', 'ts-loader': '^9.4.4', "*

 * *               "'typescript': '^5.1.5', delete: ['eslint-plugin-react-refresh']}}, "*

 * *               "'node_modules/@jridgewell/source-map': {delete: ['optional']}, "*

 * *               "'node_modules/@popperjs/core': […]*

```diff
@@ -3,24 +3,28 @@
     "name": "bowtie",
     "packages": {
         "": {
             "dependencies": {
                 "bootstrap": "^5.3.0",
                 "moment": "^2.29.4",
                 "react": "^18.2.0",
+                "react-bootstrap": "^2.8.0",
                 "react-bootstrap-icons": "^1.10.3",
                 "react-dom": "^18.2.0",
                 "react-router-dom": "^6.13.0"
             },
             "devDependencies": {
+                "@types/react": "^18.2.14",
+                "@types/react-dom": "^18.2.6",
                 "@vitejs/plugin-react": "^4.0.1",
-                "eslint": "^8.43.0",
-                "eslint-plugin-react": "^7.32.2",
-                "eslint-plugin-react-hooks": "^4.6.0",
-                "eslint-plugin-react-refresh": "^0.4.1",
+                "eslint": "8.43.0",
+                "eslint-plugin-react": "7.32.2",
+                "eslint-plugin-react-hooks": "4.6.0",
+                "ts-loader": "^9.4.4",
+                "typescript": "^5.1.5",
                 "vite": "^4.3.9"
             },
             "name": "bowtie",
             "version": "1.0.0"
         },
         "node_modules/@ampproject/remapping": {
             "dependencies": {
@@ -329,14 +333,25 @@
             "integrity": "sha512-yIiRO6yobeEIaI0RTbIr8iAK9FcBHLtZq0S89ZPjDLQXBA4xvghaKqI0etp/tF3htTM0sazJKKLz9oEiGRtu7w==",
             "peerDependencies": {
                 "@babel/core": "^7.0.0-0"
             },
             "resolved": "https://registry.npmjs.org/@babel/plugin-transform-react-jsx-source/-/plugin-transform-react-jsx-source-7.22.5.tgz",
             "version": "7.22.5"
         },
+        "node_modules/@babel/runtime": {
+            "dependencies": {
+                "regenerator-runtime": "^0.13.11"
+            },
+            "engines": {
+                "node": ">=6.9.0"
+            },
+            "integrity": "sha512-ecjvYlnAaZ/KVneE/OdKYBYfgXV3Ptu6zQWmgEF7vwKhQnvVS6bjMD2XYgj+SNvQ1GfK/pjgokfPkC/2CO8CuA==",
+            "resolved": "https://registry.npmjs.org/@babel/runtime/-/runtime-7.22.5.tgz",
+            "version": "7.22.5"
+        },
         "node_modules/@babel/template": {
             "dependencies": {
                 "@babel/code-frame": "^7.22.5",
                 "@babel/parser": "^7.22.5",
                 "@babel/types": "^7.22.5"
             },
             "dev": true,
@@ -873,15 +888,14 @@
         "node_modules/@jridgewell/source-map": {
             "dependencies": {
                 "@jridgewell/gen-mapping": "^0.3.0",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
             "dev": true,
             "integrity": "sha512-b+fsZXeLYi9fEULmfBrhxn4IrPlINf8fiNarzTof004v3lFdntdwa9PF7vFJqm3mg7s+ScJMxXaE3Acp1irZcg==",
-            "optional": true,
             "peer": true,
             "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.3.tgz",
             "version": "0.3.3"
         },
         "node_modules/@jridgewell/sourcemap-codec": {
             "dev": true,
             "integrity": "sha512-eF2rxCRulEKXHTRiDrDy6erMYWqNw4LPdQ8UQA4huuxaQsVeRPFl2oM8oDGxMFhJUWZf9McpLtJasDDZb/Bpeg==",
@@ -941,34 +955,168 @@
         },
         "node_modules/@popperjs/core": {
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/popperjs"
             },
             "integrity": "sha512-P1st0aksCrn9sGZhp8GMYwBnQsbvAWsZAX44oXNNvLHGqAOcoVxmjZiohstwQ7SqKnbR47akdNi+uleWD8+g6A==",
-            "peer": true,
             "resolved": "https://registry.npmjs.org/@popperjs/core/-/core-2.11.8.tgz",
             "version": "2.11.8"
         },
+        "node_modules/@react-aria/ssr": {
+            "dependencies": {
+                "@swc/helpers": "^0.5.0"
+            },
+            "integrity": "sha512-bfufjg4ESE5giN+Fxj1XIzS5f/YIhqcGc+Ve+vUUKU8xZ8t/Xtjlv8F3kjqDBQdk//n3mluFY7xG1wQVB9rMLQ==",
+            "peerDependencies": {
+                "react": "^16.8.0 || ^17.0.0-rc.1 || ^18.0.0"
+            },
+            "resolved": "https://registry.npmjs.org/@react-aria/ssr/-/ssr-3.7.0.tgz",
+            "version": "3.7.0"
+        },
         "node_modules/@remix-run/router": {
             "engines": {
                 "node": ">=14"
             },
             "integrity": "sha512-EXJysQ7J3veRECd0kZFQwYYd5sJMcq2O/m60zu1W2l3oVQ9xtub8jTOtYRE0+M2iomyG/W3Ps7+vp2kna0C27Q==",
             "resolved": "https://registry.npmjs.org/@remix-run/router/-/router-1.6.3.tgz",
             "version": "1.6.3"
         },
+        "node_modules/@restart/hooks": {
+            "dependencies": {
+                "dequal": "^2.0.2"
+            },
+            "integrity": "sha512-3BekqcwB6Umeya+16XPooARn4qEPW6vNvwYnlofIYe6h9qG1/VeD7UvShCWx11eFz5ELYmwIEshz+MkPX3wjcQ==",
+            "peerDependencies": {
+                "react": ">=16.8.0"
+            },
+            "resolved": "https://registry.npmjs.org/@restart/hooks/-/hooks-0.4.9.tgz",
+            "version": "0.4.9"
+        },
+        "node_modules/@restart/ui": {
+            "dependencies": {
+                "@babel/runtime": "^7.21.0",
+                "@popperjs/core": "^2.11.6",
+                "@react-aria/ssr": "^3.5.0",
+                "@restart/hooks": "^0.4.9",
+                "@types/warning": "^3.0.0",
+                "dequal": "^2.0.3",
+                "dom-helpers": "^5.2.0",
+                "uncontrollable": "^8.0.1",
+                "warning": "^4.0.3"
+            },
+            "integrity": "sha512-eC3puKuWE1SRYbojWHXnvCNHGgf3uzHCb6JOhnF4OXPibOIPEkR1sqDSkL643ydigxwh+ruCa1CmYHlzk7ikKA==",
+            "peerDependencies": {
+                "react": ">=16.14.0",
+                "react-dom": ">=16.14.0"
+            },
+            "resolved": "https://registry.npmjs.org/@restart/ui/-/ui-1.6.6.tgz",
+            "version": "1.6.6"
+        },
+        "node_modules/@restart/ui/node_modules/uncontrollable": {
+            "integrity": "sha512-/GDx+K1STGtpgTsj5Dj3J51YaKxZDblbCQHTH1zHLuoBEWodj6MjtRVv3TUijj1JYLRLSFsFzN8NV4M3QV4d9w==",
+            "peerDependencies": {
+                "react": ">=16.14.0"
+            },
+            "resolved": "https://registry.npmjs.org/uncontrollable/-/uncontrollable-8.0.2.tgz",
+            "version": "8.0.2"
+        },
+        "node_modules/@swc/helpers": {
+            "dependencies": {
+                "tslib": "^2.4.0"
+            },
+            "integrity": "sha512-sJ902EfIzn1Fa+qYmjdQqh8tPsoxyBz+8yBKC2HKUxyezKJFwPGOn7pv4WY6QuQW//ySQi5lJjA/ZT9sNWWNTg==",
+            "resolved": "https://registry.npmjs.org/@swc/helpers/-/helpers-0.5.1.tgz",
+            "version": "0.5.1"
+        },
+        "node_modules/@types/eslint": {
+            "dependencies": {
+                "@types/estree": "*",
+                "@types/json-schema": "*"
+            },
+            "dev": true,
+            "integrity": "sha512-PRVjQ4Eh9z9pmmtaq8nTjZjQwKFk7YIHIud3lRoKRBgUQjgjRmoGxxGEPXQkF+lH7QkHJRNr5F4aBgYCW0lqpQ==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-8.40.2.tgz",
+            "version": "8.40.2"
+        },
+        "node_modules/@types/eslint-scope": {
+            "dependencies": {
+                "@types/eslint": "*",
+                "@types/estree": "*"
+            },
+            "dev": true,
+            "integrity": "sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.4.tgz",
+            "version": "3.7.4"
+        },
+        "node_modules/@types/estree": {
+            "dev": true,
+            "integrity": "sha512-LG4opVs2ANWZ1TJoKc937iMmNstM/d0ae1vNbnBvBhqCSezgVUOzcLCqbI5elV8Vy6WKwKjaqR+zO9VKirBBCA==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-1.0.1.tgz",
+            "version": "1.0.1"
+        },
+        "node_modules/@types/json-schema": {
+            "dev": true,
+            "integrity": "sha512-Hr5Jfhc9eYOQNPYO5WLDq/n4jqijdHNlDXjuAQkkt+mWdQR+XJToOHrsD4cPaMXpn6KO7y2+wM8AZEs8VpBLVA==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.12.tgz",
+            "version": "7.0.12"
+        },
         "node_modules/@types/node": {
             "dev": true,
             "integrity": "sha512-EhcH/wvidPy1WeML3TtYFGR83UzjxeWRen9V402T8aUGYsCHOmfoisV3ZSg03gAFIbLq8TnWOJ0f4cALtnSEUg==",
-            "optional": true,
             "peer": true,
             "resolved": "https://registry.npmjs.org/@types/node/-/node-20.3.1.tgz",
             "version": "20.3.1"
         },
+        "node_modules/@types/prop-types": {
+            "integrity": "sha512-JCB8C6SnDoQf0cNycqd/35A7MjcnK+ZTqE7judS6o7utxUCg6imJg3QK2qzHKszlTjcj2cn+NwMB2i96ubpj7w==",
+            "resolved": "https://registry.npmjs.org/@types/prop-types/-/prop-types-15.7.5.tgz",
+            "version": "15.7.5"
+        },
+        "node_modules/@types/react": {
+            "dependencies": {
+                "@types/prop-types": "*",
+                "@types/scheduler": "*",
+                "csstype": "^3.0.2"
+            },
+            "integrity": "sha512-A0zjq+QN/O0Kpe30hA1GidzyFjatVvrpIvWLxD+xv67Vt91TWWgco9IvrJBkeyHm1trGaFS/FSGqPlhyeZRm0g==",
+            "resolved": "https://registry.npmjs.org/@types/react/-/react-18.2.14.tgz",
+            "version": "18.2.14"
+        },
+        "node_modules/@types/react-dom": {
+            "dependencies": {
+                "@types/react": "*"
+            },
+            "dev": true,
+            "integrity": "sha512-2et4PDvg6PVCyS7fuTc4gPoksV58bW0RwSxWKcPRcHZf0PRUGq03TKcD/rUHe3azfV6/5/biUBJw+HhCQjaP0A==",
+            "resolved": "https://registry.npmjs.org/@types/react-dom/-/react-dom-18.2.6.tgz",
+            "version": "18.2.6"
+        },
+        "node_modules/@types/react-transition-group": {
+            "dependencies": {
+                "@types/react": "*"
+            },
+            "integrity": "sha512-VnCdSxfcm08KjsJVQcfBmhEQAPnLB8G08hAxn39azX1qYBQ/5RVQuoHuKIcfKOdncuaUvEpFKFzEvbtIMsfVew==",
+            "resolved": "https://registry.npmjs.org/@types/react-transition-group/-/react-transition-group-4.4.6.tgz",
+            "version": "4.4.6"
+        },
+        "node_modules/@types/scheduler": {
+            "integrity": "sha512-5cJ8CB4yAx7BH1oMvdU0Jh9lrEXyPkar6F9G/ERswkCuvP4KQZfZkSjcMbAICCpQTN4OuZn8tz0HiKv9TGZgrQ==",
+            "resolved": "https://registry.npmjs.org/@types/scheduler/-/scheduler-0.16.3.tgz",
+            "version": "0.16.3"
+        },
+        "node_modules/@types/warning": {
+            "integrity": "sha512-t/Tvs5qR47OLOr+4E9ckN8AmP2Tf16gWq+/qA4iUGS/OOyHVO8wv2vjJuX8SNOUTJyWb+2t7wJm6cXILFnOROA==",
+            "resolved": "https://registry.npmjs.org/@types/warning/-/warning-3.0.0.tgz",
+            "version": "3.0.0"
+        },
         "node_modules/@vitejs/plugin-react": {
             "dependencies": {
                 "@babel/core": "^7.22.5",
                 "@babel/plugin-transform-react-jsx-self": "^7.22.5",
                 "@babel/plugin-transform-react-jsx-source": "^7.22.5",
                 "react-refresh": "^0.14.0"
             },
@@ -988,26 +1136,211 @@
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-wViHqhAd8OHeLS/IRMJjTSDHF3U9eWi62F/MledQGPdJGDhodXJ9PBLNGr6WWL7qlH12Mt3TyTpbS+hGXMjCzQ==",
             "resolved": "https://registry.npmjs.org/react-refresh/-/react-refresh-0.14.0.tgz",
             "version": "0.14.0"
         },
+        "node_modules/@webassemblyjs/ast": {
+            "dependencies": {
+                "@webassemblyjs/helper-numbers": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6"
+            },
+            "dev": true,
+            "integrity": "sha512-IN1xI7PwOvLPgjcf180gC1bqn3q/QaOCwYUahIOhbYUu8KA/3tw2RT/T0Gidi1l7Hhj5D/INhJxiICObqpMu4Q==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.6.tgz",
+            "version": "1.11.6"
+        },
+        "node_modules/@webassemblyjs/floating-point-hex-parser": {
+            "dev": true,
+            "integrity": "sha512-ejAj9hfRJ2XMsNHk/v6Fu2dGS+i4UaXBXGemOfQ/JfQ6mdQg/WXtwleQRLLS4OvfDhv8rYnVwH27YJLMyYsxhw==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.6.tgz",
+            "version": "1.11.6"
+        },
+        "node_modules/@webassemblyjs/helper-api-error": {
+            "dev": true,
+            "integrity": "sha512-o0YkoP4pVu4rN8aTJgAyj9hC2Sv5UlkzCHhxqWj8butaLvnpdc2jOwh4ewE6CX0txSfLn/UYaV/pheS2Txg//Q==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.6.tgz",
+            "version": "1.11.6"
+        },
+        "node_modules/@webassemblyjs/helper-buffer": {
+            "dev": true,
+            "integrity": "sha512-z3nFzdcp1mb8nEOFFk8DrYLpHvhKC3grJD2ardfKOzmbmJvEf/tPIqCY+sNcwZIY8ZD7IkB2l7/pqhUhqm7hLA==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.6.tgz",
+            "version": "1.11.6"
+        },
+        "node_modules/@webassemblyjs/helper-numbers": {
+            "dependencies": {
+                "@webassemblyjs/floating-point-hex-parser": "1.11.6",
+                "@webassemblyjs/helper-api-error": "1.11.6",
+                "@xtuc/long": "4.2.2"
+            },
+            "dev": true,
+            "integrity": "sha512-vUIhZ8LZoIWHBohiEObxVm6hwP034jwmc9kuq5GdHZH0wiLVLIPcMCdpJzG4C11cHoQ25TFIQj9kaVADVX7N3g==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.6.tgz",
+            "version": "1.11.6"
+        },
+        "node_modules/@webassemblyjs/helper-wasm-bytecode": {
+            "dev": true,
+            "integrity": "sha512-sFFHKwcmBprO9e7Icf0+gddyWYDViL8bpPjJJl0WHxCdETktXdmtWLGVzoHbqUcY4Be1LkNfwTmXOJUFZYSJdA==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.6.tgz",
+            "version": "1.11.6"
+        },
+        "node_modules/@webassemblyjs/helper-wasm-section": {
+            "dependencies": {
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/wasm-gen": "1.11.6"
+            },
+            "dev": true,
+            "integrity": "sha512-LPpZbSOwTpEC2cgn4hTydySy1Ke+XEu+ETXuoyvuyezHO3Kjdu90KK95Sh9xTbmjrCsUwvWwCOQQNta37VrS9g==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.6.tgz",
+            "version": "1.11.6"
+        },
+        "node_modules/@webassemblyjs/ieee754": {
+            "dependencies": {
+                "@xtuc/ieee754": "^1.2.0"
+            },
+            "dev": true,
+            "integrity": "sha512-LM4p2csPNvbij6U1f19v6WR56QZ8JcHg3QIJTlSwzFcmx6WSORicYj6I63f9yU1kEUtrpG+kjkiIAkevHpDXrg==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.6.tgz",
+            "version": "1.11.6"
+        },
+        "node_modules/@webassemblyjs/leb128": {
+            "dependencies": {
+                "@xtuc/long": "4.2.2"
+            },
+            "dev": true,
+            "integrity": "sha512-m7a0FhE67DQXgouf1tbN5XQcdWoNgaAuoULHIfGFIEVKA6tu/edls6XnIlkmS6FrXAquJRPni3ZZKjw6FSPjPQ==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.6.tgz",
+            "version": "1.11.6"
+        },
+        "node_modules/@webassemblyjs/utf8": {
+            "dev": true,
+            "integrity": "sha512-vtXf2wTQ3+up9Zsg8sa2yWiQpzSsMyXj0qViVP6xKGCUT8p8YJ6HqI7l5eCnWx1T/FYdsv07HQs2wTFbbof/RA==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.6.tgz",
+            "version": "1.11.6"
+        },
+        "node_modules/@webassemblyjs/wasm-edit": {
+            "dependencies": {
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/helper-wasm-section": "1.11.6",
+                "@webassemblyjs/wasm-gen": "1.11.6",
+                "@webassemblyjs/wasm-opt": "1.11.6",
+                "@webassemblyjs/wasm-parser": "1.11.6",
+                "@webassemblyjs/wast-printer": "1.11.6"
+            },
+            "dev": true,
+            "integrity": "sha512-Ybn2I6fnfIGuCR+Faaz7YcvtBKxvoLV3Lebn1tM4o/IAJzmi9AWYIPWpyBfU8cC+JxAO57bk4+zdsTjJR+VTOw==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.6.tgz",
+            "version": "1.11.6"
+        },
+        "node_modules/@webassemblyjs/wasm-gen": {
+            "dependencies": {
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/ieee754": "1.11.6",
+                "@webassemblyjs/leb128": "1.11.6",
+                "@webassemblyjs/utf8": "1.11.6"
+            },
+            "dev": true,
+            "integrity": "sha512-3XOqkZP/y6B4F0PBAXvI1/bky7GryoogUtfwExeP/v7Nzwo1QLcq5oQmpKlftZLbT+ERUOAZVQjuNVak6UXjPA==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.6.tgz",
+            "version": "1.11.6"
+        },
+        "node_modules/@webassemblyjs/wasm-opt": {
+            "dependencies": {
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/wasm-gen": "1.11.6",
+                "@webassemblyjs/wasm-parser": "1.11.6"
+            },
+            "dev": true,
+            "integrity": "sha512-cOrKuLRE7PCe6AsOVl7WasYf3wbSo4CeOk6PkrjS7g57MFfVUF9u6ysQBBODX0LdgSvQqRiGz3CXvIDKcPNy4g==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.6.tgz",
+            "version": "1.11.6"
+        },
+        "node_modules/@webassemblyjs/wasm-parser": {
+            "dependencies": {
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-api-error": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/ieee754": "1.11.6",
+                "@webassemblyjs/leb128": "1.11.6",
+                "@webassemblyjs/utf8": "1.11.6"
+            },
+            "dev": true,
+            "integrity": "sha512-6ZwPeGzMJM3Dqp3hCsLgESxBGtT/OeCvCZ4TA1JUPYgmhAx38tTPR9JaKy0S5H3evQpO/h2uWs2j6Yc/fjkpTQ==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.6.tgz",
+            "version": "1.11.6"
+        },
+        "node_modules/@webassemblyjs/wast-printer": {
+            "dependencies": {
+                "@webassemblyjs/ast": "1.11.6",
+                "@xtuc/long": "4.2.2"
+            },
+            "dev": true,
+            "integrity": "sha512-JM7AhRcE+yW2GWYaKeHL5vt4xqee5N2WcezptmgyhNS+ScggqcT1OtXykhAb13Sn5Yas0j2uv9tHgrjwvzAP4A==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.6.tgz",
+            "version": "1.11.6"
+        },
+        "node_modules/@xtuc/ieee754": {
+            "dev": true,
+            "integrity": "sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@xtuc/ieee754/-/ieee754-1.2.0.tgz",
+            "version": "1.2.0"
+        },
+        "node_modules/@xtuc/long": {
+            "dev": true,
+            "integrity": "sha512-NuHqBY1PB/D8xU6s/thBgOAiAP7HOYDQ32+BFZILJ8ivkUkAHQnWfn6WhL79Owj1qmUnoN/YPhktdIoucipkAQ==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@xtuc/long/-/long-4.2.2.tgz",
+            "version": "4.2.2"
+        },
         "node_modules/acorn": {
             "bin": {
                 "acorn": "bin/acorn"
             },
             "dev": true,
             "engines": {
                 "node": ">=0.4.0"
             },
             "integrity": "sha512-jaVNAFBHNLXspO543WnNNPZFRtavh3skAkITqD0/2aeMkKZTN+254PyhwxFYrk3vQ1xfY+2wbesJMs/JC8/PwQ==",
             "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.9.0.tgz",
             "version": "8.9.0"
         },
+        "node_modules/acorn-import-assertions": {
+            "dev": true,
+            "integrity": "sha512-cmMwop9x+8KFhxvKrKfPYmN6/pKTYYHBqLa0DfvVZcKMJWNyWLnaqND7dx/qn66R7ewM1UX5XMaDVP5wlVTaVA==",
+            "peer": true,
+            "peerDependencies": {
+                "acorn": "^8"
+            },
+            "resolved": "https://registry.npmjs.org/acorn-import-assertions/-/acorn-import-assertions-1.9.0.tgz",
+            "version": "1.9.0"
+        },
         "node_modules/acorn-jsx": {
             "dev": true,
             "integrity": "sha512-rq9s+JNhf0IChjtDXxllJ7g41oZk5SlXtp0LHwyA5cejwn7vKmKp4pPri6YEePv2PU65sAsegbXtIinmDFDXgQ==",
             "peerDependencies": {
                 "acorn": "^6.0.0 || ^7.0.0 || ^8.0.0"
             },
             "resolved": "https://registry.npmjs.org/acorn-jsx/-/acorn-jsx-5.3.2.tgz",
@@ -1025,14 +1358,24 @@
                 "type": "github",
                 "url": "https://github.com/sponsors/epoberezkin"
             },
             "integrity": "sha512-j3fVLgvTo527anyYyJOGTYJbG+vnnQYvE0m5mmkc1TK+nxAppkCLMIL0aZ4dblVCNoGShhm+kzE4ZUykBoMg4g==",
             "resolved": "https://registry.npmjs.org/ajv/-/ajv-6.12.6.tgz",
             "version": "6.12.6"
         },
+        "node_modules/ajv-keywords": {
+            "dev": true,
+            "integrity": "sha512-5p6WTN0DdTGVQk6VjcEju19IgaHudalcfabD7yhDGeA6bcQnmL+CpveLJq/3hvfwd1aof6L386Ougkx6RfyMIQ==",
+            "peer": true,
+            "peerDependencies": {
+                "ajv": "^6.9.1"
+            },
+            "resolved": "https://registry.npmjs.org/ajv-keywords/-/ajv-keywords-3.5.2.tgz",
+            "version": "3.5.2"
+        },
         "node_modules/ansi-regex": {
             "dev": true,
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-quJQXlTSUGL2LH9SUXo8VwsY4soanhgo6LNSm84E1LBcE8s3O0wpdiRzyR9z/ZZJMlMWv37qOOb9pdJlMUEKFQ==",
             "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-5.0.1.tgz",
@@ -1161,14 +1504,26 @@
                 "concat-map": "0.0.1"
             },
             "dev": true,
             "integrity": "sha512-iCuPHDFgrHX7H2vEI/5xpz07zSHB00TpugqhmYtVmMO6518mCuRMoOYFldEBl0g187ufozdaHgWKcYFb61qGiA==",
             "resolved": "https://registry.npmjs.org/brace-expansion/-/brace-expansion-1.1.11.tgz",
             "version": "1.1.11"
         },
+        "node_modules/braces": {
+            "dependencies": {
+                "fill-range": "^7.0.1"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=8"
+            },
+            "integrity": "sha512-b8um+L1RzM3WDSzvhm6gIz1yfTbBt6YTlcEKAvsmqCZZFw46z626lVj9j1yEPW33H5H+lBQpZMP1k8l+78Ha0A==",
+            "resolved": "https://registry.npmjs.org/braces/-/braces-3.0.2.tgz",
+            "version": "3.0.2"
+        },
         "node_modules/browserslist": {
             "bin": {
                 "browserslist": "cli.js"
             },
             "dependencies": {
                 "caniuse-lite": "^1.0.30001503",
                 "electron-to-chromium": "^1.4.431",
@@ -1196,15 +1551,14 @@
             "integrity": "sha512-M0MFoZzbUrRU4KNfCrDLnvyE7gub+peetoTid3TBIqtunaDJyXlwhakT+/VkvSXcfIzFfK/nkCs4nmyTmxdNSg==",
             "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.21.9.tgz",
             "version": "4.21.9"
         },
         "node_modules/buffer-from": {
             "dev": true,
             "integrity": "sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==",
-            "optional": true,
             "peer": true,
             "resolved": "https://registry.npmjs.org/buffer-from/-/buffer-from-1.1.2.tgz",
             "version": "1.1.2"
         },
         "node_modules/call-bind": {
             "dependencies": {
                 "function-bind": "^1.1.1",
@@ -1257,14 +1611,29 @@
             "engines": {
                 "node": ">=4"
             },
             "integrity": "sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==",
             "resolved": "https://registry.npmjs.org/chalk/-/chalk-2.4.2.tgz",
             "version": "2.4.2"
         },
+        "node_modules/chrome-trace-event": {
+            "dev": true,
+            "engines": {
+                "node": ">=6.0"
+            },
+            "integrity": "sha512-p3KULyQg4S7NIHixdwbGX+nFHkoBiA4YQmyWtjb8XngSKV124nJmRysgAeujbUVb15vh+RvFUfCPqU7rXk+hZg==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/chrome-trace-event/-/chrome-trace-event-1.0.3.tgz",
+            "version": "1.0.3"
+        },
+        "node_modules/classnames": {
+            "integrity": "sha512-CSbhY4cFEJRe6/GQzIk5qXZ4Jeg5pcsP7b5peFSDpffpe1cqjASH/n9UTjBwOp6XpMSTwQ8Za2K5V02ueA7Tmw==",
+            "resolved": "https://registry.npmjs.org/classnames/-/classnames-2.3.2.tgz",
+            "version": "2.3.2"
+        },
         "node_modules/color-convert": {
             "dependencies": {
                 "color-name": "1.1.3"
             },
             "dev": true,
             "integrity": "sha512-QfAUtd+vFdAtFQcC8CCyYt1fYWxSqAiK2cSD6zDB8N3cpsEBAvRxp9zOGg6G/SHHJYAT88/az/IuDGALsNVbGg==",
             "resolved": "https://registry.npmjs.org/color-convert/-/color-convert-1.9.3.tgz",
@@ -1298,14 +1667,19 @@
             "engines": {
                 "node": ">= 8"
             },
             "integrity": "sha512-iRDPJKUPVEND7dHPO8rkbOnPpyDygcDFtWjpeWNCgy8WP2rXcxXL8TskReQl6OrB2G7+UJrags1q15Fudc7G6w==",
             "resolved": "https://registry.npmjs.org/cross-spawn/-/cross-spawn-7.0.3.tgz",
             "version": "7.0.3"
         },
+        "node_modules/csstype": {
+            "integrity": "sha512-I7K1Uu0MBPzaFKg4nI5Q7Vs2t+3gWWW648spaF+Rg7pI9ds18Ugn+lvg4SHczUdKlHI5LWBXyqfS8+DufyBsgQ==",
+            "resolved": "https://registry.npmjs.org/csstype/-/csstype-3.1.2.tgz",
+            "version": "3.1.2"
+        },
         "node_modules/debug": {
             "dependencies": {
                 "ms": "2.1.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=6.0"
@@ -1337,32 +1711,62 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-xvqAVKGfT1+UAvPwKTVw/njhdQ8ZhXK4lI0bCIuCMrp2up9nPnaDftrLtmpTazqd1o+UY4zgzU+avtMbDP+ldA==",
             "resolved": "https://registry.npmjs.org/define-properties/-/define-properties-1.2.0.tgz",
             "version": "1.2.0"
         },
+        "node_modules/dequal": {
+            "engines": {
+                "node": ">=6"
+            },
+            "integrity": "sha512-0je+qPKHEMohvfRTCEo3CrPG6cAzAYgmzKyxRiYSSDkS6eGJdyVJm7WaYA5ECaAD9wLB2T4EEeymA5aFVcYXCA==",
+            "resolved": "https://registry.npmjs.org/dequal/-/dequal-2.0.3.tgz",
+            "version": "2.0.3"
+        },
         "node_modules/doctrine": {
             "dependencies": {
                 "esutils": "^2.0.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=6.0.0"
             },
             "integrity": "sha512-yS+Q5i3hBf7GBkd4KG8a7eBNNWNGLTaEwwYWUijIYM7zrlYDM0BFXHjjPWlWZ1Rg7UaddZeIDmi9jF3HmqiQ2w==",
             "resolved": "https://registry.npmjs.org/doctrine/-/doctrine-3.0.0.tgz",
             "version": "3.0.0"
         },
+        "node_modules/dom-helpers": {
+            "dependencies": {
+                "@babel/runtime": "^7.8.7",
+                "csstype": "^3.0.2"
+            },
+            "integrity": "sha512-nRCa7CK3VTrM2NmGkIy4cbK7IZlgBE/PYMn55rrXefr5xXDP0LdtfPnblFDoVdcAfslJ7or6iqAUnx0CCGIWQA==",
+            "resolved": "https://registry.npmjs.org/dom-helpers/-/dom-helpers-5.2.1.tgz",
+            "version": "5.2.1"
+        },
         "node_modules/electron-to-chromium": {
             "dev": true,
             "integrity": "sha512-r6dCgNpRhPwiWlxbHzZQ/d9swfPaEJGi8ekqRBwQYaR3WmA5VkqQfBWSDDjuJU1ntO+W9tHx8OHV/96Q8e0dVw==",
             "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.440.tgz",
             "version": "1.4.440"
         },
+        "node_modules/enhanced-resolve": {
+            "dependencies": {
+                "graceful-fs": "^4.2.4",
+                "tapable": "^2.2.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=10.13.0"
+            },
+            "integrity": "sha512-LXYT42KJ7lpIKECr2mAXIaMldcNCh/7E0KBKOu4KSfkHmP+mZmSs+8V5gBAqisWBy0OO4W5Oyys0GO1Y8KtdKg==",
+            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.15.0.tgz",
+            "version": "5.15.0"
+        },
         "node_modules/es-abstract": {
             "dependencies": {
                 "array-buffer-byte-length": "^1.0.0",
                 "available-typed-arrays": "^1.0.5",
                 "call-bind": "^1.0.2",
                 "es-set-tostringtag": "^2.0.1",
                 "es-to-primitive": "^1.2.1",
@@ -1403,14 +1807,21 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-y/B5POM2iBnIxCiernH1G7rC9qQoM77lLIMQLuob0zhp8C56Po81+2Nj0WFKnd0pNReDTnkYryc+zhOzpEIROg==",
             "resolved": "https://registry.npmjs.org/es-abstract/-/es-abstract-1.21.2.tgz",
             "version": "1.21.2"
         },
+        "node_modules/es-module-lexer": {
+            "dev": true,
+            "integrity": "sha512-vZK7T0N2CBmBOixhmjdqx2gWVbFZ4DXZ/NyRMZVlJXPa7CyFS+/a4QQsDGDQy9ZfEzxFuNEsMLeQJnKP2p5/JA==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-1.3.0.tgz",
+            "version": "1.3.0"
+        },
         "node_modules/es-set-tostringtag": {
             "dependencies": {
                 "get-intrinsic": "^1.1.3",
                 "has": "^1.0.3",
                 "has-tostringtag": "^1.0.0"
             },
             "dev": true,
@@ -1595,23 +2006,14 @@
             "integrity": "sha512-oFc7Itz9Qxh2x4gNHStv3BqJq54ExXmfC+a1NjAta66IAN87Wu0R/QArgIS9qKzX3dXKPI9H5crl9QchNMY9+g==",
             "peerDependencies": {
                 "eslint": "^3.0.0 || ^4.0.0 || ^5.0.0 || ^6.0.0 || ^7.0.0 || ^8.0.0-0"
             },
             "resolved": "https://registry.npmjs.org/eslint-plugin-react-hooks/-/eslint-plugin-react-hooks-4.6.0.tgz",
             "version": "4.6.0"
         },
-        "node_modules/eslint-plugin-react-refresh": {
-            "dev": true,
-            "integrity": "sha512-QgrvtRJkmV+m4w953LS146+6RwEe5waouubFVNLBfOjXJf6MLczjymO8fOcKj9jMS8aKkTCMJqiPu2WEeFI99A==",
-            "peerDependencies": {
-                "eslint": ">=7"
-            },
-            "resolved": "https://registry.npmjs.org/eslint-plugin-react-refresh/-/eslint-plugin-react-refresh-0.4.1.tgz",
-            "version": "0.4.1"
-        },
         "node_modules/eslint-plugin-react/node_modules/doctrine": {
             "dependencies": {
                 "esutils": "^2.0.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=0.10.0"
@@ -1809,14 +2211,24 @@
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-kVscqXk4OCp68SZ0dkgEKVi6/8ij300KBWTJq32P/dYeWTSwK41WyTxalN1eRmA5Z9UU/LX9D7FWSmV9SAYx6g==",
             "resolved": "https://registry.npmjs.org/esutils/-/esutils-2.0.3.tgz",
             "version": "2.0.3"
         },
+        "node_modules/events": {
+            "dev": true,
+            "engines": {
+                "node": ">=0.8.x"
+            },
+            "integrity": "sha512-mQw+2fkQbALzQ7V0MY0IqdnXNOeTtP4r0lN9z7AAawCXgqea7bDii20AYrIBrFd/Hx0M2Ocz6S111CaFkUcb0Q==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/events/-/events-3.3.0.tgz",
+            "version": "3.3.0"
+        },
         "node_modules/fast-deep-equal": {
             "dev": true,
             "integrity": "sha512-f3qQ9oQy9j2AhBe/H9VC91wLmKBCCU/gDOnKNAYG5hswO7BLKj09Hc5HYNz9cGI++xlpDCIgDaitVs03ATR84Q==",
             "resolved": "https://registry.npmjs.org/fast-deep-equal/-/fast-deep-equal-3.1.3.tgz",
             "version": "3.1.3"
         },
         "node_modules/fast-json-stable-stringify": {
@@ -1848,14 +2260,26 @@
             "engines": {
                 "node": "^10.12.0 || >=12.0.0"
             },
             "integrity": "sha512-7Gps/XWymbLk2QLYK4NzpMOrYjMhdIxXuIvy2QBsLE6ljuodKvdkWs/cpyJJ3CVIVpH0Oi1Hvg1ovbMzLdFBBg==",
             "resolved": "https://registry.npmjs.org/file-entry-cache/-/file-entry-cache-6.0.1.tgz",
             "version": "6.0.1"
         },
+        "node_modules/fill-range": {
+            "dependencies": {
+                "to-regex-range": "^5.0.1"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=8"
+            },
+            "integrity": "sha512-qOo9F+dMUmC2Lcb4BbVvnKJxTPjCm+RRpe4gDuGrzkL7mEVl/djYSu2OdQ2Pa302N4oqkSg9ir6jaLWJ2USVpQ==",
+            "resolved": "https://registry.npmjs.org/fill-range/-/fill-range-7.0.1.tgz",
+            "version": "7.0.1"
+        },
         "node_modules/find-up": {
             "dependencies": {
                 "locate-path": "^6.0.0",
                 "path-exists": "^4.0.0"
             },
             "dev": true,
             "engines": {
@@ -2017,14 +2441,21 @@
             "engines": {
                 "node": ">=10.13.0"
             },
             "integrity": "sha512-XxwI8EOhVQgWp6iDL+3b0r86f4d6AX6zSU55HfB4ydCEuXLXc5FcYeOu+nnGftS4TEju/11rt4KJPTMgbfmv4A==",
             "resolved": "https://registry.npmjs.org/glob-parent/-/glob-parent-6.0.2.tgz",
             "version": "6.0.2"
         },
+        "node_modules/glob-to-regexp": {
+            "dev": true,
+            "integrity": "sha512-lkX1HJXwyMcprw/5YUZc2s7DrpAiHB21/V+E1rHUrVNokkvB6bqMzT0VfV6/86ZNabt1k14YOIaT7nDvOX3Iiw==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/glob-to-regexp/-/glob-to-regexp-0.4.1.tgz",
+            "version": "0.4.1"
+        },
         "node_modules/globals": {
             "dev": true,
             "engines": {
                 "node": ">=4"
             },
             "integrity": "sha512-WOBp/EEGUiIsJSp7wcv/y6MO+lV9UoncWqxuFfm8eBwzWNgyfBd6Gz+IeKQ9jCmyhoH99g15M3T+QaVHFjizVA==",
             "resolved": "https://registry.npmjs.org/globals/-/globals-11.12.0.tgz",
@@ -2053,14 +2484,20 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-d65bNlIadxvpb/A2abVdlqKqV563juRnZ1Wtk6s1sIR8uNsXR70xqIzVqxVf1eTqDunwT2MkczEeaezCKTZhwA==",
             "resolved": "https://registry.npmjs.org/gopd/-/gopd-1.0.1.tgz",
             "version": "1.0.1"
         },
+        "node_modules/graceful-fs": {
+            "dev": true,
+            "integrity": "sha512-RbJ5/jmFcNNCcDV5o9eTnBLJ/HszWV0P73bc+Ff4nS/rJj+YaS6IGyiOL0VoBYX+l1Wrl3k63h/KrH+nhJ0XvQ==",
+            "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.11.tgz",
+            "version": "4.2.11"
+        },
         "node_modules/graphemer": {
             "dev": true,
             "integrity": "sha512-EtKwoO6kxCL9WO5xipiHTZlSzBm7WLT627TqC/uVRd0HKmq8NXyebnNYxDoBi7wt8eTWrUrKXCOVaFq9x1kgag==",
             "resolved": "https://registry.npmjs.org/graphemer/-/graphemer-1.4.0.tgz",
             "version": "1.4.0"
         },
         "node_modules/has": {
@@ -2204,14 +2641,22 @@
             "engines": {
                 "node": ">= 0.4"
             },
             "integrity": "sha512-Y+R5hJrzs52QCG2laLn4udYVnxsfny9CpOhNhUvk/SSSVyF6T27FzRbF0sroPidSu3X8oEAkOn2K804mjpt6UQ==",
             "resolved": "https://registry.npmjs.org/internal-slot/-/internal-slot-1.0.5.tgz",
             "version": "1.0.5"
         },
+        "node_modules/invariant": {
+            "dependencies": {
+                "loose-envify": "^1.0.0"
+            },
+            "integrity": "sha512-phJfQVBuaJM5raOpJjSfkiD6BpbCE4Ns//LaXl6wGYtUBY83nWS6Rf9tXm2e8VaK60JEjYldbPif/A2B1C2gNA==",
+            "resolved": "https://registry.npmjs.org/invariant/-/invariant-2.2.4.tgz",
+            "version": "2.2.4"
+        },
         "node_modules/is-array-buffer": {
             "dependencies": {
                 "call-bind": "^1.0.2",
                 "get-intrinsic": "^1.2.0",
                 "is-typed-array": "^1.1.10"
             },
             "dev": true,
@@ -2318,14 +2763,23 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-dqJvarLawXsFbNDeJW7zAz8ItJ9cd28YufuuFzh0G8pNHjJMnY08Dv7sYX2uF5UpQOwieAeOExEYAWWfu7ZZUA==",
             "resolved": "https://registry.npmjs.org/is-negative-zero/-/is-negative-zero-2.0.2.tgz",
             "version": "2.0.2"
         },
+        "node_modules/is-number": {
+            "dev": true,
+            "engines": {
+                "node": ">=0.12.0"
+            },
+            "integrity": "sha512-41Cifkg6e8TylSpdtTpeLVMqvSBEVzTttHvERD741+pnZ8ANv0004MRL43QKPDlK9cGvNp6NZWZUBlbGXYxxng==",
+            "resolved": "https://registry.npmjs.org/is-number/-/is-number-7.0.0.tgz",
+            "version": "7.0.0"
+        },
         "node_modules/is-number-object": {
             "dependencies": {
                 "has-tostringtag": "^1.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">= 0.4"
@@ -2437,14 +2891,55 @@
         },
         "node_modules/isexe": {
             "dev": true,
             "integrity": "sha512-RHxMLp9lnKHGHRng9QFhRCMbYAcVpn69smSGcq3f36xjgVVWThj4qqLbTLlq7Ssj8B+fIQ1EuCEGI2lKsyQeIw==",
             "resolved": "https://registry.npmjs.org/isexe/-/isexe-2.0.0.tgz",
             "version": "2.0.0"
         },
+        "node_modules/jest-worker": {
+            "dependencies": {
+                "@types/node": "*",
+                "merge-stream": "^2.0.0",
+                "supports-color": "^8.0.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">= 10.13.0"
+            },
+            "integrity": "sha512-7vuh85V5cdDofPyxn58nrPjBktZo0u9x1g8WtjQol+jZDaE+fhN+cIvTj11GndBnMnyfrUOG1sZQxCdjKh+DKg==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/jest-worker/-/jest-worker-27.5.1.tgz",
+            "version": "27.5.1"
+        },
+        "node_modules/jest-worker/node_modules/has-flag": {
+            "dev": true,
+            "engines": {
+                "node": ">=8"
+            },
+            "integrity": "sha512-EykJT/Q1KjTWctppgIAgfSO0tKVuZUjhgMr17kqTumMl6Afv3EISleU7qZUzoXDFTAHTDC4NOoG/ZxU3EvlMPQ==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/has-flag/-/has-flag-4.0.0.tgz",
+            "version": "4.0.0"
+        },
+        "node_modules/jest-worker/node_modules/supports-color": {
+            "dependencies": {
+                "has-flag": "^4.0.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=10"
+            },
+            "funding": {
+                "url": "https://github.com/chalk/supports-color?sponsor=1"
+            },
+            "integrity": "sha512-MpUEN2OodtUzxvKQl72cUF7RQ5EiHsGvSsVG0ia9c5RbWGL2CI4C7EpPS8UTBIplnlzZiNuV56w+FuNxy3ty2Q==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-8.1.1.tgz",
+            "version": "8.1.1"
+        },
         "node_modules/js-tokens": {
             "integrity": "sha512-RdJUflcE3cUzKiMqQgsCu06FPu9UdIJO0beYbPhHN4k6apgJtifcoCtT9bcxOpYBtpD2kCM6Sbzg4CausW/PKQ==",
             "resolved": "https://registry.npmjs.org/js-tokens/-/js-tokens-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/js-yaml": {
             "bin": {
@@ -2466,14 +2961,21 @@
             "engines": {
                 "node": ">=4"
             },
             "integrity": "sha512-OYu7XEzjkCQ3C5Ps3QIZsQfNpqoJyZZA99wd9aWd05NCtC5pWOkShK2mkL6HXQR6/Cy2lbNdPlZBpuQHXE63gA==",
             "resolved": "https://registry.npmjs.org/jsesc/-/jsesc-2.5.2.tgz",
             "version": "2.5.2"
         },
+        "node_modules/json-parse-even-better-errors": {
+            "dev": true,
+            "integrity": "sha512-xyFwyhro/JEof6Ghe2iz2NcXoj2sloNsWr/XsERDK/oiPCfaNhl5ONfp+jQdAZRQQ0IJWNzH9zIZF7li91kh2w==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/json-parse-even-better-errors/-/json-parse-even-better-errors-2.3.1.tgz",
+            "version": "2.3.1"
+        },
         "node_modules/json-schema-traverse": {
             "dev": true,
             "integrity": "sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==",
             "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-0.4.1.tgz",
             "version": "0.4.1"
         },
         "node_modules/json-stable-stringify-without-jsonify": {
@@ -2516,14 +3018,24 @@
             "engines": {
                 "node": ">= 0.8.0"
             },
             "integrity": "sha512-+bT2uH4E5LGE7h/n3evcS/sQlJXCpIp6ym8OWJ5eV6+67Dsql/LaaT7qJBAt2rzfoa/5QBGBhxDix1dMt2kQKQ==",
             "resolved": "https://registry.npmjs.org/levn/-/levn-0.4.1.tgz",
             "version": "0.4.1"
         },
+        "node_modules/loader-runner": {
+            "dev": true,
+            "engines": {
+                "node": ">=6.11.5"
+            },
+            "integrity": "sha512-3R/1M+yS3j5ou80Me59j7F9IMs4PXs3VqRrm0TU3AbKPxlmpoY1TNscJV/oGJXo8qCatFGTfDbY6W6ipGOYXfg==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/loader-runner/-/loader-runner-4.3.0.tgz",
+            "version": "4.3.0"
+        },
         "node_modules/locate-path": {
             "dependencies": {
                 "p-locate": "^5.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
@@ -2557,14 +3069,57 @@
                 "yallist": "^3.0.2"
             },
             "dev": true,
             "integrity": "sha512-KpNARQA3Iwv+jTA0utUVVbrh+Jlrr1Fv0e56GGzAFOXN7dk/FviaDW8LHmK52DlcH4WP2n6gI8vN1aesBFgo9w==",
             "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-5.1.1.tgz",
             "version": "5.1.1"
         },
+        "node_modules/merge-stream": {
+            "dev": true,
+            "integrity": "sha512-abv/qOcuPfk3URPfDzmZU1LKmuw8kT+0nIHvKrKgFrwifol/doWcdA4ZqsWQ8ENrFKkd67Mfpo/LovbIUsbt3w==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/merge-stream/-/merge-stream-2.0.0.tgz",
+            "version": "2.0.0"
+        },
+        "node_modules/micromatch": {
+            "dependencies": {
+                "braces": "^3.0.2",
+                "picomatch": "^2.3.1"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=8.6"
+            },
+            "integrity": "sha512-DMy+ERcEW2q8Z2Po+WNXuw3c5YaUSFjAO5GsJqfEl7UjvtIuFKO6ZrKvcItdy98dwFI2N1tg3zNIdKaQT+aNdA==",
+            "resolved": "https://registry.npmjs.org/micromatch/-/micromatch-4.0.5.tgz",
+            "version": "4.0.5"
+        },
+        "node_modules/mime-db": {
+            "dev": true,
+            "engines": {
+                "node": ">= 0.6"
+            },
+            "integrity": "sha512-sPU4uV7dYlvtWJxwwxHD0PuihVNiE7TyAbQ5SWxDCB9mUYvOgroQOwYQQOKPJ8CIbE+1ETVlOoK1UC2nU3gYvg==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/mime-db/-/mime-db-1.52.0.tgz",
+            "version": "1.52.0"
+        },
+        "node_modules/mime-types": {
+            "dependencies": {
+                "mime-db": "1.52.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">= 0.6"
+            },
+            "integrity": "sha512-ZDY+bPm5zTTF+YpCrAU9nK0UgICYPT0QtT1NZWFv4s++TNkcgVaT0g6+4R2uI4MjQjzysHB1zxuWL50hzaeXiw==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/mime-types/-/mime-types-2.1.35.tgz",
+            "version": "2.1.35"
+        },
         "node_modules/minimatch": {
             "dependencies": {
                 "brace-expansion": "^1.1.7"
             },
             "dev": true,
             "engines": {
                 "node": "*"
@@ -2607,14 +3162,21 @@
         },
         "node_modules/natural-compare": {
             "dev": true,
             "integrity": "sha512-OWND8ei3VtNC9h7V60qff3SVobHr996CTwgxubgyQYEpg290h9J0buyECNNJexkFm5sOajh5G116RYA1c8ZMSw==",
             "resolved": "https://registry.npmjs.org/natural-compare/-/natural-compare-1.4.0.tgz",
             "version": "1.4.0"
         },
+        "node_modules/neo-async": {
+            "dev": true,
+            "integrity": "sha512-Yd3UES5mWCSqR+qNT93S3UoYUkqAZ9lLg8a7g9rimsWmYGK8cVToA4/sF3RrshdyV3sAGMXVUmpMYOw+dLpOuw==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/neo-async/-/neo-async-2.6.2.tgz",
+            "version": "2.6.2"
+        },
         "node_modules/node-releases": {
             "dev": true,
             "integrity": "sha512-QzsYKWhXTWx8h1kIvqfnC++o0pEmpRQA/aenALsL2F4pqNVr7YzcdMlDij5WBnwftRbJCNJL/O7zdKaxKPHqgQ==",
             "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.12.tgz",
             "version": "2.0.12"
         },
         "node_modules/object-assign": {
@@ -2825,14 +3387,26 @@
         },
         "node_modules/picocolors": {
             "dev": true,
             "integrity": "sha512-1fygroTLlHu66zi26VoTDv8yRgm0Fccecssto+MhsZ0D/DGW2sm8E8AjW7NU5VVTRt5GxbeZ5qBuJr+HyLYkjQ==",
             "resolved": "https://registry.npmjs.org/picocolors/-/picocolors-1.0.0.tgz",
             "version": "1.0.0"
         },
+        "node_modules/picomatch": {
+            "dev": true,
+            "engines": {
+                "node": ">=8.6"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/jonschlinkert"
+            },
+            "integrity": "sha512-JU3teHTNjmE2VCGFzuY8EXzCDVwEqB2a8fsIvwaStHhAWJEeVd1o1QD80CU6+ZdEXXSLbSsuLwJjkCBWqRQUVA==",
+            "resolved": "https://registry.npmjs.org/picomatch/-/picomatch-2.3.1.tgz",
+            "version": "2.3.1"
+        },
         "node_modules/postcss": {
             "dependencies": {
                 "nanoid": "^3.3.6",
                 "picocolors": "^1.0.0",
                 "source-map-js": "^1.0.2"
             },
             "dev": true,
@@ -2872,14 +3446,26 @@
                 "object-assign": "^4.1.1",
                 "react-is": "^16.13.1"
             },
             "integrity": "sha512-oj87CgZICdulUohogVAR7AjlC0327U4el4L6eAvOqCeudMDVU0NThNaV+b9Df4dXgSP1gXMTnPdhfe/2qDH5cg==",
             "resolved": "https://registry.npmjs.org/prop-types/-/prop-types-15.8.1.tgz",
             "version": "15.8.1"
         },
+        "node_modules/prop-types-extra": {
+            "dependencies": {
+                "react-is": "^16.3.2",
+                "warning": "^4.0.0"
+            },
+            "integrity": "sha512-59+AHNnHYCdiC+vMwY52WmvP5dM3QLeoumYuEyceQDi9aEhtwN9zIQ2ZNo25sMyXnbh32h+P1ezDsUpUH3JAew==",
+            "peerDependencies": {
+                "react": ">=0.14.0"
+            },
+            "resolved": "https://registry.npmjs.org/prop-types-extra/-/prop-types-extra-1.1.1.tgz",
+            "version": "1.1.1"
+        },
         "node_modules/punycode": {
             "dev": true,
             "engines": {
                 "node": ">=6"
             },
             "integrity": "sha512-rRV+zQD8tVFys26lAGR9WUuS4iUAngJScM+ZRSKtvl5tKeZ2t5bvdNFdNHBW9FWR4guGHlgmsZ1G7BSm2wTbuA==",
             "resolved": "https://registry.npmjs.org/punycode/-/punycode-2.3.0.tgz",
@@ -2901,25 +3487,64 @@
                     "url": "https://feross.org/support"
                 }
             ],
             "integrity": "sha512-NuaNSa6flKT5JaSYQzJok04JzTL1CA6aGhv5rfLW3PgqA+M2ChpZQnAC8h8i4ZFkBS8X5RqkDBHA7r4hej3K9A==",
             "resolved": "https://registry.npmjs.org/queue-microtask/-/queue-microtask-1.2.3.tgz",
             "version": "1.2.3"
         },
+        "node_modules/randombytes": {
+            "dependencies": {
+                "safe-buffer": "^5.1.0"
+            },
+            "dev": true,
+            "integrity": "sha512-vYl3iOX+4CKUWuxGi9Ukhie6fsqXqS9FE2Zaic4tNFD2N2QQaXOMFbuKK4QmDHC0JO6B1Zp41J0LpT0oR68amQ==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/randombytes/-/randombytes-2.1.0.tgz",
+            "version": "2.1.0"
+        },
         "node_modules/react": {
             "dependencies": {
                 "loose-envify": "^1.1.0"
             },
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-/3IjMdb2L9QbBdWiW5e3P2/npwMBaU9mHCSCUzNln0ZCYbcfTsGbTJrU/kGemdH2IWmB2ioZ+zkxtmq6g09fGQ==",
             "resolved": "https://registry.npmjs.org/react/-/react-18.2.0.tgz",
             "version": "18.2.0"
         },
+        "node_modules/react-bootstrap": {
+            "dependencies": {
+                "@babel/runtime": "^7.21.0",
+                "@restart/hooks": "^0.4.9",
+                "@restart/ui": "^1.6.3",
+                "@types/react-transition-group": "^4.4.5",
+                "classnames": "^2.3.2",
+                "dom-helpers": "^5.2.1",
+                "invariant": "^2.2.4",
+                "prop-types": "^15.8.1",
+                "prop-types-extra": "^1.1.0",
+                "react-transition-group": "^4.4.5",
+                "uncontrollable": "^7.2.1",
+                "warning": "^4.0.3"
+            },
+            "integrity": "sha512-e/aNtxl0Z2ozrIaR82jr6Zz7ss9GSoaXpQaxmvtDUsTZIq/XalkduR/ZXP6vbQHz2T4syvjA+4FbtwELxxmpww==",
+            "peerDependencies": {
+                "@types/react": ">=16.14.8",
+                "react": ">=16.14.0",
+                "react-dom": ">=16.14.0"
+            },
+            "peerDependenciesMeta": {
+                "@types/react": {
+                    "optional": true
+                }
+            },
+            "resolved": "https://registry.npmjs.org/react-bootstrap/-/react-bootstrap-2.8.0.tgz",
+            "version": "2.8.0"
+        },
         "node_modules/react-bootstrap-icons": {
             "dependencies": {
                 "prop-types": "^15.7.2"
             },
             "integrity": "sha512-j4hSby6gT9/enhl3ybB1tfr1slZNAYXDVntcRrmVjxB3//2WwqrzpESVqKhyayYVaWpEtnwf9wgUQ03cuziwrw==",
             "peerDependencies": {
                 "react": ">=16.8.6"
@@ -2940,14 +3565,19 @@
             "version": "18.2.0"
         },
         "node_modules/react-is": {
             "integrity": "sha512-24e6ynE2H+OKt4kqsOvNd8kBpV65zoxbA4BVsEOB3ARVWQki/DHzaUoC5KuON/BiccDaCCTZBuOcfZs70kR8bQ==",
             "resolved": "https://registry.npmjs.org/react-is/-/react-is-16.13.1.tgz",
             "version": "16.13.1"
         },
+        "node_modules/react-lifecycles-compat": {
+            "integrity": "sha512-fBASbA6LnOU9dOU2eW7aQ8xmYBSXUIWr+UmF9b1efZBazGNO+rcXT/icdKnYm2pTwcRylVUYwW7H1PHfLekVzA==",
+            "resolved": "https://registry.npmjs.org/react-lifecycles-compat/-/react-lifecycles-compat-3.0.4.tgz",
+            "version": "3.0.4"
+        },
         "node_modules/react-router": {
             "dependencies": {
                 "@remix-run/router": "1.6.3"
             },
             "engines": {
                 "node": ">=14"
             },
@@ -2970,14 +3600,34 @@
             "peerDependencies": {
                 "react": ">=16.8",
                 "react-dom": ">=16.8"
             },
             "resolved": "https://registry.npmjs.org/react-router-dom/-/react-router-dom-6.13.0.tgz",
             "version": "6.13.0"
         },
+        "node_modules/react-transition-group": {
+            "dependencies": {
+                "@babel/runtime": "^7.5.5",
+                "dom-helpers": "^5.0.1",
+                "loose-envify": "^1.4.0",
+                "prop-types": "^15.6.2"
+            },
+            "integrity": "sha512-pZcd1MCJoiKiBR2NRxeCRg13uCXbydPnmB4EOeRrY7480qNWO8IIgQG6zlDkm6uRMsURXPuKq0GWtiM59a5Q6g==",
+            "peerDependencies": {
+                "react": ">=16.6.0",
+                "react-dom": ">=16.6.0"
+            },
+            "resolved": "https://registry.npmjs.org/react-transition-group/-/react-transition-group-4.4.5.tgz",
+            "version": "4.4.5"
+        },
+        "node_modules/regenerator-runtime": {
+            "integrity": "sha512-kY1AZVr2Ra+t+piVaJ4gxaFaReZVH40AKNo7UCX6W+dEwBo/2oZJzqfuN1qLq1oL45o56cPaTXELwrTh8Fpggg==",
+            "resolved": "https://registry.npmjs.org/regenerator-runtime/-/regenerator-runtime-0.13.11.tgz",
+            "version": "0.13.11"
+        },
         "node_modules/regexp.prototype.flags": {
             "dependencies": {
                 "call-bind": "^1.0.2",
                 "define-properties": "^1.2.0",
                 "functions-have-names": "^1.2.3"
             },
             "dev": true,
@@ -3061,14 +3711,35 @@
                     "url": "https://feross.org/support"
                 }
             ],
             "integrity": "sha512-5l4VyZR86LZ/lDxZTR6jqL8AFE2S0IFLMP26AbjsLVADxHdhB/c0GUsH+y39UfCi3dzz8OlQuPmnaJOMoDHQBA==",
             "resolved": "https://registry.npmjs.org/run-parallel/-/run-parallel-1.2.0.tgz",
             "version": "1.2.0"
         },
+        "node_modules/safe-buffer": {
+            "dev": true,
+            "funding": [
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/feross"
+                },
+                {
+                    "type": "patreon",
+                    "url": "https://www.patreon.com/feross"
+                },
+                {
+                    "type": "consulting",
+                    "url": "https://feross.org/support"
+                }
+            ],
+            "integrity": "sha512-rp3So07KcdmmKbGvgaNxQSJr7bGVSVk5S9Eq1F+ppbRo70+YeaDxkw5Dd8NPN+GD6bjnYm2VuPuCXmpuYvmCXQ==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/safe-buffer/-/safe-buffer-5.2.1.tgz",
+            "version": "5.2.1"
+        },
         "node_modules/safe-regex-test": {
             "dependencies": {
                 "call-bind": "^1.0.2",
                 "get-intrinsic": "^1.1.3",
                 "is-regex": "^1.1.4"
             },
             "dev": true,
@@ -3083,14 +3754,76 @@
             "dependencies": {
                 "loose-envify": "^1.1.0"
             },
             "integrity": "sha512-CtuThmgHNg7zIZWAXi3AsyIzA3n4xx7aNyjwC2VJldO2LMVDhFK+63xGqq6CsJH4rTAt6/M+N4GhZiDYPx9eUw==",
             "resolved": "https://registry.npmjs.org/scheduler/-/scheduler-0.23.0.tgz",
             "version": "0.23.0"
         },
+        "node_modules/schema-utils": {
+            "dependencies": {
+                "@types/json-schema": "^7.0.8",
+                "ajv": "^6.12.5",
+                "ajv-keywords": "^3.5.2"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">= 10.13.0"
+            },
+            "funding": {
+                "type": "opencollective",
+                "url": "https://opencollective.com/webpack"
+            },
+            "integrity": "sha512-pN/yOAvcC+5rQ5nERGuwrjLlYvLTbCibnZ1I7B1LaiAz9BRBlE9GMgE/eqV30P7aJQUf7Ddimy/RsbYO/GrVGg==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.3.0.tgz",
+            "version": "3.3.0"
+        },
+        "node_modules/semver": {
+            "bin": {
+                "semver": "bin/semver.js"
+            },
+            "dependencies": {
+                "lru-cache": "^6.0.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=10"
+            },
+            "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
+            "version": "7.5.3"
+        },
+        "node_modules/semver/node_modules/lru-cache": {
+            "dependencies": {
+                "yallist": "^4.0.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=10"
+            },
+            "integrity": "sha512-Jo6dJ04CmSjuznwJSS3pUeWmd/H0ffTlkXXgwZi+eq1UCmqQwCh+eLsYOYCwY991i2Fah4h1BEMCx4qThGbsiA==",
+            "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
+            "version": "6.0.0"
+        },
+        "node_modules/semver/node_modules/yallist": {
+            "dev": true,
+            "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
+            "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
+            "version": "4.0.0"
+        },
+        "node_modules/serialize-javascript": {
+            "dependencies": {
+                "randombytes": "^2.1.0"
+            },
+            "dev": true,
+            "integrity": "sha512-owoXEFjWRllis8/M1Q+Cw5k8ZH40e3zhp/ovX+Xr/vi1qj6QesbyXXViFbpNvWvPNAD62SutwEXavefrLJWj7w==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-6.0.1.tgz",
+            "version": "6.0.1"
+        },
         "node_modules/shebang-command": {
             "dependencies": {
                 "shebang-regex": "^3.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=8"
@@ -3134,26 +3867,24 @@
         "node_modules/source-map-support": {
             "dependencies": {
                 "buffer-from": "^1.0.0",
                 "source-map": "^0.6.0"
             },
             "dev": true,
             "integrity": "sha512-uBHU3L3czsIyYXKX88fdrGovxdSCoTGDRZ6SYXtSRxLZUzHg5P/66Ht6uoUlHu9EZod+inXhKo3qQgwXUT/y1w==",
-            "optional": true,
             "peer": true,
             "resolved": "https://registry.npmjs.org/source-map-support/-/source-map-support-0.5.21.tgz",
             "version": "0.5.21"
         },
         "node_modules/source-map-support/node_modules/source-map": {
             "dev": true,
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
-            "optional": true,
             "peer": true,
             "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
             "version": "0.6.1"
         },
         "node_modules/string.prototype.matchall": {
             "dependencies": {
                 "call-bind": "^1.0.2",
@@ -3262,14 +3993,23 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-ot0WnXS9fgdkgIcePe6RHNk1WA8+muPa6cSjeR3V8K27q9BB1rTE3R1p7Hv0z1ZyAc8s6Vvv8DIyWf681MAt0w==",
             "resolved": "https://registry.npmjs.org/supports-preserve-symlinks-flag/-/supports-preserve-symlinks-flag-1.0.0.tgz",
             "version": "1.0.0"
         },
+        "node_modules/tapable": {
+            "dev": true,
+            "engines": {
+                "node": ">=6"
+            },
+            "integrity": "sha512-GNzQvQTOIP6RyTfE2Qxb8ZVlNmw0n88vp1szwWRimP02mnTsx3Wtn5qRdqY9w2XduFNUgvOwhNnQsjwCp+kqaQ==",
+            "resolved": "https://registry.npmjs.org/tapable/-/tapable-2.2.1.tgz",
+            "version": "2.2.1"
+        },
         "node_modules/terser": {
             "bin": {
                 "terser": "bin/terser"
             },
             "dependencies": {
                 "@jridgewell/source-map": "^0.3.3",
                 "acorn": "^8.8.2",
@@ -3277,23 +4017,56 @@
                 "source-map-support": "~0.5.20"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
             "integrity": "sha512-j1n0Ao919h/Ai5r43VAnfV/7azUYW43GPxK7qSATzrsERfW7+y2QW9Cp9ufnRF5CQUWbnLSo7UJokSWCqg4tsQ==",
-            "optional": true,
             "peer": true,
             "resolved": "https://registry.npmjs.org/terser/-/terser-5.18.1.tgz",
             "version": "5.18.1"
         },
+        "node_modules/terser-webpack-plugin": {
+            "dependencies": {
+                "@jridgewell/trace-mapping": "^0.3.17",
+                "jest-worker": "^27.4.5",
+                "schema-utils": "^3.1.1",
+                "serialize-javascript": "^6.0.1",
+                "terser": "^5.16.8"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">= 10.13.0"
+            },
+            "funding": {
+                "type": "opencollective",
+                "url": "https://opencollective.com/webpack"
+            },
+            "integrity": "sha512-ZuXsqE07EcggTWQjXUj+Aot/OMcD0bMKGgF63f7UxYcu5/AJF53aIpK1YoP5xR9l6s/Hy2b+t1AM0bLNPRuhwA==",
+            "peer": true,
+            "peerDependencies": {
+                "webpack": "^5.1.0"
+            },
+            "peerDependenciesMeta": {
+                "@swc/core": {
+                    "optional": true
+                },
+                "esbuild": {
+                    "optional": true
+                },
+                "uglify-js": {
+                    "optional": true
+                }
+            },
+            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.9.tgz",
+            "version": "5.3.9"
+        },
         "node_modules/terser/node_modules/commander": {
             "dev": true,
             "integrity": "sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==",
-            "optional": true,
             "peer": true,
             "resolved": "https://registry.npmjs.org/commander/-/commander-2.20.3.tgz",
             "version": "2.20.3"
         },
         "node_modules/text-table": {
             "dev": true,
             "integrity": "sha512-N+8UisAXDGk8PFXP4HAzVR9nbfmVJ3zYLAWiTIoqC5v5isinhr+r5uaO8+7r3BMfuNIufIsA7RdpVgacC2cSpw==",
@@ -3305,14 +4078,120 @@
             "engines": {
                 "node": ">=4"
             },
             "integrity": "sha512-/OaKK0xYrs3DmxRYqL/yDc+FxFUVYhDlXMhRmv3z915w2HF1tnN1omB354j8VUGO/hbRzyD6Y3sA7v7GS/ceog==",
             "resolved": "https://registry.npmjs.org/to-fast-properties/-/to-fast-properties-2.0.0.tgz",
             "version": "2.0.0"
         },
+        "node_modules/to-regex-range": {
+            "dependencies": {
+                "is-number": "^7.0.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=8.0"
+            },
+            "integrity": "sha512-65P7iz6X5yEr1cwcgvQxbbIw7Uk3gOy5dIdtZ4rDveLqhrdJP+Li/Hx6tyK0NEb+2GCyneCMJiGqrADCSNk8sQ==",
+            "resolved": "https://registry.npmjs.org/to-regex-range/-/to-regex-range-5.0.1.tgz",
+            "version": "5.0.1"
+        },
+        "node_modules/ts-loader": {
+            "dependencies": {
+                "chalk": "^4.1.0",
+                "enhanced-resolve": "^5.0.0",
+                "micromatch": "^4.0.0",
+                "semver": "^7.3.4"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=12.0.0"
+            },
+            "integrity": "sha512-MLukxDHBl8OJ5Dk3y69IsKVFRA/6MwzEqBgh+OXMPB/OD01KQuWPFd1WAQP8a5PeSCAxfnkhiuWqfmFJzJQt9w==",
+            "peerDependencies": {
+                "typescript": "*",
+                "webpack": "^5.0.0"
+            },
+            "resolved": "https://registry.npmjs.org/ts-loader/-/ts-loader-9.4.4.tgz",
+            "version": "9.4.4"
+        },
+        "node_modules/ts-loader/node_modules/ansi-styles": {
+            "dependencies": {
+                "color-convert": "^2.0.1"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=8"
+            },
+            "funding": {
+                "url": "https://github.com/chalk/ansi-styles?sponsor=1"
+            },
+            "integrity": "sha512-zbB9rCJAT1rbjiVDb2hqKFHNYLxgtk8NURxZ3IZwD3F6NtxbXZQCnnSi1Lkx+IDohdPlFp222wVALIheZJQSEg==",
+            "resolved": "https://registry.npmjs.org/ansi-styles/-/ansi-styles-4.3.0.tgz",
+            "version": "4.3.0"
+        },
+        "node_modules/ts-loader/node_modules/chalk": {
+            "dependencies": {
+                "ansi-styles": "^4.1.0",
+                "supports-color": "^7.1.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=10"
+            },
+            "funding": {
+                "url": "https://github.com/chalk/chalk?sponsor=1"
+            },
+            "integrity": "sha512-oKnbhFyRIXpUuez8iBMmyEa4nbj4IOQyuhc/wy9kY7/WVPcwIO9VA668Pu8RkO7+0G76SLROeyw9CpQ061i4mA==",
+            "resolved": "https://registry.npmjs.org/chalk/-/chalk-4.1.2.tgz",
+            "version": "4.1.2"
+        },
+        "node_modules/ts-loader/node_modules/color-convert": {
+            "dependencies": {
+                "color-name": "~1.1.4"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=7.0.0"
+            },
+            "integrity": "sha512-RRECPsj7iu/xb5oKYcsFHSppFNnsj/52OVTRKb4zP5onXwVF3zVmmToNcOfGC+CRDpfK/U584fMg38ZHCaElKQ==",
+            "resolved": "https://registry.npmjs.org/color-convert/-/color-convert-2.0.1.tgz",
+            "version": "2.0.1"
+        },
+        "node_modules/ts-loader/node_modules/color-name": {
+            "dev": true,
+            "integrity": "sha512-dOy+3AuW3a2wNbZHIuMZpTcgjGuLU/uBL/ubcZF9OXbDo8ff4O8yVp5Bf0efS8uEoYo5q4Fx7dY9OgQGXgAsQA==",
+            "resolved": "https://registry.npmjs.org/color-name/-/color-name-1.1.4.tgz",
+            "version": "1.1.4"
+        },
+        "node_modules/ts-loader/node_modules/has-flag": {
+            "dev": true,
+            "engines": {
+                "node": ">=8"
+            },
+            "integrity": "sha512-EykJT/Q1KjTWctppgIAgfSO0tKVuZUjhgMr17kqTumMl6Afv3EISleU7qZUzoXDFTAHTDC4NOoG/ZxU3EvlMPQ==",
+            "resolved": "https://registry.npmjs.org/has-flag/-/has-flag-4.0.0.tgz",
+            "version": "4.0.0"
+        },
+        "node_modules/ts-loader/node_modules/supports-color": {
+            "dependencies": {
+                "has-flag": "^4.0.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=8"
+            },
+            "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
+            "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
+            "version": "7.2.0"
+        },
+        "node_modules/tslib": {
+            "integrity": "sha512-7At1WUettjcSRHXCyYtTselblcHl9PJFFVKiCAy/bY97+BPZXSQ2wbq0P9s8tK2G7dFQfNnlJnPAiArVBVBsfA==",
+            "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.6.0.tgz",
+            "version": "2.6.0"
+        },
         "node_modules/type-check": {
             "dependencies": {
                 "prelude-ls": "^1.2.1"
             },
             "dev": true,
             "engines": {
                 "node": ">= 0.8.0"
@@ -3343,14 +4222,27 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-KjZypGq+I/H7HI5HlOoGHkWUUGq+Q0TPhQurLbyrVrvnKTBgzLhIJ7j6J/XTQOi0d1RjyZ0wdas8bKs2p0x3Ng==",
             "resolved": "https://registry.npmjs.org/typed-array-length/-/typed-array-length-1.0.4.tgz",
             "version": "1.0.4"
         },
+        "node_modules/typescript": {
+            "bin": {
+                "tsc": "bin/tsc",
+                "tsserver": "bin/tsserver"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=14.17"
+            },
+            "integrity": "sha512-FOH+WN/DQjUvN6WgW+c4Ml3yi0PH+a/8q+kNIfRehv1wLhWONedw85iu+vQ39Wp49IzTJEsZ2lyLXpBF7mkF1g==",
+            "resolved": "https://registry.npmjs.org/typescript/-/typescript-5.1.5.tgz",
+            "version": "5.1.5"
+        },
         "node_modules/unbox-primitive": {
             "dependencies": {
                 "call-bind": "^1.0.2",
                 "has-bigints": "^1.0.2",
                 "has-symbols": "^1.0.3",
                 "which-boxed-primitive": "^1.0.2"
             },
@@ -3358,14 +4250,28 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-61pPlCD9h51VoreyJ0BReideM3MDKMKnh6+V9L08331ipq6Q8OFXZYiqP6n/tbHx4s5I9uRhcye6BrbkizkBDw==",
             "resolved": "https://registry.npmjs.org/unbox-primitive/-/unbox-primitive-1.0.2.tgz",
             "version": "1.0.2"
         },
+        "node_modules/uncontrollable": {
+            "dependencies": {
+                "@babel/runtime": "^7.6.3",
+                "@types/react": ">=16.9.11",
+                "invariant": "^2.2.4",
+                "react-lifecycles-compat": "^3.0.4"
+            },
+            "integrity": "sha512-svtcfoTADIB0nT9nltgjujTi7BzVmwjZClOmskKu/E8FW9BXzg9os8OLr4f8Dlnk0rYWJIWr4wv9eKUXiQvQwQ==",
+            "peerDependencies": {
+                "react": ">=15.0.0"
+            },
+            "resolved": "https://registry.npmjs.org/uncontrollable/-/uncontrollable-7.2.1.tgz",
+            "version": "7.2.1"
+        },
         "node_modules/update-browserslist-db": {
             "bin": {
                 "update-browserslist-db": "cli.js"
             },
             "dependencies": {
                 "escalade": "^3.1.1",
                 "picocolors": "^1.0.0"
@@ -3461,14 +4367,118 @@
             "integrity": "sha512-tywOR+rwIt5m2ZAWSe5AIJcTat8vGlnPFAv15ycCrw33t6iFsXZ6mzHVFh2psSjxQPmI+xgzMZZizUAukBI4aQ==",
             "optionalDependencies": {
                 "fsevents": "~2.3.2"
             },
             "resolved": "https://registry.npmjs.org/rollup/-/rollup-3.25.1.tgz",
             "version": "3.25.1"
         },
+        "node_modules/warning": {
+            "dependencies": {
+                "loose-envify": "^1.0.0"
+            },
+            "integrity": "sha512-rpJyN222KWIvHJ/F53XSZv0Zl/accqHR8et1kpaMTD/fLCRxtV8iX8czMzY7sVZupTI3zcUTg8eycS2kNF9l6w==",
+            "resolved": "https://registry.npmjs.org/warning/-/warning-4.0.3.tgz",
+            "version": "4.0.3"
+        },
+        "node_modules/watchpack": {
+            "dependencies": {
+                "glob-to-regexp": "^0.4.1",
+                "graceful-fs": "^4.1.2"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=10.13.0"
+            },
+            "integrity": "sha512-Lcvm7MGST/4fup+ifyKi2hjyIAwcdI4HRgtvTpIUxBRhB+RFtUh8XtDOxUfctVCnhVi+QQj49i91OyvzkJl6cg==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/watchpack/-/watchpack-2.4.0.tgz",
+            "version": "2.4.0"
+        },
+        "node_modules/webpack": {
+            "bin": {
+                "webpack": "bin/webpack.js"
+            },
+            "dependencies": {
+                "@types/eslint-scope": "^3.7.3",
+                "@types/estree": "^1.0.0",
+                "@webassemblyjs/ast": "^1.11.5",
+                "@webassemblyjs/wasm-edit": "^1.11.5",
+                "@webassemblyjs/wasm-parser": "^1.11.5",
+                "acorn": "^8.7.1",
+                "acorn-import-assertions": "^1.9.0",
+                "browserslist": "^4.14.5",
+                "chrome-trace-event": "^1.0.2",
+                "enhanced-resolve": "^5.15.0",
+                "es-module-lexer": "^1.2.1",
+                "eslint-scope": "5.1.1",
+                "events": "^3.2.0",
+                "glob-to-regexp": "^0.4.1",
+                "graceful-fs": "^4.2.9",
+                "json-parse-even-better-errors": "^2.3.1",
+                "loader-runner": "^4.2.0",
+                "mime-types": "^2.1.27",
+                "neo-async": "^2.6.2",
+                "schema-utils": "^3.2.0",
+                "tapable": "^2.1.1",
+                "terser-webpack-plugin": "^5.3.7",
+                "watchpack": "^2.4.0",
+                "webpack-sources": "^3.2.3"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=10.13.0"
+            },
+            "funding": {
+                "type": "opencollective",
+                "url": "https://opencollective.com/webpack"
+            },
+            "integrity": "sha512-FROX3TxQnC/ox4N+3xQoWZzvGXSuscxR32rbzjpXgEzWudJFEJBpdlkkob2ylrv5yzzufD1zph1OoFsLtm6stQ==",
+            "peer": true,
+            "peerDependenciesMeta": {
+                "webpack-cli": {
+                    "optional": true
+                }
+            },
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.88.1.tgz",
+            "version": "5.88.1"
+        },
+        "node_modules/webpack-sources": {
+            "dev": true,
+            "engines": {
+                "node": ">=10.13.0"
+            },
+            "integrity": "sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/webpack-sources/-/webpack-sources-3.2.3.tgz",
+            "version": "3.2.3"
+        },
+        "node_modules/webpack/node_modules/eslint-scope": {
+            "dependencies": {
+                "esrecurse": "^4.3.0",
+                "estraverse": "^4.1.1"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=8.0.0"
+            },
+            "integrity": "sha512-2NxwbF/hZ0KpepYN0cNbo+FN6XoK7GaHlQhgx/hIZl6Va0bF45RQOOwhLIy8lQDbuCiadSLCBnH2CFYquit5bw==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/eslint-scope/-/eslint-scope-5.1.1.tgz",
+            "version": "5.1.1"
+        },
+        "node_modules/webpack/node_modules/estraverse": {
+            "dev": true,
+            "engines": {
+                "node": ">=4.0"
+            },
+            "integrity": "sha512-39nnKffWz8xN1BU/2c79n9nB9HDzo0niYUqx6xyqUnyoAnQyyWpOTdZEeiCch8BBu515t4wp9ZmgVfVhn9EBpw==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/estraverse/-/estraverse-4.3.0.tgz",
+            "version": "4.3.0"
+        },
         "node_modules/which": {
             "bin": {
                 "node-which": "bin/node-which"
             },
             "dependencies": {
                 "isexe": "^2.0.0"
             },
```

### Comparing `bowtie_json_schema-2023.7.2/frontend/package.json` & `bowtie_json_schema-2023.7.3/frontend/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9406415343915344%*

 * *Differences: {"'dependencies'": "{'react-bootstrap': '^2.8.0'}",*

 * * "'devDependencies'": "{'@types/react': '^18.2.14', '@types/react-dom': '^18.2.6', 'ts-loader': "*

 * *                      "'^9.4.4', 'typescript': '^5.1.5'}",*

 * * "'scripts'": "{'build': 'tsc && vite build'}"}*

```diff
@@ -1,26 +1,31 @@
 {
     "dependencies": {
         "bootstrap": "^5.3.0",
         "moment": "^2.29.4",
         "react": "^18.2.0",
+        "react-bootstrap": "^2.8.0",
         "react-bootstrap-icons": "^1.10.3",
         "react-dom": "^18.2.0",
         "react-router-dom": "^6.13.0"
     },
     "description": "The UI displays the outcomes generated by Bowtie, which serves as a meta-validator for the JSON Schema specification",
     "devDependencies": {
+        "@types/react": "^18.2.14",
+        "@types/react-dom": "^18.2.6",
         "@vitejs/plugin-react": "^4.0.1",
         "eslint": "8.43.0",
         "eslint-plugin-react": "7.32.2",
         "eslint-plugin-react-hooks": "4.6.0",
+        "ts-loader": "^9.4.4",
+        "typescript": "^5.1.5",
         "vite": "^4.3.9"
     },
     "name": "bowtie",
     "scripts": {
-        "build": "vite build",
+        "build": "tsc && vite build",
         "lint": "eslint src --ext js,jsx --max-warnings 0",
         "preview": "vite preview",
         "start": "vite"
     },
     "version": "1.0.0"
 }
```

### Comparing `bowtie_json_schema-2023.7.2/frontend/public/favicon.ico` & `bowtie_json_schema-2023.7.3/frontend/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/frontend/src/index.jsx` & `bowtie_json_schema-2023.7.3/frontend/src/index.jsx`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import { createRoot } from "react-dom/client";
 import ReportDataHandler from "./ReportDataHandler";
 import { createHashRouter, RouterProvider } from "react-router-dom";
 import ThemeContextProvider from "./context/ThemeContext";
 import { MainContainer } from "./MainContainer";
 import { BowtieVersionContextProvider } from "./context/BowtieVersionContext";
 import { DragAndDrop } from "./components/DragAndDrop/DragAndDrop";
+import { parseReportData } from "./data/parseReportData";
 
 const reportUrl =
   import.meta.env.MODE === "development"
     ? "https://bowtie-json-schema.github.io/bowtie"
     : import.meta.env.BASE_URL;
 const titleTag = document.getElementsByTagName("title")[0];
 const dialectToName = {
@@ -24,18 +25,19 @@
 };
 
 const fetchReportData = async (dialect) => {
   const dialectName = dialectToName[dialect] ?? dialect;
   titleTag.textContent = `Bowtie - ${dialectName}`;
   const response = await fetch(`${reportUrl}/${dialect}.json`);
   const jsonl = await response.text();
-  return jsonl
+  const lines = jsonl
     .trim()
     .split(/\r?\n/)
     .map((line) => JSON.parse(line));
+  return parseReportData(lines);
 };
 
 const router = createHashRouter([
   {
     path: "/",
     Component: MainContainer,
```

### Comparing `bowtie_json_schema-2023.7.2/frontend/src/components/CopyToClipboard.jsx` & `bowtie_json_schema-2023.7.3/frontend/src/components/CopyToClipboard.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/frontend/src/components/LoadingAnimation.jsx` & `bowtie_json_schema-2023.7.3/frontend/src/components/LoadingAnimation.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/frontend/src/components/NavBar.jsx` & `bowtie_json_schema-2023.7.3/frontend/src/components/NavBar.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/frontend/src/components/Cases/SchemaDisplay.jsx` & `bowtie_json_schema-2023.7.3/frontend/src/components/Cases/SchemaDisplay.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/frontend/src/components/DragAndDrop/DragAndDrop.jsx` & `bowtie_json_schema-2023.7.3/frontend/src/components/DragAndDrop/DragAndDrop.jsx`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import { useRef, useState } from "react";
 import { CloudArrowUpFill } from "react-bootstrap-icons";
 import "./DragAndDrop.css";
 import { ReportView } from "../../ReportView";
+import { parseReportData } from "../../data/parseReportData";
 
 export const DragAndDrop = () => {
   const [dragActive, setDragActive] = useState(false);
   const [invalidFile, setInvalidFile] = useState(false);
   const [lines, setLines] = useState();
   const inputRef = useRef(null);
 
@@ -47,29 +48,29 @@
 
   const handleFiles = (file) => {
     const reader = new FileReader();
     reader.onload = (e) => {
       try {
         const dataObjectsArray = e.target.result.trim().split(/\r?\n/);
         const lines = dataObjectsArray.map((line) => JSON.parse(line));
-        setLines(lines);
+        setLines(parseReportData(lines));
       } catch (error) {
         setInvalidFile(true);
         setTimeout(() => {
           setDragActive(false);
           setInvalidFile(false);
         }, 4000);
         console.error("Error :", error);
       }
     };
     reader.readAsText(file);
   };
 
   if (lines) {
-    return <ReportView lines={lines} />;
+    return <ReportView reportData={lines} />;
   }
 
   return (
     <div>
       <div aria-live="polite" aria-atomic="true"></div>
       <div className="card-body d-grid justify-content-center">
         <form
```

### Comparing `bowtie_json_schema-2023.7.2/frontend/src/components/RunInfo/RunInfoSection.jsx` & `bowtie_json_schema-2023.7.3/frontend/src/components/RunInfo/RunInfoSection.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2023.7.3/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/frontend/src/components/Summary/SummarySection.jsx` & `bowtie_json_schema-2023.7.3/frontend/src/components/Summary/SummarySection.jsx`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-import { RunInfo } from "../../data/runInfo";
 import SummaryTable from "./SummaryTable";
 
-const SummarySection = (props) => {
-  const lines = props.lines;
-  const runInfo = new RunInfo(lines);
-  const summary = runInfo.createSummary();
+const SummarySection = ({ reportData }) => {
   return (
     <div className="card mx-auto mb-3 w-75" id="summary">
       <div className="card-header">Summary</div>
       <div className="card-body">
-        <SummaryTable lines={lines} />
-        {summary.did_fail_fast && (
+        <SummaryTable reportData={reportData} />
+        {reportData.didFailFast && (
           <div className="alert alert-warning" role="alert">
             This run failed fast, so some input cases may not have been run.
           </div>
         )}
       </div>
     </div>
   );
```

### Comparing `bowtie_json_schema-2023.7.2/frontend/src/context/ThemeContext.jsx` & `bowtie_json_schema-2023.7.3/frontend/src/context/ThemeContext.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/tests/test_integration.py` & `bowtie_json_schema-2023.7.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/tests/fauxmplementations/badsonschema/badsonschema` & `bowtie_json_schema-2023.7.3/tests/fauxmplementations/badsonschema/badsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2023.7.3/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/tests/fauxmplementations/lintsonschema/io-schema.json` & `bowtie_json_schema-2023.7.3/tests/fauxmplementations/lintsonschema/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2023.7.3/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/bowtie/templates/report.html.j2` & `bowtie_json_schema-2023.7.3/bowtie/templates/report.html.j2`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/bowtie/schemas/io-schema.json` & `bowtie_json_schema-2023.7.3/bowtie/schemas/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/.gitignore` & `bowtie_json_schema-2023.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/LICENSE` & `bowtie_json_schema-2023.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/README.rst` & `bowtie_json_schema-2023.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/pyproject.toml` & `bowtie_json_schema-2023.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.2/PKG-INFO` & `bowtie_json_schema-2023.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bowtie-json-schema
-Version: 2023.7.2
+Version: 2023.7.3
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://bowtie-json-schema.readthedocs.io/
 Project-URL: Homepage, https://github.com/bowtie-json-schema/bowtie
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author: Julian Berman
 Author-email: Julian+bowtie@GrayVines.com
```

