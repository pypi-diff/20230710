# Comparing `tmp/tomaserial-0.1.1.tar.gz` & `tmp/tomaserial-0.1.2.tar.gz`

## Comparing `tomaserial-0.1.1.tar` & `tomaserial-0.1.2.tar`

### file list

```diff
@@ -1,1988 +1,1988 @@
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 tomaserial-0.1.1/publish.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tomaserial-0.1.1/serial/__init__.py
--rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 tomaserial-0.1.1/serial/serial.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/.gitignore
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/pyvenv.cfg
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/_virtualenv.pth
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/_virtualenv.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/distutils-precedence.pth
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/easy-install.pth
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/serial.egg-link
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools-57.0.0.virtualenv
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/six.py
--rw-r--r--   0        0        0    84065 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/typing_extensions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel-0.36.2.virtualenv
--rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/Pygments-2.14.0.dist-info/AUTHORS
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/Pygments-2.14.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/Pygments-2.14.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/Pygments-2.14.0.dist-info/METADATA
--rw-r--r--   0        0        0    41872 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/Pygments-2.14.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/Pygments-2.14.0.dist-info/WHEEL
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/Pygments-2.14.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/Pygments-2.14.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/_distutils_hack/override.py
--rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/callbacks.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/css_sanitizer.py
--rw-r--r--   0        0        0    22779 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/html5lib_shim.py
--rw-r--r--   0        0        0    22350 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/linkifier.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/parse_shim.py
--rw-r--r--   0        0        0    21934 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/sanitizer.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/__init__.py
--rw-r--r--   0        0        0    39023 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/parse.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/parse.py.SHA256SUM
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/vendor.txt
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/vendor_install.sh
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/__init__.py
--rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/_ihatexml.py
--rw-r--r--   0        0        0    32300 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/_inputstream.py
--rw-r--r--   0        0        0    77028 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/_tokenizer.py
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/_utils.py
--rw-r--r--   0        0        0    83464 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/constants.py
--rw-r--r--   0        0        0   117174 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/html5parser.py
--rw-r--r--   0        0        0    15747 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/serializer.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/__init__.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/_base.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/py.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/__init__.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/base.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/lint.py
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py
--rw-r--r--   0        0        0    26885 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/whitespace.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py
--rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py
--rw-r--r--   0        0        0    14553 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/base.py
--rw-r--r--   0        0        0     8925 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py
--rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py
--rw-r--r--   0        0        0    14754 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py
--rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/base.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py
--rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/AUTHORS.rst
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/LICENSE
--rw-r--r--   0        0        0    16076 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/METADATA
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/REQUESTED
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach-6.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach-6.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0    29799 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach-6.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach-6.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach-6.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/bleach-6.0.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/build-0.10.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/build-0.10.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/build-0.10.0.dist-info/METADATA
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/build-0.10.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/build-0.10.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/build-0.10.0.dist-info/WHEEL
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/build-0.10.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/certifi/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/certifi/__main__.py
--rw-r--r--   0        0        0   275233 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/certifi/cacert.pem
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/certifi/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/certifi/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/certifi-2022.12.7.dist-info/INSTALLER
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/certifi-2022.12.7.dist-info/LICENSE
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/certifi-2022.12.7.dist-info/METADATA
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/certifi-2022.12.7.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/certifi-2022.12.7.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/certifi-2022.12.7.dist-info/top_level.txt
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/__init__.py
--rw-r--r--   0        0        0    19154 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/api.py
--rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/cd.py
--rw-r--r--   0        0        0    19596 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/constant.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/legacy.py
--rw-r--r--   0        0        0    18829 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/md.py
--rw-r--r--   0        0        0    11829 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/py.typed
--rw-r--r--   0        0        0    11966 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/utils.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/version.py
--rw-r--r--   0        0        0    21509 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/assets/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/cli/__init__.py
--rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/cli/normalizer.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/LICENSE
--rw-r--r--   0        0        0    27664 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/METADATA
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/RECORD
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/WHEEL
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/top_level.txt
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama-0.4.6.dist-info/INSTALLER
--rw-r--r--   0        0        0    17158 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama-0.4.6.dist-info/METADATA
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama-0.4.6.dist-info/RECORD
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama-0.4.6.dist-info/WHEEL
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt
--rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/__init__.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/__main__.py
--rw-r--r--   0        0        0    30945 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/core.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/examples.py
--rw-r--r--   0        0        0    39697 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/frontend.py
--rw-r--r--   0        0        0    21271 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/io.py
--rw-r--r--   0        0        0    80986 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/nodes.py
--rw-r--r--   0        0        0    56956 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/statemachine.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/af.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/ar.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/ca.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/cs.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/da.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/de.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/en.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/eo.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/es.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/fa.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/fi.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/fr.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/gl.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/he.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/it.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/ja.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/ko.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/lt.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/lv.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/nl.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/pl.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/pt_br.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/ru.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/sk.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/sv.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/zh_cn.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/zh_tw.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/__init__.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/commonmark_wrapper.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/null.py
--rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py
--rw-r--r--   0        0        0    15985 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/__init__.py
--rw-r--r--   0        0        0    16119 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/roles.py
--rw-r--r--   0        0        0   132550 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/states.py
--rw-r--r--   0        0        0    20912 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/tableparser.py
--rw-r--r--   0        0        0    14653 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/__init__.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py
--rw-r--r--   0        0        0     9883 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/body.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/html.py
--rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/images.py
--rw-r--r--   0        0        0    26770 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/misc.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/parts.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/references.py
--rw-r--r--   0        0        0    22227 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/tables.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/README.txt
--rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsa.txt
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsb.txt
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsc.txt
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsn.txt
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isoamso.txt
--rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsr.txt
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isobox.txt
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr1.txt
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr2.txt
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isodia.txt
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk1.txt
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk2.txt
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk3.txt
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4.txt
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isolat1.txt
--rw-r--r--   0        0        0     8466 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isolat2.txt
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk.txt
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf-wide.txt
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf.txt
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr-wide.txt
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr.txt
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isonum.txt
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isopub.txt
--rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isotech.txt
--rw-r--r--   0        0        0    45428 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/mmlalias.txt
--rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt
--rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra.txt
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/s5defs.txt
--rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-special.txt
--rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/__init__.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/af.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/ar.py
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/ca.py
--rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/cs.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/da.py
--rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/de.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/en.py
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/eo.py
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/es.py
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/fa.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/fi.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/fr.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/gl.py
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/he.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/it.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/ja.py
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/ko.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/lt.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/lv.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/nl.py
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/pl.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/ru.py
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/sk.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/sv.py
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/readers/__init__.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/readers/doctree.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/readers/pep.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/readers/standalone.py
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/__init__.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/components.py
--rw-r--r--   0        0        0    20276 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/frontmatter.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/misc.py
--rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/parts.py
--rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/peps.py
--rw-r--r--   0        0        0    36544 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/references.py
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/universal.py
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/writer_aux.py
--rw-r--r--   0        0        0    28742 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/__init__.py
--rw-r--r--   0        0        0     4943 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/code_analyzer.py
--rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/error_reporting.py
--rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/punctuation_chars.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/roman.py
--rw-r--r--   0        0        0    38945 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/smartquotes.py
--rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/urischemes.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/math/__init__.py
--rw-r--r--   0        0        0    51043 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/math/latex2mathml.py
--rw-r--r--   0        0        0    98692 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/math/math2html.py
--rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py
--rw-r--r--   0        0        0    36734 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/math/tex2unichar.py
--rw-r--r--   0        0        0    18393 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/math/unichar2tex.py
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/__init__.py
--rw-r--r--   0        0        0    70253 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/_html_base.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/docutils_xml.py
--rw-r--r--   0        0        0    36527 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/manpage.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/null.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/pseudoxml.py
--rw-r--r--   0        0        0    37638 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html4css1/__init__.py
--rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html4css1/html4css1.css
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html4css1/template.txt
--rw-r--r--   0        0        0    18212 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py
--rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html5_polyglot/math.css
--rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html5_polyglot/minimal.css
--rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html5_polyglot/plain.css
--rw-r--r--   0        0        0    11736 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html5_polyglot/responsive.css
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html5_polyglot/template.txt
--rw-r--r--   0        0        0    12042 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html5_polyglot/tuftig.css
--rw-r--r--   0        0        0   136872 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/latex2e/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/latex2e/default.tex
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/latex2e/docutils.sty
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/latex2e/titlepage.tex
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/latex2e/titlingpage.tex
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/latex2e/xelatex.tex
--rw-r--r--   0        0        0   132399 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/odf_odt/__init__.py
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py
--rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/odf_odt/styles.odt
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/pep_html/__init__.py
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/pep_html/pep.css
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/pep_html/template.txt
--rw-r--r--   0        0        0    14627 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/__init__.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/README.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/__base__
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/framing.css
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/framing.css
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/framing.css
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/opera.css
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/outline.css
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/pretty.css
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/print.css
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/s5-core.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.css
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.js
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/__base__
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-black/__base__
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/framing.css
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/xetex/__init__.py
--rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/COPYING.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/INSTALLER
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/METADATA
--rw-r--r--   0        0        0    27888 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/RECORD
--rw-r--r--   0        0        0    26094 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/SOURCES.html
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/WHEEL
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/dependency_links.html
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/entry_points.txt
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/top_level.html
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/top_level.txt
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/idna/package_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/idna/py.typed
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/idna/uts46data.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/idna-3.4.dist-info/INSTALLER
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/idna-3.4.dist-info/LICENSE.md
--rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/idna-3.4.dist-info/METADATA
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/idna-3.4.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/idna-3.4.dist-info/WHEEL
--rw-r--r--   0        0        0    26490 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/__init__.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_adapters.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_collections.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_compat.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_functools.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_itertools.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_meta.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_py39compat.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/top_level.txt
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/_common.py
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/_compat.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/abc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/py.typed
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/readers.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/__init__.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/_compat.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/_path.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_compatibilty_files.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_contents.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_custom.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_files.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_open.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_path.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_read.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_reader.py
--rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_resource.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/update-zips.py
--rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/data01/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/data01/binary.file
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/data01/utf-16.file
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/data01/utf-8.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/data01/subdirectory/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/data01/subdirectory/binary.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/data02/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/data02/one/__init__.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/data02/one/resource1.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/data02/subdirectory/subsubdir/resource.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/data02/two/__init__.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/data02/two/resource2.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/namespacedata01/binary.file
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/namespacedata01/utf-16.file
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/namespacedata01/utf-8.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/zipdata01/__init__.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/zipdata01/ziptestdata.zip
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/zipdata02/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/zipdata02/ziptestdata.zip
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/METADATA
--rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/WHEEL
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/jaraco/classes/__init__.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/jaraco/classes/ancestry.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/jaraco/classes/meta.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/jaraco/classes/properties.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/INSTALLER
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/LICENSE
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/METADATA
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/WHEEL
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/top_level.txt
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/__main__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/_compat.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/_properties_compat.py
--rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/backend.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/backend_complete.zsh
--rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/cli.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/completion.py
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/core.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/credentials.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/devpi_client.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/errors.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/http.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/py.typed
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/py312compat.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/OS_X.py
--rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/SecretService.py
--rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/Windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/__init__.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/chainer.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/fail.py
--rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/kwallet.py
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/libsecret.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/null.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/macOS/__init__.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/macOS/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/testing/__init__.py
--rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/testing/backend.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/testing/util.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/util/__init__.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/util/platform_.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring/util/properties.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring-23.13.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring-23.13.1.dist-info/LICENSE
--rw-r--r--   0        0        0    20647 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring-23.13.1.dist-info/METADATA
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring-23.13.1.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring-23.13.1.dist-info/WHEEL
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring-23.13.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/keyring-23.13.1.dist-info/top_level.txt
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/_compat.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/_punycode.py
--rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/main.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/parser_block.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/parser_core.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/parser_inline.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/port.yaml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/py.typed
--rw-r--r--   0        0        0    10041 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/renderer.py
--rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/ruler.py
--rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/token.py
--rw-r--r--   0        0        0    11052 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/tree.py
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/cli/__init__.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/cli/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/common/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/common/entities.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/common/html_blocks.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/common/html_re.py
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/common/normalize_url.py
--rw-r--r--   0        0        0    10894 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/common/utils.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/helpers/__init__.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/helpers/parse_link_destination.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/helpers/parse_link_label.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/helpers/parse_link_title.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/presets/__init__.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/presets/commonmark.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/presets/default.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/presets/zero.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/__init__.py
--rw-r--r--   0        0        0     9057 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/blockquote.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/code.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/fence.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/heading.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/hr.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/html_block.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/lheading.py
--rw-r--r--   0        0        0     9944 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/list.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/paragraph.py
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/reference.py
--rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/state_block.py
--rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/table.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_core/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_core/block.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_core/inline.py
--rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_core/linkify.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_core/normalize.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_core/replacements.py
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_core/smartquotes.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_core/state_core.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/__init__.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/autolink.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/backticks.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/emphasis.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/entity.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/escape.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/html_inline.py
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/image.py
--rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/link.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/newline.py
--rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/state_inline.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/strikethrough.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/text.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/text_collapse.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE.markdown-it
--rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/METADATA
--rw-r--r--   0        0        0    10455 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/WHEEL
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/mdurl/__init__.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/mdurl/_decode.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/mdurl/_encode.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/mdurl/_format.py
--rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/mdurl/_parse.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/mdurl/_url.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/mdurl/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/mdurl-0.1.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/mdurl-0.1.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/mdurl-0.1.2.dist-info/METADATA
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/mdurl-0.1.2.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/mdurl-0.1.2.dist-info/WHEEL
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/more_itertools/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/more_itertools/__init__.pyi
--rw-r--r--   0        0        0   133336 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/more_itertools/more.py
--rw-r--r--   0        0        0    20297 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/more_itertools/more.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/more_itertools/py.typed
--rw-r--r--   0        0        0    22975 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/more_itertools/recipes.py
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/more_itertools/recipes.pyi
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0    31266 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging/_elffile.py
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging/_musllinux.py
--rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging/_structures.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging/markers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging/py.typed
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging/requirements.py
--rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging/specifiers.py
--rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging/tags.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging/utils.py
--rw-r--r--   0        0        0    16295 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging/version.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging-23.0.dist-info/INSTALLER
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging-23.0.dist-info/LICENSE
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging-23.0.dist-info/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging-23.0.dist-info/LICENSE.BSD
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging-23.0.dist-info/METADATA
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging-23.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/packaging-23.0.dist-info/WHEEL
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/py.typed
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    24244 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    13079 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    29497 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18172 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    32389 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    18602 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    16507 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py
--rw-r--r--   0        0        0    27407 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    16611 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    35763 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24045 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24129 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    18963 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    27878 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    22253 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0    80114 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   275233 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/t32.exe
--rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe
--rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/version.py
--rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/w32.exe
--rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe
--rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34557 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0   108287 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    32005 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35441 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    70232 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    53376 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213344 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33240 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    17592 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6819 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    97992 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     7954 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    37414 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59836 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24224 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    26332 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    34995 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    45686 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    26070 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    18364 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20070 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39095 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14298 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip-23.0.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip-23.0.1.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip-23.0.1.dist-info/METADATA
--rw-r--r--   0        0        0    76692 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip-23.0.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip-23.0.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip-23.0.1.dist-info/WHEEL
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip-23.0.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pip-23.0.1.dist-info/top_level.txt
--rw-r--r--   0        0        0   108202 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
--rw-r--r--   0        0        0   232056 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_compat.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_typing.py
--rw-r--r--   0        0        0     9518 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    31944 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    24067 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/__init__.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/__init__.pyi
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/bdist.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/bdist.pyi
--rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/commandline.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/commandline.pyi
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/develop.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/develop.pyi
--rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/distribution.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/distribution.pyi
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/index.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/index.pyi
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/installed.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/installed.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/py.typed
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/sdist.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/sdist.pyi
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/utils.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/utils.pyi
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/wheel.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/wheel.pyi
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/__init__.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_bdist.py
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_commandline.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_develop.py
--rw-r--r--   0        0        0    19377 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_distribution.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_index.py
--rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_installed.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_sdist.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_utils.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_wheel.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/INSTALLER
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/LICENSE.txt
--rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/METADATA
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/WHEEL
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/entry_points.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/top_level.txt
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/__init__.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/__main__.py
--rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/filter.py
--rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatter.py
--rw-r--r--   0        0        0    31987 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/modeline.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/scanner.py
--rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/sphinxext.py
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/token.py
--rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/unistring.py
--rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/util.py
--rw-r--r--   0        0        0    40338 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/filters/__init__.py
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35565 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/html.py
--rw-r--r--   0        0        0    21914 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/img.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19303 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/other.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    11116 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/__init__.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_ada_builtins.py
--rw-r--r--   0        0        0    27287 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_asy_builtins.py
--rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_cl_builtins.py
--rw-r--r--   0        0        0   105182 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_cocoa_builtins.py
--rw-r--r--   0        0        0    18414 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_csound_builtins.py
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_css_builtins.py
--rw-r--r--   0        0        0    11883 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_julia_builtins.py
--rw-r--r--   0        0        0   134510 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_lasso_builtins.py
--rw-r--r--   0        0        0   106781 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_lilypond_builtins.py
--rw-r--r--   0        0        0     8080 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_lua_builtins.py
--rw-r--r--   0        0        0    64980 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    24713 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_mql_builtins.py
--rw-r--r--   0        0        0    25806 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_mysql_builtins.py
--rw-r--r--   0        0        0    49398 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_openedge_builtins.py
--rw-r--r--   0        0        0   107876 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_php_builtins.py
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_postgres_builtins.py
--rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_qlik_builtins.py
--rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_scheme_builtins.py
--rw-r--r--   0        0        0    52377 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_scilab_builtins.py
--rw-r--r--   0        0        0    26745 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py
--rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_stan_builtins.py
--rw-r--r--   0        0        0    27227 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_stata_builtins.py
--rw-r--r--   0        0        0    15460 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_tsql_builtins.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_usd_builtins.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_vbscript_builtins.py
--rw-r--r--   0        0        0    57066 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_vim_builtins.py
--rw-r--r--   0        0        0    11676 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/actionscript.py
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ada.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/agile.py
--rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/algebra.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ambient.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/amdgpu.py
--rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ampl.py
--rw-r--r--   0        0        0    26654 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/apdlexer.py
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/apl.py
--rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/archetype.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/arrow.py
--rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/arturo.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/asc.py
--rw-r--r--   0        0        0    41243 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/asm.py
--rw-r--r--   0        0        0    19815 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/automation.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/bare.py
--rw-r--r--   0        0        0    27923 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/basic.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/bdd.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/berry.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/bibtex.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/boa.py
--rw-r--r--   0        0        0    28112 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/business.py
--rw-r--r--   0        0        0    17791 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/c_cpp.py
--rw-r--r--   0        0        0    29206 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/c_like.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/capnproto.py
--rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/cddl.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/chapel.py
--rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/clean.py
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/comal.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/compiled.py
--rw-r--r--   0        0        0    41825 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/configs.py
--rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/console.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/cplint.py
--rw-r--r--   0        0        0    15756 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/crystal.py
--rw-r--r--   0        0        0    16994 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/csound.py
--rw-r--r--   0        0        0    25314 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/css.py
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/d.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/dalvik.py
--rw-r--r--   0        0        0    26940 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/data.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/devicetree.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/diff.py
--rw-r--r--   0        0        0    29696 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/dotnet.py
--rw-r--r--   0        0        0    36774 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/dsls.py
--rw-r--r--   0        0        0    10380 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/dylan.py
--rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ecl.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/eiffel.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/elm.py
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/elpi.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/email.py
--rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/erlang.py
--rw-r--r--   0        0        0    10396 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/esoteric.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ezhil.py
--rw-r--r--   0        0        0    19531 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/factor.py
--rw-r--r--   0        0        0    10197 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/fantom.py
--rw-r--r--   0        0        0     9646 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/felix.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/fift.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/floscript.py
--rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/forth.py
--rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/fortran.py
--rw-r--r--   0        0        0    26212 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/foxpro.py
--rw-r--r--   0        0        0    26914 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/freefem.py
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/func.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/functional.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/futhark.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/gcodelexer.py
--rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/gdscript.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/go.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/grammar_notation.py
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/graph.py
--rw-r--r--   0        0        0    38931 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/graphics.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/graphviz.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/gsql.py
--rw-r--r--   0        0        0    32898 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/haskell.py
--rw-r--r--   0        0        0    30976 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/haxe.py
--rw-r--r--   0        0        0    22520 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/hdl.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/hexdump.py
--rw-r--r--   0        0        0    19879 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/html.py
--rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/idl.py
--rw-r--r--   0        0        0    30631 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/igor.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/inferno.py
--rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/installers.py
--rw-r--r--   0        0        0    57119 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/int_fiction.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/iolang.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/j.py
--rw-r--r--   0        0        0    62859 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/javascript.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/jmespath.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/jslt.py
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/jsonnet.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/julia.py
--rw-r--r--   0        0        0    72929 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/jvm.py
--rw-r--r--   0        0        0    11406 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/kuin.py
--rw-r--r--   0        0        0     9753 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/lilypond.py
--rw-r--r--   0        0        0   144039 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/lisp.py
--rw-r--r--   0        0        0    31914 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/macaulay2.py
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/make.py
--rw-r--r--   0        0        0    26797 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/markup.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/math.py
--rw-r--r--   0        0        0   132852 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/matlab.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/maxima.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/meson.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/mime.py
--rw-r--r--   0        0        0    13846 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/minecraft.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/mips.py
--rw-r--r--   0        0        0    35324 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ml.py
--rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/modeling.py
--rw-r--r--   0        0        0    53073 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/modula2.py
--rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/monte.py
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/mosel.py
--rw-r--r--   0        0        0    63962 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ncl.py
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/nimrod.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/nit.py
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/nix.py
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/oberon.py
--rw-r--r--   0        0        0    22961 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/objective.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ooc.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/other.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/parasail.py
--rw-r--r--   0        0        0    25904 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/parsers.py
--rw-r--r--   0        0        0    30880 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/pascal.py
--rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/pawn.py
--rw-r--r--   0        0        0    39170 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/perl.py
--rw-r--r--   0        0        0    23252 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/phix.py
--rw-r--r--   0        0        0    12505 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/php.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/pointless.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/pony.py
--rw-r--r--   0        0        0    12677 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/praat.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/procfile.py
--rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/prolog.py
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/promql.py
--rw-r--r--   0        0        0    53524 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/python.py
--rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/q.py
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/qlik.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/qvt.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/r.py
--rw-r--r--   0        0        0    15790 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/rdf.py
--rw-r--r--   0        0        0    18600 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/rebol.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/resource.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ride.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/rita.py
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/rnc.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/roboconf.py
--rw-r--r--   0        0        0    18449 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/robotframework.py
--rw-r--r--   0        0        0    22775 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ruby.py
--rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/rust.py
--rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/sas.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/savi.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/scdoc.py
--rw-r--r--   0        0        0    70014 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/scripting.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/sgf.py
--rw-r--r--   0        0        0    36344 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/shell.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/sieve.py
--rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/slash.py
--rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/smalltalk.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/smithy.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/smv.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/snobol.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/solidity.py
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/sophia.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/special.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/spice.py
--rw-r--r--   0        0        0    34151 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/sql.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/srcinfo.py
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/stata.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/supercollider.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/tal.py
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/tcl.py
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/teal.py
--rw-r--r--   0        0        0    72695 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/templates.py
--rw-r--r--   0        0        0     9719 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/teraterm.py
--rw-r--r--   0        0        0    10767 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/testing.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/text.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/textedit.py
--rw-r--r--   0        0        0    15192 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/textfmts.py
--rw-r--r--   0        0        0    20157 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/theorem.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/thingsdb.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/tlb.py
--rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/tnt.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/trafficscript.py
--rw-r--r--   0        0        0     8207 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/typoscript.py
--rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ul4.py
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/unicon.py
--rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/urbi.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/usd.py
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/varnish.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/verification.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/web.py
--rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/webassembly.py
--rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/webidl.py
--rw-r--r--   0        0        0    40549 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/webmisc.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/whiley.py
--rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/wowtoc.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/wren.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/x10.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/xorg.py
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/yang.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/zig.py
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/__init__.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/abap.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/algol.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/algol_nu.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/arduino.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/autumn.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/borland.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/bw.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/colorful.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/default.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/dracula.py
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/emacs.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/friendly.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/friendly_grayscale.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/fruity.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/gh_dark.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/gruvbox.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/igor.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/inkpot.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/lilypond.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/lovelace.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/manni.py
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/material.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/monokai.py
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/murphy.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/native.py
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/nord.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/onedark.py
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/paraiso_dark.py
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/paraiso_light.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/pastie.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/perldoc.py
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/rainbow_dash.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/rrt.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/sas.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/solarized.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/staroffice.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/stata_dark.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/stata_light.py
--rw-r--r--   0        0        0     7039 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/tango.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/trac.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/vim.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/vs.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/xcode.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/zenburn.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/LICENSE.txt
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/METADATA
--rw-r--r--   0        0        0     5598 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/RECORD
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/WHEEL
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer/__about__.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer/__init__.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer/__main__.py
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer/clean.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer/markdown.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer/py.typed
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer/rst.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer/txt.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer-37.3.dist-info/INSTALLER
--rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer-37.3.dist-info/LICENSE
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer-37.3.dist-info/METADATA
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer-37.3.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer-37.3.dist-info/WHEEL
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer-37.3.dist-info/top_level.txt
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/__version__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/_internal_utils.py
--rw-r--r--   0        0        0    21287 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/adapters.py
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/auth.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/certs.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/cookies.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/exceptions.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/hooks.py
--rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/models.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/packages.py
--rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/structures.py
--rw-r--r--   0        0        0    33228 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests/utils.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests-2.28.2.dist-info/INSTALLER
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests-2.28.2.dist-info/LICENSE
--rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests-2.28.2.dist-info/METADATA
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests-2.28.2.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests-2.28.2.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests-2.28.2.dist-info/top_level.txt
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/__init__.py
--rw-r--r--   0        0        0     9512 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/_compat.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/exceptions.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/sessions.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/streaming_iterator.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/adapters/__init__.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/adapters/appengine.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/adapters/socket_options.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/adapters/source.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/adapters/ssl.py
--rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/adapters/x509.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/auth/__init__.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/auth/guess.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/auth/handler.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/cookies/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/cookies/forgetful.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/downloadutils/__init__.py
--rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/downloadutils/stream.py
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/downloadutils/tee.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/multipart/__init__.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/multipart/decoder.py
--rw-r--r--   0        0        0    20769 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/multipart/encoder.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/threaded/__init__.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/threaded/pool.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/threaded/thread.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/utils/__init__.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/utils/deprecated.py
--rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/utils/dump.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/utils/formdata.py
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/utils/user_agent.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/AUTHORS.rst
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/INSTALLER
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/LICENSE
--rw-r--r--   0        0        0    14003 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/METADATA
--rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/WHEEL
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/top_level.txt
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/__init__.py
--rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/_mixin.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/abnf_regexp.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/api.py
--rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/builder.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/compat.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/exceptions.py
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/iri.py
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/misc.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/normalizers.py
--rw-r--r--   0        0        0    14599 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/parseresult.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/uri.py
--rw-r--r--   0        0        0    13676 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/validators.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/__init__.py
--rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_export_format.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_inspect.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_pick.py
--rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_timer.py
--rw-r--r--   0        0        0    22784 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_win32_console.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_windows.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/_wrap.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/abc.py
--rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/align.py
--rw-r--r--   0        0        0     6819 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/bar.py
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/box.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/cells.py
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/columns.py
--rw-r--r--   0        0        0    99018 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/containers.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/control.py
--rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/default_styles.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/diagnose.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/filesize.py
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/highlighter.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/json.py
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/jupyter.py
--rw-r--r--   0        0        0    13947 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/layout.py
--rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/live.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/live_render.py
--rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/logging.py
--rw-r--r--   0        0        0    22368 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/markdown.py
--rw-r--r--   0        0        0     8174 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/measure.py
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/pager.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/palette.py
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/panel.py
--rw-r--r--   0        0        0    37348 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/pretty.py
--rw-r--r--   0        0        0    59668 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/progress.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/progress_bar.py
--rw-r--r--   0        0        0    11291 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/prompt.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/py.typed
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/region.py
--rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/repr.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/rule.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/scope.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/screen.py
--rw-r--r--   0        0        0    24195 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/status.py
--rw-r--r--   0        0        0    26332 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/style.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/styled.py
--rw-r--r--   0        0        0    34868 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/syntax.py
--rw-r--r--   0        0        0    39648 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/terminal_theme.py
--rw-r--r--   0        0        0    45670 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/themes.py
--rw-r--r--   0        0        0    29102 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/traceback.py
--rw-r--r--   0        0        0     9109 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich/tree.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich-13.3.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich-13.3.1.dist-info/LICENSE
--rw-r--r--   0        0        0    18759 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich-13.3.1.dist-info/METADATA
--rw-r--r--   0        0        0     9572 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich-13.3.1.dist-info/RECORD
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/rich-13.3.1.dist-info/WHEEL
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_deprecation_warning.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_imp.py
--rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/archive_util.py
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/build_meta.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/cli-32.exe
--rwxr-xr-x   0        0        0    74752 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/cli-64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/cli.exe
--rw-r--r--   0        0        0    22279 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/config.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/dep_util.py
--rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/depends.py
--rw-r--r--   0        0        0    42374 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/dist.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/errors.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/extension.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/glob.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/gui-32.exe
--rwxr-xr-x   0        0        0    75264 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/gui-64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/gui.exe
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/installer.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/launch.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/lib2to3_ex.py
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/monkey.py
--rw-r--r--   0        0        0    50561 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/msvc.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/namespaces.py
--rw-r--r--   0        0        0    40173 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/package_index.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/py34compat.py
--rw-r--r--   0        0        0    14151 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/sandbox.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/script.tmpl
--rw-r--r--   0        0        0     8565 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/ssl_support.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/version.py
--rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/wheel.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/windows_support.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0        0        0    20813 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0        0        0    14894 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0        0        0    47607 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0        0        0    18079 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/cmd.py
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0        0        0     8876 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0        0        0    16380 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0        0        0     7778 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0        0        0    50421 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0        0        0    17784 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0        0        0     8148 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0        0        0    12832 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0        0        0    30453 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0        0        0    23540 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/py35compat.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0        0        0    21349 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0        0        0    12483 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0        0        0    14696 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0        0        0    20985 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0        0        0    35579 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_msi.py
--rw-r--r--   0        0        0    21537 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0        0        0    16030 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_wininst.py
--rw-r--r--   0        0        0     5767 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0        0        0    31685 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0        0        0    17190 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0        0        0    13117 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0        0        0    27482 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0        0        0    19005 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
--rw-r--r--   0        0        0   232056 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/pyparsing.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0   117968 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_compat.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_typing.py
--rw-r--r--   0        0        0     9509 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    31944 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    24067 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/__init__.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/alias.py
--rw-r--r--   0        0        0    16604 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0        0        0     8930 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/build_py.py
--rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/develop.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0        0        0    85308 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0        0        0    25335 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/install.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/register.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/rotate.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/sdist.py
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/setopt.py
--rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/test.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/upload.py
--rw-r--r--   0        0        0     7218 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools-57.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools-57.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools-57.0.0.dist-info/METADATA
--rw-r--r--   0        0        0    21856 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools-57.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools-57.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools-57.0.0.dist-info/dependency_links.txt
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools-57.0.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/setuptools-57.0.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/six-1.16.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/six-1.16.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/six-1.16.0.dist-info/METADATA
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/six-1.16.0.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/six-1.16.0.dist-info/WHEEL
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/six-1.16.0.dist-info/top_level.txt
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/tomli/_types.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/tomli/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/tomli-2.0.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/tomli-2.0.1.dist-info/LICENSE
--rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/tomli-2.0.1.dist-info/METADATA
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/tomli-2.0.1.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/tomli-2.0.1.dist-info/WHEEL
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/__init__.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/__main__.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/auth.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/cli.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/exceptions.py
--rw-r--r--   0        0        0    11024 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/py.typed
--rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/repository.py
--rw-r--r--   0        0        0    12269 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/settings.py
--rw-r--r--   0        0        0    10867 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/utils.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/wheel.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/wininst.py
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/commands/__init__.py
--rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/commands/check.py
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/commands/register.py
--rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine/commands/upload.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine-4.0.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine-4.0.2.dist-info/LICENSE
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine-4.0.2.dist-info/METADATA
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine-4.0.2.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine-4.0.2.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine-4.0.2.dist-info/WHEEL
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine-4.0.2.dist-info/entry_points.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/twine-4.0.2.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/LICENSE
--rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/METADATA
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/WHEEL
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/_version.py
--rw-r--r--   0        0        0    20070 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/connection.py
--rw-r--r--   0        0        0    39095 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/filepost.py
--rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/poolmanager.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/request.py
--rw-r--r--   0        0        0    30761 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11012 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17055 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34416 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/queue.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/response.py
--rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/retry.py
--rw-r--r--   0        0        0    17165 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14281 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/wait.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3-1.26.14.dist-info/INSTALLER
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3-1.26.14.dist-info/LICENSE.txt
--rw-r--r--   0        0        0    47722 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3-1.26.14.dist-info/METADATA
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3-1.26.14.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3-1.26.14.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/urllib3-1.26.14.dist-info/top_level.txt
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/webencodings/x_user_defined.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/webencodings-0.5.1.dist-info/DESCRIPTION.rst
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/webencodings-0.5.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/webencodings-0.5.1.dist-info/METADATA
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/webencodings-0.5.1.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/webencodings-0.5.1.dist-info/WHEEL
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/webencodings-0.5.1.dist-info/metadata.json
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/webencodings-0.5.1.dist-info/top_level.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/__init__.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/__main__.py
--rw-r--r--   0        0        0    19075 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/bdist_wheel.py
--rw-r--r--   0        0        0    15931 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/macosx_libfile.py
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/metadata.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/pkginfo.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/util.py
--rw-r--r--   0        0        0     7336 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/wheelfile.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/cli/__init__.py
--rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/cli/convert.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/cli/pack.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/cli/unpack.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/vendored/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/vendored/packaging/__init__.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/vendored/packaging/_typing.py
--rw-r--r--   0        0        0    28937 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel/vendored/packaging/tags.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel-0.36.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel-0.36.2.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel-0.36.2.dist-info/METADATA
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel-0.36.2.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel-0.36.2.dist-info/WHEEL
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel-0.36.2.dist-info/entry_points.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/wheel-0.36.2.dist-info/top_level.txt
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/__init__.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/pywintypes.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/version.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/win32api.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/win32cred.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/__init__.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/_winerrors.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/compat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/cffi/__init__.py
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/cffi/_authentication.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/cffi/_common.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/cffi/_dll.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/cffi/_nl_support.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/cffi/_resource.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/cffi/_system_information.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/cffi/_time.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/cffi/_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/ctypes/__init__.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/ctypes/_common.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/ctypes/_dll.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/ctypes/_nl_support.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/ctypes/_resource.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/ctypes/_time.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/ctypes/_util.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/pywin32/__init__.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/pywin32/pywintypes.py
--rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/pywin32/win32api.py
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/pywin32/win32cred.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/tests/__init__.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/tests/compat.py
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/tests/test_win32api.py
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/tests/test_win32cred.py
--rw-r--r--   0        0        0    10455 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/zipp/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/zipp/py310compat.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/zipp-3.14.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/zipp-3.14.0.dist-info/LICENSE
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/zipp-3.14.0.dist-info/METADATA
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/zipp-3.14.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/zipp-3.14.0.dist-info/WHEEL
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Lib/site-packages/zipp-3.14.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/activate
--rwxr-xr-x   0        0        0     1020 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/activate.bat
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/activate.fish
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/activate.ps1
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/activate.xsh
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/activate_this.py
--rwxr-xr-x   0        0        0      510 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/deactivate.bat
--rwxr-xr-x   0        0        0    97136 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/docutils.exe
--rwxr-xr-x   0        0        0    97130 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/keyring.exe
--rwxr-xr-x   0        0        0    97140 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/markdown-it.exe
--rwxr-xr-x   0        0        0    97164 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/normalizer.exe
--rwxr-xr-x   0        0        0    98165 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/pip.exe
--rwxr-xr-x   0        0        0    98165 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/pip3.7.exe
--rwxr-xr-x   0        0        0    98165 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/pip3.exe
--rwxr-xr-x   0        0        0    97138 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/pkginfo.exe
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/pydoc.bat
--rwxr-xr-x   0        0        0    97135 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/pygmentize.exe
--rwxr-xr-x   0        0        0    97145 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/pyproject-build.exe
--rwxr-xr-x   0        0        0   413712 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/python.exe
--rwxr-xr-x   0        0        0   412688 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/pythonw.exe
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/rst2html.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/rst2html4.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/rst2html5.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/rst2latex.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/rst2man.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/rst2odt.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/rst2odt_prepstyles.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/rst2pseudoxml.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/rst2s5.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/rst2xetex.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/rst2xml.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/rstpep2html.py
--rwxr-xr-x   0        0        0    97133 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/twine.exe
--rwxr-xr-x   0        0        0    97128 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/wheel-3.7.exe
--rwxr-xr-x   0        0        0    97128 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/wheel.exe
--rwxr-xr-x   0        0        0    97128 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/wheel3.7.exe
--rwxr-xr-x   0        0        0    97128 2020-02-02 00:00:00.000000 tomaserial-0.1.1/venv/Scripts/wheel3.exe
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 tomaserial-0.1.1/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 tomaserial-0.1.1/LICENSE
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tomaserial-0.1.1/README.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 tomaserial-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tomaserial-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 tomaserial-0.1.2/publish.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tomaserial-0.1.2/serial/__init__.py
+-rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 tomaserial-0.1.2/serial/serial.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/.gitignore
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/pyvenv.cfg
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/distutils-precedence.pth
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/easy-install.pth
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/serial.egg-link
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools-57.0.0.virtualenv
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/six.py
+-rw-r--r--   0        0        0    84065 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/typing_extensions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel-0.36.2.virtualenv
+-rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/Pygments-2.14.0.dist-info/AUTHORS
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/Pygments-2.14.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/Pygments-2.14.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/Pygments-2.14.0.dist-info/METADATA
+-rw-r--r--   0        0        0    41872 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/Pygments-2.14.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/Pygments-2.14.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/Pygments-2.14.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/Pygments-2.14.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/_distutils_hack/override.py
+-rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/callbacks.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/css_sanitizer.py
+-rw-r--r--   0        0        0    22779 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/html5lib_shim.py
+-rw-r--r--   0        0        0    22350 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/linkifier.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/parse_shim.py
+-rw-r--r--   0        0        0    21934 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/sanitizer.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/__init__.py
+-rw-r--r--   0        0        0    39023 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/parse.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/parse.py.SHA256SUM
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/vendor.txt
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/vendor_install.sh
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/__init__.py
+-rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_ihatexml.py
+-rw-r--r--   0        0        0    32300 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_inputstream.py
+-rw-r--r--   0        0        0    77028 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_tokenizer.py
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_utils.py
+-rw-r--r--   0        0        0    83464 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/constants.py
+-rw-r--r--   0        0        0   117174 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/html5parser.py
+-rw-r--r--   0        0        0    15747 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/serializer.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/__init__.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/_base.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/py.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/__init__.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/base.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/lint.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py
+-rw-r--r--   0        0        0    26885 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/whitespace.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py
+-rw-r--r--   0        0        0    14553 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/base.py
+-rw-r--r--   0        0        0     8925 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py
+-rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py
+-rw-r--r--   0        0        0    14754 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py
+-rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/base.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py
+-rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/AUTHORS.rst
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    16076 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/METADATA
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach-6.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach-6.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    29799 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach-6.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach-6.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach-6.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/bleach-6.0.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/build-0.10.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/build-0.10.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/build-0.10.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/build-0.10.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/build-0.10.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/build-0.10.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/build-0.10.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/certifi/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/certifi/__main__.py
+-rw-r--r--   0        0        0   275233 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/certifi/cacert.pem
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/certifi/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/certifi/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/certifi-2022.12.7.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/certifi-2022.12.7.dist-info/LICENSE
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/certifi-2022.12.7.dist-info/METADATA
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/certifi-2022.12.7.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/certifi-2022.12.7.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/certifi-2022.12.7.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/__init__.py
+-rw-r--r--   0        0        0    19154 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/api.py
+-rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/cd.py
+-rw-r--r--   0        0        0    19596 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/constant.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/legacy.py
+-rw-r--r--   0        0        0    18829 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/md.py
+-rw-r--r--   0        0        0    11829 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/py.typed
+-rw-r--r--   0        0        0    11966 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/utils.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/version.py
+-rw-r--r--   0        0        0    21509 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/assets/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/cli/__init__.py
+-rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/cli/normalizer.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    27664 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/METADATA
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/RECORD
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/WHEEL
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama-0.4.6.dist-info/INSTALLER
+-rw-r--r--   0        0        0    17158 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama-0.4.6.dist-info/METADATA
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama-0.4.6.dist-info/RECORD
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama-0.4.6.dist-info/WHEEL
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/__init__.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/__main__.py
+-rw-r--r--   0        0        0    30945 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/core.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/examples.py
+-rw-r--r--   0        0        0    39697 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/frontend.py
+-rw-r--r--   0        0        0    21271 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/io.py
+-rw-r--r--   0        0        0    80986 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/nodes.py
+-rw-r--r--   0        0        0    56956 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/statemachine.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/af.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/ar.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/ca.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/cs.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/da.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/de.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/en.py
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/eo.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/es.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/fa.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/fi.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/fr.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/gl.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/he.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/it.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/ja.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/ko.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/lt.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/lv.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/nl.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/pl.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/pt_br.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/ru.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/sk.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/sv.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/zh_cn.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/zh_tw.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/__init__.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/commonmark_wrapper.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/null.py
+-rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py
+-rw-r--r--   0        0        0    15985 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/__init__.py
+-rw-r--r--   0        0        0    16119 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/roles.py
+-rw-r--r--   0        0        0   132550 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/states.py
+-rw-r--r--   0        0        0    20912 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/tableparser.py
+-rw-r--r--   0        0        0    14653 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/__init__.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py
+-rw-r--r--   0        0        0     9883 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/body.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/html.py
+-rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/images.py
+-rw-r--r--   0        0        0    26770 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/misc.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/parts.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/references.py
+-rw-r--r--   0        0        0    22227 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/tables.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/README.txt
+-rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsa.txt
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsb.txt
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsc.txt
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsn.txt
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamso.txt
+-rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsr.txt
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isobox.txt
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr1.txt
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr2.txt
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isodia.txt
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk1.txt
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk2.txt
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk3.txt
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4.txt
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isolat1.txt
+-rw-r--r--   0        0        0     8466 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isolat2.txt
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk.txt
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf-wide.txt
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf.txt
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr-wide.txt
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr.txt
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isonum.txt
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isopub.txt
+-rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isotech.txt
+-rw-r--r--   0        0        0    45428 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/mmlalias.txt
+-rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt
+-rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra.txt
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/s5defs.txt
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-special.txt
+-rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/__init__.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/af.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ar.py
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ca.py
+-rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/cs.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/da.py
+-rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/de.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/en.py
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/eo.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/es.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/fa.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/fi.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/fr.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/gl.py
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/he.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/it.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ja.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ko.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/lt.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/lv.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/nl.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/pl.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ru.py
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/sk.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/sv.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/readers/__init__.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/readers/doctree.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/readers/pep.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/readers/standalone.py
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/components.py
+-rw-r--r--   0        0        0    20276 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/frontmatter.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/misc.py
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/parts.py
+-rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/peps.py
+-rw-r--r--   0        0        0    36544 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/references.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/universal.py
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/writer_aux.py
+-rw-r--r--   0        0        0    28742 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/__init__.py
+-rw-r--r--   0        0        0     4943 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/code_analyzer.py
+-rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/error_reporting.py
+-rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/punctuation_chars.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/roman.py
+-rw-r--r--   0        0        0    38945 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/smartquotes.py
+-rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/urischemes.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/math/__init__.py
+-rw-r--r--   0        0        0    51043 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/math/latex2mathml.py
+-rw-r--r--   0        0        0    98692 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/math/math2html.py
+-rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py
+-rw-r--r--   0        0        0    36734 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/math/tex2unichar.py
+-rw-r--r--   0        0        0    18393 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/math/unichar2tex.py
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/__init__.py
+-rw-r--r--   0        0        0    70253 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/_html_base.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/docutils_xml.py
+-rw-r--r--   0        0        0    36527 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/manpage.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/null.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/pseudoxml.py
+-rw-r--r--   0        0        0    37638 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html4css1/__init__.py
+-rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html4css1/html4css1.css
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html4css1/template.txt
+-rw-r--r--   0        0        0    18212 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py
+-rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/math.css
+-rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/minimal.css
+-rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/plain.css
+-rw-r--r--   0        0        0    11736 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/responsive.css
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/template.txt
+-rw-r--r--   0        0        0    12042 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/tuftig.css
+-rw-r--r--   0        0        0   136872 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/latex2e/__init__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/latex2e/default.tex
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/latex2e/docutils.sty
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/latex2e/titlepage.tex
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/latex2e/titlingpage.tex
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/latex2e/xelatex.tex
+-rw-r--r--   0        0        0   132399 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/odf_odt/__init__.py
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py
+-rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/odf_odt/styles.odt
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/pep_html/__init__.py
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/pep_html/pep.css
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/pep_html/template.txt
+-rw-r--r--   0        0        0    14627 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/__init__.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/README.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/__base__
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/framing.css
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/framing.css
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/framing.css
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/opera.css
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/outline.css
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/pretty.css
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/print.css
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/s5-core.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.css
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.js
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/__base__
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-black/__base__
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/framing.css
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/xetex/__init__.py
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/COPYING.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/METADATA
+-rw-r--r--   0        0        0    27888 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/RECORD
+-rw-r--r--   0        0        0    26094 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/SOURCES.html
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/WHEEL
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/dependency_links.html
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/top_level.html
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/top_level.txt
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/idna/package_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/idna/py.typed
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/idna/uts46data.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/idna-3.4.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/idna-3.4.dist-info/LICENSE.md
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/idna-3.4.dist-info/METADATA
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/idna-3.4.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/idna-3.4.dist-info/WHEEL
+-rw-r--r--   0        0        0    26490 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/__init__.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_adapters.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_collections.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_compat.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_functools.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_itertools.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_meta.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_py39compat.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/_compat.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/abc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/py.typed
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/__init__.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/_compat.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/_path.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_compatibilty_files.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_contents.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_custom.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_files.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_open.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_path.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_read.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_reader.py
+-rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_resource.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/update-zips.py
+-rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/data01/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/data01/binary.file
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/data01/utf-16.file
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/data01/utf-8.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/data01/subdirectory/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/data01/subdirectory/binary.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/data02/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/data02/one/__init__.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/data02/one/resource1.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/data02/subdirectory/subsubdir/resource.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/data02/two/__init__.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/data02/two/resource2.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/namespacedata01/binary.file
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/namespacedata01/utf-16.file
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/namespacedata01/utf-8.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/zipdata01/__init__.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/zipdata01/ziptestdata.zip
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/zipdata02/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/zipdata02/ziptestdata.zip
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/METADATA
+-rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/jaraco/classes/__init__.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/jaraco/classes/ancestry.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/jaraco/classes/meta.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/jaraco/classes/properties.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/top_level.txt
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/__main__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/_compat.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/_properties_compat.py
+-rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/backend.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/backend_complete.zsh
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/cli.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/completion.py
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/core.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/credentials.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/devpi_client.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/errors.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/http.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/py.typed
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/py312compat.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/OS_X.py
+-rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/SecretService.py
+-rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/Windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/__init__.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/chainer.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/fail.py
+-rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/kwallet.py
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/libsecret.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/null.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/macOS/__init__.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/macOS/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/testing/__init__.py
+-rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/testing/backend.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/testing/util.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/util/__init__.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/util/platform_.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring/util/properties.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring-23.13.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring-23.13.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    20647 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring-23.13.1.dist-info/METADATA
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring-23.13.1.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring-23.13.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring-23.13.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/keyring-23.13.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/_compat.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/_punycode.py
+-rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/main.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/parser_block.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/parser_core.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/parser_inline.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/port.yaml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/py.typed
+-rw-r--r--   0        0        0    10041 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/renderer.py
+-rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/ruler.py
+-rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/token.py
+-rw-r--r--   0        0        0    11052 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/tree.py
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/cli/__init__.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/cli/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/common/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/common/entities.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/common/html_blocks.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/common/html_re.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/common/normalize_url.py
+-rw-r--r--   0        0        0    10894 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/common/utils.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/helpers/__init__.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/helpers/parse_link_destination.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/helpers/parse_link_label.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/helpers/parse_link_title.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/presets/__init__.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/presets/commonmark.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/presets/default.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/presets/zero.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/__init__.py
+-rw-r--r--   0        0        0     9057 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/blockquote.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/code.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/fence.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/heading.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/hr.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/html_block.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/lheading.py
+-rw-r--r--   0        0        0     9944 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/list.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/paragraph.py
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/reference.py
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/state_block.py
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/table.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_core/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_core/block.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_core/inline.py
+-rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_core/linkify.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_core/normalize.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_core/replacements.py
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_core/smartquotes.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_core/state_core.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/__init__.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/autolink.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/backticks.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/emphasis.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/entity.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/escape.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/html_inline.py
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/image.py
+-rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/link.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/newline.py
+-rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/state_inline.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/strikethrough.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/text.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/text_collapse.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE.markdown-it
+-rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/METADATA
+-rw-r--r--   0        0        0    10455 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/mdurl/__init__.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/mdurl/_decode.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/mdurl/_encode.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/mdurl/_format.py
+-rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/mdurl/_parse.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/mdurl/_url.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/mdurl/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/mdurl-0.1.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/mdurl-0.1.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/mdurl-0.1.2.dist-info/METADATA
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/mdurl-0.1.2.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/mdurl-0.1.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/more_itertools/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/more_itertools/__init__.pyi
+-rw-r--r--   0        0        0   133336 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/more_itertools/more.py
+-rw-r--r--   0        0        0    20297 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/more_itertools/more.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/more_itertools/py.typed
+-rw-r--r--   0        0        0    22975 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/more_itertools/recipes.py
+-rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/more_itertools/recipes.pyi
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    31266 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging/_elffile.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging/_musllinux.py
+-rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging/_structures.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging/markers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging/py.typed
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging/requirements.py
+-rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging/specifiers.py
+-rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging/utils.py
+-rw-r--r--   0        0        0    16295 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging/version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging-23.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging-23.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging-23.0.dist-info/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging-23.0.dist-info/LICENSE.BSD
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging-23.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging-23.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/packaging-23.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    24244 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    13079 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    29497 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18172 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    32389 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    18602 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    16507 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py
+-rw-r--r--   0        0        0    27407 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    16611 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    35763 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    24045 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24129 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    18963 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    27878 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    22253 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0    80114 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   275233 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
+-rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/t32.exe
+-rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/version.py
+-rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/w32.exe
+-rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    34557 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   108287 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    32005 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35441 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    70232 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    53376 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   213344 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    33240 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    17592 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     6819 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0    97992 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     7954 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    37414 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    59836 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24224 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    26332 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    34995 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    45686 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    26070 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    18364 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20070 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    39095 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14298 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip-23.0.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip-23.0.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip-23.0.1.dist-info/METADATA
+-rw-r--r--   0        0        0    76692 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip-23.0.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip-23.0.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip-23.0.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip-23.0.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pip-23.0.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0   108202 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
+-rw-r--r--   0        0        0   232056 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_compat.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_typing.py
+-rw-r--r--   0        0        0     9518 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    31944 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    24067 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/extern/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/__init__.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/__init__.pyi
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/bdist.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/bdist.pyi
+-rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/commandline.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/commandline.pyi
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/develop.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/develop.pyi
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/distribution.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/distribution.pyi
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/index.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/index.pyi
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/installed.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/installed.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/py.typed
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/sdist.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/sdist.pyi
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/utils.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/utils.pyi
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/wheel.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/wheel.pyi
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/__init__.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_bdist.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_commandline.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_develop.py
+-rw-r--r--   0        0        0    19377 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_distribution.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_index.py
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_installed.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_sdist.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_utils.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_wheel.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/METADATA
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/WHEEL
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/top_level.txt
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/__init__.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/__main__.py
+-rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/filter.py
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatter.py
+-rw-r--r--   0        0        0    31987 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/modeline.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/scanner.py
+-rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/token.py
+-rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/unistring.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/util.py
+-rw-r--r--   0        0        0    40338 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35565 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21914 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/img.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19303 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    11116 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_ada_builtins.py
+-rw-r--r--   0        0        0    27287 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_asy_builtins.py
+-rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_cl_builtins.py
+-rw-r--r--   0        0        0   105182 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_cocoa_builtins.py
+-rw-r--r--   0        0        0    18414 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_csound_builtins.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_css_builtins.py
+-rw-r--r--   0        0        0    11883 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_julia_builtins.py
+-rw-r--r--   0        0        0   134510 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_lasso_builtins.py
+-rw-r--r--   0        0        0   106781 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_lilypond_builtins.py
+-rw-r--r--   0        0        0     8080 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_lua_builtins.py
+-rw-r--r--   0        0        0    64980 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    24713 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_mql_builtins.py
+-rw-r--r--   0        0        0    25806 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_mysql_builtins.py
+-rw-r--r--   0        0        0    49398 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_openedge_builtins.py
+-rw-r--r--   0        0        0   107876 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_php_builtins.py
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_postgres_builtins.py
+-rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_qlik_builtins.py
+-rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_scheme_builtins.py
+-rw-r--r--   0        0        0    52377 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_scilab_builtins.py
+-rw-r--r--   0        0        0    26745 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py
+-rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_stan_builtins.py
+-rw-r--r--   0        0        0    27227 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_stata_builtins.py
+-rw-r--r--   0        0        0    15460 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_tsql_builtins.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_usd_builtins.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_vbscript_builtins.py
+-rw-r--r--   0        0        0    57066 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_vim_builtins.py
+-rw-r--r--   0        0        0    11676 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/actionscript.py
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ada.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/agile.py
+-rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/algebra.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ambient.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/amdgpu.py
+-rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ampl.py
+-rw-r--r--   0        0        0    26654 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/apdlexer.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/apl.py
+-rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/archetype.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/arrow.py
+-rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/arturo.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/asc.py
+-rw-r--r--   0        0        0    41243 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/asm.py
+-rw-r--r--   0        0        0    19815 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/automation.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/bare.py
+-rw-r--r--   0        0        0    27923 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/basic.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/bdd.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/berry.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/bibtex.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/boa.py
+-rw-r--r--   0        0        0    28112 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/business.py
+-rw-r--r--   0        0        0    17791 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/c_cpp.py
+-rw-r--r--   0        0        0    29206 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/c_like.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/capnproto.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/cddl.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/chapel.py
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/clean.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/comal.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/compiled.py
+-rw-r--r--   0        0        0    41825 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/configs.py
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/console.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/cplint.py
+-rw-r--r--   0        0        0    15756 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/crystal.py
+-rw-r--r--   0        0        0    16994 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/csound.py
+-rw-r--r--   0        0        0    25314 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/css.py
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/d.py
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/dalvik.py
+-rw-r--r--   0        0        0    26940 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/data.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/devicetree.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/diff.py
+-rw-r--r--   0        0        0    29696 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/dotnet.py
+-rw-r--r--   0        0        0    36774 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/dsls.py
+-rw-r--r--   0        0        0    10380 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/dylan.py
+-rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ecl.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/eiffel.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/elm.py
+-rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/elpi.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/email.py
+-rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/erlang.py
+-rw-r--r--   0        0        0    10396 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/esoteric.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ezhil.py
+-rw-r--r--   0        0        0    19531 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/factor.py
+-rw-r--r--   0        0        0    10197 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/fantom.py
+-rw-r--r--   0        0        0     9646 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/felix.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/fift.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/floscript.py
+-rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/forth.py
+-rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/fortran.py
+-rw-r--r--   0        0        0    26212 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/foxpro.py
+-rw-r--r--   0        0        0    26914 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/freefem.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/func.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/functional.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/futhark.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/gcodelexer.py
+-rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/gdscript.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/go.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/grammar_notation.py
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/graph.py
+-rw-r--r--   0        0        0    38931 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/graphics.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/graphviz.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/gsql.py
+-rw-r--r--   0        0        0    32898 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/haskell.py
+-rw-r--r--   0        0        0    30976 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/haxe.py
+-rw-r--r--   0        0        0    22520 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/hdl.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/hexdump.py
+-rw-r--r--   0        0        0    19879 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/html.py
+-rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/idl.py
+-rw-r--r--   0        0        0    30631 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/igor.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/inferno.py
+-rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/installers.py
+-rw-r--r--   0        0        0    57119 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/int_fiction.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/iolang.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/j.py
+-rw-r--r--   0        0        0    62859 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/javascript.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/jmespath.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/jslt.py
+-rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/jsonnet.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/julia.py
+-rw-r--r--   0        0        0    72929 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/jvm.py
+-rw-r--r--   0        0        0    11406 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/kuin.py
+-rw-r--r--   0        0        0     9753 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/lilypond.py
+-rw-r--r--   0        0        0   144039 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/lisp.py
+-rw-r--r--   0        0        0    31914 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/macaulay2.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/make.py
+-rw-r--r--   0        0        0    26797 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/markup.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/math.py
+-rw-r--r--   0        0        0   132852 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/matlab.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/maxima.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/meson.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/mime.py
+-rw-r--r--   0        0        0    13846 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/minecraft.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/mips.py
+-rw-r--r--   0        0        0    35324 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ml.py
+-rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/modeling.py
+-rw-r--r--   0        0        0    53073 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/modula2.py
+-rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/monte.py
+-rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/mosel.py
+-rw-r--r--   0        0        0    63962 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ncl.py
+-rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/nimrod.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/nit.py
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/nix.py
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/oberon.py
+-rw-r--r--   0        0        0    22961 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/objective.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ooc.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/other.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/parasail.py
+-rw-r--r--   0        0        0    25904 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/parsers.py
+-rw-r--r--   0        0        0    30880 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/pascal.py
+-rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/pawn.py
+-rw-r--r--   0        0        0    39170 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/perl.py
+-rw-r--r--   0        0        0    23252 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/phix.py
+-rw-r--r--   0        0        0    12505 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/php.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/pointless.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/pony.py
+-rw-r--r--   0        0        0    12677 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/praat.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/procfile.py
+-rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/prolog.py
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/promql.py
+-rw-r--r--   0        0        0    53524 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/python.py
+-rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/q.py
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/qlik.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/qvt.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/r.py
+-rw-r--r--   0        0        0    15790 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/rdf.py
+-rw-r--r--   0        0        0    18600 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/rebol.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/resource.py
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ride.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/rita.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/rnc.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/roboconf.py
+-rw-r--r--   0        0        0    18449 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/robotframework.py
+-rw-r--r--   0        0        0    22775 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ruby.py
+-rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/rust.py
+-rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/sas.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/savi.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/scdoc.py
+-rw-r--r--   0        0        0    70014 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/scripting.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/sgf.py
+-rw-r--r--   0        0        0    36344 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/shell.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/sieve.py
+-rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/slash.py
+-rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/smalltalk.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/smithy.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/smv.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/snobol.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/solidity.py
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/sophia.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/special.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/spice.py
+-rw-r--r--   0        0        0    34151 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/sql.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/srcinfo.py
+-rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/stata.py
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/supercollider.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/tal.py
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/tcl.py
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/teal.py
+-rw-r--r--   0        0        0    72695 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/templates.py
+-rw-r--r--   0        0        0     9719 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/teraterm.py
+-rw-r--r--   0        0        0    10767 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/testing.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/text.py
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/textedit.py
+-rw-r--r--   0        0        0    15192 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/textfmts.py
+-rw-r--r--   0        0        0    20157 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/theorem.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/thingsdb.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/tlb.py
+-rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/tnt.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/trafficscript.py
+-rw-r--r--   0        0        0     8207 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/typoscript.py
+-rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ul4.py
+-rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/unicon.py
+-rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/urbi.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/usd.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/varnish.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/verification.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/web.py
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/webassembly.py
+-rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/webidl.py
+-rw-r--r--   0        0        0    40549 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/webmisc.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/whiley.py
+-rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/wowtoc.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/wren.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/x10.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/xorg.py
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/yang.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/zig.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/__init__.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/abap.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/algol.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/algol_nu.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/arduino.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/autumn.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/borland.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/bw.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/colorful.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/default.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/dracula.py
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/emacs.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/friendly.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/friendly_grayscale.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/fruity.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/gh_dark.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/gruvbox.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/igor.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/inkpot.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/lilypond.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/lovelace.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/manni.py
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/material.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/monokai.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/murphy.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/native.py
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/nord.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/onedark.py
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/paraiso_dark.py
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/paraiso_light.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/pastie.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/perldoc.py
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/rainbow_dash.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/rrt.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/sas.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/solarized.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/staroffice.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/stata_dark.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/stata_light.py
+-rw-r--r--   0        0        0     7039 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/tango.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/trac.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/vim.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/vs.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/xcode.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/zenburn.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/METADATA
+-rw-r--r--   0        0        0     5598 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/RECORD
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer/__about__.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer/__init__.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer/__main__.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer/clean.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer/markdown.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer/py.typed
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer/rst.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer/txt.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer-37.3.dist-info/INSTALLER
+-rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer-37.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer-37.3.dist-info/METADATA
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer-37.3.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer-37.3.dist-info/WHEEL
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer-37.3.dist-info/top_level.txt
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/__version__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/_internal_utils.py
+-rw-r--r--   0        0        0    21287 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/adapters.py
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/auth.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/certs.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/cookies.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/exceptions.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/hooks.py
+-rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/models.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/packages.py
+-rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/structures.py
+-rw-r--r--   0        0        0    33228 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests/utils.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests-2.28.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests-2.28.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests-2.28.2.dist-info/METADATA
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests-2.28.2.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests-2.28.2.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests-2.28.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/__init__.py
+-rw-r--r--   0        0        0     9512 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/_compat.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/exceptions.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/sessions.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/streaming_iterator.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/adapters/__init__.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/adapters/appengine.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/adapters/socket_options.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/adapters/source.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/adapters/ssl.py
+-rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/adapters/x509.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/auth/__init__.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/auth/guess.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/auth/handler.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/cookies/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/cookies/forgetful.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/downloadutils/__init__.py
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/downloadutils/stream.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/downloadutils/tee.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/multipart/__init__.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/multipart/decoder.py
+-rw-r--r--   0        0        0    20769 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/multipart/encoder.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/threaded/__init__.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/threaded/pool.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/threaded/thread.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/utils/__init__.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/utils/deprecated.py
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/utils/dump.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/utils/formdata.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/utils/user_agent.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/AUTHORS.rst
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    14003 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/METADATA
+-rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/WHEEL
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/__init__.py
+-rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/_mixin.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/abnf_regexp.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/api.py
+-rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/builder.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/compat.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/exceptions.py
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/iri.py
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/misc.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/normalizers.py
+-rw-r--r--   0        0        0    14599 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/parseresult.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/uri.py
+-rw-r--r--   0        0        0    13676 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/validators.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/__init__.py
+-rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_export_format.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_extension.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_fileno.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_inspect.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_loop.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_pick.py
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_timer.py
+-rw-r--r--   0        0        0    22784 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_win32_console.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_windows.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/_wrap.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/abc.py
+-rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/align.py
+-rw-r--r--   0        0        0     6819 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/bar.py
+-rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/box.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/cells.py
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/columns.py
+-rw-r--r--   0        0        0    99018 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/containers.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/control.py
+-rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/default_styles.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/diagnose.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/filesize.py
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/highlighter.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/json.py
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/jupyter.py
+-rw-r--r--   0        0        0    13947 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/layout.py
+-rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/live.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/live_render.py
+-rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/logging.py
+-rw-r--r--   0        0        0    22368 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/markdown.py
+-rw-r--r--   0        0        0     8174 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/measure.py
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/pager.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/palette.py
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/panel.py
+-rw-r--r--   0        0        0    37348 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/pretty.py
+-rw-r--r--   0        0        0    59668 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/progress.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/progress_bar.py
+-rw-r--r--   0        0        0    11291 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/prompt.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/py.typed
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/region.py
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/repr.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/rule.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/scope.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/screen.py
+-rw-r--r--   0        0        0    24195 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/segment.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/status.py
+-rw-r--r--   0        0        0    26332 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/style.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/styled.py
+-rw-r--r--   0        0        0    34868 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/syntax.py
+-rw-r--r--   0        0        0    39648 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/terminal_theme.py
+-rw-r--r--   0        0        0    45670 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/text.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/themes.py
+-rw-r--r--   0        0        0    29102 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/traceback.py
+-rw-r--r--   0        0        0     9109 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich/tree.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich-13.3.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich-13.3.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    18759 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich-13.3.1.dist-info/METADATA
+-rw-r--r--   0        0        0     9572 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich-13.3.1.dist-info/RECORD
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/rich-13.3.1.dist-info/WHEEL
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_deprecation_warning.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_imp.py
+-rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/archive_util.py
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/build_meta.py
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/cli-32.exe
+-rwxr-xr-x   0        0        0    74752 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/cli-64.exe
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/cli.exe
+-rw-r--r--   0        0        0    22279 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/config.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/dep_util.py
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/depends.py
+-rw-r--r--   0        0        0    42374 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/dist.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/errors.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/extension.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/glob.py
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/gui-32.exe
+-rwxr-xr-x   0        0        0    75264 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/gui-64.exe
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/gui.exe
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/installer.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/launch.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/lib2to3_ex.py
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/monkey.py
+-rw-r--r--   0        0        0    50561 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/msvc.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/namespaces.py
+-rw-r--r--   0        0        0    40173 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/package_index.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/py34compat.py
+-rw-r--r--   0        0        0    14151 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/sandbox.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/script (dev).tmpl
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/script.tmpl
+-rw-r--r--   0        0        0     8565 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/ssl_support.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/version.py
+-rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/wheel.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/windows_support.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0        0        0    20813 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0        0        0    14894 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0        0        0    47607 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0        0        0    18079 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/cmd.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0        0        0     8876 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0        0        0    16380 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0        0        0     7778 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0        0        0    50421 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0        0        0    17784 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0        0        0     8148 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0        0        0    12832 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0        0        0    30453 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0        0        0    23540 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/py35compat.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0        0        0    21349 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0        0        0    12483 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0        0        0    14696 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0        0        0    20985 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0        0        0    35579 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist_msi.py
+-rw-r--r--   0        0        0    21537 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0        0        0    16030 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist_wininst.py
+-rw-r--r--   0        0        0     5767 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0        0        0    31685 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0        0        0    17190 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0        0        0    13117 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0        0        0    27482 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0        0        0    19005 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0        0        0   232056 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0   117968 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_compat.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_typing.py
+-rw-r--r--   0        0        0     9509 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    31944 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    24067 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/alias.py
+-rw-r--r--   0        0        0    16604 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0        0        0     8930 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/develop.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0        0        0    85308 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0        0        0    25335 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/install.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/launcher manifest.xml
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/register.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/test.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/upload.py
+-rw-r--r--   0        0        0     7218 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools-57.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools-57.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools-57.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0    21856 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools-57.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools-57.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools-57.0.0.dist-info/dependency_links.txt
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools-57.0.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/setuptools-57.0.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/six-1.16.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/six-1.16.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/six-1.16.0.dist-info/METADATA
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/six-1.16.0.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/six-1.16.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/six-1.16.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/tomli/_types.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/tomli/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/tomli-2.0.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/tomli-2.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/tomli-2.0.1.dist-info/METADATA
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/tomli-2.0.1.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/tomli-2.0.1.dist-info/WHEEL
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/__init__.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/__main__.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/auth.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/cli.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/exceptions.py
+-rw-r--r--   0        0        0    11024 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/py.typed
+-rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/repository.py
+-rw-r--r--   0        0        0    12269 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/settings.py
+-rw-r--r--   0        0        0    10867 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/utils.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/wheel.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/wininst.py
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/commands/__init__.py
+-rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/commands/check.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/commands/register.py
+-rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine/commands/upload.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine-4.0.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine-4.0.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine-4.0.2.dist-info/METADATA
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine-4.0.2.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine-4.0.2.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine-4.0.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine-4.0.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/twine-4.0.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/METADATA
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/_version.py
+-rw-r--r--   0        0        0    20070 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/connection.py
+-rw-r--r--   0        0        0    39095 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/filepost.py
+-rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/request.py
+-rw-r--r--   0        0        0    30761 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11012 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17055 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34416 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/queue.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/response.py
+-rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17165 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14281 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/wait.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3-1.26.14.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3-1.26.14.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0    47722 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3-1.26.14.dist-info/METADATA
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3-1.26.14.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3-1.26.14.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/urllib3-1.26.14.dist-info/top_level.txt
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/webencodings-0.5.1.dist-info/DESCRIPTION.rst
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/webencodings-0.5.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/webencodings-0.5.1.dist-info/METADATA
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/webencodings-0.5.1.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/webencodings-0.5.1.dist-info/WHEEL
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/webencodings-0.5.1.dist-info/metadata.json
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/webencodings-0.5.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/__init__.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/__main__.py
+-rw-r--r--   0        0        0    19075 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/bdist_wheel.py
+-rw-r--r--   0        0        0    15931 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/macosx_libfile.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/metadata.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/pkginfo.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/util.py
+-rw-r--r--   0        0        0     7336 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/wheelfile.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/cli/__init__.py
+-rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/cli/convert.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/cli/pack.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/cli/unpack.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/vendored/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/vendored/packaging/__init__.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/vendored/packaging/_typing.py
+-rw-r--r--   0        0        0    28937 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel/vendored/packaging/tags.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel-0.36.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel-0.36.2.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel-0.36.2.dist-info/METADATA
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel-0.36.2.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel-0.36.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel-0.36.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/wheel-0.36.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/pywintypes.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/version.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/win32api.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/win32cred.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/__init__.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/_winerrors.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/compat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/cffi/__init__.py
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/cffi/_authentication.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/cffi/_common.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/cffi/_dll.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/cffi/_nl_support.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/cffi/_resource.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/cffi/_system_information.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/cffi/_time.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/cffi/_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/ctypes/__init__.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_common.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_dll.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_nl_support.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_resource.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_time.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_util.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/pywin32/__init__.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/pywin32/pywintypes.py
+-rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/pywin32/win32api.py
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/pywin32/win32cred.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/tests/__init__.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/tests/compat.py
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/tests/test_win32api.py
+-rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/tests/test_win32cred.py
+-rw-r--r--   0        0        0    10455 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/zipp/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/zipp/py310compat.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/zipp-3.14.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/zipp-3.14.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/zipp-3.14.0.dist-info/METADATA
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/zipp-3.14.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/zipp-3.14.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Lib/site-packages/zipp-3.14.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/activate
+-rwxr-xr-x   0        0        0     1020 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/activate.bat
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/activate.fish
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/activate.ps1
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/activate.xsh
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/activate_this.py
+-rwxr-xr-x   0        0        0      510 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/deactivate.bat
+-rwxr-xr-x   0        0        0    97136 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/docutils.exe
+-rwxr-xr-x   0        0        0    97130 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/keyring.exe
+-rwxr-xr-x   0        0        0    97140 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/markdown-it.exe
+-rwxr-xr-x   0        0        0    97164 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/normalizer.exe
+-rwxr-xr-x   0        0        0    98165 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/pip.exe
+-rwxr-xr-x   0        0        0    98165 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/pip3.7.exe
+-rwxr-xr-x   0        0        0    98165 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/pip3.exe
+-rwxr-xr-x   0        0        0    97138 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/pkginfo.exe
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/pydoc.bat
+-rwxr-xr-x   0        0        0    97135 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/pygmentize.exe
+-rwxr-xr-x   0        0        0    97145 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/pyproject-build.exe
+-rwxr-xr-x   0        0        0   413712 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/python.exe
+-rwxr-xr-x   0        0        0   412688 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/pythonw.exe
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/rst2html.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/rst2html4.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/rst2html5.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/rst2latex.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/rst2man.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/rst2odt.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/rst2odt_prepstyles.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/rst2pseudoxml.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/rst2s5.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/rst2xetex.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/rst2xml.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/rstpep2html.py
+-rwxr-xr-x   0        0        0    97133 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/twine.exe
+-rwxr-xr-x   0        0        0    97128 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/wheel-3.7.exe
+-rwxr-xr-x   0        0        0    97128 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/wheel.exe
+-rwxr-xr-x   0        0        0    97128 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/wheel3.7.exe
+-rwxr-xr-x   0        0        0    97128 2020-02-02 00:00:00.000000 tomaserial-0.1.2/venv/Scripts/wheel3.exe
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 tomaserial-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 tomaserial-0.1.2/LICENSE
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tomaserial-0.1.2/README.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 tomaserial-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tomaserial-0.1.2/PKG-INFO
```

