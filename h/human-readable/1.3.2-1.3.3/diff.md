# Comparing `tmp/human_readable-1.3.2.tar.gz` & `tmp/human_readable-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "human_readable-1.3.2.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `human_readable-1.3.2.tar` & `human_readable-1.3.3.tar`

### file list

```diff
@@ -1,33 +1,77 @@
--rw-r--r--   0        0        0     1056 2023-01-29 17:57:03.198703 human_readable-1.3.2/LICENSE
--rw-r--r--   0        0        0     6846 2023-01-29 17:57:03.198703 human_readable-1.3.2/README.md
--rw-r--r--   0        0        0     1991 2023-01-29 17:57:27.915069 human_readable-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     1116 2023-01-29 17:57:03.198703 human_readable-1.3.2/src/human_readable/__init__.py
--rw-r--r--   0        0        0     1711 2023-01-29 17:57:03.198703 human_readable-1.3.2/src/human_readable/files.py
--rw-r--r--   0        0        0     3294 2023-01-29 17:57:03.198703 human_readable-1.3.2/src/human_readable/i18n.py
--rw-r--r--   0        0        0      937 2023-01-29 17:57:03.198703 human_readable-1.3.2/src/human_readable/lists.py
--rw-r--r--   0        0        0     3539 2023-01-29 17:57:03.198703 human_readable-1.3.2/src/human_readable/locale/de_DE/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     1932 2023-01-29 17:57:03.198703 human_readable-1.3.2/src/human_readable/locale/en_ABBR/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3466 2023-01-29 17:57:03.198703 human_readable-1.3.2/src/human_readable/locale/es_ES/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3053 2023-01-29 17:57:03.198703 human_readable-1.3.2/src/human_readable/locale/fa_IR/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3128 2023-01-29 17:57:03.198703 human_readable-1.3.2/src/human_readable/locale/fi_FI/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     2629 2023-01-29 17:57:03.198703 human_readable-1.3.2/src/human_readable/locale/fr_FR/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3155 2023-01-29 17:57:03.198703 human_readable-1.3.2/src/human_readable/locale/id_ID/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3372 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/locale/it_IT/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3122 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/locale/ja_JP/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     2992 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/locale/ko_KR/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3398 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/locale/nl_NL/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3705 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/locale/pl_PL/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     8663 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/locale/pt_BR/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     4515 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/locale/pt_PT/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     4139 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/locale/ru_RU/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3730 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/locale/sk_SK/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3344 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/locale/tr_TR/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     4290 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/locale/uk_UA/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3199 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/locale/vi_VI/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3280 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/locale/zh_CN/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     3059 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/locale/zh_TW/LC_MESSAGES/human_readable.mo
--rw-r--r--   0        0        0     7260 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/numbers.py
--rw-r--r--   0        0        0        0 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/py.typed
--rw-r--r--   0        0        0    28493 2023-01-29 17:57:03.202703 human_readable-1.3.2/src/human_readable/times.py
--rw-r--r--   0        0        0     9148 1970-01-01 00:00:00.000000 human_readable-1.3.2/setup.py
--rw-r--r--   0        0        0     7892 1970-01-01 00:00:00.000000 human_readable-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 human_readable-1.3.3/.cookiecutter.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 human_readable-1.3.3/.flake8
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 human_readable-1.3.3/.gitattributes
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 human_readable-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 human_readable-1.3.3/.readthedocs.yml
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 human_readable-1.3.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 human_readable-1.3.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 human_readable-1.3.3/bandit.yml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 human_readable-1.3.3/codecov.yml
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/labels.yml
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/release-drafter.yml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/workflows/hatch-constraints.txt
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/workflows/labeler.yml
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 human_readable-1.3.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 human_readable-1.3.3/docs/codeofconduct.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 human_readable-1.3.3/docs/conf.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 human_readable-1.3.3/docs/contributing.md
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 human_readable-1.3.3/docs/index.md
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 human_readable-1.3.3/docs/license.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 human_readable-1.3.3/docs/requirements.txt
+-rw-r--r--   0        0        0     9820 2020-02-02 00:00:00.000000 human_readable-1.3.3/docs/usage.md
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/__init__.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/files.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/i18n.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/lists.py
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/numbers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/py.typed
+-rw-r--r--   0        0        0    28493 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/times.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/de_DE/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/en_ABBR/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/es_ES/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/fa_IR/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/fi_FI/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/fr_FR/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/id_ID/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/it_IT/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/ja_JP/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/ko_KR/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/nl_NL/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/pl_PL/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/pt_BR/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/pt_PT/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/ru_RU/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/sk_SK/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/tr_TR/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/uk_UA/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/vi_VI/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/zh_CN/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 human_readable-1.3.3/src/human_readable/locale/zh_TW/LC_MESSAGES/human_readable.mo
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/__init__.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/conftest.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/en_ABBR/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/en_ABBR/test_numbers.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/en_ABBR/test_times.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/fr_FR/__init__.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/fr_FR/test_numbers.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/pt_BR/__init__.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/pt_BR/test_numbers.py
+-rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/pt_BR/test_times.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/ru_RU/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/ru_RU/test_numbers.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/functional/ru_RU/test_times.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/unit/__init__.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/unit/test_files.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/unit/test_i18n.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/unit/test_lists.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/unit/test_numbers.py
+-rw-r--r--   0        0        0    21943 2020-02-02 00:00:00.000000 human_readable-1.3.3/tests/unit/test_times.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 human_readable-1.3.3/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 human_readable-1.3.3/LICENSE
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 human_readable-1.3.3/README.md
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 human_readable-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 human_readable-1.3.3/PKG-INFO
```

### Comparing `human_readable-1.3.2/LICENSE` & `human_readable-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/README.md` & `human_readable-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/__init__.py` & `human_readable-1.3.3/src/human_readable/__init__.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/files.py` & `human_readable-1.3.3/src/human_readable/files.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/i18n.py` & `human_readable-1.3.3/src/human_readable/i18n.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/lists.py` & `human_readable-1.3.3/src/human_readable/lists.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/de_DE/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/de_DE/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/en_ABBR/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/en_ABBR/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/es_ES/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/es_ES/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/fa_IR/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/fa_IR/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/fi_FI/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/fi_FI/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/fr_FR/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/fr_FR/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/id_ID/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/id_ID/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/it_IT/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/it_IT/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/ja_JP/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/ja_JP/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/ko_KR/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/ko_KR/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/nl_NL/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/nl_NL/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/pl_PL/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/pl_PL/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/pt_BR/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/pt_BR/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/pt_PT/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/pt_PT/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/ru_RU/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/ru_RU/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/sk_SK/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/sk_SK/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/tr_TR/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/tr_TR/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/uk_UA/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/uk_UA/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/vi_VI/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/vi_VI/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/zh_CN/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/zh_CN/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/locale/zh_TW/LC_MESSAGES/human_readable.mo` & `human_readable-1.3.3/src/human_readable/locale/zh_TW/LC_MESSAGES/human_readable.mo`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/numbers.py` & `human_readable-1.3.3/src/human_readable/numbers.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/src/human_readable/times.py` & `human_readable-1.3.3/src/human_readable/times.py`

 * *Files identical despite different names*

### Comparing `human_readable-1.3.2/PKG-INFO` & `human_readable-1.3.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 Metadata-Version: 2.1
 Name: human-readable
-Version: 1.3.2
+Version: 1.3.3
 Summary: Human Readable
-Home-page: https://github.com/staticdev/human-readable
-License: MIT
-Author: staticdev
-Author-email: staticdev-support@proton.me
-Requires-Python: >=3.8
+Project-URL: homepage, https://github.com/staticdev/human-readable
+Project-URL: repository, https://github.com/staticdev/human-readable
+Project-URL: documentation, https://human-readable.readthedocs.io
+Project-URL: changelog, https://github.com/staticdev/human-readable/releases
+Author-email: staticdev <staticdev-support@proton.me>
+License-Expression: MIT
+License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Project-URL: Changelog, https://github.com/staticdev/human-readable/releases
-Project-URL: Documentation, https://human-readable.readthedocs.io
-Project-URL: Repository, https://github.com/staticdev/human-readable
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Human Readable
 
 [![PyPI](https://img.shields.io/pypi/v/human-readable.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/human-readable.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/human-readable)][pypi status]
@@ -295,8 +289,7 @@
 
 [license]: https://github.com/staticdev/human-readable/blob/main/LICENSE
 [contributor guide]: https://github.com/staticdev/human-readable/blob/main/CONTRIBUTING.md
 [cookiecutter]: https://github.com/audreyr/cookiecutter
 [human-readable.readthedocs.io]: https://human-readable.readthedocs.io
 [humanize]: https://github.com/jmoiron/humanize
 [mit]: http://opensource.org/licenses/MIT
-
```