### Comparing `tomaserial-0.1.1/publish.py` & `tomaserial-0.1.2/publish.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/serial/serial.py` & `tomaserial-0.1.2/serial/serial.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/_virtualenv.py` & `tomaserial-0.1.2/venv/Lib/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/six.py` & `tomaserial-0.1.2/venv/Lib/site-packages/six.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/typing_extensions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/Pygments-2.14.0.dist-info/AUTHORS` & `tomaserial-0.1.2/venv/Lib/site-packages/Pygments-2.14.0.dist-info/AUTHORS`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/Pygments-2.14.0.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/Pygments-2.14.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/Pygments-2.14.0.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/Pygments-2.14.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/Pygments-2.14.0.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/Pygments-2.14.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/_distutils_hack/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/callbacks.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/callbacks.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/css_sanitizer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/css_sanitizer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/html5lib_shim.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/html5lib_shim.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/linkifier.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/linkifier.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/sanitizer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/sanitizer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/README.rst` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/README.rst`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/parse.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/parse.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/_ihatexml.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_ihatexml.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/_inputstream.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_inputstream.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/_tokenizer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/_utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/constants.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/constants.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/html5parser.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/html5parser.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/serializer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/serializer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/_base.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/_base.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/py.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/py.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/lint.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/lint.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/whitespace.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/filters/whitespace.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/base.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/base.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/base.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/base.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/AUTHORS.rst` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach-6.0.0.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach-6.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach-6.0.0.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach-6.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/bleach-6.0.0.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/bleach-6.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/build-0.10.0.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/build-0.10.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/build-0.10.0.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/build-0.10.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/build-0.10.0.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/build-0.10.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/certifi/cacert.pem` & `tomaserial-0.1.2/venv/Lib/site-packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/certifi/core.py` & `tomaserial-0.1.2/venv/Lib/site-packages/certifi/core.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/certifi-2022.12.7.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/certifi-2022.12.7.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/certifi-2022.12.7.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/certifi-2022.12.7.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/certifi-2022.12.7.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/certifi-2022.12.7.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/api.py` & `tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/api.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/cd.py` & `tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/cd.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/constant.py` & `tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/constant.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/legacy.py` & `tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/legacy.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/md.py` & `tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/md.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/models.py` & `tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/models.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/assets/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer/cli/normalizer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer/cli/normalizer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/charset_normalizer-3.0.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/colorama/ansi.py` & `tomaserial-0.1.2/venv/Lib/site-packages/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/colorama/ansitowin32.py` & `tomaserial-0.1.2/venv/Lib/site-packages/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/colorama/initialise.py` & `tomaserial-0.1.2/venv/Lib/site-packages/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/colorama/win32.py` & `tomaserial-0.1.2/venv/Lib/site-packages/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/colorama/winterm.py` & `tomaserial-0.1.2/venv/Lib/site-packages/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/colorama/tests/ansi_test.py` & `tomaserial-0.1.2/venv/Lib/site-packages/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/colorama/tests/ansitowin32_test.py` & `tomaserial-0.1.2/venv/Lib/site-packages/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/colorama/tests/initialise_test.py` & `tomaserial-0.1.2/venv/Lib/site-packages/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/colorama/tests/isatty_test.py` & `tomaserial-0.1.2/venv/Lib/site-packages/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/colorama/tests/utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/colorama/tests/winterm_test.py` & `tomaserial-0.1.2/venv/Lib/site-packages/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/colorama-0.4.6.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/colorama-0.4.6.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/colorama-0.4.6.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/colorama-0.4.6.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/__main__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/__main__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/core.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/core.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/examples.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/examples.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/frontend.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/frontend.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/io.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/io.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/nodes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/nodes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/statemachine.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/statemachine.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/af.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/af.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/ar.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/ar.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/ca.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/ca.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/cs.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/cs.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/da.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/da.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/de.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/de.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/en.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/en.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/eo.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/eo.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/es.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/es.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/fa.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/fa.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/fi.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/fi.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/fr.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/fr.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/gl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/gl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/he.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/he.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/it.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/it.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/ja.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/ja.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/ko.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/ko.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/lt.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/lt.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/lv.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/lv.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/nl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/nl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/pl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/pl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/pt_br.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/pt_br.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/ru.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/ru.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/sk.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/sk.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/sv.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/sv.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/zh_cn.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/zh_cn.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/languages/zh_tw.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/languages/zh_tw.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/commonmark_wrapper.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/commonmark_wrapper.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/roles.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/roles.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/states.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/states.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/tableparser.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/tableparser.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/body.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/body.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/html.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/html.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/images.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/images.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/misc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/misc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/parts.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/parts.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/references.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/references.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/directives/tables.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/directives/tables.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/README.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/README.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsa.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsa.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsb.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsb.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsc.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsc.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsn.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsn.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isoamso.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamso.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsr.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isoamsr.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isobox.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isobox.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr1.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr1.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr2.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isocyr2.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isodia.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isodia.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk1.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk1.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk2.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk2.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk3.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk3.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isolat1.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isolat1.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isolat2.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isolat2.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf-wide.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf-wide.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomopf.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr-wide.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr-wide.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isomscr.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isonum.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isonum.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isopub.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isopub.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/isotech.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/isotech.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/mmlalias.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/mmlalias.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/s5defs.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/s5defs.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-special.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-special.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/af.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/af.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/ar.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ar.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/ca.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ca.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/cs.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/cs.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/da.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/da.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/de.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/de.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/en.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/en.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/eo.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/eo.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/es.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/es.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/fa.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/fa.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/fi.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/fi.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/fr.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/fr.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/gl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/gl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/he.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/he.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/it.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/it.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/ja.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ja.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/ko.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ko.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/lt.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/lt.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/lv.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/lv.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/nl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/nl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/pl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/pl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/ru.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/ru.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/sk.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/sk.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/sv.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/sv.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/readers/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/readers/doctree.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/readers/doctree.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/readers/pep.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/readers/pep.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/readers/standalone.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/readers/standalone.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/components.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/components.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/frontmatter.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/frontmatter.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/misc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/misc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/parts.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/parts.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/peps.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/peps.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/references.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/references.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/universal.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/universal.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/transforms/writer_aux.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/transforms/writer_aux.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/code_analyzer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/code_analyzer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/error_reporting.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/error_reporting.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/punctuation_chars.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/punctuation_chars.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/roman.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/roman.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/smartquotes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/smartquotes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/urischemes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/urischemes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/math/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/math/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/math/latex2mathml.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/math/latex2mathml.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/math/math2html.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/math/math2html.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/math/tex2unichar.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/math/tex2unichar.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/utils/math/unichar2tex.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/utils/math/unichar2tex.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/_html_base.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/_html_base.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/docutils_xml.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/docutils_xml.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/manpage.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/manpage.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/pseudoxml.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/pseudoxml.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html4css1/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html4css1/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html4css1/html4css1.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html4css1/html4css1.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html5_polyglot/math.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/math.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html5_polyglot/minimal.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/minimal.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html5_polyglot/plain.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/plain.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html5_polyglot/responsive.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/responsive.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/html5_polyglot/tuftig.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/html5_polyglot/tuftig.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/latex2e/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/latex2e/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/latex2e/docutils.sty` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/latex2e/docutils.sty`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/latex2e/titlepage.tex` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/latex2e/titlepage.tex`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/latex2e/xelatex.tex` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/latex2e/xelatex.tex`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/odf_odt/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/odf_odt/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/odf_odt/styles.odt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/odf_odt/styles.odt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/pep_html/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/pep_html/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/pep_html/pep.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/pep_html/pep.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/pep_html/template.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/pep_html/template.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/framing.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/framing.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/framing.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/framing.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/framing.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/framing.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/outline.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/outline.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/pretty.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/pretty.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/print.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/print.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.js` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.js`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/framing.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/framing.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils/writers/xetex/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils/writers/xetex/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/COPYING.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/COPYING.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/SOURCES.html` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/SOURCES.html`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/dependency_links.html` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/dependency_links.html`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/docutils-0.19.dist-info/top_level.html` & `tomaserial-0.1.2/venv/Lib/site-packages/docutils-0.19.dist-info/top_level.html`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/idna/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/idna/codec.py` & `tomaserial-0.1.2/venv/Lib/site-packages/idna/codec.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/idna/core.py` & `tomaserial-0.1.2/venv/Lib/site-packages/idna/core.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/idna/idnadata.py` & `tomaserial-0.1.2/venv/Lib/site-packages/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/idna/intranges.py` & `tomaserial-0.1.2/venv/Lib/site-packages/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/idna/uts46data.py` & `tomaserial-0.1.2/venv/Lib/site-packages/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/idna-3.4.dist-info/LICENSE.md` & `tomaserial-0.1.2/venv/Lib/site-packages/idna-3.4.dist-info/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/idna-3.4.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/idna-3.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/idna-3.4.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/idna-3.4.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_adapters.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_collections.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_functools.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_itertools.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_meta.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_py39compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata/_text.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_metadata-6.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/_adapters.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/_common.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/_compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/_itertools.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/_legacy.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/abc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/readers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/simple.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/_compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/_compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/_path.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/_path.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_compatibilty_files.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_compatibilty_files.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_contents.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_custom.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_files.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_open.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_path.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_read.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_reader.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/test_resource.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/update-zips.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/update-zips.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/zipdata01/ziptestdata.zip` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/zipdata01/ziptestdata.zip`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources/tests/zipdata02/ziptestdata.zip` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources/tests/zipdata02/ziptestdata.zip`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/importlib_resources-5.12.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/jaraco/classes/ancestry.py` & `tomaserial-0.1.2/venv/Lib/site-packages/jaraco/classes/ancestry.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/jaraco/classes/meta.py` & `tomaserial-0.1.2/venv/Lib/site-packages/jaraco/classes/meta.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/jaraco/classes/properties.py` & `tomaserial-0.1.2/venv/Lib/site-packages/jaraco/classes/properties.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/_properties_compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/_properties_compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/backend.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/backend.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/cli.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/cli.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/completion.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/completion.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/core.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/core.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/credentials.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/credentials.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/devpi_client.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/devpi_client.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/errors.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/errors.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/http.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/http.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/SecretService.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/SecretService.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/Windows.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/Windows.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/chainer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/chainer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/fail.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/fail.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/kwallet.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/kwallet.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/libsecret.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/libsecret.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/macOS/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/macOS/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/backends/macOS/api.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/backends/macOS/api.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/testing/backend.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/testing/backend.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/testing/util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/testing/util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/util/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring/util/platform_.py` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring/util/platform_.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring-23.13.1.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring-23.13.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring-23.13.1.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring-23.13.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/keyring-23.13.1.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/keyring-23.13.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/_punycode.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/_punycode.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/main.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/main.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/parser_block.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/parser_block.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/parser_core.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/parser_core.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/parser_inline.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/parser_inline.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/port.yaml` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/port.yaml`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/renderer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/renderer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/ruler.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/ruler.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/token.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/token.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/tree.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/tree.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/cli/parse.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/cli/parse.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/common/html_blocks.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/common/html_blocks.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/common/html_re.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/common/html_re.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/common/normalize_url.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/common/normalize_url.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/common/utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/common/utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/helpers/parse_link_destination.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/helpers/parse_link_destination.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/helpers/parse_link_label.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/helpers/parse_link_label.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/helpers/parse_link_title.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/helpers/parse_link_title.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/presets/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/presets/commonmark.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/presets/commonmark.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/presets/default.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/presets/default.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/presets/zero.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/presets/zero.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/blockquote.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/blockquote.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/code.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/code.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/fence.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/fence.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/heading.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/heading.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/hr.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/hr.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/html_block.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/html_block.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/lheading.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/lheading.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/list.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/list.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/paragraph.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/paragraph.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/reference.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/reference.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/state_block.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/state_block.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_block/table.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_block/table.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_core/linkify.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_core/linkify.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_core/replacements.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_core/replacements.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_core/smartquotes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_core/smartquotes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_core/state_core.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_core/state_core.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/autolink.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/autolink.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/backticks.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/backticks.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/emphasis.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/emphasis.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/entity.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/entity.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/escape.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/escape.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/html_inline.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/html_inline.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/image.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/image.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/link.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/link.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/newline.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/newline.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/state_inline.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/state_inline.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/strikethrough.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/strikethrough.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/text.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/text.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it/rules_inline/text_collapse.py` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it/rules_inline/text_collapse.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE.markdown-it` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/LICENSE.markdown-it`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/mdurl/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/mdurl/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/mdurl/_decode.py` & `tomaserial-0.1.2/venv/Lib/site-packages/mdurl/_decode.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/mdurl/_encode.py` & `tomaserial-0.1.2/venv/Lib/site-packages/mdurl/_encode.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/mdurl/_format.py` & `tomaserial-0.1.2/venv/Lib/site-packages/mdurl/_format.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/mdurl/_parse.py` & `tomaserial-0.1.2/venv/Lib/site-packages/mdurl/_parse.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/mdurl-0.1.2.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/mdurl-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/mdurl-0.1.2.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/mdurl-0.1.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/mdurl-0.1.2.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/mdurl-0.1.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/more_itertools/more.py` & `tomaserial-0.1.2/venv/Lib/site-packages/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/more_itertools/more.pyi` & `tomaserial-0.1.2/venv/Lib/site-packages/more_itertools/more.pyi`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/more_itertools/recipes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/more_itertools/recipes.pyi` & `tomaserial-0.1.2/venv/Lib/site-packages/more_itertools/recipes.pyi`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/more_itertools-9.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging/_elffile.py` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging/_manylinux.py` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging/_musllinux.py` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging/_parser.py` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging/_structures.py` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging/_tokenizer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging/markers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging/requirements.py` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging/specifiers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging/tags.py` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging/utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging/version.py` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging/version.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging-23.0.dist-info/LICENSE.APACHE` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging-23.0.dist-info/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging-23.0.dist-info/LICENSE.BSD` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging-23.0.dist-info/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging-23.0.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging-23.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/packaging-23.0.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/packaging-23.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/__main__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/__pip-runner__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/build_env.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cache.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/configuration.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/exceptions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/pyproject.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/self_outdated_check.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/wheel_builder.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/base_command.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/command_context.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/main.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/main_parser.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/parser.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/req_command.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/cli/spinners.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/cache.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/check.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/completion.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/configuration.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/debug.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/download.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/freeze.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/hash.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/help.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/index.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/inspect.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/install.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/list.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/search.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/show.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/uninstall.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/commands/wheel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/distributions/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/distributions/base.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/distributions/installed.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/distributions/sdist.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/distributions/wheel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/index/collector.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/index/package_finder.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/index/sources.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/locations/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/locations/_distutils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/locations/base.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/metadata/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/metadata/_json.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/metadata/base.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/candidate.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/direct_url.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/format_control.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/index.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/installation_report.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/link.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/scheme.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/search_scope.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/target_python.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/models/wheel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/network/auth.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/network/cache.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/network/download.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/network/session.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/network/utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/operations/check.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/operations/freeze.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/operations/prepare.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/req/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/req/constructors.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/req/req_file.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/req/req_install.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/req/req_set.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/base.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/_log.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/appdirs.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/deprecation.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/egg_link.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/encoding.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/filesystem.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/filetypes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/glibc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/hashes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/logging.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/misc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/models.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/packaging.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/subprocess.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/unpacking.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/urls.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/utils/wheel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/vcs/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/vcs/git.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/vcs/subversion.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/six.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/typing_extensions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/certifi/core.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/enums.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/win32.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/database.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/index.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/locators.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/markers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/resources.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/t32.exe` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/t64.exe` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/version.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/w32.exe` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/w64.exe` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distro/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/distro/distro.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/idna/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/idna/codec.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/idna/core.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/idna/intranges.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/markers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/tags.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/packaging/version.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/console.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/filter.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/style.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/token.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/adapters.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/api.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/auth.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/certs.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/cookies.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/help.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/hooks.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/models.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/packages.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/sessions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/structures.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/requests/utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/__main__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_loop.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_null_file.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_windows.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/abc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/align.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/ansi.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/bar.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/box.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/cells.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/color.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/columns.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/console.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/constrain.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/containers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/control.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/emoji.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/errors.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/filesize.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/json.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/layout.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/live.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/live_render.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/logging.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/markup.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/measure.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/padding.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/pager.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/palette.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/panel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/pretty.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/progress.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/prompt.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/protocol.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/repr.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/rule.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/scope.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/screen.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/segment.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/spinner.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/status.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/style.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/styled.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/syntax.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/table.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/text.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/theme.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/traceback.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/rich/tree.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/after.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/before.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/tomli/_re.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/request.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/response.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip-23.0.1.dist-info/LICENSE.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/pip-23.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip-23.0.1.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/pip-23.0.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pip-23.0.1.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/pip-23.0.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_typing.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkg_resources/extern/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/bdist.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/bdist.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/commandline.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/commandline.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/commandline.pyi` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/commandline.pyi`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/develop.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/develop.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/distribution.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/distribution.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/distribution.pyi` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/distribution.pyi`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/index.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/index.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/installed.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/installed.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/sdist.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/sdist.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/wheel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/wheel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_bdist.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_bdist.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_commandline.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_commandline.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_develop.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_develop.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_distribution.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_index.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_installed.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_installed.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_sdist.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_sdist.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo/tests/test_wheel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/LICENSE.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/pkginfo-1.9.6.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/cmdline.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/console.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/console.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/filter.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatter.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/modeline.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/plugin.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/regexopt.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/scanner.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/sphinxext.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/style.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/style.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/token.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/token.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/unistring.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/filters/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/_mapping.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/bbcode.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/groff.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/html.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/img.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/irc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/latex.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/other.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/pangomarkup.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/rtf.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/svg.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/terminal.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/formatters/terminal256.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_ada_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_ada_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_asy_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_asy_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_cl_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_cl_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_cocoa_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_cocoa_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_csound_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_csound_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_css_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_css_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_julia_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_julia_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_lasso_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_lasso_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_lilypond_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_lilypond_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_lua_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_lua_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_mapping.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_mql_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_mql_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_mysql_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_mysql_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_openedge_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_openedge_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_php_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_php_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_postgres_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_postgres_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_qlik_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_qlik_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_scheme_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_scheme_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_scilab_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_scilab_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_stan_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_stan_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_stata_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_stata_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_tsql_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_tsql_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_usd_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_usd_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_vbscript_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_vbscript_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/_vim_builtins.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/_vim_builtins.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/actionscript.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/actionscript.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ada.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ada.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/agile.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/agile.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/algebra.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/algebra.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ambient.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ambient.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/amdgpu.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/amdgpu.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ampl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ampl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/apdlexer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/apdlexer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/apl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/apl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/archetype.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/archetype.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/arrow.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/arrow.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/arturo.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/arturo.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/asc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/asc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/asm.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/asm.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/automation.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/automation.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/bare.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/bare.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/basic.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/basic.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/bdd.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/bdd.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/berry.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/berry.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/bibtex.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/bibtex.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/boa.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/boa.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/business.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/business.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/c_cpp.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/c_cpp.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/c_like.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/c_like.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/capnproto.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/capnproto.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/cddl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/cddl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/chapel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/chapel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/clean.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/clean.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/comal.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/comal.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/compiled.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/compiled.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/configs.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/configs.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/console.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/console.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/cplint.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/cplint.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/crystal.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/crystal.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/csound.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/csound.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/css.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/css.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/d.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/d.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/dalvik.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/dalvik.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/data.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/data.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/devicetree.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/devicetree.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/diff.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/diff.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/dotnet.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/dotnet.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/dsls.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/dsls.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/dylan.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/dylan.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ecl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ecl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/eiffel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/eiffel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/elm.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/elm.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/elpi.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/elpi.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/email.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/email.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/erlang.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/erlang.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/esoteric.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/esoteric.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ezhil.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ezhil.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/factor.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/factor.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/fantom.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/fantom.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/felix.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/felix.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/fift.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/fift.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/floscript.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/floscript.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/forth.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/forth.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/fortran.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/fortran.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/foxpro.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/foxpro.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/freefem.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/freefem.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/func.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/func.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/functional.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/functional.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/futhark.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/futhark.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/gcodelexer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/gcodelexer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/gdscript.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/gdscript.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/go.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/go.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/grammar_notation.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/grammar_notation.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/graph.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/graph.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/graphics.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/graphics.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/graphviz.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/graphviz.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/gsql.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/gsql.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/haskell.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/haskell.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/haxe.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/haxe.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/hdl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/hdl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/hexdump.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/hexdump.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/html.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/html.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/idl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/idl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/igor.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/igor.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/inferno.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/inferno.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/installers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/installers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/int_fiction.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/int_fiction.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/iolang.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/iolang.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/j.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/j.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/javascript.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/javascript.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/jmespath.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/jmespath.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/jslt.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/jslt.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/jsonnet.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/jsonnet.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/julia.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/julia.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/jvm.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/jvm.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/kuin.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/kuin.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/lilypond.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/lilypond.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/lisp.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/lisp.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/macaulay2.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/macaulay2.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/make.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/make.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/markup.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/markup.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/math.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/math.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/matlab.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/matlab.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/maxima.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/maxima.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/meson.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/meson.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/mime.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/mime.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/minecraft.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/minecraft.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/mips.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/mips.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ml.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ml.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/modeling.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/modeling.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/modula2.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/modula2.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/monte.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/monte.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/mosel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/mosel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ncl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ncl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/nimrod.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/nimrod.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/nit.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/nit.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/nix.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/nix.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/oberon.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/oberon.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/objective.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/objective.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ooc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ooc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/other.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/other.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/parasail.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/parasail.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/parsers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/parsers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/pascal.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/pascal.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/pawn.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/pawn.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/perl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/perl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/phix.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/phix.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/php.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/php.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/pointless.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/pointless.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/pony.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/pony.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/praat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/praat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/procfile.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/procfile.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/prolog.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/prolog.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/promql.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/promql.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/python.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/q.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/q.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/qlik.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/qlik.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/qvt.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/qvt.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/r.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/r.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/rdf.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/rdf.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/rebol.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/rebol.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/resource.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/resource.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ride.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ride.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/rita.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/rita.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/rnc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/rnc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/roboconf.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/roboconf.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/robotframework.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/robotframework.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ruby.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ruby.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/rust.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/rust.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/sas.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/sas.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/savi.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/savi.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/scdoc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/scdoc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/scripting.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/scripting.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/sgf.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/sgf.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/shell.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/shell.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/sieve.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/sieve.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/slash.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/slash.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/smalltalk.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/smalltalk.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/smithy.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/smithy.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/smv.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/smv.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/snobol.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/snobol.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/solidity.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/solidity.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/sophia.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/sophia.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/special.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/special.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/spice.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/spice.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/sql.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/sql.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/srcinfo.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/srcinfo.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/stata.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/stata.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/supercollider.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/supercollider.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/tal.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/tal.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/tcl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/tcl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/teal.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/teal.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/templates.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/templates.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/teraterm.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/teraterm.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/testing.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/testing.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/text.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/text.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/textedit.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/textedit.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/textfmts.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/textfmts.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/theorem.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/theorem.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/thingsdb.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/thingsdb.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/tlb.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/tlb.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/tnt.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/tnt.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/trafficscript.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/trafficscript.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/typoscript.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/typoscript.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/ul4.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/ul4.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/unicon.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/unicon.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/urbi.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/urbi.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/usd.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/usd.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/varnish.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/varnish.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/verification.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/verification.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/web.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/web.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/webassembly.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/webassembly.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/webidl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/webidl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/webmisc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/webmisc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/whiley.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/whiley.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/wowtoc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/wowtoc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/wren.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/wren.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/x10.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/x10.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/xorg.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/xorg.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/yang.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/yang.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/lexers/zig.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/lexers/zig.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/abap.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/abap.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/algol.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/algol.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/algol_nu.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/algol_nu.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/arduino.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/arduino.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/autumn.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/autumn.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/borland.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/borland.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/bw.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/bw.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/colorful.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/colorful.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/default.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/default.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/dracula.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/dracula.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/emacs.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/emacs.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/friendly.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/friendly.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/friendly_grayscale.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/friendly_grayscale.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/fruity.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/fruity.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/gh_dark.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/gh_dark.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/gruvbox.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/gruvbox.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/igor.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/igor.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/inkpot.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/inkpot.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/lilypond.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/lilypond.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/lovelace.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/lovelace.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/manni.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/manni.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/material.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/material.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/monokai.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/monokai.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/murphy.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/murphy.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/native.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/native.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/nord.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/nord.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/onedark.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/onedark.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/paraiso_dark.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/paraiso_dark.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/paraiso_light.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/paraiso_light.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/pastie.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/pastie.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/perldoc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/perldoc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/rainbow_dash.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/rainbow_dash.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/rrt.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/rrt.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/sas.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/sas.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/solarized.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/solarized.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/staroffice.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/staroffice.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/stata_dark.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/stata_dark.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/stata_light.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/stata_light.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/tango.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/tango.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/trac.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/trac.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/vim.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/vim.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/vs.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/vs.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/xcode.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/xcode.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pygments/styles/zenburn.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pygments/styles/zenburn.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks/_impl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks/_in_process/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py` & `tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/LICENSE.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer/__about__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer/__about__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer/__main__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer/__main__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer/clean.py` & `tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer/clean.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer/markdown.py` & `tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer/markdown.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer/rst.py` & `tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer/rst.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer/txt.py` & `tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer/txt.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer-37.3.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer-37.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer-37.3.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer-37.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/readme_renderer-37.3.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/readme_renderer-37.3.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/_internal_utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/adapters.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/api.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/api.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/auth.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/auth.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/cookies.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/exceptions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/help.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/help.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/hooks.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/models.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/models.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/packages.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/packages.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/sessions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/status_codes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/structures.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/structures.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests/utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests/utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests-2.28.2.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/requests-2.28.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests-2.28.2.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/requests-2.28.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests-2.28.2.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/requests-2.28.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/_compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/_compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/exceptions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/exceptions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/sessions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/sessions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/streaming_iterator.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/streaming_iterator.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/adapters/appengine.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/adapters/appengine.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/adapters/socket_options.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/adapters/socket_options.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/adapters/source.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/adapters/source.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/adapters/ssl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/adapters/ssl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/adapters/x509.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/adapters/x509.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/auth/guess.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/auth/guess.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/auth/handler.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/auth/handler.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/downloadutils/stream.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/downloadutils/stream.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/downloadutils/tee.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/downloadutils/tee.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/multipart/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/multipart/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/multipart/decoder.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/multipart/decoder.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/multipart/encoder.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/multipart/encoder.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/threaded/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/threaded/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/threaded/pool.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/threaded/pool.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/threaded/thread.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/threaded/thread.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/utils/deprecated.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/utils/dump.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/utils/dump.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/utils/formdata.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/utils/formdata.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt/utils/user_agent.py` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/AUTHORS.rst` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/_mixin.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/_mixin.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/abnf_regexp.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/abnf_regexp.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/api.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/api.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/builder.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/builder.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/exceptions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/exceptions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/iri.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/iri.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/misc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/misc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/normalizers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/normalizers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/parseresult.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/parseresult.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/uri.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/uri.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986/validators.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986/validators.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/rfc3986-2.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/__main__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_cell_widths.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_emoji_codes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_emoji_replace.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_export_format.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_fileno.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_inspect.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_log_render.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_loop.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_null_file.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_palettes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_ratio.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_spinners.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_win32_console.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_windows.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_windows_renderer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/_wrap.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/abc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/abc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/align.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/align.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/ansi.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/bar.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/bar.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/box.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/box.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/cells.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/cells.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/color.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/color.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/color_triplet.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/columns.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/columns.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/console.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/console.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/constrain.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/containers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/containers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/control.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/control.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/default_styles.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/diagnose.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/emoji.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/errors.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/errors.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/file_proxy.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/filesize.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/highlighter.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/json.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/json.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/jupyter.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/layout.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/layout.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/live.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/live.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/live_render.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/logging.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/logging.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/markdown.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/markdown.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/markup.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/markup.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/measure.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/measure.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/padding.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/padding.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/pager.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/pager.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/palette.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/palette.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/panel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/panel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/pretty.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/progress.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/progress.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/progress_bar.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/prompt.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/protocol.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/repr.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/repr.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/rule.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/rule.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/scope.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/scope.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/screen.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/screen.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/segment.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/segment.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/spinner.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/status.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/status.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/style.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/style.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/styled.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/styled.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/syntax.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/table.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/table.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/terminal_theme.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/text.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/text.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/theme.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/theme.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/traceback.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich/tree.py` & `tomaserial-0.1.2/venv/Lib/site-packages/rich/tree.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich-13.3.1.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/rich-13.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich-13.3.1.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/rich-13.3.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/rich-13.3.1.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/rich-13.3.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_imp.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/archive_util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/build_meta.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/cli-32.exe` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/cli-32.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/cli-64.exe` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/cli-64.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/cli.exe` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/cli.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/config.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/config.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/dep_util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/depends.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/dist.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/errors.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/extension.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/glob.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/gui-32.exe` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/gui-32.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/gui-64.exe` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/gui-64.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/gui.exe` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/gui.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/installer.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/launch.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/lib2to3_ex.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/lib2to3_ex.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/monkey.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/msvc.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/namespaces.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/package_index.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/sandbox.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/ssl_support.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/ssl_support.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/unicode_utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/wheel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/windows_support.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/archive_util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/cmd.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/config.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/core.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/dep_util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/dir_util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/dist.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/errors.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/extension.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/file_util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/filelist.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/log.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/spawn.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/text_file.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/version.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_msi.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist_msi.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_wininst.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/bdist_wininst.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/build.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/check.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/clean.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/config.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/install.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/register.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_distutils/command/upload.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/pyparsing.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_typing.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/alias.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/bdist_egg.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/bdist_rpm.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/build_clib.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/build_ext.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/build_py.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/develop.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/dist_info.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/easy_install.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/egg_info.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/install.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/install_egg_info.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/install_lib.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/install_scripts.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/launcher manifest.xml` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/py36compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/rotate.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/saveopts.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/sdist.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/setopt.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/test.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/command/upload_docs.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools/extern/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools-57.0.0.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools-57.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools-57.0.0.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools-57.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools-57.0.0.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools-57.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/setuptools-57.0.0.dist-info/entry_points.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/setuptools-57.0.0.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/six-1.16.0.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/six-1.16.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/six-1.16.0.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/six-1.16.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/six-1.16.0.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/six-1.16.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/tomli/_parser.py` & `tomaserial-0.1.2/venv/Lib/site-packages/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/tomli/_re.py` & `tomaserial-0.1.2/venv/Lib/site-packages/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/tomli-2.0.1.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/tomli-2.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/tomli-2.0.1.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/tomli-2.0.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/tomli-2.0.1.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/tomli-2.0.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/twine/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine/__main__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/twine/__main__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine/auth.py` & `tomaserial-0.1.2/venv/Lib/site-packages/twine/auth.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine/cli.py` & `tomaserial-0.1.2/venv/Lib/site-packages/twine/cli.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine/exceptions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/twine/exceptions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine/package.py` & `tomaserial-0.1.2/venv/Lib/site-packages/twine/package.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine/repository.py` & `tomaserial-0.1.2/venv/Lib/site-packages/twine/repository.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine/settings.py` & `tomaserial-0.1.2/venv/Lib/site-packages/twine/settings.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine/utils.py` & `tomaserial-0.1.2/venv/Lib/site-packages/twine/utils.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine/wheel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/twine/wheel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine/wininst.py` & `tomaserial-0.1.2/venv/Lib/site-packages/twine/wininst.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine/commands/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/twine/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine/commands/check.py` & `tomaserial-0.1.2/venv/Lib/site-packages/twine/commands/check.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine/commands/register.py` & `tomaserial-0.1.2/venv/Lib/site-packages/twine/commands/register.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine/commands/upload.py` & `tomaserial-0.1.2/venv/Lib/site-packages/twine/commands/upload.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine-4.0.2.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/twine-4.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine-4.0.2.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/twine-4.0.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/twine-4.0.2.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/twine-4.0.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/typing_extensions-4.5.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/_collections.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/connection.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/connectionpool.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/exceptions.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/fields.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/filepost.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/poolmanager.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/request.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/response.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/_appengine_environ.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/appengine.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/ntlmpool.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/pyopenssl.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/securetransport.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/socks.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/_securetransport/bindings.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/contrib/_securetransport/low_level.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/packages/six.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/packages/backports/makefile.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/connection.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/proxy.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/request.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/response.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/retry.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/ssl_.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/ssl_match_hostname.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/ssltransport.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/timeout.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/url.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3/util/wait.py` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3-1.26.14.dist-info/LICENSE.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3-1.26.14.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3-1.26.14.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3-1.26.14.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/urllib3-1.26.14.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/urllib3-1.26.14.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/webencodings/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/webencodings/labels.py` & `tomaserial-0.1.2/venv/Lib/site-packages/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/webencodings/mklabels.py` & `tomaserial-0.1.2/venv/Lib/site-packages/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/webencodings/tests.py` & `tomaserial-0.1.2/venv/Lib/site-packages/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/webencodings/x_user_defined.py` & `tomaserial-0.1.2/venv/Lib/site-packages/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/webencodings-0.5.1.dist-info/DESCRIPTION.rst` & `tomaserial-0.1.2/venv/Lib/site-packages/webencodings-0.5.1.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/webencodings-0.5.1.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/webencodings-0.5.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/webencodings-0.5.1.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/webencodings-0.5.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/webencodings-0.5.1.dist-info/metadata.json` & `tomaserial-0.1.2/venv/Lib/site-packages/webencodings-0.5.1.dist-info/metadata.json`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/wheel/bdist_wheel.py` & `tomaserial-0.1.2/venv/Lib/site-packages/wheel/bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/wheel/macosx_libfile.py` & `tomaserial-0.1.2/venv/Lib/site-packages/wheel/macosx_libfile.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/wheel/metadata.py` & `tomaserial-0.1.2/venv/Lib/site-packages/wheel/metadata.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/wheel/pkginfo.py` & `tomaserial-0.1.2/venv/Lib/site-packages/wheel/pkginfo.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/wheel/util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/wheel/util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/wheel/wheelfile.py` & `tomaserial-0.1.2/venv/Lib/site-packages/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/wheel/cli/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/wheel/cli/convert.py` & `tomaserial-0.1.2/venv/Lib/site-packages/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/wheel/cli/pack.py` & `tomaserial-0.1.2/venv/Lib/site-packages/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/wheel/cli/unpack.py` & `tomaserial-0.1.2/venv/Lib/site-packages/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/wheel/vendored/packaging/_typing.py` & `tomaserial-0.1.2/venv/Lib/site-packages/wheel/vendored/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/wheel/vendored/packaging/tags.py` & `tomaserial-0.1.2/venv/Lib/site-packages/wheel/vendored/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/wheel-0.36.2.dist-info/LICENSE.txt` & `tomaserial-0.1.2/venv/Lib/site-packages/wheel-0.36.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/wheel-0.36.2.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/wheel-0.36.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/wheel-0.36.2.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/wheel-0.36.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/cffi/_authentication.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/cffi/_authentication.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/cffi/_common.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/cffi/_common.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/cffi/_dll.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/cffi/_dll.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/cffi/_resource.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/cffi/_resource.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/cffi/_system_information.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/cffi/_system_information.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/cffi/_util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/cffi/_util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/ctypes/_common.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_common.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/ctypes/_dll.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_dll.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/ctypes/_resource.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_resource.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/core/ctypes/_util.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/core/ctypes/_util.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/pywin32/pywintypes.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/pywin32/pywintypes.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/pywin32/win32api.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/pywin32/win32api.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/pywin32/win32cred.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/pywin32/win32cred.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/tests/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/tests/compat.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/tests/compat.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/tests/test_win32api.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/tests/test_win32api.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/win32ctypes/tests/test_win32cred.py` & `tomaserial-0.1.2/venv/Lib/site-packages/win32ctypes/tests/test_win32cred.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/zipp/__init__.py` & `tomaserial-0.1.2/venv/Lib/site-packages/zipp/__init__.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/zipp-3.14.0.dist-info/LICENSE` & `tomaserial-0.1.2/venv/Lib/site-packages/zipp-3.14.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/zipp-3.14.0.dist-info/METADATA` & `tomaserial-0.1.2/venv/Lib/site-packages/zipp-3.14.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Lib/site-packages/zipp-3.14.0.dist-info/RECORD` & `tomaserial-0.1.2/venv/Lib/site-packages/zipp-3.14.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/activate` & `tomaserial-0.1.2/venv/Scripts/activate`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/activate.bat` & `tomaserial-0.1.2/venv/Scripts/activate.bat`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/activate.fish` & `tomaserial-0.1.2/venv/Scripts/activate.fish`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/activate.ps1` & `tomaserial-0.1.2/venv/Scripts/activate.ps1`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/activate.xsh` & `tomaserial-0.1.2/venv/Scripts/activate.xsh`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/activate_this.py` & `tomaserial-0.1.2/venv/Scripts/activate_this.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/docutils.exe` & `tomaserial-0.1.2/venv/Scripts/docutils.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/keyring.exe` & `tomaserial-0.1.2/venv/Scripts/keyring.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/markdown-it.exe` & `tomaserial-0.1.2/venv/Scripts/markdown-it.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/normalizer.exe` & `tomaserial-0.1.2/venv/Scripts/normalizer.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/pip.exe` & `tomaserial-0.1.2/venv/Scripts/pip.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/pip3.7.exe` & `tomaserial-0.1.2/venv/Scripts/pip3.7.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/pip3.exe` & `tomaserial-0.1.2/venv/Scripts/pip3.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/pkginfo.exe` & `tomaserial-0.1.2/venv/Scripts/pkginfo.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/pygmentize.exe` & `tomaserial-0.1.2/venv/Scripts/pygmentize.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/pyproject-build.exe` & `tomaserial-0.1.2/venv/Scripts/pyproject-build.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/python.exe` & `tomaserial-0.1.2/venv/Scripts/python.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/pythonw.exe` & `tomaserial-0.1.2/venv/Scripts/pythonw.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/rst2html.py` & `tomaserial-0.1.2/venv/Scripts/rst2html.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/rst2html4.py` & `tomaserial-0.1.2/venv/Scripts/rst2html4.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/rst2html5.py` & `tomaserial-0.1.2/venv/Scripts/rst2html5.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/rst2latex.py` & `tomaserial-0.1.2/venv/Scripts/rst2latex.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/rst2man.py` & `tomaserial-0.1.2/venv/Scripts/rst2man.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/rst2odt.py` & `tomaserial-0.1.2/venv/Scripts/rst2odt.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/rst2odt_prepstyles.py` & `tomaserial-0.1.2/venv/Scripts/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/rst2pseudoxml.py` & `tomaserial-0.1.2/venv/Scripts/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/rst2s5.py` & `tomaserial-0.1.2/venv/Scripts/rst2s5.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/rst2xetex.py` & `tomaserial-0.1.2/venv/Scripts/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/rst2xml.py` & `tomaserial-0.1.2/venv/Scripts/rst2xml.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/rstpep2html.py` & `tomaserial-0.1.2/venv/Scripts/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/twine.exe` & `tomaserial-0.1.2/venv/Scripts/twine.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/wheel-3.7.exe` & `tomaserial-0.1.2/venv/Scripts/wheel-3.7.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/wheel.exe` & `tomaserial-0.1.2/venv/Scripts/wheel.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/wheel3.7.exe` & `tomaserial-0.1.2/venv/Scripts/wheel3.7.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/venv/Scripts/wheel3.exe` & `tomaserial-0.1.2/venv/Scripts/wheel3.exe`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/LICENSE` & `tomaserial-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tomaserial-0.1.1/pyproject.toml` & `tomaserial-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "*/.__pycache/",
     "*/.pytest_cache/",
     "*/*test.py"
 ]
 
 [project]
 name = "tomaserial"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name = "sunlulu.tomato", email = "sunlulu.tomato@bytedance.com" },
 ]
 description = "python serial and deserial"
 readme = "README.md"
 license = { file = 'LICENSE' }
 requires-python = ">=3.7"
```

### Comparing `tomaserial-0.1.1/PKG-INFO` & `tomaserial-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomaserial
-Version: 0.1.1
+Version: 0.1.2
 Summary: python serial and deserial
 Project-URL: Homepage, https://github.com/sunlulu427/tomato
 Project-URL: Bug Tracker, https://github.com/sunlulu427/tomato/issues
 Author-email: "sunlulu.tomato" <sunlulu.tomato@bytedance.com>
 License: Copyright (c) <2023> <copyright sunlulu.tomato@bytedance.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

