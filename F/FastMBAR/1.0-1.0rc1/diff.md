# Comparing `tmp/fastmbar-1.0.tar.gz` & `tmp/fastmbar-1.0rc1.tar.gz`

## Comparing `fastmbar-1.0.tar` & `fastmbar-1.0rc1.tar`

### file list

```diff
@@ -1,210 +1,215 @@
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastmbar-1.0/.readthedocs.yaml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastmbar-1.0/.travis.yml
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fastmbar-1.0/build.sh
--rw-r--r--   0        0        0    33346 2020-02-02 00:00:00.000000 fastmbar-1.0/energy_matrix.pdf
--rw-r--r--   0        0        0   459263 2020-02-02 00:00:00.000000 fastmbar-1.0/energy_matrix.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fastmbar-1.0/.vscode/settings.json
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 fastmbar-1.0/FastMBAR/__init__.py
--rw-r--r--   0        0        0    29126 2020-02-02 00:00:00.000000 fastmbar-1.0/FastMBAR/fastmbar.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 fastmbar-1.0/FastMBAR/test_FastMBAR.py
--rw-r--r--   0        0        0     9701 2020-02-02 00:00:00.000000 fastmbar-1.0/FastMBAR/utils/analyzer.py
--rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 fastmbar-1.0/FastMBAR/utils/fastmbartools.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/.gitignore
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/Makefile
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/requirements.txt
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/.buildinfo
--rw-r--r--   0        0        0    30535 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/API.html
--rw-r--r--   0        0        0    56378 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/butane_PMF.html
--rw-r--r--   0        0        0    67565 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/dialanine_PMF.html
--rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/examples.html
--rw-r--r--   0        0        0    12093 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/genindex.html
--rw-r--r--   0        0        0    16014 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/index.html
--rw-r--r--   0        0        0    36805 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/installation.html
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/objects.inv
--rw-r--r--   0        0        0    12811 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/references.html
--rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/search.html
--rw-r--r--   0        0        0    15370 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/searchindex.js
--rw-r--r--   0        0        0    26667 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/usage.html
--rw-r--r--   0        0        0    68887 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/.doctrees/API.doctree
--rw-r--r--   0        0        0    41990 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/.doctrees/butane_PMF.doctree
--rw-r--r--   0        0        0    51030 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/.doctrees/dialanine_PMF.doctree
--rw-r--r--   0        0        0    61760 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/.doctrees/environment.pickle
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/.doctrees/examples.doctree
--rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/.doctrees/index.doctree
--rw-r--r--   0        0        0    33251 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/.doctrees/installation.doctree
--rw-r--r--   0        0        0     8759 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/.doctrees/references.doctree
--rw-r--r--   0        0        0    28287 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/.doctrees/usage.doctree
--rw-r--r--   0        0        0   187708 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_images/Fig_1.png
--rw-r--r--   0        0        0   211402 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_images/Fig_11.png
--rw-r--r--   0        0        0   172324 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_images/Fig_2.png
--rw-r--r--   0        0        0   193626 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_images/Fig_21.png
--rw-r--r--   0        0        0   156671 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_images/PMF.png
--rw-r--r--   0        0        0   116954 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_images/PMF1.png
--rw-r--r--   0        0        0   459263 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_images/energy_matrix.png
--rw-r--r--   0        0        0    10181 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_modules/index.html
--rw-r--r--   0        0        0   125225 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_modules/FastMBAR/fastmbar.html
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_sources/API.rst
--rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_sources/butane_PMF.rst
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_sources/dialanine_PMF.rst
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_sources/examples.rst
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_sources/index.rst
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_sources/installation.rst
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_sources/references.rst
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_sources/usage.rst
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    15228 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/basic.css
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/check-solid.svg
--rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/clipboard.min.js
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/copy-button.svg
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/copybutton.css
--rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/copybutton.js
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/copybutton_funcs.js
--rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/doctools.js
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/file.png
--rw-r--r--   0        0        0   288580 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/jquery-3.6.0.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/jquery.js
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/language_data.js
--rw-r--r--   0        0        0  1201731 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/logo.ai
--rw-r--r--   0        0        0  1249206 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/logo.eps
--rw-r--r--   0        0        0   119173 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/logo.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/plus.png
--rw-r--r--   0        0        0    12757 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/pygments.css
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/sbt-webpack-macros.html
--rw-r--r--   0        0        0    17088 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/searchtools.js
--rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/underscore-1.13.1.js
--rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/underscore.js
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/webpack-macros.html
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/images/logo_binder.svg
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/images/logo_colab.png
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/images/logo_deepnote.svg
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/images/logo_jupyterhub.svg
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/da/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/da/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/de/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/de/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/el/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/el/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/es/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/es/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/et/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/et/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/id/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/id/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/it/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/it/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/no/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/no/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/te/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/te/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/th/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/th/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0    80813 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/scripts/bootstrap.js
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0        0        0   335757 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/scripts/bootstrap.js.map
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0        0        0   176654 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/styles/bootstrap.css
--rw-r--r--   0        0        0    63341 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0        0        0    13841 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/styles/sphinx-book-theme.css
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/styles/theme.css
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/LICENSE.txt
--rw-r--r--   0        0        0   101691 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/css/all.min.css
--rw-r--r--   0        0        0   181264 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   105112 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    60236 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    24028 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   389948 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   154840 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/source/API.rst
--rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/source/butane_PMF.rst
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/source/conf.py
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/source/dialanine_PMF.rst
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/source/examples.rst
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/source/index.rst
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/source/installation.rst
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/source/references.rst
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/source/usage.rst
--rw-r--r--   0        0        0  1201731 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/source/_static/logo.ai
--rw-r--r--   0        0        0  1249206 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/source/_static/logo.eps
--rw-r--r--   0        0        0   119173 2020-02-02 00:00:00.000000 fastmbar-1.0/docs/source/_static/logo.png
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 fastmbar-1.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 fastmbar-1.0/LICENSE
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastmbar-1.0/README.rst
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 fastmbar-1.0/pyproject.toml
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 fastmbar-1.0/PKG-INFO
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/.travis.yml
+-rw-r--r--   0        0        0    33346 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/energy_matrix.pdf
+-rw-r--r--   0        0        0   459263 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/energy_matrix.png
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/setup_backup.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/.vscode/settings.json
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/FastMBAR/__init__.py
+-rw-r--r--   0        0        0    29126 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/FastMBAR/fastmbar.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/FastMBAR/test_installation.py
+-rw-r--r--   0        0        0     9701 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/FastMBAR/utils/analyzer.py
+-rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/FastMBAR/utils/fastmbartools.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/conda/README.md
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/conda/bld.bat
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/conda/build.sh
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/conda/meta.yaml
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/conda/conda_build/.gitignore
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/.gitignore
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/Makefile
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/requirements.txt
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/.buildinfo
+-rw-r--r--   0        0        0    30535 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/API.html
+-rw-r--r--   0        0        0    56378 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/butane_PMF.html
+-rw-r--r--   0        0        0    67565 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/dialanine_PMF.html
+-rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/examples.html
+-rw-r--r--   0        0        0    12093 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/genindex.html
+-rw-r--r--   0        0        0    16014 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/index.html
+-rw-r--r--   0        0        0    23786 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/installation.html
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/objects.inv
+-rw-r--r--   0        0        0    12811 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/references.html
+-rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/search.html
+-rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/searchindex.js
+-rw-r--r--   0        0        0    26667 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/usage.html
+-rw-r--r--   0        0        0    68887 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/.doctrees/API.doctree
+-rw-r--r--   0        0        0    41990 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/.doctrees/butane_PMF.doctree
+-rw-r--r--   0        0        0    51030 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/.doctrees/dialanine_PMF.doctree
+-rw-r--r--   0        0        0    61735 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/.doctrees/environment.pickle
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/.doctrees/examples.doctree
+-rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/.doctrees/index.doctree
+-rw-r--r--   0        0        0    24305 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/.doctrees/installation.doctree
+-rw-r--r--   0        0        0     8759 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/.doctrees/references.doctree
+-rw-r--r--   0        0        0    28287 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/.doctrees/usage.doctree
+-rw-r--r--   0        0        0   187708 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_images/Fig_1.png
+-rw-r--r--   0        0        0   211402 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_images/Fig_11.png
+-rw-r--r--   0        0        0   172324 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_images/Fig_2.png
+-rw-r--r--   0        0        0   193626 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_images/Fig_21.png
+-rw-r--r--   0        0        0   156671 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_images/PMF.png
+-rw-r--r--   0        0        0   116954 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_images/PMF1.png
+-rw-r--r--   0        0        0   459263 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_images/energy_matrix.png
+-rw-r--r--   0        0        0    10181 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_modules/index.html
+-rw-r--r--   0        0        0   125225 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_modules/FastMBAR/fastmbar.html
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_sources/API.rst
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_sources/butane_PMF.rst
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_sources/dialanine_PMF.rst
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_sources/examples.rst
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_sources/index.rst
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_sources/installation.rst
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_sources/references.rst
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_sources/usage.rst
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    15228 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/basic.css
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/check-solid.svg
+-rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/clipboard.min.js
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/copy-button.svg
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/copybutton.css
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/copybutton.js
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/copybutton_funcs.js
+-rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/doctools.js
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/file.png
+-rw-r--r--   0        0        0   288580 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/jquery-3.6.0.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/jquery.js
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/language_data.js
+-rw-r--r--   0        0        0  1201731 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/logo.ai
+-rw-r--r--   0        0        0  1249206 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/logo.eps
+-rw-r--r--   0        0        0   119173 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/logo.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/plus.png
+-rw-r--r--   0        0        0    12757 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/pygments.css
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/sbt-webpack-macros.html
+-rw-r--r--   0        0        0    17088 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/searchtools.js
+-rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/underscore-1.13.1.js
+-rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/underscore.js
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/webpack-macros.html
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/images/logo_binder.svg
+-rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/images/logo_colab.png
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/images/logo_deepnote.svg
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/da/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/da/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/de/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/de/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/el/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/el/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/es/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/es/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/et/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/et/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/id/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/id/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/it/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/it/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/no/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/no/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/te/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/te/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/th/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/th/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0    80813 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/scripts/bootstrap.js
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0        0        0   335757 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/scripts/bootstrap.js.map
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0        0        0   176654 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/styles/bootstrap.css
+-rw-r--r--   0        0        0    63341 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0        0        0    13841 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/styles/theme.css
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+-rw-r--r--   0        0        0   101691 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/css/all.min.css
+-rw-r--r--   0        0        0   181264 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   105112 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    60236 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    24028 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   389948 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   154840 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/source/API.rst
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/source/butane_PMF.rst
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/source/conf.py
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/source/dialanine_PMF.rst
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/source/examples.rst
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/source/index.rst
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/source/installation.rst
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/source/references.rst
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/source/usage.rst
+-rw-r--r--   0        0        0  1201731 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/source/_static/logo.ai
+-rw-r--r--   0        0        0  1249206 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/source/_static/logo.eps
+-rw-r--r--   0        0        0   119173 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/docs/source/_static/logo.png
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/test/test_FastMBAR.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/LICENSE
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/README.rst
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 fastmbar-1.0rc1/PKG-INFO
```

### Comparing `fastmbar-1.0/energy_matrix.pdf` & `fastmbar-1.0rc1/energy_matrix.pdf`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/energy_matrix.png` & `fastmbar-1.0rc1/energy_matrix.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/FastMBAR/fastmbar.py` & `fastmbar-1.0rc1/FastMBAR/fastmbar.py`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/FastMBAR/test_FastMBAR.py` & `fastmbar-1.0rc1/test/test_FastMBAR.py`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/FastMBAR/utils/analyzer.py` & `fastmbar-1.0rc1/FastMBAR/utils/analyzer.py`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/FastMBAR/utils/fastmbartools.py` & `fastmbar-1.0rc1/FastMBAR/utils/fastmbartools.py`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/Makefile` & `fastmbar-1.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/API.html` & `fastmbar-1.0rc1/docs/build/API.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/butane_PMF.html` & `fastmbar-1.0rc1/docs/build/butane_PMF.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/dialanine_PMF.html` & `fastmbar-1.0rc1/docs/build/dialanine_PMF.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/examples.html` & `fastmbar-1.0rc1/docs/build/examples.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/genindex.html` & `fastmbar-1.0rc1/docs/build/genindex.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/index.html` & `fastmbar-1.0rc1/docs/build/index.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/references.html` & `fastmbar-1.0rc1/docs/build/references.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/search.html` & `fastmbar-1.0rc1/docs/build/search.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/searchindex.js` & `fastmbar-1.0rc1/docs/build/searchindex.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -7,28 +7,28 @@
         "energi": [0, 1, 2, 4, 6, 7],
         "union": 0,
         "ndarrai": 0,
         "tensor": 0,
         "num_conf": [0, 1, 2, 7],
         "cuda": [0, 1, 2, 5, 7],
         "bool": 0,
-        "fals": [0, 1, 2, 5, 7],
+        "fals": [0, 1, 2, 7],
         "cuda_batch_mod": 0,
         "option": 0,
         "none": 0,
-        "bootstrap": [0, 7],
+        "bootstrap": [0, 5, 7],
         "bootstrap_block_s": 0,
         "int": [0, 7],
         "3": [0, 4],
         "bootstrap_num_rep": 0,
-        "100": [0, 1, 2, 5],
+        "100": [0, 1, 2],
         "verbos": [0, 1, 2, 7],
         "method": [0, 1, 2],
         "str": 0,
-        "newton": [0, 5],
+        "newton": 0,
         "sourc": [0, 1, 2],
         "The": [0, 1, 2, 3, 5, 7],
         "initi": [0, 1, 2, 7],
         "an": [0, 3, 7],
         "matrix": [0, 1, 2, 7],
         "arrai": [0, 1, 2, 7],
         "num": 0,
@@ -42,22 +42,24 @@
         "rel": [0, 1, 2, 4, 7],
         "free": [0, 1, 2, 4, 6, 7],
         "state": [0, 1, 2, 4, 6, 7],
         "us": [0, 3, 5, 6],
         "calcul": [0, 1, 2, 3, 4, 5, 6, 7],
         "calculate_free_energies_for_perturbed_st": 0,
         "can": [0, 1, 2, 3, 4, 5, 7],
+        "calcualt": [],
         "perturb": [0, 7],
         "__init__": 0,
+        "initizl": [],
         "paramet": 0,
         "2d": [0, 3],
         "It": [0, 3, 4, 7],
         "ha": [0, 1, 2, 5, 7],
         "size": [0, 1, 2, 4],
-        "m": [0, 1, 2, 7],
+        "m": [0, 1, 2, 5, 7],
         "x": [0, 1, 2, 7],
         "n": [0, 1, 2, 7],
         "where": [0, 1, 2, 7],
         "number": [0, 1, 2, 4, 7],
         "total": [0, 7],
         "entri": 0,
         "i": [0, 1, 2, 5, 7],
@@ -75,116 +77,112 @@
         "occpi": 0,
         "continu": 0,
         "chunk": 0,
         "collumn": 0,
         "k": [0, 1, 2, 7],
         "occupi": 0,
         "left": [0, 7],
-        "l": [0, 1, 2, 5, 6, 7],
+        "l": [0, 1, 2, 6, 7],
         "doe": [0, 1, 2],
         "1d": 0,
         "should": [0, 1, 2, 3, 5, 7],
         "have": [0, 1, 2, 3, 5, 7],
         "np": [0, 1, 2, 7],
         "sum": 0,
         "equal": 0,
-        "all": [0, 1, 2, 3, 7],
+        "all": [0, 1, 2, 3, 5, 7],
         "strictli": 0,
         "greater": 0,
         "than": 0,
         "0": [0, 1, 2, 5],
         "default": [0, 1, 2],
         "set": [0, 1, 2, 7],
         "true": [0, 1, 2, 5, 7],
         "run": [0, 3, 5, 7],
         "graphic": 0,
         "process": [0, 3],
         "unit": [0, 1, 2, 7],
         "gpu": [0, 4, 5, 7],
-        "batch": 0,
-        "mode": 0,
+        "batch": [0, 5],
+        "mode": [0, 5],
         "turn": 0,
         "when": [0, 1, 2, 4],
         "too": [0, 3, 7],
         "larg": [0, 4, 6],
         "memori": [0, 4],
         "split": [0, 1, 2],
         "multipl": [0, 1, 2, 4, 6],
         "which": [0, 1, 2, 5, 7],
-        "ar": [0, 1, 2, 7],
+        "ar": [0, 1, 2, 5, 7],
         "sequenti": [0, 1, 2],
         "automat": 0,
         "base": [0, 1, 2, 6, 7],
-        "avaibl": [0, 5],
+        "avaibl": 0,
         "devic": 0,
         "estim": [0, 3, 6, 7],
         "block": 0,
         "repreat": 0,
-        "detail": [0, 5],
+        "detail": 0,
         "inform": [0, 1, 2, 5],
         "print": [0, 1, 2, 5, 7],
         "s": 0,
-        "properti": [0, 1, 2],
-        "f": [0, 1, 2, 7],
-        "under": 0,
-        "constraint": [0, 1, 2],
-        "sum_": [0, 7],
+        "calculate_free_energies_of_perturbed_st": [0, 1, 2, 7],
+        "energy_perturb": 0,
+        "2": [0, 3, 4],
+        "d": [0, 6],
+        "float": 0,
+        "each": [0, 1, 2, 7],
+        "row": [0, 7],
+        "repres": [0, 1, 2, 7],
+        "valu": 0,
+        "th": [0, 1, 2, 7],
+        "return": [0, 5],
+        "f_mean": [],
         "1": [0, 3, 4],
-        "n_k": [0, 7],
-        "f_k": [0, 7],
+        "mean": [4, 5, 7],
         "f_std": [0, 1, 7],
         "standard": [0, 7],
         "deviat": [0, 7],
+        "f": [0, 1, 2, 7],
+        "esim": [],
+        "off": [],
+        "properti": [0, 1, 2],
+        "f_bootstrap": [],
+        "constrain": [1, 2],
+        "zero": [1, 2],
+        "under": 0,
+        "contraint": [],
         "f_cov": 0,
         "covari": 0,
         "deltaf": 0,
         "differ": [0, 1, 2, 6, 7],
         "between": [0, 1, 2],
-        "mathrm": 0,
         "e": [0, 1, 2, 7],
         "deltaf_std": 0,
         "log_prob_mix": 0,
         "log": 0,
         "probabl": [0, 7],
         "densiti": 0,
         "mixtur": 0,
         "distribut": [0, 5, 7],
-        "calculate_free_energies_of_perturbed_st": [0, 1, 2, 7],
-        "energy_perturb": 0,
-        "2": [0, 3, 4],
-        "d": [0, 6],
-        "float": 0,
-        "each": [0, 1, 2, 7],
-        "row": [0, 7],
-        "repres": [0, 1, 2, 7],
-        "valu": 0,
-        "th": [0, 1, 2, 7],
-        "return": [0, 5],
-        "result": [0, 1, 2],
-        "dictionari": 0,
-        "contain": [0, 1, 2],
-        "follow": [0, 1, 2, 3, 5, 6, 7],
-        "kei": 0,
-        "type": [0, 3],
-        "dict": 0,
         "thi": [1, 2, 5],
         "includ": [1, 2, 7],
         "step": [1, 2, 3, 5, 7],
-        "descript": [1, 2, 7],
+        "discript": [],
         "its": 1,
         "four": [1, 2],
         "carbon": 1,
         "atom": [1, 2],
         "exhaust": [1, 2],
-        "relev": [1, 2],
+        "relav": [],
         "configur": [1, 2],
         "center": [1, 2],
         "around": [1, 2],
         "here": [1, 2, 3, 7],
-        "reweigh": [1, 2],
+        "reweight": 7,
         "To": [1, 2, 3, 5, 7],
         "your": [1, 2, 3, 5, 6],
         "local": [1, 2],
         "you": [1, 2, 3, 4, 5, 7],
         "clone": [1, 2],
         "download": [1, 2, 5],
         "git": [1, 2],
@@ -193,29 +191,30 @@
         "after": [1, 2, 5, 7],
         "chang": [1, 2],
         "current": [1, 2, 5],
         "work": [1, 2],
         "directori": [1, 2],
         "befor": [1, 2, 5],
         "start": [1, 2, 5],
+        "follow": [0, 1, 2, 3, 5, 6, 7],
         "script": [1, 2],
         "insid": [1, 2],
         "python": [1, 2, 4, 7],
         "interpret": [1, 2],
         "import": [1, 2, 5, 7],
         "requir": [1, 2, 4, 7],
         "packag": [1, 2, 3, 5, 7],
         "os": [1, 2],
         "math": [1, 2],
         "sy": [1, 2],
         "numpi": [1, 2, 7],
         "matplotlib": [1, 2],
         "pyplot": [1, 2],
         "plt": [1, 2],
-        "app": [1, 2, 5],
+        "app": [1, 2],
         "omm_app": [1, 2],
         "omm": [1, 2],
         "tqdm": [1, 2, 3],
         "mdtraj": [1, 2, 3],
         "becaus": [1, 2, 5],
         "we": [1, 2, 3, 7],
         "our": [1, 2],
@@ -233,31 +232,34 @@
         "so": [1, 2, 3],
         "bias": [1, 2],
         "potenti": [1, 2, 4, 7],
         "read": [1, 2, 5, 7],
         "psf": [1, 2],
         "pdb": [1, 2],
         "file": [1, 2],
-        "topolog": [1, 2],
+        "contain": [0, 1, 2],
+        "topolgi": [],
         "charmm": [1, 2, 3],
         "gener": [1, 2, 7],
         "In": [1, 2, 5, 7],
         "studi": [1, 2, 3],
         "usual": [1, 2],
-        "alreadi": [1, 2],
+        "alreai": [],
+        "topolog": [1, 2],
         "variou": [1, 2],
         "softwar": [1, 2],
         "gromac": [1, 2, 3],
         "amber": [1, 2, 3],
         "among": [1, 2],
         "other": [1, 2, 3],
         "just": [1, 2, 3, 4],
         "note": [1, 2, 7],
         "sever": [1, 2, 3],
         "parser": [1, 2],
+        "foramt": [],
         "charmmpsffil": [1, 2],
         "data": [1, 2, 6],
         "pdbfile": [1, 2],
         "forc": [1, 2, 4, 7],
         "field": [1, 2],
         "param": 1,
         "charmmparameterset": [1, 2],
@@ -280,14 +282,15 @@
         "code": [1, 2],
         "do": [1, 2, 5, 7],
         "tell": [1, 2],
         "formula": [1, 2],
         "degre": [1, 2],
         "freedom": [1, 2],
         "want": [1, 2, 3, 4, 5, 7],
+        "creai": [],
         "createsystem": [1, 2],
         "nonbondedmethod": [1, 2],
         "nocutoff": [1, 2],
         "bias_tors": 1,
         "5": [1, 2],
         "dtheta": [1, 2],
         "min": [1, 2],
@@ -320,15 +323,15 @@
         "output": [1, 2, 5],
         "w": [1, 2],
         "file_handl": [1, 2],
         "write": [1, 2],
         "xmlserial": [1, 2],
         "serial": [1, 2],
         "window": [1, 2],
-        "restrain": [1, 2],
+        "restraint": [],
         "thei": [1, 2, 7],
         "parallel": [1, 2],
         "cluster": [1, 2],
         "node": [1, 2],
         "r": [1, 2, 6],
         "deseri": [1, 2],
         "context": [1, 2],
@@ -338,21 +341,22 @@
         "abov": [1, 2, 5, 7],
         "specifi": [1, 2],
         "kind": [1, 2, 3],
         "langevin": [1, 2],
         "dynam": [1, 2, 3, 6],
         "nvt": [1, 2],
         "ensembl": [1, 2],
-        "langevinmiddleintegr": [1, 2],
+        "langevinintegr": [],
         "hardwar": [1, 2],
         "choos": [1, 2],
         "cpu": [1, 2, 4, 5],
         "quit": [1, 7],
         "small": 1,
         "getplatformbynam": [1, 2],
+        "intergr": [],
         "298": [1, 2],
         "15": [1, 2],
         "kelvin": [1, 2],
         "temperatur": [1, 2, 4, 7],
         "friccoef": [1, 2],
         "10": [1, 2],
         "picosecond": [1, 2],
@@ -382,15 +386,15 @@
         "index": [1, 2],
         "out": [1, 2],
         "setposit": [1, 2],
         "posit": [1, 2],
         "getstat": [1, 2],
         "getenergi": [1, 2],
         "getpotentialenergi": [1, 2],
-        "50": [1, 2, 5],
+        "50": [1, 2],
         "localenergyminim": [1, 2],
         "equilibrium": [1, 2, 6],
         "5000": [1, 2],
         "product": [1, 2],
         "trajectori": [1, 2, 3],
         "dcd": [1, 2],
         "traj": [1, 2],
@@ -411,14 +415,16 @@
         "compute_dihedr": [1, 2],
         "dihedral_": 1,
         "fmt": 1,
         "5f": 1,
         "two": [1, 2, 7],
         "firstli": [1, 2],
         "secondli": [1, 2],
+        "umbreal": [],
+        "umbrealla": [],
         "view": [1, 2],
         "thermodynam": [1, 2, 4, 7],
         "As": [1, 2, 7],
         "shown": [1, 2, 7],
         "usag": [1, 2, 4],
         "a_": [1, 2, 7],
         "fig": [1, 2],
@@ -432,50 +438,51 @@
         "coordin": [1, 2],
         "compar": [1, 2],
         "special": [1, 2],
         "common": [1, 2],
         "compon": [1, 2],
         "remov": [1, 2],
         "affect": [1, 2],
-        "omit": [1, 2],
+        "ommit": [],
+        "enegi": 7,
         "loadtxt": 1,
         "append": [1, 2],
         "len": 1,
         "concaten": 1,
         "A": [1, 2, 7],
-        "zero": [1, 2],
         "kbt": [1, 2],
         "boltzmann_constant_kb": [1, 2],
         "avogadro_constant_na": [1, 2],
         "value_in_unit": [1, 2],
         "kilojoule_per_mol": [1, 2],
         "current_theta0": 1,
         "minimum": [1, 2],
         "now": [1, 2],
         "readi": [1, 2],
         "yield": [1, 2],
         "know": [1, 2],
         "enabl": [1, 2],
-        "procedur": [1, 2],
+        "procesur": [],
         "b_": [1, 2, 7],
         "theta_": 1,
         "theta_l": 1,
-        "constrain": [1, 2],
+        "constraint": [0, 1, 2],
         "r_l": 1,
         "enforc": [1, 2],
         "infin": [1, 2],
         "otherwis": [1, 2],
-        "b": [1, 2, 5, 7],
-        "25": [1, 2, 5],
+        "b": [1, 2, 7],
+        "25": [1, 2],
         "theta_pmf": 1,
         "width": [1, 2],
         "theta_cent": 1,
         "theta_low": 1,
         "theta_high": 1,
         "inf": [1, 2],
+        "result": [0, 1, 2, 5],
         "pmf_uncertainti": 1,
         "plot": [1, 2],
         "figur": [1, 2, 7],
         "clf": [1, 2],
         "errorbar": 1,
         "180": [1, 2],
         "yerr": 1,
@@ -485,32 +492,33 @@
         "capsiz": 1,
         "capthick": 1,
         "markers": 1,
         "xlim": 1,
         "xlabel": [1, 2],
         "ylabel": [1, 2],
         "savefig": [1, 2],
-        "pmf_fastmbar": [1, 2],
+        "pmf_fast_mbar": [],
         "pdf": [1, 2],
         "like": [1, 2],
         "dimension": [2, 4, 7],
         "charmm_toppar": 2,
         "top_all36_prot": 2,
         "par_all36_prot": 2,
         "psi": 2,
-        "8": [2, 5],
+        "8": 2,
         "14": 2,
         "phi": 2,
-        "16": [2, 5],
+        "16": 2,
         "torsion": 2,
         "bias_torsion_psi": 2,
         "k_psi": 2,
         "tmp": 2,
         "bias_torsion_phi": 2,
         "k_phi": 2,
+        "dianalin": [],
         "nvp": 2,
         "idx": 2,
         "psi_index": 2,
         "phi_index": 2,
         "traj_psi_": 2,
         "_phi_": 2,
         "alanin": 2,
@@ -572,25 +580,25 @@
         "essenti": 3,
         "provid": [3, 5, 7],
         "progress": 3,
         "bar": 3,
         "wall": 3,
         "time": [3, 7],
         "umbrella": [3, 4, 7],
+        "type": [0, 3],
         "pip": [3, 4],
         "pmf": [3, 4, 7],
         "dihedr": 3,
         "butan": 3,
         "dialanin": 3,
         "solver": [4, 6],
         "scale": [4, 6],
         "uwham": 4,
         "both": [4, 7],
         "alchem": [4, 6, 7],
-        "mean": [4, 5, 7],
         "hamiltonian": [4, 7],
         "replica": [4, 7],
         "exchang": [4, 7],
         "extram": 4,
         "fast": [4, 6],
         "wham": 4,
         "moreov": 4,
@@ -604,30 +612,30 @@
         "instal": 4,
         "new": 4,
         "test": 4,
         "api": 4,
         "exampl": [4, 7],
         "extra": 4,
         "packg": 4,
-        "refer": 4,
+        "refer": [4, 5],
         "high": 5,
         "level": 5,
         "program": 5,
         "languag": 5,
         "highli": 5,
         "recommend": 5,
         "manag": 5,
         "http": 5,
         "www": 5,
         "com": 5,
         "without": 5,
         "support": 5,
         "still": 5,
         "pytorch": 5,
-        "get": [],
+        "get": 5,
         "specif": 5,
         "could": 5,
         "depend": 5,
         "oper": 5,
         "system": [5, 7],
         "version": 5,
         "check": 5,
@@ -647,23 +655,23 @@
         "is_avail": 5,
         "correctli": 5,
         "pleas": [5, 6],
         "go": 5,
         "back": 5,
         "reinstal": 5,
         "more": 5,
-        "detal": [],
+        "detal": 5,
         "successfulli": 5,
         "been": 5,
-        "test_instal": [],
+        "test_instal": 5,
         "similar": 5,
-        "rmsd": [],
-        "05": [],
+        "rmsd": 5,
+        "05": 5,
         "pass": 5,
-        "With": 7,
+        "With": [5, 7],
         "consid": 6,
         "cite": 6,
         "project": 6,
         "xinqiang": 6,
         "ding": 6,
         "jonah": 6,
         "z": 6,
@@ -696,14 +704,15 @@
         "analysi": 6,
         "phy": 6,
         "h": 6,
         "1976": 6,
         "effici": 6,
         "mont": [6, 7],
         "carlo": [6, 7],
+        "descript": [1, 2, 7],
         "help": 7,
         "better": 7,
         "undertand": 7,
         "might": 7,
         "thu": 7,
         "abstract": 7,
         "firt": 7,
@@ -723,98 +732,71 @@
         "invers": 7,
         "beta": 7,
         "k_bt": 7,
         "origin": 7,
         "e_k": 7,
         "defin": 7,
         "quantiti": 7,
+        "f_k": [0, 7],
         "ln": 7,
         "dx": 7,
         "also": 7,
         "convert": 7,
         "mutipli": 7,
         "There": 7,
         "mani": 7,
         "wai": 7,
         "separ": 7,
         "either": 7,
         "dynamci": 7,
-        "reweight": 7,
+        "n_k": [0, 7],
         "_k": 7,
         "second": 7,
         "prime": 7,
         "_l": 7,
         "situat": 7,
         "describ": 7,
         "input": 7,
         "vector": 7,
-        "v": [5, 7],
+        "v": 7,
         "conduct": 7,
         "blue": 7,
         "bracket": 7,
         "column": 7,
+        "sum_": [0, 7],
         "evalu": 7,
         "These": 7,
         "constitu": 7,
         "construct": 7,
         "n_1": 7,
         "n_2": 7,
         "n_m": 7,
         "calcuat": 7,
         "store": 7,
         "respect": 7,
         "seper": 7,
         "previou": 7,
         "red": 7,
         "term": 7,
-        "enegi": 7,
         "f_perturb": 7,
         "f_perturbed_std": 7,
-        "_": [],
-        "pytest": 5,
-        "pyarg": 5,
-        "session": 5,
-        "linux": 5,
-        "11": 5,
-        "4": 5,
-        "7": 5,
-        "pluggi": 5,
-        "home": 5,
-        "xqding": 5,
-        "miniconda3": 5,
-        "env": 5,
-        "bin": 5,
-        "python3": 5,
-        "cachedir": 5,
-        "pytest_cach": 5,
-        "rootdir": 5,
-        "collect": 5,
-        "12": 5,
-        "item": 5,
-        "lib": [],
-        "site": [],
-        "test_fastmbar": 5,
-        "py": 5,
-        "test_fastmbar_cpu": 5,
-        "bfg": 5,
-        "33": 5,
-        "test_fastmbar_gpu": 5,
-        "41": 5,
-        "58": 5,
-        "66": 5,
-        "75": 5,
-        "83": 5,
-        "91": 5,
-        "111": 5,
-        "64": 5,
-        "01": 5,
-        "51": 5,
-        "skip": 5,
-        "29": 5,
-        "67": 5
+        "pmf_fastmbar": [1, 2],
+        "relev": [1, 2],
+        "reweigh": [1, 2],
+        "alreadi": [1, 2],
+        "restrain": [1, 2],
+        "langevinmiddleintegr": [1, 2],
+        "omit": [1, 2],
+        "procedur": [1, 2],
+        "mathrm": 0,
+        "dictionari": 0,
+        "kei": 0,
+        "l1": [],
+        "l2": [],
+        "dict": 0
     },
     "objects": {
         "FastMBAR": [
             [0, 0, 1, "", "FastMBAR"]
         ],
         "FastMBAR.FastMBAR": [
             [0, 1, 1, "", "DeltaF"],
```

### Comparing `fastmbar-1.0/docs/build/usage.html` & `fastmbar-1.0rc1/docs/build/usage.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/.doctrees/API.doctree` & `fastmbar-1.0rc1/docs/build/.doctrees/API.doctree`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/.doctrees/butane_PMF.doctree` & `fastmbar-1.0rc1/docs/build/.doctrees/butane_PMF.doctree`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/.doctrees/dialanine_PMF.doctree` & `fastmbar-1.0rc1/docs/build/.doctrees/dialanine_PMF.doctree`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/.doctrees/environment.pickle` & `fastmbar-1.0rc1/docs/build/.doctrees/environment.pickle`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 9535 f100 0000 0000 008c 1273 7068  ...5.........sph
+00000000: 8005 951c f100 0000 0000 008c 1273 7068  .............sph
 00000010: 696e 782e 656e 7669 726f 6e6d 656e 7494  inx.environment.
 00000020: 8c10 4275 696c 6445 6e76 6972 6f6e 6d65  ..BuildEnvironme
 00000030: 6e74 9493 9429 8194 7d94 288c 0361 7070  nt...)..}.(..app
 00000040: 944e 8c0a 646f 6374 7265 6564 6972 948c  .N..doctreedir..
 00000050: 642f 5573 6572 732f 6469 6e67 7871 2f4c  d/Users/dingxq/L
 00000060: 6962 7261 7279 2f43 6c6f 7564 5374 6f72  ibrary/CloudStor
 00000070: 6167 652f 426f 782d 426f 782f 5265 7365  age/Box-Box/Rese
@@ -777,20 +777,20 @@
 00003080: 7573 944b 018c 1363 6f6e 6669 675f 7374  us.K...config_st
 00003090: 6174 7573 5f65 7874 7261 9468 6c8c 0665  atus_extra.hl..e
 000030a0: 7665 6e74 7394 4e8c 0770 726f 6a65 6374  vents.N..project
 000030b0: 948c 0e73 7068 696e 782e 7072 6f6a 6563  ...sphinx.projec
 000030c0: 7494 8c07 5072 6f6a 6563 7494 9394 2981  t...Project...).
 000030d0: 947d 9428 8c06 7372 6364 6972 9468 0968  .}.(..srcdir.h.h
 000030e0: 5a68 5e8c 0864 6f63 6e61 6d65 7394 8f94  Zh^..docnames...
-000030f0: 288c 0c69 6e73 7461 6c6c 6174 696f 6e94  (..installation.
-00003100: 8c0d 6469 616c 616e 696e 655f 504d 4694  ..dialanine_PMF.
-00003110: 8c05 7573 6167 6594 8c03 4150 4994 8c08  ..usage...API...
-00003120: 6578 616d 706c 6573 948c 0a62 7574 616e  examples...butan
-00003130: 655f 504d 4694 8c0a 7265 6665 7265 6e63  e_PMF...referenc
-00003140: 6573 948c 0569 6e64 6578 9490 7562 8c07  es...index..ub..
+000030f0: 288c 0865 7861 6d70 6c65 7394 8c05 696e  (..examples...in
+00003100: 6465 7894 8c03 4150 4994 8c0a 7265 6665  dex...API...refe
+00003110: 7265 6e63 6573 948c 0d64 6961 6c61 6e69  rences...dialani
+00003120: 6e65 5f50 4d46 948c 0c69 6e73 7461 6c6c  ne_PMF...install
+00003130: 6174 696f 6e94 8c05 7573 6167 6594 8c0a  ation...usage...
+00003140: 6275 7461 6e65 5f50 4d46 9490 7562 8c07  butane_PMF..ub..
 00003150: 7665 7273 696f 6e94 7d94 288c 1073 7068  version.}.(..sph
 00003160: 696e 782e 646f 6d61 696e 732e 6394 4b02  inx.domains.c.K.
 00003170: 8c18 7370 6869 6e78 2e64 6f6d 6169 6e73  ..sphinx.domains
 00003180: 2e63 6861 6e67 6573 6574 944b 018c 1773  .changeset.K...s
 00003190: 7068 696e 782e 646f 6d61 696e 732e 6369  phinx.domains.ci
 000031a0: 7461 7469 6f6e 944b 018c 1273 7068 696e  tation.K...sphin
 000031b0: 782e 646f 6d61 696e 732e 6370 7094 4b06  x.domains.cpp.K.
@@ -833,3028 +833,3027 @@
 00003400: 6e61 626c 6564 9488 8c13 736d 6172 7471  nabled....smartq
 00003410: 756f 7465 735f 6c6f 6361 6c65 7394 5d94  uotes_locales.].
 00003420: 8c03 656e 7694 6803 8c1d 7472 696d 5f66  ..env.h...trim_f
 00003430: 6f6f 746e 6f74 655f 7265 6665 7265 6e63  ootnote_referenc
 00003440: 655f 7370 6163 6594 898c 0d6c 616e 6775  e_space....langu
 00003450: 6167 655f 636f 6465 9468 1b8c 0c73 6d61  age_code.h...sma
 00003460: 7274 5f71 756f 7465 7394 8875 8c08 616c  rt_quotes..u..al
-00003470: 6c5f 646f 6373 947d 9428 8c03 4150 4994  l_docs.}.(..API.
-00003480: 4741 d92b 09a4 2201 b88c 0a62 7574 616e  GA.+.."....butan
-00003490: 655f 504d 4694 4741 d92b 09a4 23bd 418c  e_PMF.GA.+..#.A.
-000034a0: 0d64 6961 6c61 6e69 6e65 5f50 4d46 9447  .dialanine_PMF.G
-000034b0: 41d9 2b09 a425 9026 8c08 6578 616d 706c  A.+..%.&..exampl
-000034c0: 6573 9447 41d9 2b09 a426 34e7 8c05 696e  es.GA.+..&4...in
-000034d0: 6465 7894 4741 d92b 09a4 2695 9a8c 0a72  dex.GA.+..&....r
-000034e0: 6566 6572 656e 6365 7394 4741 d92b 09a4  eferences.GA.+..
-000034f0: 27d5 678c 0575 7361 6765 9447 41d9 2b09  '.g..usage.GA.+.
-00003500: a429 1bf0 6ae7 0200 0047 41d9 2b11 629c  .)..j....GA.+.b.
-00003510: 0abb 758c 0c64 6570 656e 6465 6e63 6965  ..u..dependencie
-00003520: 7394 685b 8c0b 6465 6661 756c 7464 6963  s.h[..defaultdic
-00003530: 7494 9394 8c08 6275 696c 7469 6e73 948c  t.....builtins..
-00003540: 0373 6574 9493 9485 9452 9428 6a1c 0300  .set.....R.(j...
-00003550: 008f 9428 8c1a 2e2e 2f2e 2e2f 4661 7374  ...(..../../Fast
-00003560: 4d42 4152 2f66 6173 746d 6261 722e 7079  MBAR/fastmbar.py
-00003570: 9490 6a1d 0300 008f 9428 8c24 2e2e 2f2e  ..j......(.$../.
-00003580: 2e2f 6578 616d 706c 6573 2f62 7574 616e  ./examples/butan
-00003590: 652f 6461 7461 2f46 6967 5f31 2e70 6e67  e/data/Fig_1.png
-000035a0: 948c 1a2e 2e2f 2e2e 2f46 6173 744d 4241  ...../../FastMBA
-000035b0: 522f 6661 7374 6d62 6172 2e70 7994 8c22  R/fastmbar.py.."
-000035c0: 2e2e 2f2e 2e2f 6578 616d 706c 6573 2f62  ../../examples/b
-000035d0: 7574 616e 652f 6461 7461 2f50 4d46 2e70  utane/data/PMF.p
-000035e0: 6e67 948c 242e 2e2f 2e2e 2f65 7861 6d70  ng..$../../examp
-000035f0: 6c65 732f 6275 7461 6e65 2f64 6174 612f  les/butane/data/
-00003600: 4669 675f 322e 706e 6794 906a 1e03 0000  Fig_2.png..j....
-00003610: 8f94 288c 1a2e 2e2f 2e2e 2f46 6173 744d  ..(..../../FastM
-00003620: 4241 522f 6661 7374 6d62 6172 2e70 7994  BAR/fastmbar.py.
-00003630: 8c25 2e2e 2f2e 2e2f 6578 616d 706c 6573  .%../../examples
-00003640: 2f64 6961 6c61 6e69 6e65 2f64 6174 612f  /dialanine/data/
-00003650: 504d 462e 706e 6794 8c27 2e2e 2f2e 2e2f  PMF.png..'../../
-00003660: 6578 616d 706c 6573 2f64 6961 6c61 6e69  examples/dialani
-00003670: 6e65 2f64 6174 612f 4669 675f 322e 706e  ne/data/Fig_2.pn
-00003680: 6794 8c27 2e2e 2f2e 2e2f 6578 616d 706c  g..'../../exampl
-00003690: 6573 2f64 6961 6c61 6e69 6e65 2f64 6174  es/dialanine/dat
-000036a0: 612f 4669 675f 312e 706e 6794 906a 1f03  a/Fig_1.png..j..
-000036b0: 0000 8f94 288c 1a2e 2e2f 2e2e 2f46 6173  ....(..../../Fas
-000036c0: 744d 4241 522f 6661 7374 6d62 6172 2e70  tMBAR/fastmbar.p
-000036d0: 7994 906a 2003 0000 8f94 288c 1a2e 2e2f  y..j .....(..../
-000036e0: 2e2e 2f46 6173 744d 4241 522f 6661 7374  ../FastMBAR/fast
-000036f0: 6d62 6172 2e70 7994 906a 2103 0000 8f94  mbar.py..j!.....
-00003700: 288c 1a2e 2e2f 2e2e 2f46 6173 744d 4241  (..../../FastMBA
-00003710: 522f 6661 7374 6d62 6172 2e70 7994 906a  R/fastmbar.py..j
-00003720: 2203 0000 8f94 288c 1a2e 2e2f 2e2e 2f46  ".....(..../../F
-00003730: 6173 744d 4241 522f 6661 7374 6d62 6172  astMBAR/fastmbar
-00003740: 2e70 7994 8c17 2e2e 2f2e 2e2f 656e 6572  .py...../../ener
-00003750: 6779 5f6d 6174 7269 782e 706e 6794 9075  gy_matrix.png..u
-00003760: 8c08 696e 636c 7564 6564 946a 2503 0000  ..included.j%...
-00003770: 6a28 0300 0085 9452 948c 0d72 6572 6561  j(.....R...rerea
-00003780: 645f 616c 7761 7973 948f 948c 086d 6574  d_always.....met
-00003790: 6164 6174 6194 6a25 0300 006a 2603 0000  adata.j%...j&...
-000037a0: 8c04 6469 6374 9493 9485 9452 948c 0674  ..dict.....R...t
-000037b0: 6974 6c65 7394 7d94 286a 1c03 0000 8c0e  itles.}.(j......
-000037c0: 646f 6375 7469 6c73 2e6e 6f64 6573 948c  docutils.nodes..
-000037d0: 0574 6974 6c65 9493 9429 8194 7d94 288c  .title...)..}.(.
-000037e0: 0972 6177 736f 7572 6365 9468 6c8c 0863  .rawsource.hl..c
-000037f0: 6869 6c64 7265 6e94 5d94 6a4c 0300 008c  hildren.].jL....
-00003800: 0454 6578 7494 9394 8c0c 4661 7374 4d42  .Text.....FastMB
-00003810: 4152 2041 5049 9485 9481 947d 948c 0670  AR API.....}...p
-00003820: 6172 656e 7494 6a4f 0300 0073 6261 8c0a  arent.jO...sba..
-00003830: 6174 7472 6962 7574 6573 947d 9428 8c03  attributes.}.(..
-00003840: 6964 7394 5d94 8c07 636c 6173 7365 7394  ids.]...classes.
-00003850: 5d94 8c05 6e61 6d65 7394 5d94 8c08 6475  ]...names.]...du
-00003860: 706e 616d 6573 945d 948c 0862 6163 6b72  pnames.]...backr
-00003870: 6566 7394 5d94 758c 0774 6167 6e61 6d65  efs.].u..tagname
-00003880: 948c 0574 6974 6c65 9475 626a 1d03 0000  ...title.ubj....
-00003890: 6a4e 0300 0029 8194 7d94 286a 5103 0000  jN...)..}.(jQ...
-000038a0: 686c 6a52 0300 005d 946a 5503 0000 8c34  hljR...].jU....4
-000038b0: 4578 616d 706c 6520 312e 2043 6f6d 7075  Example 1. Compu
-000038c0: 7465 2074 6865 2050 4d46 206f 6620 6120  te the PMF of a 
-000038d0: 6469 6865 6472 616c 2066 6f72 2062 7574  dihedral for but
-000038e0: 616e 652e 9485 9481 947d 946a 5a03 0000  ane......}.jZ...
-000038f0: 6a69 0300 0073 6261 6a5b 0300 007d 9428  ji...sbaj[...}.(
-00003900: 6a5d 0300 005d 946a 5f03 0000 5d94 6a61  j]...].j_...].ja
-00003910: 0300 005d 946a 6303 0000 5d94 6a65 0300  ...].jc...].je..
-00003920: 005d 9475 6a67 0300 006a 6803 0000 7562  .].ujg...jh...ub
-00003930: 6a1e 0300 006a 4e03 0000 2981 947d 9428  j....jN...)..}.(
-00003940: 6a51 0300 0068 6c6a 5203 0000 5d94 6a55  jQ...hljR...].jU
-00003950: 0300 008c 3745 7861 6d70 6c65 2032 2e20  ....7Example 2. 
-00003960: 436f 6d70 7574 6520 6120 3244 2d50 4d46  Compute a 2D-PMF
-00003970: 206f 6620 6469 6865 6472 616c 7320 666f   of dihedrals fo
-00003980: 7220 6469 616c 616e 696e 652e 9485 9481  r dialanine.....
-00003990: 947d 946a 5a03 0000 6a76 0300 0073 6261  .}.jZ...jv...sba
-000039a0: 6a5b 0300 007d 9428 6a5d 0300 005d 946a  j[...}.(j]...].j
-000039b0: 5f03 0000 5d94 6a61 0300 005d 946a 6303  _...].ja...].jc.
-000039c0: 0000 5d94 6a65 0300 005d 9475 6a67 0300  ..].je...].ujg..
-000039d0: 006a 6803 0000 7562 6a1f 0300 006a 4e03  .jh...ubj....jN.
-000039e0: 0000 2981 947d 9428 6a51 0300 0068 6c6a  ..)..}.(jQ...hlj
-000039f0: 5203 0000 5d94 6a55 0300 008c 0845 7861  R...].jU.....Exa
-00003a00: 6d70 6c65 7394 8594 8194 7d94 6a5a 0300  mples.....}.jZ..
-00003a10: 006a 8303 0000 7362 616a 5b03 0000 7d94  .j....sbaj[...}.
-00003a20: 286a 5d03 0000 5d94 6a5f 0300 005d 946a  (j]...].j_...].j
-00003a30: 6103 0000 5d94 6a63 0300 005d 946a 6503  a...].jc...].je.
-00003a40: 0000 5d94 756a 6703 0000 6a68 0300 0075  ..].ujg...jh...u
-00003a50: 626a 2003 0000 6a4e 0300 0029 8194 7d94  bj ...jN...)..}.
-00003a60: 286a 5103 0000 686c 6a52 0300 005d 946a  (jQ...hljR...].j
-00003a70: 5503 0000 8c14 5765 6c63 6f6d 6520 746f  U.....Welcome to
-00003a80: 2046 6173 744d 4241 5221 9485 9481 947d   FastMBAR!.....}
-00003a90: 946a 5a03 0000 6a90 0300 0073 6261 6a5b  .jZ...j....sbaj[
-00003aa0: 0300 007d 9428 6a5d 0300 005d 946a 5f03  ...}.(j]...].j_.
-00003ab0: 0000 5d94 6a61 0300 005d 946a 6303 0000  ..].ja...].jc...
-00003ac0: 5d94 6a65 0300 005d 9475 6a67 0300 006a  ].je...].ujg...j
-00003ad0: 6803 0000 7562 6a21 0300 006a 4e03 0000  h...ubj!...jN...
-00003ae0: 2981 947d 9428 6a51 0300 0068 6c6a 5203  )..}.(jQ...hljR.
-00003af0: 0000 5d94 6a55 0300 008c 0a52 6566 6572  ..].jU.....Refer
-00003b00: 656e 6365 7394 8594 8194 7d94 6a5a 0300  ences.....}.jZ..
-00003b10: 006a 9d03 0000 7362 616a 5b03 0000 7d94  .j....sbaj[...}.
-00003b20: 286a 5d03 0000 5d94 6a5f 0300 005d 946a  (j]...].j_...].j
-00003b30: 6103 0000 5d94 6a63 0300 005d 946a 6503  a...].jc...].je.
-00003b40: 0000 5d94 756a 6703 0000 6a68 0300 0075  ..].ujg...jh...u
-00003b50: 626a 2203 0000 6a4e 0300 0029 8194 7d94  bj"...jN...)..}.
-00003b60: 286a 5103 0000 686c 6a52 0300 005d 946a  (jQ...hljR...].j
-00003b70: 5503 0000 8c05 5573 6167 6594 8594 8194  U.....Usage.....
-00003b80: 7d94 6a5a 0300 006a aa03 0000 7362 616a  }.jZ...j....sbaj
-00003b90: 5b03 0000 7d94 286a 5d03 0000 5d94 6a5f  [...}.(j]...].j_
-00003ba0: 0300 005d 946a 6103 0000 5d94 6a63 0300  ...].ja...].jc..
-00003bb0: 005d 946a 6503 0000 5d94 756a 6703 0000  .].je...].ujg...
-00003bc0: 6a68 0300 0075 626a e702 0000 6a4e 0300  jh...ubj....jN..
-00003bd0: 0029 8194 7d94 286a 5103 0000 686c 6a52  .)..}.(jQ...hljR
-00003be0: 0300 005d 946a 5503 0000 8c0c 496e 7374  ...].jU.....Inst
-00003bf0: 616c 6c61 7469 6f6e 9485 9481 947d 946a  allation.....}.j
-00003c00: 5a03 0000 6ab7 0300 0073 6261 6a5b 0300  Z...j....sbaj[..
-00003c10: 007d 9428 8c03 6964 7394 5d94 8c07 636c  .}.(..ids.]...cl
-00003c20: 6173 7365 7394 5d94 8c05 6e61 6d65 7394  asses.]...names.
-00003c30: 5d94 8c08 6475 706e 616d 6573 945d 948c  ]...dupnames.]..
-00003c40: 0862 6163 6b72 6566 7394 5d94 756a 6703  .backrefs.].ujg.
-00003c50: 0000 6a4d 0300 0075 6275 8c0a 6c6f 6e67  ..jM...ubu..long
-00003c60: 7469 746c 6573 947d 9428 6a1c 0300 006a  titles.}.(j....j
-00003c70: 4f03 0000 6a1d 0300 006a 6903 0000 6a1e  O...j....ji...j.
-00003c80: 0300 006a 7603 0000 6a1f 0300 006a 8303  ...jv...j....j..
-00003c90: 0000 6a20 0300 006a 9003 0000 6a21 0300  ..j ...j....j!..
-00003ca0: 006a 9d03 0000 6a22 0300 006a aa03 0000  .j....j"...j....
-00003cb0: 6ae7 0200 006a b703 0000 758c 0474 6f63  j....j....u..toc
-00003cc0: 7394 7d94 286a 1c03 0000 6a4c 0300 008c  s.}.(j....jL....
-00003cd0: 0b62 756c 6c65 745f 6c69 7374 9493 9429  .bullet_list...)
-00003ce0: 8194 7d94 286a 5103 0000 686c 6a52 0300  ..}.(jQ...hljR..
-00003cf0: 005d 946a 4c03 0000 8c09 6c69 7374 5f69  .].jL.....list_i
-00003d00: 7465 6d94 9394 2981 947d 9428 6a51 0300  tem...)..}.(jQ..
-00003d10: 0068 6c6a 5203 0000 5d94 8c0f 7370 6869  .hljR...]...sphi
-00003d20: 6e78 2e61 6464 6e6f 6465 7394 8c11 636f  nx.addnodes...co
-00003d30: 6d70 6163 745f 7061 7261 6772 6170 6894  mpact_paragraph.
-00003d40: 9394 2981 947d 9428 6a51 0300 0068 6c6a  ..)..}.(jQ...hlj
-00003d50: 5203 0000 5d94 6a4c 0300 008c 0972 6566  R...].jL.....ref
-00003d60: 6572 656e 6365 9493 9429 8194 7d94 286a  erence...)..}.(j
-00003d70: 5103 0000 686c 6a52 0300 005d 946a 5503  Q...hljR...].jU.
-00003d80: 0000 8c0c 4661 7374 4d42 4152 2041 5049  ....FastMBAR API
-00003d90: 9485 9481 947d 946a 5a03 0000 6adf 0300  .....}.jZ...j...
-00003da0: 0073 6261 6a5b 0300 007d 9428 6a5d 0300  .sbaj[...}.(j]..
-00003db0: 005d 946a 5f03 0000 5d94 6a61 0300 005d  .].j_...].ja...]
-00003dc0: 946a 6303 0000 5d94 6a65 0300 005d 948c  .jc...].je...]..
-00003dd0: 0869 6e74 6572 6e61 6c94 888c 0672 6566  .internal....ref
-00003de0: 7572 6994 6a1c 0300 008c 0a61 6e63 686f  uri.j......ancho
-00003df0: 726e 616d 6594 686c 756a 6703 0000 8c09  rname.hlujg.....
-00003e00: 7265 6665 7265 6e63 6594 6a5a 0300 006a  reference.jZ...j
-00003e10: da03 0000 7562 616a 5b03 0000 7d94 286a  ....ubaj[...}.(j
-00003e20: 5d03 0000 5d94 6a5f 0300 005d 946a 6103  ]...].j_...].ja.
-00003e30: 0000 5d94 6a63 0300 005d 946a 6503 0000  ..].jc...].je...
-00003e40: 5d94 756a 6703 0000 8c11 636f 6d70 6163  ].ujg.....compac
-00003e50: 745f 7061 7261 6772 6170 6894 6a5a 0300  t_paragraph.jZ..
-00003e60: 006a d403 0000 7562 616a 5b03 0000 7d94  .j....ubaj[...}.
-00003e70: 286a 5d03 0000 5d94 6a5f 0300 005d 946a  (j]...].j_...].j
-00003e80: 6103 0000 5d94 6a63 0300 005d 946a 6503  a...].jc...].je.
-00003e90: 0000 5d94 756a 6703 0000 8c09 6c69 7374  ..].ujg.....list
-00003ea0: 5f69 7465 6d94 6a5a 0300 006a cf03 0000  _item.jZ...j....
-00003eb0: 7562 616a 5b03 0000 7d94 286a 5d03 0000  ubaj[...}.(j]...
-00003ec0: 5d94 6a5f 0300 005d 946a 6103 0000 5d94  ].j_...].ja...].
-00003ed0: 6a63 0300 005d 946a 6503 0000 5d94 756a  jc...].je...].uj
-00003ee0: 6703 0000 8c0b 6275 6c6c 6574 5f6c 6973  g.....bullet_lis
-00003ef0: 7494 7562 6a1d 0300 006a ce03 0000 2981  t.ubj....j....).
-00003f00: 947d 9428 6a51 0300 0068 6c6a 5203 0000  .}.(jQ...hljR...
-00003f10: 5d94 6ad3 0300 0029 8194 7d94 286a 5103  ].j....)..}.(jQ.
-00003f20: 0000 686c 6a52 0300 005d 9428 6ad9 0300  ..hljR...].(j...
-00003f30: 0029 8194 7d94 286a 5103 0000 686c 6a52  .)..}.(jQ...hljR
-00003f40: 0300 005d 946a de03 0000 2981 947d 9428  ...].j....)..}.(
-00003f50: 6a51 0300 0068 6c6a 5203 0000 5d94 6a55  jQ...hljR...].jU
-00003f60: 0300 008c 3445 7861 6d70 6c65 2031 2e20  ....4Example 1. 
-00003f70: 436f 6d70 7574 6520 7468 6520 504d 4620  Compute the PMF 
-00003f80: 6f66 2061 2064 6968 6564 7261 6c20 666f  of a dihedral fo
-00003f90: 7220 6275 7461 6e65 2e94 8594 8194 7d94  r butane......}.
-00003fa0: 6a5a 0300 006a 0e04 0000 7362 616a 5b03  jZ...j....sbaj[.
-00003fb0: 0000 7d94 286a 5d03 0000 5d94 6a5f 0300  ..}.(j]...].j_..
-00003fc0: 005d 946a 6103 0000 5d94 6a63 0300 005d  .].ja...].jc...]
-00003fd0: 946a 6503 0000 5d94 8c08 696e 7465 726e  .je...]...intern
-00003fe0: 616c 9488 8c06 7265 6675 7269 946a 1d03  al....refuri.j..
-00003ff0: 0000 8c0a 616e 6368 6f72 6e61 6d65 9468  ....anchorname.h
-00004000: 6c75 6a67 0300 006a ef03 0000 6a5a 0300  lujg...j....jZ..
-00004010: 006a 0b04 0000 7562 616a 5b03 0000 7d94  .j....ubaj[...}.
-00004020: 286a 5d03 0000 5d94 6a5f 0300 005d 946a  (j]...].j_...].j
-00004030: 6103 0000 5d94 6a63 0300 005d 946a 6503  a...].jc...].je.
-00004040: 0000 5d94 756a 6703 0000 6af6 0300 006a  ..].ujg...j....j
-00004050: 5a03 0000 6a08 0400 0075 626a ce03 0000  Z...j....ubj....
-00004060: 2981 947d 9428 6a51 0300 0068 6c6a 5203  )..}.(jQ...hljR.
-00004070: 0000 5d94 286a d303 0000 2981 947d 9428  ..].(j....)..}.(
-00004080: 6a51 0300 0068 6c6a 5203 0000 5d94 6ad9  jQ...hljR...].j.
-00004090: 0300 0029 8194 7d94 286a 5103 0000 686c  ...)..}.(jQ...hl
-000040a0: 6a52 0300 005d 946a de03 0000 2981 947d  jR...].j....)..}
-000040b0: 9428 6a51 0300 0068 6c6a 5203 0000 5d94  .(jQ...hljR...].
-000040c0: 6a55 0300 008c 2731 2e20 436f 6e73 7472  jU....'1. Constr
-000040d0: 7563 7420 616e 204f 7065 6e4d 4d20 7379  uct an OpenMM sy
-000040e0: 7374 656d 206f 6620 6275 7461 6e65 9485  stem of butane..
-000040f0: 9481 947d 946a 5a03 0000 6a2d 0400 0073  ...}.jZ...j-...s
-00004100: 6261 6a5b 0300 007d 9428 6a5d 0300 005d  baj[...}.(j]...]
-00004110: 946a 5f03 0000 5d94 6a61 0300 005d 946a  .j_...].ja...].j
-00004120: 6303 0000 5d94 6a65 0300 005d 948c 0869  c...].je...]...i
-00004130: 6e74 6572 6e61 6c94 888c 0672 6566 7572  nternal....refur
-00004140: 6994 6a1d 0300 008c 0a61 6e63 686f 726e  i.j......anchorn
-00004150: 616d 6594 8c25 2363 6f6e 7374 7275 6374  ame..%#construct
-00004160: 2d61 6e2d 6f70 656e 6d6d 2d73 7973 7465  -an-openmm-syste
-00004170: 6d2d 6f66 2d62 7574 616e 6594 756a 6703  m-of-butane.ujg.
-00004180: 0000 6aef 0300 006a 5a03 0000 6a2a 0400  ..j....jZ...j*..
-00004190: 0075 6261 6a5b 0300 007d 9428 6a5d 0300  .ubaj[...}.(j]..
-000041a0: 005d 946a 5f03 0000 5d94 6a61 0300 005d  .].j_...].ja...]
-000041b0: 946a 6303 0000 5d94 6a65 0300 005d 9475  .jc...].je...].u
-000041c0: 6a67 0300 006a f603 0000 6a5a 0300 006a  jg...j....jZ...j
-000041d0: 2704 0000 7562 616a 5b03 0000 7d94 286a  '...ubaj[...}.(j
-000041e0: 5d03 0000 5d94 6a5f 0300 005d 946a 6103  ]...].j_...].ja.
-000041f0: 0000 5d94 6a63 0300 005d 946a 6503 0000  ..].jc...].je...
-00004200: 5d94 756a 6703 0000 6afd 0300 006a 5a03  ].ujg...j....jZ.
-00004210: 0000 6a24 0400 0075 626a d303 0000 2981  ..j$...ubj....).
-00004220: 947d 9428 6a51 0300 0068 6c6a 5203 0000  .}.(jQ...hljR...
-00004230: 5d94 6ad9 0300 0029 8194 7d94 286a 5103  ].j....)..}.(jQ.
-00004240: 0000 686c 6a52 0300 005d 946a de03 0000  ..hljR...].j....
-00004250: 2981 947d 9428 6a51 0300 0068 6c6a 5203  )..}.(jQ...hljR.
-00004260: 0000 5d94 6a55 0300 008c 1832 2e20 5275  ..].jU.....2. Ru
-00004270: 6e20 756d 6272 656c 6c61 2073 616d 706c  n umbrella sampl
-00004280: 696e 6794 8594 8194 7d94 6a5a 0300 006a  ing.....}.jZ...j
-00004290: 5004 0000 7362 616a 5b03 0000 7d94 286a  P...sbaj[...}.(j
-000042a0: 5d03 0000 5d94 6a5f 0300 005d 946a 6103  ]...].j_...].ja.
-000042b0: 0000 5d94 6a63 0300 005d 946a 6503 0000  ..].jc...].je...
-000042c0: 5d94 8c08 696e 7465 726e 616c 9488 8c06  ]...internal....
-000042d0: 7265 6675 7269 946a 1d03 0000 8c0a 616e  refuri.j......an
-000042e0: 6368 6f72 6e61 6d65 948c 1623 7275 6e2d  chorname...#run-
-000042f0: 756d 6272 656c 6c61 2d73 616d 706c 696e  umbrella-samplin
-00004300: 6794 756a 6703 0000 6aef 0300 006a 5a03  g.ujg...j....jZ.
-00004310: 0000 6a4d 0400 0075 6261 6a5b 0300 007d  ..jM...ubaj[...}
-00004320: 9428 6a5d 0300 005d 946a 5f03 0000 5d94  .(j]...].j_...].
-00004330: 6a61 0300 005d 946a 6303 0000 5d94 6a65  ja...].jc...].je
-00004340: 0300 005d 9475 6a67 0300 006a f603 0000  ...].ujg...j....
-00004350: 6a5a 0300 006a 4a04 0000 7562 616a 5b03  jZ...jJ...ubaj[.
-00004360: 0000 7d94 286a 5d03 0000 5d94 6a5f 0300  ..}.(j]...].j_..
-00004370: 005d 946a 6103 0000 5d94 6a63 0300 005d  .].ja...].jc...]
-00004380: 946a 6503 0000 5d94 756a 6703 0000 6afd  .je...].ujg...j.
-00004390: 0300 006a 5a03 0000 6a24 0400 0075 626a  ...jZ...j$...ubj
-000043a0: d303 0000 2981 947d 9428 6a51 0300 0068  ....)..}.(jQ...h
-000043b0: 6c6a 5203 0000 5d94 6ad9 0300 0029 8194  ljR...].j....)..
-000043c0: 7d94 286a 5103 0000 686c 6a52 0300 005d  }.(jQ...hljR...]
-000043d0: 946a de03 0000 2981 947d 9428 6a51 0300  .j....)..}.(jQ..
-000043e0: 0068 6c6a 5203 0000 5d94 6a55 0300 008c  .hljR...].jU....
-000043f0: 3133 2e20 436f 6d70 7574 6520 616e 6420  13. Compute and 
-00004400: 636f 6c6c 6563 7420 7468 6520 6275 7461  collect the buta
-00004410: 6e65 2064 6968 6564 7261 6c20 7661 6c75  ne dihedral valu
-00004420: 6573 9485 9481 947d 946a 5a03 0000 6a73  es.....}.jZ...js
-00004430: 0400 0073 6261 6a5b 0300 007d 9428 6a5d  ...sbaj[...}.(j]
-00004440: 0300 005d 946a 5f03 0000 5d94 6a61 0300  ...].j_...].ja..
-00004450: 005d 946a 6303 0000 5d94 6a65 0300 005d  .].jc...].je...]
-00004460: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
-00004470: 6566 7572 6994 6a1d 0300 008c 0a61 6e63  efuri.j......anc
-00004480: 686f 726e 616d 6594 8c2f 2363 6f6d 7075  horname../#compu
-00004490: 7465 2d61 6e64 2d63 6f6c 6c65 6374 2d74  te-and-collect-t
-000044a0: 6865 2d62 7574 616e 652d 6469 6865 6472  he-butane-dihedr
-000044b0: 616c 2d76 616c 7565 7394 756a 6703 0000  al-values.ujg...
-000044c0: 6aef 0300 006a 5a03 0000 6a70 0400 0075  j....jZ...jp...u
-000044d0: 6261 6a5b 0300 007d 9428 6a5d 0300 005d  baj[...}.(j]...]
-000044e0: 946a 5f03 0000 5d94 6a61 0300 005d 946a  .j_...].ja...].j
-000044f0: 6303 0000 5d94 6a65 0300 005d 9475 6a67  c...].je...].ujg
-00004500: 0300 006a f603 0000 6a5a 0300 006a 6d04  ...j....jZ...jm.
-00004510: 0000 7562 616a 5b03 0000 7d94 286a 5d03  ..ubaj[...}.(j].
-00004520: 0000 5d94 6a5f 0300 005d 946a 6103 0000  ..].j_...].ja...
-00004530: 5d94 6a63 0300 005d 946a 6503 0000 5d94  ].jc...].je...].
-00004540: 756a 6703 0000 6afd 0300 006a 5a03 0000  ujg...j....jZ...
-00004550: 6a24 0400 0075 626a d303 0000 2981 947d  j$...ubj....)..}
-00004560: 9428 6a51 0300 0068 6c6a 5203 0000 5d94  .(jQ...hljR...].
-00004570: 6ad9 0300 0029 8194 7d94 286a 5103 0000  j....)..}.(jQ...
-00004580: 686c 6a52 0300 005d 946a de03 0000 2981  hljR...].j....).
-00004590: 947d 9428 6a51 0300 0068 6c6a 5203 0000  .}.(jQ...hljR...
-000045a0: 5d94 6a55 0300 008c 4134 2e20 5573 6520  ].jU....A4. Use 
-000045b0: 4661 7374 4d42 4152 2074 6f20 736f 6c76  FastMBAR to solv
-000045c0: 6520 4d42 4152 2f55 5748 414d 2065 7175  e MBAR/UWHAM equ
-000045d0: 6174 696f 6e73 2061 6e64 2063 6f6d 7075  ations and compu
-000045e0: 7465 2074 6865 2050 4d46 9485 9481 947d  te the PMF.....}
-000045f0: 946a 5a03 0000 6a96 0400 0073 6261 6a5b  .jZ...j....sbaj[
-00004600: 0300 007d 9428 6a5d 0300 005d 946a 5f03  ...}.(j]...].j_.
-00004610: 0000 5d94 6a61 0300 005d 946a 6303 0000  ..].ja...].jc...
-00004620: 5d94 6a65 0300 005d 948c 0869 6e74 6572  ].je...]...inter
-00004630: 6e61 6c94 888c 0672 6566 7572 6994 6a1d  nal....refuri.j.
-00004640: 0300 008c 0a61 6e63 686f 726e 616d 6594  .....anchorname.
-00004650: 8c3f 2375 7365 2d66 6173 746d 6261 722d  .?#use-fastmbar-
-00004660: 746f 2d73 6f6c 7665 2d6d 6261 722d 7577  to-solve-mbar-uw
-00004670: 6861 6d2d 6571 7561 7469 6f6e 732d 616e  ham-equations-an
-00004680: 642d 636f 6d70 7574 652d 7468 652d 706d  d-compute-the-pm
-00004690: 6694 756a 6703 0000 6aef 0300 006a 5a03  f.ujg...j....jZ.
-000046a0: 0000 6a93 0400 0075 6261 6a5b 0300 007d  ..j....ubaj[...}
-000046b0: 9428 6a5d 0300 005d 946a 5f03 0000 5d94  .(j]...].j_...].
-000046c0: 6a61 0300 005d 946a 6303 0000 5d94 6a65  ja...].jc...].je
-000046d0: 0300 005d 9475 6a67 0300 006a f603 0000  ...].ujg...j....
-000046e0: 6a5a 0300 006a 9004 0000 7562 616a 5b03  jZ...j....ubaj[.
-000046f0: 0000 7d94 286a 5d03 0000 5d94 6a5f 0300  ..}.(j]...].j_..
-00004700: 005d 946a 6103 0000 5d94 6a63 0300 005d  .].ja...].jc...]
-00004710: 946a 6503 0000 5d94 756a 6703 0000 6afd  .je...].ujg...j.
-00004720: 0300 006a 5a03 0000 6a24 0400 0075 6265  ...jZ...j$...ube
-00004730: 6a5b 0300 007d 9428 6a5d 0300 005d 946a  j[...}.(j]...].j
-00004740: 5f03 0000 5d94 6a61 0300 005d 946a 6303  _...].ja...].jc.
-00004750: 0000 5d94 6a65 0300 005d 9475 6a67 0300  ..].je...].ujg..
-00004760: 006a 0404 0000 6a5a 0300 006a 0804 0000  .j....jZ...j....
-00004770: 7562 656a 5b03 0000 7d94 286a 5d03 0000  ubej[...}.(j]...
-00004780: 5d94 6a5f 0300 005d 946a 6103 0000 5d94  ].j_...].ja...].
-00004790: 6a63 0300 005d 946a 6503 0000 5d94 756a  jc...].je...].uj
-000047a0: 6703 0000 6afd 0300 006a 5a03 0000 6a05  g...j....jZ...j.
-000047b0: 0400 0075 6261 6a5b 0300 007d 9428 6a5d  ...ubaj[...}.(j]
-000047c0: 0300 005d 946a 5f03 0000 5d94 6a61 0300  ...].j_...].ja..
-000047d0: 005d 946a 6303 0000 5d94 6a65 0300 005d  .].jc...].je...]
-000047e0: 9475 6a67 0300 006a 0404 0000 7562 6a1e  .ujg...j....ubj.
-000047f0: 0300 006a ce03 0000 2981 947d 9428 6a51  ...j....)..}.(jQ
-00004800: 0300 0068 6c6a 5203 0000 5d94 6ad3 0300  ...hljR...].j...
-00004810: 0029 8194 7d94 286a 5103 0000 686c 6a52  .)..}.(jQ...hljR
-00004820: 0300 005d 9428 6ad9 0300 0029 8194 7d94  ...].(j....)..}.
-00004830: 286a 5103 0000 686c 6a52 0300 005d 946a  (jQ...hljR...].j
-00004840: de03 0000 2981 947d 9428 6a51 0300 0068  ....)..}.(jQ...h
-00004850: 6c6a 5203 0000 5d94 6a55 0300 008c 3745  ljR...].jU....7E
-00004860: 7861 6d70 6c65 2032 2e20 436f 6d70 7574  xample 2. Comput
-00004870: 6520 6120 3244 2d50 4d46 206f 6620 6469  e a 2D-PMF of di
-00004880: 6865 6472 616c 7320 666f 7220 6469 616c  hedrals for dial
-00004890: 616e 696e 652e 9485 9481 947d 946a 5a03  anine......}.jZ.
-000048a0: 0000 6ace 0400 0073 6261 6a5b 0300 007d  ..j....sbaj[...}
-000048b0: 9428 6a5d 0300 005d 946a 5f03 0000 5d94  .(j]...].j_...].
-000048c0: 6a61 0300 005d 946a 6303 0000 5d94 6a65  ja...].jc...].je
+00003470: 6c5f 646f 6373 947d 9428 8c0d 6469 616c  l_docs.}.(..dial
+00003480: 616e 696e 655f 504d 4694 4741 d92b 05d6  anine_PMF.GA.+..
+00003490: c947 b26a e902 0000 4741 d92b 0767 6303  .G.j....GA.+.gc.
+000034a0: c56a ee02 0000 4741 d92b 0767 64b2 d96a  .j....GA.+.gd..j
+000034b0: e702 0000 4741 d92b 0767 6547 f16a e802  ....GA.+.geG.j..
+000034c0: 0000 4741 d92b 0767 65b7 456a ec02 0000  ..GA.+.ge.Ej....
+000034d0: 4741 d92b 0767 669c 516a ea02 0000 4741  GA.+.gf.Qj....GA
+000034e0: d92b 0767 66f2 c76a ed02 0000 4741 d92b  .+.gf..j....GA.+
+000034f0: 0767 6829 2d75 8c0c 6465 7065 6e64 656e  .gh)-u..dependen
+00003500: 6369 6573 9468 5b8c 0b64 6566 6175 6c74  cies.h[..default
+00003510: 6469 6374 9493 948c 0862 7569 6c74 696e  dict.....builtin
+00003520: 7394 8c03 7365 7494 9394 8594 5294 286a  s...set.....R.(j
+00003530: 1c03 0000 8f94 288c 252e 2e2f 2e2e 2f65  ......(.%../../e
+00003540: 7861 6d70 6c65 732f 6469 616c 616e 696e  xamples/dialanin
+00003550: 652f 6461 7461 2f50 4d46 2e70 6e67 948c  e/data/PMF.png..
+00003560: 272e 2e2f 2e2e 2f65 7861 6d70 6c65 732f  '../../examples/
+00003570: 6469 616c 616e 696e 652f 6461 7461 2f46  dialanine/data/F
+00003580: 6967 5f31 2e70 6e67 948c 272e 2e2f 2e2e  ig_1.png..'../..
+00003590: 2f65 7861 6d70 6c65 732f 6469 616c 616e  /examples/dialan
+000035a0: 696e 652f 6461 7461 2f46 6967 5f32 2e70  ine/data/Fig_2.p
+000035b0: 6e67 9490 6ae9 0200 008f 9428 8c1a 2e2e  ng..j......(....
+000035c0: 2f2e 2e2f 4661 7374 4d42 4152 2f66 6173  /../FastMBAR/fas
+000035d0: 746d 6261 722e 7079 9490 6aee 0200 008f  tmbar.py..j.....
+000035e0: 9428 8c24 2e2e 2f2e 2e2f 6578 616d 706c  .(.$../../exampl
+000035f0: 6573 2f62 7574 616e 652f 6461 7461 2f46  es/butane/data/F
+00003600: 6967 5f31 2e70 6e67 948c 222e 2e2f 2e2e  ig_1.png.."../..
+00003610: 2f65 7861 6d70 6c65 732f 6275 7461 6e65  /examples/butane
+00003620: 2f64 6174 612f 504d 462e 706e 6794 8c1a  /data/PMF.png...
+00003630: 2e2e 2f2e 2e2f 4661 7374 4d42 4152 2f66  ../../FastMBAR/f
+00003640: 6173 746d 6261 722e 7079 948c 242e 2e2f  astmbar.py..$../
+00003650: 2e2e 2f65 7861 6d70 6c65 732f 6275 7461  ../examples/buta
+00003660: 6e65 2f64 6174 612f 4669 675f 322e 706e  ne/data/Fig_2.pn
+00003670: 6794 906a e702 0000 8f94 288c 1a2e 2e2f  g..j......(..../
+00003680: 2e2e 2f46 6173 744d 4241 522f 6661 7374  ../FastMBAR/fast
+00003690: 6d62 6172 2e70 7994 906a e802 0000 8f94  mbar.py..j......
+000036a0: 288c 1a2e 2e2f 2e2e 2f46 6173 744d 4241  (..../../FastMBA
+000036b0: 522f 6661 7374 6d62 6172 2e70 7994 906a  R/fastmbar.py..j
+000036c0: ec02 0000 8f94 288c 1a2e 2e2f 2e2e 2f46  ......(..../../F
+000036d0: 6173 744d 4241 522f 6661 7374 6d62 6172  astMBAR/fastmbar
+000036e0: 2e70 7994 906a ea02 0000 8f94 288c 1a2e  .py..j......(...
+000036f0: 2e2f 2e2e 2f46 6173 744d 4241 522f 6661  ./../FastMBAR/fa
+00003700: 7374 6d62 6172 2e70 7994 906a ed02 0000  stmbar.py..j....
+00003710: 8f94 288c 172e 2e2f 2e2e 2f65 6e65 7267  ..(..../../energ
+00003720: 795f 6d61 7472 6978 2e70 6e67 948c 1a2e  y_matrix.png....
+00003730: 2e2f 2e2e 2f46 6173 744d 4241 522f 6661  ./../FastMBAR/fa
+00003740: 7374 6d62 6172 2e70 7994 9075 8c08 696e  stmbar.py..u..in
+00003750: 636c 7564 6564 946a 1f03 0000 6a22 0300  cluded.j....j"..
+00003760: 0085 9452 948c 0d72 6572 6561 645f 616c  ...R...reread_al
+00003770: 7761 7973 948f 948c 086d 6574 6164 6174  ways.....metadat
+00003780: 6194 6a1f 0300 006a 2003 0000 8c04 6469  a.j....j .....di
+00003790: 6374 9493 9485 9452 948c 0674 6974 6c65  ct.....R...title
+000037a0: 7394 7d94 286a 1c03 0000 8c0e 646f 6375  s.}.(j......docu
+000037b0: 7469 6c73 2e6e 6f64 6573 948c 0574 6974  tils.nodes...tit
+000037c0: 6c65 9493 9429 8194 7d94 288c 0972 6177  le...)..}.(..raw
+000037d0: 736f 7572 6365 9468 6c8c 0863 6869 6c64  source.hl..child
+000037e0: 7265 6e94 5d94 6a47 0300 008c 0454 6578  ren.].jG.....Tex
+000037f0: 7494 9394 8c37 4578 616d 706c 6520 322e  t....7Example 2.
+00003800: 2043 6f6d 7075 7465 2061 2032 442d 504d   Compute a 2D-PM
+00003810: 4620 6f66 2064 6968 6564 7261 6c73 2066  F of dihedrals f
+00003820: 6f72 2064 6961 6c61 6e69 6e65 2e94 8594  or dialanine....
+00003830: 8194 7d94 8c06 7061 7265 6e74 946a 4a03  ..}...parent.jJ.
+00003840: 0000 7362 618c 0a61 7474 7269 6275 7465  ..sba..attribute
+00003850: 7394 7d94 288c 0369 6473 945d 948c 0763  s.}.(..ids.]...c
+00003860: 6c61 7373 6573 945d 948c 056e 616d 6573  lasses.]...names
+00003870: 945d 948c 0864 7570 6e61 6d65 7394 5d94  .]...dupnames.].
+00003880: 8c08 6261 636b 7265 6673 945d 9475 8c07  ..backrefs.].u..
+00003890: 7461 676e 616d 6594 8c05 7469 746c 6594  tagname...title.
+000038a0: 7562 6ae9 0200 006a 4903 0000 2981 947d  ubj....jI...)..}
+000038b0: 9428 6a4c 0300 0068 6c6a 4d03 0000 5d94  .(jL...hljM...].
+000038c0: 6a50 0300 008c 0c46 6173 744d 4241 5220  jP.....FastMBAR 
+000038d0: 4150 4994 8594 8194 7d94 6a55 0300 006a  API.....}.jU...j
+000038e0: 6403 0000 7362 616a 5603 0000 7d94 288c  d...sbajV...}.(.
+000038f0: 0369 6473 945d 948c 0763 6c61 7373 6573  .ids.]...classes
+00003900: 945d 948c 056e 616d 6573 945d 948c 0864  .]...names.]...d
+00003910: 7570 6e61 6d65 7394 5d94 8c08 6261 636b  upnames.]...back
+00003920: 7265 6673 945d 9475 6a62 0300 006a 4803  refs.].ujb...jH.
+00003930: 0000 7562 6aee 0200 006a 4903 0000 2981  ..ubj....jI...).
+00003940: 947d 9428 6a4c 0300 0068 6c6a 4d03 0000  .}.(jL...hljM...
+00003950: 5d94 6a50 0300 008c 3445 7861 6d70 6c65  ].jP....4Example
+00003960: 2031 2e20 436f 6d70 7574 6520 7468 6520   1. Compute the 
+00003970: 504d 4620 6f66 2061 2064 6968 6564 7261  PMF of a dihedra
+00003980: 6c20 666f 7220 6275 7461 6e65 2e94 8594  l for butane....
+00003990: 8194 7d94 6a55 0300 006a 7603 0000 7362  ..}.jU...jv...sb
+000039a0: 616a 5603 0000 7d94 286a 6c03 0000 5d94  ajV...}.(jl...].
+000039b0: 6a6e 0300 005d 946a 7003 0000 5d94 6a72  jn...].jp...].jr
+000039c0: 0300 005d 946a 7403 0000 5d94 756a 6203  ...].jt...].ujb.
+000039d0: 0000 6a48 0300 0075 626a e702 0000 6a49  ..jH...ubj....jI
+000039e0: 0300 0029 8194 7d94 286a 4c03 0000 686c  ...)..}.(jL...hl
+000039f0: 6a4d 0300 005d 946a 5003 0000 8c08 4578  jM...].jP.....Ex
+00003a00: 616d 706c 6573 9485 9481 947d 946a 5503  amples.....}.jU.
+00003a10: 0000 6a83 0300 0073 6261 6a56 0300 007d  ..j....sbajV...}
+00003a20: 9428 6a6c 0300 005d 946a 6e03 0000 5d94  .(jl...].jn...].
+00003a30: 6a70 0300 005d 946a 7203 0000 5d94 6a74  jp...].jr...].jt
+00003a40: 0300 005d 9475 6a62 0300 006a 4803 0000  ...].ujb...jH...
+00003a50: 7562 6ae8 0200 006a 4903 0000 2981 947d  ubj....jI...)..}
+00003a60: 9428 6a4c 0300 0068 6c6a 4d03 0000 5d94  .(jL...hljM...].
+00003a70: 6a50 0300 008c 1457 656c 636f 6d65 2074  jP.....Welcome t
+00003a80: 6f20 4661 7374 4d42 4152 2194 8594 8194  o FastMBAR!.....
+00003a90: 7d94 6a55 0300 006a 9003 0000 7362 616a  }.jU...j....sbaj
+00003aa0: 5603 0000 7d94 286a 6c03 0000 5d94 6a6e  V...}.(jl...].jn
+00003ab0: 0300 005d 946a 7003 0000 5d94 6a72 0300  ...].jp...].jr..
+00003ac0: 005d 946a 7403 0000 5d94 756a 6203 0000  .].jt...].ujb...
+00003ad0: 6a48 0300 0075 626a ec02 0000 6a49 0300  jH...ubj....jI..
+00003ae0: 0029 8194 7d94 286a 4c03 0000 686c 6a4d  .)..}.(jL...hljM
+00003af0: 0300 005d 946a 5003 0000 8c0c 496e 7374  ...].jP.....Inst
+00003b00: 616c 6c61 7469 6f6e 9485 9481 947d 946a  allation.....}.j
+00003b10: 5503 0000 6a9d 0300 0073 6261 6a56 0300  U...j....sbajV..
+00003b20: 007d 9428 6a6c 0300 005d 946a 6e03 0000  .}.(jl...].jn...
+00003b30: 5d94 6a70 0300 005d 946a 7203 0000 5d94  ].jp...].jr...].
+00003b40: 6a74 0300 005d 9475 6a62 0300 006a 4803  jt...].ujb...jH.
+00003b50: 0000 7562 6aea 0200 006a 4903 0000 2981  ..ubj....jI...).
+00003b60: 947d 9428 6a4c 0300 0068 6c6a 4d03 0000  .}.(jL...hljM...
+00003b70: 5d94 6a50 0300 008c 0a52 6566 6572 656e  ].jP.....Referen
+00003b80: 6365 7394 8594 8194 7d94 6a55 0300 006a  ces.....}.jU...j
+00003b90: aa03 0000 7362 616a 5603 0000 7d94 286a  ....sbajV...}.(j
+00003ba0: 6c03 0000 5d94 6a6e 0300 005d 946a 7003  l...].jn...].jp.
+00003bb0: 0000 5d94 6a72 0300 005d 946a 7403 0000  ..].jr...].jt...
+00003bc0: 5d94 756a 6203 0000 6a48 0300 0075 626a  ].ujb...jH...ubj
+00003bd0: ed02 0000 6a49 0300 0029 8194 7d94 286a  ....jI...)..}.(j
+00003be0: 4c03 0000 686c 6a4d 0300 005d 946a 5003  L...hljM...].jP.
+00003bf0: 0000 8c05 5573 6167 6594 8594 8194 7d94  ....Usage.....}.
+00003c00: 6a55 0300 006a b703 0000 7362 616a 5603  jU...j....sbajV.
+00003c10: 0000 7d94 286a 6c03 0000 5d94 6a6e 0300  ..}.(jl...].jn..
+00003c20: 005d 946a 7003 0000 5d94 6a72 0300 005d  .].jp...].jr...]
+00003c30: 946a 7403 0000 5d94 756a 6203 0000 6a48  .jt...].ujb...jH
+00003c40: 0300 0075 6275 8c0a 6c6f 6e67 7469 746c  ...ubu..longtitl
+00003c50: 6573 947d 9428 6a1c 0300 006a 4a03 0000  es.}.(j....jJ...
+00003c60: 6ae9 0200 006a 6403 0000 6aee 0200 006a  j....jd...j....j
+00003c70: 7603 0000 6ae7 0200 006a 8303 0000 6ae8  v...j....j....j.
+00003c80: 0200 006a 9003 0000 6aec 0200 006a 9d03  ...j....j....j..
+00003c90: 0000 6aea 0200 006a aa03 0000 6aed 0200  ..j....j....j...
+00003ca0: 006a b703 0000 758c 0474 6f63 7394 7d94  .j....u..tocs.}.
+00003cb0: 286a 1c03 0000 6a47 0300 008c 0b62 756c  (j....jG.....bul
+00003cc0: 6c65 745f 6c69 7374 9493 9429 8194 7d94  let_list...)..}.
+00003cd0: 286a 4c03 0000 686c 6a4d 0300 005d 946a  (jL...hljM...].j
+00003ce0: 4703 0000 8c09 6c69 7374 5f69 7465 6d94  G.....list_item.
+00003cf0: 9394 2981 947d 9428 6a4c 0300 0068 6c6a  ..)..}.(jL...hlj
+00003d00: 4d03 0000 5d94 288c 0f73 7068 696e 782e  M...].(..sphinx.
+00003d10: 6164 646e 6f64 6573 948c 1163 6f6d 7061  addnodes...compa
+00003d20: 6374 5f70 6172 6167 7261 7068 9493 9429  ct_paragraph...)
+00003d30: 8194 7d94 286a 4c03 0000 686c 6a4d 0300  ..}.(jL...hljM..
+00003d40: 005d 946a 4703 0000 8c09 7265 6665 7265  .].jG.....refere
+00003d50: 6e63 6594 9394 2981 947d 9428 6a4c 0300  nce...)..}.(jL..
+00003d60: 0068 6c6a 4d03 0000 5d94 6a50 0300 008c  .hljM...].jP....
+00003d70: 3745 7861 6d70 6c65 2032 2e20 436f 6d70  7Example 2. Comp
+00003d80: 7574 6520 6120 3244 2d50 4d46 206f 6620  ute a 2D-PMF of 
+00003d90: 6469 6865 6472 616c 7320 666f 7220 6469  dihedrals for di
+00003da0: 616c 616e 696e 652e 9485 9481 947d 946a  alanine......}.j
+00003db0: 5503 0000 6ada 0300 0073 6261 6a56 0300  U...j....sbajV..
+00003dc0: 007d 9428 6a58 0300 005d 946a 5a03 0000  .}.(jX...].jZ...
+00003dd0: 5d94 6a5c 0300 005d 946a 5e03 0000 5d94  ].j\...].j^...].
+00003de0: 6a60 0300 005d 948c 0869 6e74 6572 6e61  j`...]...interna
+00003df0: 6c94 888c 0672 6566 7572 6994 6a1c 0300  l....refuri.j...
+00003e00: 008c 0a61 6e63 686f 726e 616d 6594 686c  ...anchorname.hl
+00003e10: 756a 6203 0000 8c09 7265 6665 7265 6e63  ujb.....referenc
+00003e20: 6594 6a55 0300 006a d503 0000 7562 616a  e.jU...j....ubaj
+00003e30: 5603 0000 7d94 286a 5803 0000 5d94 6a5a  V...}.(jX...].jZ
+00003e40: 0300 005d 946a 5c03 0000 5d94 6a5e 0300  ...].j\...].j^..
+00003e50: 005d 946a 6003 0000 5d94 756a 6203 0000  .].j`...].ujb...
+00003e60: 8c11 636f 6d70 6163 745f 7061 7261 6772  ..compact_paragr
+00003e70: 6170 6894 6a55 0300 006a cf03 0000 7562  aph.jU...j....ub
+00003e80: 6ac9 0300 0029 8194 7d94 286a 4c03 0000  j....)..}.(jL...
+00003e90: 686c 6a4d 0300 005d 9428 6ace 0300 0029  hljM...].(j....)
+00003ea0: 8194 7d94 286a 4c03 0000 686c 6a4d 0300  ..}.(jL...hljM..
+00003eb0: 005d 946a d403 0000 2981 947d 9428 6a4c  .].j....)..}.(jL
+00003ec0: 0300 0068 6c6a 4d03 0000 5d94 6ad9 0300  ...hljM...].j...
+00003ed0: 0029 8194 7d94 286a 4c03 0000 686c 6a4d  .)..}.(jL...hljM
+00003ee0: 0300 005d 946a 5003 0000 8c2a 312e 2043  ...].jP....*1. C
+00003ef0: 6f6e 7374 7275 6374 2061 6e20 4f70 656e  onstruct an Open
+00003f00: 4d4d 2073 7973 7465 6d20 6f66 2064 6961  MM system of dia
+00003f10: 6c61 6e69 6e65 9485 9481 947d 946a 5503  lanine.....}.jU.
+00003f20: 0000 6afb 0300 0073 6261 6a56 0300 007d  ..j....sbajV...}
+00003f30: 9428 6a58 0300 005d 946a 5a03 0000 5d94  .(jX...].jZ...].
+00003f40: 6a5c 0300 005d 946a 5e03 0000 5d94 6a60  j\...].j^...].j`
+00003f50: 0300 005d 948c 0869 6e74 6572 6e61 6c94  ...]...internal.
+00003f60: 888c 0672 6566 7572 6994 6a1c 0300 008c  ...refuri.j.....
+00003f70: 0a61 6e63 686f 726e 616d 6594 8c28 2363  .anchorname..(#c
+00003f80: 6f6e 7374 7275 6374 2d61 6e2d 6f70 656e  onstruct-an-open
+00003f90: 6d6d 2d73 7973 7465 6d2d 6f66 2d64 6961  mm-system-of-dia
+00003fa0: 6c61 6e69 6e65 9475 6a62 0300 006a ea03  lanine.ujb...j..
+00003fb0: 0000 6a55 0300 006a f803 0000 7562 616a  ..jU...j....ubaj
+00003fc0: 5603 0000 7d94 286a 5803 0000 5d94 6a5a  V...}.(jX...].jZ
+00003fd0: 0300 005d 946a 5c03 0000 5d94 6a5e 0300  ...].j\...].j^..
+00003fe0: 005d 946a 6003 0000 5d94 756a 6203 0000  .].j`...].ujb...
+00003ff0: 6af1 0300 006a 5503 0000 6af5 0300 0075  j....jU...j....u
+00004000: 6261 6a56 0300 007d 9428 6a58 0300 005d  bajV...}.(jX...]
+00004010: 946a 5a03 0000 5d94 6a5c 0300 005d 946a  .jZ...].j\...].j
+00004020: 5e03 0000 5d94 6a60 0300 005d 9475 6a62  ^...].j`...].ujb
+00004030: 0300 008c 096c 6973 745f 6974 656d 946a  .....list_item.j
+00004040: 5503 0000 6af2 0300 0075 626a ce03 0000  U...j....ubj....
+00004050: 2981 947d 9428 6a4c 0300 0068 6c6a 4d03  )..}.(jL...hljM.
+00004060: 0000 5d94 6ad4 0300 0029 8194 7d94 286a  ..].j....)..}.(j
+00004070: 4c03 0000 686c 6a4d 0300 005d 946a d903  L...hljM...].j..
+00004080: 0000 2981 947d 9428 6a4c 0300 0068 6c6a  ..)..}.(jL...hlj
+00004090: 4d03 0000 5d94 6a50 0300 008c 1832 2e20  M...].jP.....2. 
+000040a0: 5275 6e20 756d 6272 656c 6c61 2073 616d  Run umbrella sam
+000040b0: 706c 696e 6794 8594 8194 7d94 6a55 0300  pling.....}.jU..
+000040c0: 006a 1f04 0000 7362 616a 5603 0000 7d94  .j....sbajV...}.
+000040d0: 286a 5803 0000 5d94 6a5a 0300 005d 946a  (jX...].jZ...].j
+000040e0: 5c03 0000 5d94 6a5e 0300 005d 946a 6003  \...].j^...].j`.
+000040f0: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
+00004100: 8c06 7265 6675 7269 946a 1c03 0000 8c0a  ..refuri.j......
+00004110: 616e 6368 6f72 6e61 6d65 948c 1623 7275  anchorname...#ru
+00004120: 6e2d 756d 6272 656c 6c61 2d73 616d 706c  n-umbrella-sampl
+00004130: 696e 6794 756a 6203 0000 6aea 0300 006a  ing.ujb...j....j
+00004140: 5503 0000 6a1c 0400 0075 6261 6a56 0300  U...j....ubajV..
+00004150: 007d 9428 6a58 0300 005d 946a 5a03 0000  .}.(jX...].jZ...
+00004160: 5d94 6a5c 0300 005d 946a 5e03 0000 5d94  ].j\...].j^...].
+00004170: 6a60 0300 005d 9475 6a62 0300 006a f103  j`...].ujb...j..
+00004180: 0000 6a55 0300 006a 1904 0000 7562 616a  ..jU...j....ubaj
+00004190: 5603 0000 7d94 286a 5803 0000 5d94 6a5a  V...}.(jX...].jZ
+000041a0: 0300 005d 946a 5c03 0000 5d94 6a5e 0300  ...].j\...].j^..
+000041b0: 005d 946a 6003 0000 5d94 756a 6203 0000  .].j`...].ujb...
+000041c0: 6a18 0400 006a 5503 0000 6af2 0300 0075  j....jU...j....u
+000041d0: 626a ce03 0000 2981 947d 9428 6a4c 0300  bj....)..}.(jL..
+000041e0: 0068 6c6a 4d03 0000 5d94 6ad4 0300 0029  .hljM...].j....)
+000041f0: 8194 7d94 286a 4c03 0000 686c 6a4d 0300  ..}.(jL...hljM..
+00004200: 005d 946a d903 0000 2981 947d 9428 6a4c  .].j....)..}.(jL
+00004210: 0300 0068 6c6a 4d03 0000 5d94 6a50 0300  ...hljM...].jP..
+00004220: 008c 3833 2e20 436f 6d70 7574 6520 616e  ..83. Compute an
+00004230: 6420 636f 6c6c 6563 7420 7661 6c75 6573  d collect values
+00004240: 206f 6620 626f 7468 2064 6961 6c61 6e69   of both dialani
+00004250: 6e65 2064 6968 6564 7261 6c94 8594 8194  ne dihedral.....
+00004260: 7d94 6a55 0300 006a 4204 0000 7362 616a  }.jU...jB...sbaj
+00004270: 5603 0000 7d94 286a 5803 0000 5d94 6a5a  V...}.(jX...].jZ
+00004280: 0300 005d 946a 5c03 0000 5d94 6a5e 0300  ...].j\...].j^..
+00004290: 005d 946a 6003 0000 5d94 8c08 696e 7465  .].j`...]...inte
+000042a0: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
+000042b0: 1c03 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
+000042c0: 948c 3623 636f 6d70 7574 652d 616e 642d  ..6#compute-and-
+000042d0: 636f 6c6c 6563 742d 7661 6c75 6573 2d6f  collect-values-o
+000042e0: 662d 626f 7468 2d64 6961 6c61 6e69 6e65  f-both-dialanine
+000042f0: 2d64 6968 6564 7261 6c94 756a 6203 0000  -dihedral.ujb...
+00004300: 6aea 0300 006a 5503 0000 6a3f 0400 0075  j....jU...j?...u
+00004310: 6261 6a56 0300 007d 9428 6a58 0300 005d  bajV...}.(jX...]
+00004320: 946a 5a03 0000 5d94 6a5c 0300 005d 946a  .jZ...].j\...].j
+00004330: 5e03 0000 5d94 6a60 0300 005d 9475 6a62  ^...].j`...].ujb
+00004340: 0300 006a f103 0000 6a55 0300 006a 3c04  ...j....jU...j<.
+00004350: 0000 7562 616a 5603 0000 7d94 286a 5803  ..ubajV...}.(jX.
+00004360: 0000 5d94 6a5a 0300 005d 946a 5c03 0000  ..].jZ...].j\...
+00004370: 5d94 6a5e 0300 005d 946a 6003 0000 5d94  ].j^...].j`...].
+00004380: 756a 6203 0000 6a18 0400 006a 5503 0000  ujb...j....jU...
+00004390: 6af2 0300 0075 626a ce03 0000 2981 947d  j....ubj....)..}
+000043a0: 9428 6a4c 0300 0068 6c6a 4d03 0000 5d94  .(jL...hljM...].
+000043b0: 6ad4 0300 0029 8194 7d94 286a 4c03 0000  j....)..}.(jL...
+000043c0: 686c 6a4d 0300 005d 946a d903 0000 2981  hljM...].j....).
+000043d0: 947d 9428 6a4c 0300 0068 6c6a 4d03 0000  .}.(jL...hljM...
+000043e0: 5d94 6a50 0300 008c 4134 2e20 5573 6520  ].jP....A4. Use 
+000043f0: 4661 7374 4d42 4152 2074 6f20 736f 6c76  FastMBAR to solv
+00004400: 6520 4d42 4152 2f55 5748 414d 2065 7175  e MBAR/UWHAM equ
+00004410: 6174 696f 6e73 2061 6e64 2063 6f6d 7075  ations and compu
+00004420: 7465 2074 6865 2050 4d46 9485 9481 947d  te the PMF.....}
+00004430: 946a 5503 0000 6a65 0400 0073 6261 6a56  .jU...je...sbajV
+00004440: 0300 007d 9428 6a58 0300 005d 946a 5a03  ...}.(jX...].jZ.
+00004450: 0000 5d94 6a5c 0300 005d 946a 5e03 0000  ..].j\...].j^...
+00004460: 5d94 6a60 0300 005d 948c 0869 6e74 6572  ].j`...]...inter
+00004470: 6e61 6c94 888c 0672 6566 7572 6994 6a1c  nal....refuri.j.
+00004480: 0300 008c 0a61 6e63 686f 726e 616d 6594  .....anchorname.
+00004490: 8c3f 2375 7365 2d66 6173 746d 6261 722d  .?#use-fastmbar-
+000044a0: 746f 2d73 6f6c 7665 2d6d 6261 722d 7577  to-solve-mbar-uw
+000044b0: 6861 6d2d 6571 7561 7469 6f6e 732d 616e  ham-equations-an
+000044c0: 642d 636f 6d70 7574 652d 7468 652d 706d  d-compute-the-pm
+000044d0: 6694 756a 6203 0000 6aea 0300 006a 5503  f.ujb...j....jU.
+000044e0: 0000 6a62 0400 0075 6261 6a56 0300 007d  ..jb...ubajV...}
+000044f0: 9428 6a58 0300 005d 946a 5a03 0000 5d94  .(jX...].jZ...].
+00004500: 6a5c 0300 005d 946a 5e03 0000 5d94 6a60  j\...].j^...].j`
+00004510: 0300 005d 9475 6a62 0300 006a f103 0000  ...].ujb...j....
+00004520: 6a55 0300 006a 5f04 0000 7562 616a 5603  jU...j_...ubajV.
+00004530: 0000 7d94 286a 5803 0000 5d94 6a5a 0300  ..}.(jX...].jZ..
+00004540: 005d 946a 5c03 0000 5d94 6a5e 0300 005d  .].j\...].j^...]
+00004550: 946a 6003 0000 5d94 756a 6203 0000 6a18  .j`...].ujb...j.
+00004560: 0400 006a 5503 0000 6af2 0300 0075 6265  ...jU...j....ube
+00004570: 6a56 0300 007d 9428 6a58 0300 005d 946a  jV...}.(jX...].j
+00004580: 5a03 0000 5d94 6a5c 0300 005d 946a 5e03  Z...].j\...].j^.
+00004590: 0000 5d94 6a60 0300 005d 9475 6a62 0300  ..].j`...].ujb..
+000045a0: 008c 0b62 756c 6c65 745f 6c69 7374 946a  ...bullet_list.j
+000045b0: 5503 0000 6acf 0300 0075 6265 6a56 0300  U...j....ubejV..
+000045c0: 007d 9428 6a58 0300 005d 946a 5a03 0000  .}.(jX...].jZ...
+000045d0: 5d94 6a5c 0300 005d 946a 5e03 0000 5d94  ].j\...].j^...].
+000045e0: 6a60 0300 005d 9475 6a62 0300 006a 1804  j`...].ujb...j..
+000045f0: 0000 6a55 0300 006a ca03 0000 7562 616a  ..jU...j....ubaj
+00004600: 5603 0000 7d94 286a 5803 0000 5d94 6a5a  V...}.(jX...].jZ
+00004610: 0300 005d 946a 5c03 0000 5d94 6a5e 0300  ...].j\...].j^..
+00004620: 005d 946a 6003 0000 5d94 756a 6203 0000  .].j`...].ujb...
+00004630: 6a88 0400 0075 626a e902 0000 6ac9 0300  j....ubj....j...
+00004640: 0029 8194 7d94 286a 4c03 0000 686c 6a4d  .)..}.(jL...hljM
+00004650: 0300 005d 946a ce03 0000 2981 947d 9428  ...].j....)..}.(
+00004660: 6a4c 0300 0068 6c6a 4d03 0000 5d94 6ad4  jL...hljM...].j.
+00004670: 0300 0029 8194 7d94 286a 4c03 0000 686c  ...)..}.(jL...hl
+00004680: 6a4d 0300 005d 946a d903 0000 2981 947d  jM...].j....)..}
+00004690: 9428 6a4c 0300 0068 6c6a 4d03 0000 5d94  .(jL...hljM...].
+000046a0: 6a50 0300 008c 0c46 6173 744d 4241 5220  jP.....FastMBAR 
+000046b0: 4150 4994 8594 8194 7d94 6a55 0300 006a  API.....}.jU...j
+000046c0: 9e04 0000 7362 616a 5603 0000 7d94 286a  ....sbajV...}.(j
+000046d0: 6c03 0000 5d94 6a6e 0300 005d 946a 7003  l...].jn...].jp.
+000046e0: 0000 5d94 6a72 0300 005d 946a 7403 0000  ..].jr...].jt...
+000046f0: 5d94 8c08 696e 7465 726e 616c 9488 8c06  ]...internal....
+00004700: 7265 6675 7269 946a e902 0000 8c0a 616e  refuri.j......an
+00004710: 6368 6f72 6e61 6d65 9468 6c75 6a62 0300  chorname.hlujb..
+00004720: 006a d803 0000 6a55 0300 006a 9b04 0000  .j....jU...j....
+00004730: 7562 616a 5603 0000 7d94 286a 6c03 0000  ubajV...}.(jl...
+00004740: 5d94 6a6e 0300 005d 946a 7003 0000 5d94  ].jn...].jp...].
+00004750: 6a72 0300 005d 946a 7403 0000 5d94 756a  jr...].jt...].uj
+00004760: 6203 0000 6ad3 0300 006a 5503 0000 6a98  b...j....jU...j.
+00004770: 0400 0075 6261 6a56 0300 007d 9428 6a6c  ...ubajV...}.(jl
+00004780: 0300 005d 946a 6e03 0000 5d94 6a70 0300  ...].jn...].jp..
+00004790: 005d 946a 7203 0000 5d94 6a74 0300 005d  .].jr...].jt...]
+000047a0: 9475 6a62 0300 006a cd03 0000 6a55 0300  .ujb...j....jU..
+000047b0: 006a 9504 0000 7562 616a 5603 0000 7d94  .j....ubajV...}.
+000047c0: 286a 6c03 0000 5d94 6a6e 0300 005d 946a  (jl...].jn...].j
+000047d0: 7003 0000 5d94 6a72 0300 005d 946a 7403  p...].jr...].jt.
+000047e0: 0000 5d94 756a 6203 0000 6ac8 0300 0075  ..].ujb...j....u
+000047f0: 626a ee02 0000 6ac9 0300 0029 8194 7d94  bj....j....)..}.
+00004800: 286a 4c03 0000 686c 6a4d 0300 005d 946a  (jL...hljM...].j
+00004810: ce03 0000 2981 947d 9428 6a4c 0300 0068  ....)..}.(jL...h
+00004820: 6c6a 4d03 0000 5d94 286a d403 0000 2981  ljM...].(j....).
+00004830: 947d 9428 6a4c 0300 0068 6c6a 4d03 0000  .}.(jL...hljM...
+00004840: 5d94 6ad9 0300 0029 8194 7d94 286a 4c03  ].j....)..}.(jL.
+00004850: 0000 686c 6a4d 0300 005d 946a 5003 0000  ..hljM...].jP...
+00004860: 8c34 4578 616d 706c 6520 312e 2043 6f6d  .4Example 1. Com
+00004870: 7075 7465 2074 6865 2050 4d46 206f 6620  pute the PMF of 
+00004880: 6120 6469 6865 6472 616c 2066 6f72 2062  a dihedral for b
+00004890: 7574 616e 652e 9485 9481 947d 946a 5503  utane......}.jU.
+000048a0: 0000 6ac9 0400 0073 6261 6a56 0300 007d  ..j....sbajV...}
+000048b0: 9428 6a6c 0300 005d 946a 6e03 0000 5d94  .(jl...].jn...].
+000048c0: 6a70 0300 005d 946a 7203 0000 5d94 6a74  jp...].jr...].jt
 000048d0: 0300 005d 948c 0869 6e74 6572 6e61 6c94  ...]...internal.
-000048e0: 888c 0672 6566 7572 6994 6a1e 0300 008c  ...refuri.j.....
+000048e0: 888c 0672 6566 7572 6994 6aee 0200 008c  ...refuri.j.....
 000048f0: 0a61 6e63 686f 726e 616d 6594 686c 756a  .anchorname.hluj
-00004900: 6703 0000 6aef 0300 006a 5a03 0000 6acb  g...j....jZ...j.
-00004910: 0400 0075 6261 6a5b 0300 007d 9428 6a5d  ...ubaj[...}.(j]
-00004920: 0300 005d 946a 5f03 0000 5d94 6a61 0300  ...].j_...].ja..
-00004930: 005d 946a 6303 0000 5d94 6a65 0300 005d  .].jc...].je...]
-00004940: 9475 6a67 0300 006a f603 0000 6a5a 0300  .ujg...j....jZ..
-00004950: 006a c804 0000 7562 6ace 0300 0029 8194  .j....ubj....)..
-00004960: 7d94 286a 5103 0000 686c 6a52 0300 005d  }.(jQ...hljR...]
-00004970: 9428 6ad3 0300 0029 8194 7d94 286a 5103  .(j....)..}.(jQ.
-00004980: 0000 686c 6a52 0300 005d 946a d903 0000  ..hljR...].j....
-00004990: 2981 947d 9428 6a51 0300 0068 6c6a 5203  )..}.(jQ...hljR.
-000049a0: 0000 5d94 6ade 0300 0029 8194 7d94 286a  ..].j....)..}.(j
-000049b0: 5103 0000 686c 6a52 0300 005d 946a 5503  Q...hljR...].jU.
-000049c0: 0000 8c2a 312e 2043 6f6e 7374 7275 6374  ...*1. Construct
+00004900: 6203 0000 6ad8 0300 006a 5503 0000 6ac6  b...j....jU...j.
+00004910: 0400 0075 6261 6a56 0300 007d 9428 6a6c  ...ubajV...}.(jl
+00004920: 0300 005d 946a 6e03 0000 5d94 6a70 0300  ...].jn...].jp..
+00004930: 005d 946a 7203 0000 5d94 6a74 0300 005d  .].jr...].jt...]
+00004940: 9475 6a62 0300 006a d303 0000 6a55 0300  .ujb...j....jU..
+00004950: 006a c304 0000 7562 6ac9 0300 0029 8194  .j....ubj....)..
+00004960: 7d94 286a 4c03 0000 686c 6a4d 0300 005d  }.(jL...hljM...]
+00004970: 9428 6ace 0300 0029 8194 7d94 286a 4c03  .(j....)..}.(jL.
+00004980: 0000 686c 6a4d 0300 005d 946a d403 0000  ..hljM...].j....
+00004990: 2981 947d 9428 6a4c 0300 0068 6c6a 4d03  )..}.(jL...hljM.
+000049a0: 0000 5d94 6ad9 0300 0029 8194 7d94 286a  ..].j....)..}.(j
+000049b0: 4c03 0000 686c 6a4d 0300 005d 946a 5003  L...hljM...].jP.
+000049c0: 0000 8c27 312e 2043 6f6e 7374 7275 6374  ...'1. Construct
 000049d0: 2061 6e20 4f70 656e 4d4d 2073 7973 7465   an OpenMM syste
-000049e0: 6d20 6f66 2064 6961 6c61 6e69 6e65 9485  m of dialanine..
-000049f0: 9481 947d 946a 5a03 0000 6aed 0400 0073  ...}.jZ...j....s
-00004a00: 6261 6a5b 0300 007d 9428 6a5d 0300 005d  baj[...}.(j]...]
-00004a10: 946a 5f03 0000 5d94 6a61 0300 005d 946a  .j_...].ja...].j
-00004a20: 6303 0000 5d94 6a65 0300 005d 948c 0869  c...].je...]...i
-00004a30: 6e74 6572 6e61 6c94 888c 0672 6566 7572  nternal....refur
-00004a40: 6994 6a1e 0300 008c 0a61 6e63 686f 726e  i.j......anchorn
-00004a50: 616d 6594 8c28 2363 6f6e 7374 7275 6374  ame..(#construct
-00004a60: 2d61 6e2d 6f70 656e 6d6d 2d73 7973 7465  -an-openmm-syste
-00004a70: 6d2d 6f66 2d64 6961 6c61 6e69 6e65 9475  m-of-dialanine.u
-00004a80: 6a67 0300 006a ef03 0000 6a5a 0300 006a  jg...j....jZ...j
-00004a90: ea04 0000 7562 616a 5b03 0000 7d94 286a  ....ubaj[...}.(j
-00004aa0: 5d03 0000 5d94 6a5f 0300 005d 946a 6103  ]...].j_...].ja.
-00004ab0: 0000 5d94 6a63 0300 005d 946a 6503 0000  ..].jc...].je...
-00004ac0: 5d94 756a 6703 0000 6af6 0300 006a 5a03  ].ujg...j....jZ.
-00004ad0: 0000 6ae7 0400 0075 6261 6a5b 0300 007d  ..j....ubaj[...}
-00004ae0: 9428 6a5d 0300 005d 946a 5f03 0000 5d94  .(j]...].j_...].
-00004af0: 6a61 0300 005d 946a 6303 0000 5d94 6a65  ja...].jc...].je
-00004b00: 0300 005d 9475 6a67 0300 006a fd03 0000  ...].ujg...j....
-00004b10: 6a5a 0300 006a e404 0000 7562 6ad3 0300  jZ...j....ubj...
-00004b20: 0029 8194 7d94 286a 5103 0000 686c 6a52  .)..}.(jQ...hljR
-00004b30: 0300 005d 946a d903 0000 2981 947d 9428  ...].j....)..}.(
-00004b40: 6a51 0300 0068 6c6a 5203 0000 5d94 6ade  jQ...hljR...].j.
-00004b50: 0300 0029 8194 7d94 286a 5103 0000 686c  ...)..}.(jQ...hl
-00004b60: 6a52 0300 005d 946a 5503 0000 8c18 322e  jR...].jU.....2.
-00004b70: 2052 756e 2075 6d62 7265 6c6c 6120 7361   Run umbrella sa
-00004b80: 6d70 6c69 6e67 9485 9481 947d 946a 5a03  mpling.....}.jZ.
-00004b90: 0000 6a10 0500 0073 6261 6a5b 0300 007d  ..j....sbaj[...}
-00004ba0: 9428 6a5d 0300 005d 946a 5f03 0000 5d94  .(j]...].j_...].
-00004bb0: 6a61 0300 005d 946a 6303 0000 5d94 6a65  ja...].jc...].je
-00004bc0: 0300 005d 948c 0869 6e74 6572 6e61 6c94  ...]...internal.
-00004bd0: 888c 0672 6566 7572 6994 6a1e 0300 008c  ...refuri.j.....
-00004be0: 0a61 6e63 686f 726e 616d 6594 8c16 2372  .anchorname...#r
-00004bf0: 756e 2d75 6d62 7265 6c6c 612d 7361 6d70  un-umbrella-samp
-00004c00: 6c69 6e67 9475 6a67 0300 006a ef03 0000  ling.ujg...j....
-00004c10: 6a5a 0300 006a 0d05 0000 7562 616a 5b03  jZ...j....ubaj[.
-00004c20: 0000 7d94 286a 5d03 0000 5d94 6a5f 0300  ..}.(j]...].j_..
-00004c30: 005d 946a 6103 0000 5d94 6a63 0300 005d  .].ja...].jc...]
-00004c40: 946a 6503 0000 5d94 756a 6703 0000 6af6  .je...].ujg...j.
-00004c50: 0300 006a 5a03 0000 6a0a 0500 0075 6261  ...jZ...j....uba
-00004c60: 6a5b 0300 007d 9428 6a5d 0300 005d 946a  j[...}.(j]...].j
-00004c70: 5f03 0000 5d94 6a61 0300 005d 946a 6303  _...].ja...].jc.
-00004c80: 0000 5d94 6a65 0300 005d 9475 6a67 0300  ..].je...].ujg..
-00004c90: 006a fd03 0000 6a5a 0300 006a e404 0000  .j....jZ...j....
-00004ca0: 7562 6ad3 0300 0029 8194 7d94 286a 5103  ubj....)..}.(jQ.
-00004cb0: 0000 686c 6a52 0300 005d 946a d903 0000  ..hljR...].j....
-00004cc0: 2981 947d 9428 6a51 0300 0068 6c6a 5203  )..}.(jQ...hljR.
-00004cd0: 0000 5d94 6ade 0300 0029 8194 7d94 286a  ..].j....)..}.(j
-00004ce0: 5103 0000 686c 6a52 0300 005d 946a 5503  Q...hljR...].jU.
-00004cf0: 0000 8c38 332e 2043 6f6d 7075 7465 2061  ...83. Compute a
-00004d00: 6e64 2063 6f6c 6c65 6374 2076 616c 7565  nd collect value
-00004d10: 7320 6f66 2062 6f74 6820 6469 616c 616e  s of both dialan
-00004d20: 696e 6520 6469 6865 6472 616c 9485 9481  ine dihedral....
-00004d30: 947d 946a 5a03 0000 6a33 0500 0073 6261  .}.jZ...j3...sba
-00004d40: 6a5b 0300 007d 9428 6a5d 0300 005d 946a  j[...}.(j]...].j
-00004d50: 5f03 0000 5d94 6a61 0300 005d 946a 6303  _...].ja...].jc.
-00004d60: 0000 5d94 6a65 0300 005d 948c 0869 6e74  ..].je...]...int
-00004d70: 6572 6e61 6c94 888c 0672 6566 7572 6994  ernal....refuri.
-00004d80: 6a1e 0300 008c 0a61 6e63 686f 726e 616d  j......anchornam
-00004d90: 6594 8c36 2363 6f6d 7075 7465 2d61 6e64  e..6#compute-and
-00004da0: 2d63 6f6c 6c65 6374 2d76 616c 7565 732d  -collect-values-
-00004db0: 6f66 2d62 6f74 682d 6469 616c 616e 696e  of-both-dialanin
-00004dc0: 652d 6469 6865 6472 616c 9475 6a67 0300  e-dihedral.ujg..
-00004dd0: 006a ef03 0000 6a5a 0300 006a 3005 0000  .j....jZ...j0...
-00004de0: 7562 616a 5b03 0000 7d94 286a 5d03 0000  ubaj[...}.(j]...
-00004df0: 5d94 6a5f 0300 005d 946a 6103 0000 5d94  ].j_...].ja...].
-00004e00: 6a63 0300 005d 946a 6503 0000 5d94 756a  jc...].je...].uj
-00004e10: 6703 0000 6af6 0300 006a 5a03 0000 6a2d  g...j....jZ...j-
-00004e20: 0500 0075 6261 6a5b 0300 007d 9428 6a5d  ...ubaj[...}.(j]
-00004e30: 0300 005d 946a 5f03 0000 5d94 6a61 0300  ...].j_...].ja..
-00004e40: 005d 946a 6303 0000 5d94 6a65 0300 005d  .].jc...].je...]
-00004e50: 9475 6a67 0300 006a fd03 0000 6a5a 0300  .ujg...j....jZ..
-00004e60: 006a e404 0000 7562 6ad3 0300 0029 8194  .j....ubj....)..
-00004e70: 7d94 286a 5103 0000 686c 6a52 0300 005d  }.(jQ...hljR...]
-00004e80: 946a d903 0000 2981 947d 9428 6a51 0300  .j....)..}.(jQ..
-00004e90: 0068 6c6a 5203 0000 5d94 6ade 0300 0029  .hljR...].j....)
-00004ea0: 8194 7d94 286a 5103 0000 686c 6a52 0300  ..}.(jQ...hljR..
-00004eb0: 005d 946a 5503 0000 8c41 342e 2055 7365  .].jU....A4. Use
-00004ec0: 2046 6173 744d 4241 5220 746f 2073 6f6c   FastMBAR to sol
-00004ed0: 7665 204d 4241 522f 5557 4841 4d20 6571  ve MBAR/UWHAM eq
-00004ee0: 7561 7469 6f6e 7320 616e 6420 636f 6d70  uations and comp
-00004ef0: 7574 6520 7468 6520 504d 4694 8594 8194  ute the PMF.....
-00004f00: 7d94 6a5a 0300 006a 5605 0000 7362 616a  }.jZ...jV...sbaj
-00004f10: 5b03 0000 7d94 286a 5d03 0000 5d94 6a5f  [...}.(j]...].j_
-00004f20: 0300 005d 946a 6103 0000 5d94 6a63 0300  ...].ja...].jc..
-00004f30: 005d 946a 6503 0000 5d94 8c08 696e 7465  .].je...]...inte
-00004f40: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
-00004f50: 1e03 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
-00004f60: 948c 3f23 7573 652d 6661 7374 6d62 6172  ..?#use-fastmbar
-00004f70: 2d74 6f2d 736f 6c76 652d 6d62 6172 2d75  -to-solve-mbar-u
-00004f80: 7768 616d 2d65 7175 6174 696f 6e73 2d61  wham-equations-a
-00004f90: 6e64 2d63 6f6d 7075 7465 2d74 6865 2d70  nd-compute-the-p
-00004fa0: 6d66 9475 6a67 0300 006a ef03 0000 6a5a  mf.ujg...j....jZ
-00004fb0: 0300 006a 5305 0000 7562 616a 5b03 0000  ...jS...ubaj[...
-00004fc0: 7d94 286a 5d03 0000 5d94 6a5f 0300 005d  }.(j]...].j_...]
-00004fd0: 946a 6103 0000 5d94 6a63 0300 005d 946a  .ja...].jc...].j
-00004fe0: 6503 0000 5d94 756a 6703 0000 6af6 0300  e...].ujg...j...
-00004ff0: 006a 5a03 0000 6a50 0500 0075 6261 6a5b  .jZ...jP...ubaj[
-00005000: 0300 007d 9428 6a5d 0300 005d 946a 5f03  ...}.(j]...].j_.
-00005010: 0000 5d94 6a61 0300 005d 946a 6303 0000  ..].ja...].jc...
-00005020: 5d94 6a65 0300 005d 9475 6a67 0300 006a  ].je...].ujg...j
-00005030: fd03 0000 6a5a 0300 006a e404 0000 7562  ....jZ...j....ub
-00005040: 656a 5b03 0000 7d94 286a 5d03 0000 5d94  ej[...}.(j]...].
-00005050: 6a5f 0300 005d 946a 6103 0000 5d94 6a63  j_...].ja...].jc
-00005060: 0300 005d 946a 6503 0000 5d94 756a 6703  ...].je...].ujg.
-00005070: 0000 6a04 0400 006a 5a03 0000 6ac8 0400  ..j....jZ...j...
-00005080: 0075 6265 6a5b 0300 007d 9428 6a5d 0300  .ubej[...}.(j]..
-00005090: 005d 946a 5f03 0000 5d94 6a61 0300 005d  .].j_...].ja...]
-000050a0: 946a 6303 0000 5d94 6a65 0300 005d 9475  .jc...].je...].u
-000050b0: 6a67 0300 006a fd03 0000 6a5a 0300 006a  jg...j....jZ...j
-000050c0: c504 0000 7562 616a 5b03 0000 7d94 286a  ....ubaj[...}.(j
-000050d0: 5d03 0000 5d94 6a5f 0300 005d 946a 6103  ]...].j_...].ja.
-000050e0: 0000 5d94 6a63 0300 005d 946a 6503 0000  ..].jc...].je...
-000050f0: 5d94 756a 6703 0000 6a04 0400 0075 626a  ].ujg...j....ubj
-00005100: 1f03 0000 6ace 0300 0029 8194 7d94 286a  ....j....)..}.(j
-00005110: 5103 0000 686c 6a52 0300 005d 946a d303  Q...hljR...].j..
-00005120: 0000 2981 947d 9428 6a51 0300 0068 6c6a  ..)..}.(jQ...hlj
-00005130: 5203 0000 5d94 286a d903 0000 2981 947d  R...].(j....)..}
-00005140: 9428 6a51 0300 0068 6c6a 5203 0000 5d94  .(jQ...hljR...].
-00005150: 6ade 0300 0029 8194 7d94 286a 5103 0000  j....)..}.(jQ...
-00005160: 686c 6a52 0300 005d 946a 5503 0000 8c08  hljR...].jU.....
-00005170: 4578 616d 706c 6573 9485 9481 947d 946a  Examples.....}.j
-00005180: 5a03 0000 6a8e 0500 0073 6261 6a5b 0300  Z...j....sbaj[..
-00005190: 007d 9428 6a5d 0300 005d 946a 5f03 0000  .}.(j]...].j_...
-000051a0: 5d94 6a61 0300 005d 946a 6303 0000 5d94  ].ja...].jc...].
-000051b0: 6a65 0300 005d 948c 0869 6e74 6572 6e61  je...]...interna
-000051c0: 6c94 888c 0672 6566 7572 6994 6a1f 0300  l....refuri.j...
-000051d0: 008c 0a61 6e63 686f 726e 616d 6594 686c  ...anchorname.hl
-000051e0: 756a 6703 0000 6aef 0300 006a 5a03 0000  ujg...j....jZ...
-000051f0: 6a8b 0500 0075 6261 6a5b 0300 007d 9428  j....ubaj[...}.(
-00005200: 6a5d 0300 005d 946a 5f03 0000 5d94 6a61  j]...].j_...].ja
-00005210: 0300 005d 946a 6303 0000 5d94 6a65 0300  ...].jc...].je..
-00005220: 005d 9475 6a67 0300 006a f603 0000 6a5a  .].ujg...j....jZ
-00005230: 0300 006a 8805 0000 7562 6ace 0300 0029  ...j....ubj....)
-00005240: 8194 7d94 286a 5103 0000 686c 6a52 0300  ..}.(jQ...hljR..
-00005250: 005d 9428 6ad3 0300 0029 8194 7d94 286a  .].(j....)..}.(j
-00005260: 5103 0000 686c 6a52 0300 005d 946a d903  Q...hljR...].j..
-00005270: 0000 2981 947d 9428 6a51 0300 0068 6c6a  ..)..}.(jQ...hlj
-00005280: 5203 0000 5d94 6ade 0300 0029 8194 7d94  R...].j....)..}.
-00005290: 286a 5103 0000 686c 6a52 0300 005d 946a  (jQ...hljR...].j
-000052a0: 5503 0000 8c25 496e 7374 616c 6c20 4578  U....%Install Ex
-000052b0: 7472 6120 5265 7175 6972 6564 2050 7974  tra Required Pyt
-000052c0: 686f 6e20 5061 636b 6765 7394 8594 8194  hon Packges.....
-000052d0: 7d94 6a5a 0300 006a ad05 0000 7362 616a  }.jZ...j....sbaj
-000052e0: 5b03 0000 7d94 286a 5d03 0000 5d94 6a5f  [...}.(j]...].j_
-000052f0: 0300 005d 946a 6103 0000 5d94 6a63 0300  ...].ja...].jc..
-00005300: 005d 946a 6503 0000 5d94 8c08 696e 7465  .].je...]...inte
-00005310: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
-00005320: 1f03 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
-00005330: 948c 2623 696e 7374 616c 6c2d 6578 7472  ..&#install-extr
-00005340: 612d 7265 7175 6972 6564 2d70 7974 686f  a-required-pytho
-00005350: 6e2d 7061 636b 6765 7394 756a 6703 0000  n-packges.ujg...
-00005360: 6aef 0300 006a 5a03 0000 6aaa 0500 0075  j....jZ...j....u
-00005370: 6261 6a5b 0300 007d 9428 6a5d 0300 005d  baj[...}.(j]...]
-00005380: 946a 5f03 0000 5d94 6a61 0300 005d 946a  .j_...].ja...].j
-00005390: 6303 0000 5d94 6a65 0300 005d 9475 6a67  c...].je...].ujg
-000053a0: 0300 006a f603 0000 6a5a 0300 006a a705  ...j....jZ...j..
-000053b0: 0000 7562 616a 5b03 0000 7d94 286a 5d03  ..ubaj[...}.(j].
-000053c0: 0000 5d94 6a5f 0300 005d 946a 6103 0000  ..].j_...].ja...
-000053d0: 5d94 6a63 0300 005d 946a 6503 0000 5d94  ].jc...].je...].
-000053e0: 756a 6703 0000 6afd 0300 006a 5a03 0000  ujg...j....jZ...
-000053f0: 6aa4 0500 0075 626a d303 0000 2981 947d  j....ubj....)..}
-00005400: 9428 6a51 0300 0068 6c6a 5203 0000 5d94  .(jQ...hljR...].
-00005410: 286a d903 0000 2981 947d 9428 6a51 0300  (j....)..}.(jQ..
-00005420: 0068 6c6a 5203 0000 5d94 6ade 0300 0029  .hljR...].j....)
-00005430: 8194 7d94 286a 5103 0000 686c 6a52 0300  ..}.(jQ...hljR..
-00005440: 005d 946a 5503 0000 8c08 4578 616d 706c  .].jU.....Exampl
-00005450: 6573 9485 9481 947d 946a 5a03 0000 6ad0  es.....}.jZ...j.
-00005460: 0500 0073 6261 6a5b 0300 007d 9428 6a5d  ...sbaj[...}.(j]
-00005470: 0300 005d 946a 5f03 0000 5d94 6a61 0300  ...].j_...].ja..
-00005480: 005d 946a 6303 0000 5d94 6a65 0300 005d  .].jc...].je...]
-00005490: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
-000054a0: 6566 7572 6994 6a1f 0300 008c 0a61 6e63  efuri.j......anc
-000054b0: 686f 726e 616d 6594 8c04 2369 6432 9475  horname...#id2.u
-000054c0: 6a67 0300 006a ef03 0000 6a5a 0300 006a  jg...j....jZ...j
-000054d0: cd05 0000 7562 616a 5b03 0000 7d94 286a  ....ubaj[...}.(j
-000054e0: 5d03 0000 5d94 6a5f 0300 005d 946a 6103  ]...].j_...].ja.
-000054f0: 0000 5d94 6a63 0300 005d 946a 6503 0000  ..].jc...].je...
-00005500: 5d94 756a 6703 0000 6af6 0300 006a 5a03  ].ujg...j....jZ.
-00005510: 0000 6aca 0500 0075 626a ce03 0000 2981  ..j....ubj....).
-00005520: 947d 9428 6a51 0300 0068 6c6a 5203 0000  .}.(jQ...hljR...
-00005530: 5d94 6ad7 0300 008c 0774 6f63 7472 6565  ].j......toctree
-00005540: 9493 9429 8194 7d94 286a 5103 0000 686c  ...)..}.(jQ...hl
-00005550: 6a52 0300 005d 946a 5b03 0000 7d94 286a  jR...].j[...}.(j
-00005560: 5d03 0000 5d94 6a5f 0300 005d 946a 6103  ]...].j_...].ja.
-00005570: 0000 5d94 6a63 0300 005d 946a 6503 0000  ..].jc...].je...
-00005580: 5d94 8c06 7061 7265 6e74 946a 1f03 0000  ]...parent.j....
-00005590: 8c07 656e 7472 6965 7394 5d94 284e 8c0a  ..entries.].(N..
-000055a0: 6275 7461 6e65 5f50 4d46 9486 944e 8c0d  butane_PMF...N..
-000055b0: 6469 616c 616e 696e 655f 504d 4694 8694  dialanine_PMF...
-000055c0: 658c 0c69 6e63 6c75 6465 6669 6c65 7394  e..includefiles.
-000055d0: 5d94 286a f805 0000 6afa 0500 0065 8c08  ].(j....j....e..
-000055e0: 6d61 7864 6570 7468 944b 018c 0763 6170  maxdepth.K...cap
-000055f0: 7469 6f6e 944e 8c04 676c 6f62 9489 8c06  tion.N..glob....
-00005600: 6869 6464 656e 9489 8c0d 696e 636c 7564  hidden....includ
-00005610: 6568 6964 6465 6e94 898c 086e 756d 6265  ehidden....numbe
-00005620: 7265 6494 4b00 8c0a 7469 746c 6573 6f6e  red.K...titleson
-00005630: 6c79 9489 8c0a 7261 7765 6e74 7269 6573  ly....rawentries
-00005640: 945d 9475 6a67 0300 008c 0774 6f63 7472  .].ujg.....toctr
-00005650: 6565 948c 0673 6f75 7263 6594 8c68 2f55  ee...source..h/U
-00005660: 7365 7273 2f64 696e 6778 712f 4c69 6272  sers/dingxq/Libr
-00005670: 6172 792f 436c 6f75 6453 746f 7261 6765  ary/CloudStorage
-00005680: 2f42 6f78 2d42 6f78 2f52 6573 6561 7263  /Box-Box/Researc
-00005690: 682f 5072 6f6a 6563 7473 5f6f 6e5f 4769  h/Projects_on_Gi
-000056a0: 7468 7562 2f46 6173 744d 4241 522f 646f  thub/FastMBAR/do
-000056b0: 6373 2f73 6f75 7263 652f 6578 616d 706c  cs/source/exampl
-000056c0: 6573 2e72 7374 948c 046c 696e 6594 4b2e  es.rst...line.K.
-000056d0: 6a5a 0300 006a e705 0000 7562 616a 5b03  jZ...j....ubaj[.
-000056e0: 0000 7d94 286a 5d03 0000 5d94 6a5f 0300  ..}.(j]...].j_..
-000056f0: 005d 946a 6103 0000 5d94 6a63 0300 005d  .].ja...].jc...]
-00005700: 946a 6503 0000 5d94 756a 6703 0000 6a04  .je...].ujg...j.
-00005710: 0400 006a 5a03 0000 6aca 0500 0075 6265  ...jZ...j....ube
-00005720: 6a5b 0300 007d 9428 6a5d 0300 005d 946a  j[...}.(j]...].j
-00005730: 5f03 0000 5d94 6a61 0300 005d 946a 6303  _...].ja...].jc.
-00005740: 0000 5d94 6a65 0300 005d 9475 6a67 0300  ..].je...].ujg..
-00005750: 006a fd03 0000 6a5a 0300 006a a405 0000  .j....jZ...j....
-00005760: 7562 656a 5b03 0000 7d94 286a 5d03 0000  ubej[...}.(j]...
-00005770: 5d94 6a5f 0300 005d 946a 6103 0000 5d94  ].j_...].ja...].
-00005780: 6a63 0300 005d 946a 6503 0000 5d94 756a  jc...].je...].uj
-00005790: 6703 0000 6a04 0400 006a 5a03 0000 6a88  g...j....jZ...j.
-000057a0: 0500 0075 6265 6a5b 0300 007d 9428 6a5d  ...ubej[...}.(j]
-000057b0: 0300 005d 946a 5f03 0000 5d94 6a61 0300  ...].j_...].ja..
-000057c0: 005d 946a 6303 0000 5d94 6a65 0300 005d  .].jc...].je...]
-000057d0: 9475 6a67 0300 006a fd03 0000 6a5a 0300  .ujg...j....jZ..
-000057e0: 006a 8505 0000 7562 616a 5b03 0000 7d94  .j....ubaj[...}.
-000057f0: 286a 5d03 0000 5d94 6a5f 0300 005d 946a  (j]...].j_...].j
-00005800: 6103 0000 5d94 6a63 0300 005d 946a 6503  a...].jc...].je.
-00005810: 0000 5d94 756a 6703 0000 6a04 0400 0075  ..].ujg...j....u
-00005820: 626a 2003 0000 6ace 0300 0029 8194 7d94  bj ...j....)..}.
-00005830: 286a 5103 0000 686c 6a52 0300 005d 946a  (jQ...hljR...].j
-00005840: d303 0000 2981 947d 9428 6a51 0300 0068  ....)..}.(jQ...h
-00005850: 6c6a 5203 0000 5d94 286a d903 0000 2981  ljR...].(j....).
-00005860: 947d 9428 6a51 0300 0068 6c6a 5203 0000  .}.(jQ...hljR...
-00005870: 5d94 6ade 0300 0029 8194 7d94 286a 5103  ].j....)..}.(jQ.
-00005880: 0000 686c 6a52 0300 005d 946a 5503 0000  ..hljR...].jU...
-00005890: 8c14 5765 6c63 6f6d 6520 746f 2046 6173  ..Welcome to Fas
-000058a0: 744d 4241 5221 9485 9481 947d 946a 5a03  tMBAR!.....}.jZ.
-000058b0: 0000 6a32 0600 0073 6261 6a5b 0300 007d  ..j2...sbaj[...}
-000058c0: 9428 6a5d 0300 005d 946a 5f03 0000 5d94  .(j]...].j_...].
-000058d0: 6a61 0300 005d 946a 6303 0000 5d94 6a65  ja...].jc...].je
-000058e0: 0300 005d 948c 0869 6e74 6572 6e61 6c94  ...]...internal.
-000058f0: 888c 0672 6566 7572 6994 6a20 0300 008c  ...refuri.j ....
-00005900: 0a61 6e63 686f 726e 616d 6594 686c 756a  .anchorname.hluj
-00005910: 6703 0000 6aef 0300 006a 5a03 0000 6a2f  g...j....jZ...j/
-00005920: 0600 0075 6261 6a5b 0300 007d 9428 6a5d  ...ubaj[...}.(j]
-00005930: 0300 005d 946a 5f03 0000 5d94 6a61 0300  ...].j_...].ja..
-00005940: 005d 946a 6303 0000 5d94 6a65 0300 005d  .].jc...].je...]
-00005950: 9475 6a67 0300 006a f603 0000 6a5a 0300  .ujg...j....jZ..
-00005960: 006a 2c06 0000 7562 6ace 0300 0029 8194  .j,...ubj....)..
-00005970: 7d94 286a 5103 0000 686c 6a52 0300 005d  }.(jQ...hljR...]
-00005980: 9428 6ad3 0300 0029 8194 7d94 286a 5103  .(j....)..}.(jQ.
-00005990: 0000 686c 6a52 0300 005d 946a d903 0000  ..hljR...].j....
-000059a0: 2981 947d 9428 6a51 0300 0068 6c6a 5203  )..}.(jQ...hljR.
-000059b0: 0000 5d94 6ade 0300 0029 8194 7d94 286a  ..].j....)..}.(j
-000059c0: 5103 0000 686c 6a52 0300 005d 946a 5503  Q...hljR...].jU.
-000059d0: 0000 8c11 5768 6174 2069 7320 4661 7374  ....What is Fast
-000059e0: 4d42 4152 3f94 8594 8194 7d94 6a5a 0300  MBAR?.....}.jZ..
-000059f0: 006a 5106 0000 7362 616a 5b03 0000 7d94  .jQ...sbaj[...}.
-00005a00: 286a 5d03 0000 5d94 6a5f 0300 005d 946a  (j]...].j_...].j
-00005a10: 6103 0000 5d94 6a63 0300 005d 946a 6503  a...].jc...].je.
-00005a20: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
-00005a30: 8c06 7265 6675 7269 946a 2003 0000 8c0a  ..refuri.j .....
-00005a40: 616e 6368 6f72 6e61 6d65 948c 1123 7768  anchorname...#wh
-00005a50: 6174 2d69 732d 6661 7374 6d62 6172 9475  at-is-fastmbar.u
-00005a60: 6a67 0300 006a ef03 0000 6a5a 0300 006a  jg...j....jZ...j
-00005a70: 4e06 0000 7562 616a 5b03 0000 7d94 286a  N...ubaj[...}.(j
-00005a80: 5d03 0000 5d94 6a5f 0300 005d 946a 6103  ]...].j_...].ja.
-00005a90: 0000 5d94 6a63 0300 005d 946a 6503 0000  ..].jc...].je...
-00005aa0: 5d94 756a 6703 0000 6af6 0300 006a 5a03  ].ujg...j....jZ.
-00005ab0: 0000 6a4b 0600 0075 6261 6a5b 0300 007d  ..jK...ubaj[...}
-00005ac0: 9428 6a5d 0300 005d 946a 5f03 0000 5d94  .(j]...].j_...].
-00005ad0: 6a61 0300 005d 946a 6303 0000 5d94 6a65  ja...].jc...].je
-00005ae0: 0300 005d 9475 6a67 0300 006a fd03 0000  ...].ujg...j....
-00005af0: 6a5a 0300 006a 4806 0000 7562 6ad3 0300  jZ...jH...ubj...
-00005b00: 0029 8194 7d94 286a 5103 0000 686c 6a52  .)..}.(jQ...hljR
+000049e0: 6d20 6f66 2062 7574 616e 6594 8594 8194  m of butane.....
+000049f0: 7d94 6a55 0300 006a e804 0000 7362 616a  }.jU...j....sbaj
+00004a00: 5603 0000 7d94 286a 6c03 0000 5d94 6a6e  V...}.(jl...].jn
+00004a10: 0300 005d 946a 7003 0000 5d94 6a72 0300  ...].jp...].jr..
+00004a20: 005d 946a 7403 0000 5d94 8c08 696e 7465  .].jt...]...inte
+00004a30: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
+00004a40: ee02 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
+00004a50: 948c 2523 636f 6e73 7472 7563 742d 616e  ..%#construct-an
+00004a60: 2d6f 7065 6e6d 6d2d 7379 7374 656d 2d6f  -openmm-system-o
+00004a70: 662d 6275 7461 6e65 9475 6a62 0300 006a  f-butane.ujb...j
+00004a80: d803 0000 6a55 0300 006a e504 0000 7562  ....jU...j....ub
+00004a90: 616a 5603 0000 7d94 286a 6c03 0000 5d94  ajV...}.(jl...].
+00004aa0: 6a6e 0300 005d 946a 7003 0000 5d94 6a72  jn...].jp...].jr
+00004ab0: 0300 005d 946a 7403 0000 5d94 756a 6203  ...].jt...].ujb.
+00004ac0: 0000 6ad3 0300 006a 5503 0000 6ae2 0400  ..j....jU...j...
+00004ad0: 0075 6261 6a56 0300 007d 9428 6a6c 0300  .ubajV...}.(jl..
+00004ae0: 005d 946a 6e03 0000 5d94 6a70 0300 005d  .].jn...].jp...]
+00004af0: 946a 7203 0000 5d94 6a74 0300 005d 9475  .jr...].jt...].u
+00004b00: 6a62 0300 006a cd03 0000 6a55 0300 006a  jb...j....jU...j
+00004b10: df04 0000 7562 6ace 0300 0029 8194 7d94  ....ubj....)..}.
+00004b20: 286a 4c03 0000 686c 6a4d 0300 005d 946a  (jL...hljM...].j
+00004b30: d403 0000 2981 947d 9428 6a4c 0300 0068  ....)..}.(jL...h
+00004b40: 6c6a 4d03 0000 5d94 6ad9 0300 0029 8194  ljM...].j....)..
+00004b50: 7d94 286a 4c03 0000 686c 6a4d 0300 005d  }.(jL...hljM...]
+00004b60: 946a 5003 0000 8c18 322e 2052 756e 2075  .jP.....2. Run u
+00004b70: 6d62 7265 6c6c 6120 7361 6d70 6c69 6e67  mbrella sampling
+00004b80: 9485 9481 947d 946a 5503 0000 6a0b 0500  .....}.jU...j...
+00004b90: 0073 6261 6a56 0300 007d 9428 6a6c 0300  .sbajV...}.(jl..
+00004ba0: 005d 946a 6e03 0000 5d94 6a70 0300 005d  .].jn...].jp...]
+00004bb0: 946a 7203 0000 5d94 6a74 0300 005d 948c  .jr...].jt...]..
+00004bc0: 0869 6e74 6572 6e61 6c94 888c 0672 6566  .internal....ref
+00004bd0: 7572 6994 6aee 0200 008c 0a61 6e63 686f  uri.j......ancho
+00004be0: 726e 616d 6594 8c16 2372 756e 2d75 6d62  rname...#run-umb
+00004bf0: 7265 6c6c 612d 7361 6d70 6c69 6e67 9475  rella-sampling.u
+00004c00: 6a62 0300 006a d803 0000 6a55 0300 006a  jb...j....jU...j
+00004c10: 0805 0000 7562 616a 5603 0000 7d94 286a  ....ubajV...}.(j
+00004c20: 6c03 0000 5d94 6a6e 0300 005d 946a 7003  l...].jn...].jp.
+00004c30: 0000 5d94 6a72 0300 005d 946a 7403 0000  ..].jr...].jt...
+00004c40: 5d94 756a 6203 0000 6ad3 0300 006a 5503  ].ujb...j....jU.
+00004c50: 0000 6a05 0500 0075 6261 6a56 0300 007d  ..j....ubajV...}
+00004c60: 9428 6a6c 0300 005d 946a 6e03 0000 5d94  .(jl...].jn...].
+00004c70: 6a70 0300 005d 946a 7203 0000 5d94 6a74  jp...].jr...].jt
+00004c80: 0300 005d 9475 6a62 0300 006a cd03 0000  ...].ujb...j....
+00004c90: 6a55 0300 006a df04 0000 7562 6ace 0300  jU...j....ubj...
+00004ca0: 0029 8194 7d94 286a 4c03 0000 686c 6a4d  .)..}.(jL...hljM
+00004cb0: 0300 005d 946a d403 0000 2981 947d 9428  ...].j....)..}.(
+00004cc0: 6a4c 0300 0068 6c6a 4d03 0000 5d94 6ad9  jL...hljM...].j.
+00004cd0: 0300 0029 8194 7d94 286a 4c03 0000 686c  ...)..}.(jL...hl
+00004ce0: 6a4d 0300 005d 946a 5003 0000 8c31 332e  jM...].jP....13.
+00004cf0: 2043 6f6d 7075 7465 2061 6e64 2063 6f6c   Compute and col
+00004d00: 6c65 6374 2074 6865 2062 7574 616e 6520  lect the butane 
+00004d10: 6469 6865 6472 616c 2076 616c 7565 7394  dihedral values.
+00004d20: 8594 8194 7d94 6a55 0300 006a 2e05 0000  ....}.jU...j....
+00004d30: 7362 616a 5603 0000 7d94 286a 6c03 0000  sbajV...}.(jl...
+00004d40: 5d94 6a6e 0300 005d 946a 7003 0000 5d94  ].jn...].jp...].
+00004d50: 6a72 0300 005d 946a 7403 0000 5d94 8c08  jr...].jt...]...
+00004d60: 696e 7465 726e 616c 9488 8c06 7265 6675  internal....refu
+00004d70: 7269 946a ee02 0000 8c0a 616e 6368 6f72  ri.j......anchor
+00004d80: 6e61 6d65 948c 2f23 636f 6d70 7574 652d  name../#compute-
+00004d90: 616e 642d 636f 6c6c 6563 742d 7468 652d  and-collect-the-
+00004da0: 6275 7461 6e65 2d64 6968 6564 7261 6c2d  butane-dihedral-
+00004db0: 7661 6c75 6573 9475 6a62 0300 006a d803  values.ujb...j..
+00004dc0: 0000 6a55 0300 006a 2b05 0000 7562 616a  ..jU...j+...ubaj
+00004dd0: 5603 0000 7d94 286a 6c03 0000 5d94 6a6e  V...}.(jl...].jn
+00004de0: 0300 005d 946a 7003 0000 5d94 6a72 0300  ...].jp...].jr..
+00004df0: 005d 946a 7403 0000 5d94 756a 6203 0000  .].jt...].ujb...
+00004e00: 6ad3 0300 006a 5503 0000 6a28 0500 0075  j....jU...j(...u
+00004e10: 6261 6a56 0300 007d 9428 6a6c 0300 005d  bajV...}.(jl...]
+00004e20: 946a 6e03 0000 5d94 6a70 0300 005d 946a  .jn...].jp...].j
+00004e30: 7203 0000 5d94 6a74 0300 005d 9475 6a62  r...].jt...].ujb
+00004e40: 0300 006a cd03 0000 6a55 0300 006a df04  ...j....jU...j..
+00004e50: 0000 7562 6ace 0300 0029 8194 7d94 286a  ..ubj....)..}.(j
+00004e60: 4c03 0000 686c 6a4d 0300 005d 946a d403  L...hljM...].j..
+00004e70: 0000 2981 947d 9428 6a4c 0300 0068 6c6a  ..)..}.(jL...hlj
+00004e80: 4d03 0000 5d94 6ad9 0300 0029 8194 7d94  M...].j....)..}.
+00004e90: 286a 4c03 0000 686c 6a4d 0300 005d 946a  (jL...hljM...].j
+00004ea0: 5003 0000 8c41 342e 2055 7365 2046 6173  P....A4. Use Fas
+00004eb0: 744d 4241 5220 746f 2073 6f6c 7665 204d  tMBAR to solve M
+00004ec0: 4241 522f 5557 4841 4d20 6571 7561 7469  BAR/UWHAM equati
+00004ed0: 6f6e 7320 616e 6420 636f 6d70 7574 6520  ons and compute 
+00004ee0: 7468 6520 504d 4694 8594 8194 7d94 6a55  the PMF.....}.jU
+00004ef0: 0300 006a 5105 0000 7362 616a 5603 0000  ...jQ...sbajV...
+00004f00: 7d94 286a 6c03 0000 5d94 6a6e 0300 005d  }.(jl...].jn...]
+00004f10: 946a 7003 0000 5d94 6a72 0300 005d 946a  .jp...].jr...].j
+00004f20: 7403 0000 5d94 8c08 696e 7465 726e 616c  t...]...internal
+00004f30: 9488 8c06 7265 6675 7269 946a ee02 0000  ....refuri.j....
+00004f40: 8c0a 616e 6368 6f72 6e61 6d65 948c 3f23  ..anchorname..?#
+00004f50: 7573 652d 6661 7374 6d62 6172 2d74 6f2d  use-fastmbar-to-
+00004f60: 736f 6c76 652d 6d62 6172 2d75 7768 616d  solve-mbar-uwham
+00004f70: 2d65 7175 6174 696f 6e73 2d61 6e64 2d63  -equations-and-c
+00004f80: 6f6d 7075 7465 2d74 6865 2d70 6d66 9475  ompute-the-pmf.u
+00004f90: 6a62 0300 006a d803 0000 6a55 0300 006a  jb...j....jU...j
+00004fa0: 4e05 0000 7562 616a 5603 0000 7d94 286a  N...ubajV...}.(j
+00004fb0: 6c03 0000 5d94 6a6e 0300 005d 946a 7003  l...].jn...].jp.
+00004fc0: 0000 5d94 6a72 0300 005d 946a 7403 0000  ..].jr...].jt...
+00004fd0: 5d94 756a 6203 0000 6ad3 0300 006a 5503  ].ujb...j....jU.
+00004fe0: 0000 6a4b 0500 0075 6261 6a56 0300 007d  ..jK...ubajV...}
+00004ff0: 9428 6a6c 0300 005d 946a 6e03 0000 5d94  .(jl...].jn...].
+00005000: 6a70 0300 005d 946a 7203 0000 5d94 6a74  jp...].jr...].jt
+00005010: 0300 005d 9475 6a62 0300 006a cd03 0000  ...].ujb...j....
+00005020: 6a55 0300 006a df04 0000 7562 656a 5603  jU...j....ubejV.
+00005030: 0000 7d94 286a 6c03 0000 5d94 6a6e 0300  ..}.(jl...].jn..
+00005040: 005d 946a 7003 0000 5d94 6a72 0300 005d  .].jp...].jr...]
+00005050: 946a 7403 0000 5d94 756a 6203 0000 6ac8  .jt...].ujb...j.
+00005060: 0300 006a 5503 0000 6ac3 0400 0075 6265  ...jU...j....ube
+00005070: 6a56 0300 007d 9428 6a6c 0300 005d 946a  jV...}.(jl...].j
+00005080: 6e03 0000 5d94 6a70 0300 005d 946a 7203  n...].jp...].jr.
+00005090: 0000 5d94 6a74 0300 005d 9475 6a62 0300  ..].jt...].ujb..
+000050a0: 006a cd03 0000 6a55 0300 006a c004 0000  .j....jU...j....
+000050b0: 7562 616a 5603 0000 7d94 286a 6c03 0000  ubajV...}.(jl...
+000050c0: 5d94 6a6e 0300 005d 946a 7003 0000 5d94  ].jn...].jp...].
+000050d0: 6a72 0300 005d 946a 7403 0000 5d94 756a  jr...].jt...].uj
+000050e0: 6203 0000 6ac8 0300 0075 626a e702 0000  b...j....ubj....
+000050f0: 6ac9 0300 0029 8194 7d94 286a 4c03 0000  j....)..}.(jL...
+00005100: 686c 6a4d 0300 005d 946a ce03 0000 2981  hljM...].j....).
+00005110: 947d 9428 6a4c 0300 0068 6c6a 4d03 0000  .}.(jL...hljM...
+00005120: 5d94 286a d403 0000 2981 947d 9428 6a4c  ].(j....)..}.(jL
+00005130: 0300 0068 6c6a 4d03 0000 5d94 6ad9 0300  ...hljM...].j...
+00005140: 0029 8194 7d94 286a 4c03 0000 686c 6a4d  .)..}.(jL...hljM
+00005150: 0300 005d 946a 5003 0000 8c08 4578 616d  ...].jP.....Exam
+00005160: 706c 6573 9485 9481 947d 946a 5503 0000  ples.....}.jU...
+00005170: 6a89 0500 0073 6261 6a56 0300 007d 9428  j....sbajV...}.(
+00005180: 6a6c 0300 005d 946a 6e03 0000 5d94 6a70  jl...].jn...].jp
+00005190: 0300 005d 946a 7203 0000 5d94 6a74 0300  ...].jr...].jt..
+000051a0: 005d 948c 0869 6e74 6572 6e61 6c94 888c  .]...internal...
+000051b0: 0672 6566 7572 6994 6ae7 0200 008c 0a61  .refuri.j......a
+000051c0: 6e63 686f 726e 616d 6594 686c 756a 6203  nchorname.hlujb.
+000051d0: 0000 6ad8 0300 006a 5503 0000 6a86 0500  ..j....jU...j...
+000051e0: 0075 6261 6a56 0300 007d 9428 6a6c 0300  .ubajV...}.(jl..
+000051f0: 005d 946a 6e03 0000 5d94 6a70 0300 005d  .].jn...].jp...]
+00005200: 946a 7203 0000 5d94 6a74 0300 005d 9475  .jr...].jt...].u
+00005210: 6a62 0300 006a d303 0000 6a55 0300 006a  jb...j....jU...j
+00005220: 8305 0000 7562 6ac9 0300 0029 8194 7d94  ....ubj....)..}.
+00005230: 286a 4c03 0000 686c 6a4d 0300 005d 9428  (jL...hljM...].(
+00005240: 6ace 0300 0029 8194 7d94 286a 4c03 0000  j....)..}.(jL...
+00005250: 686c 6a4d 0300 005d 946a d403 0000 2981  hljM...].j....).
+00005260: 947d 9428 6a4c 0300 0068 6c6a 4d03 0000  .}.(jL...hljM...
+00005270: 5d94 6ad9 0300 0029 8194 7d94 286a 4c03  ].j....)..}.(jL.
+00005280: 0000 686c 6a4d 0300 005d 946a 5003 0000  ..hljM...].jP...
+00005290: 8c25 496e 7374 616c 6c20 4578 7472 6120  .%Install Extra 
+000052a0: 5265 7175 6972 6564 2050 7974 686f 6e20  Required Python 
+000052b0: 5061 636b 6765 7394 8594 8194 7d94 6a55  Packges.....}.jU
+000052c0: 0300 006a a805 0000 7362 616a 5603 0000  ...j....sbajV...
+000052d0: 7d94 286a 6c03 0000 5d94 6a6e 0300 005d  }.(jl...].jn...]
+000052e0: 946a 7003 0000 5d94 6a72 0300 005d 946a  .jp...].jr...].j
+000052f0: 7403 0000 5d94 8c08 696e 7465 726e 616c  t...]...internal
+00005300: 9488 8c06 7265 6675 7269 946a e702 0000  ....refuri.j....
+00005310: 8c0a 616e 6368 6f72 6e61 6d65 948c 2623  ..anchorname..&#
+00005320: 696e 7374 616c 6c2d 6578 7472 612d 7265  install-extra-re
+00005330: 7175 6972 6564 2d70 7974 686f 6e2d 7061  quired-python-pa
+00005340: 636b 6765 7394 756a 6203 0000 6ad8 0300  ckges.ujb...j...
+00005350: 006a 5503 0000 6aa5 0500 0075 6261 6a56  .jU...j....ubajV
+00005360: 0300 007d 9428 6a6c 0300 005d 946a 6e03  ...}.(jl...].jn.
+00005370: 0000 5d94 6a70 0300 005d 946a 7203 0000  ..].jp...].jr...
+00005380: 5d94 6a74 0300 005d 9475 6a62 0300 006a  ].jt...].ujb...j
+00005390: d303 0000 6a55 0300 006a a205 0000 7562  ....jU...j....ub
+000053a0: 616a 5603 0000 7d94 286a 6c03 0000 5d94  ajV...}.(jl...].
+000053b0: 6a6e 0300 005d 946a 7003 0000 5d94 6a72  jn...].jp...].jr
+000053c0: 0300 005d 946a 7403 0000 5d94 756a 6203  ...].jt...].ujb.
+000053d0: 0000 6acd 0300 006a 5503 0000 6a9f 0500  ..j....jU...j...
+000053e0: 0075 626a ce03 0000 2981 947d 9428 6a4c  .ubj....)..}.(jL
+000053f0: 0300 0068 6c6a 4d03 0000 5d94 286a d403  ...hljM...].(j..
+00005400: 0000 2981 947d 9428 6a4c 0300 0068 6c6a  ..)..}.(jL...hlj
+00005410: 4d03 0000 5d94 6ad9 0300 0029 8194 7d94  M...].j....)..}.
+00005420: 286a 4c03 0000 686c 6a4d 0300 005d 946a  (jL...hljM...].j
+00005430: 5003 0000 8c08 4578 616d 706c 6573 9485  P.....Examples..
+00005440: 9481 947d 946a 5503 0000 6acb 0500 0073  ...}.jU...j....s
+00005450: 6261 6a56 0300 007d 9428 6a6c 0300 005d  bajV...}.(jl...]
+00005460: 946a 6e03 0000 5d94 6a70 0300 005d 946a  .jn...].jp...].j
+00005470: 7203 0000 5d94 6a74 0300 005d 948c 0869  r...].jt...]...i
+00005480: 6e74 6572 6e61 6c94 888c 0672 6566 7572  nternal....refur
+00005490: 6994 6ae7 0200 008c 0a61 6e63 686f 726e  i.j......anchorn
+000054a0: 616d 6594 8c04 2369 6432 9475 6a62 0300  ame...#id2.ujb..
+000054b0: 006a d803 0000 6a55 0300 006a c805 0000  .j....jU...j....
+000054c0: 7562 616a 5603 0000 7d94 286a 6c03 0000  ubajV...}.(jl...
+000054d0: 5d94 6a6e 0300 005d 946a 7003 0000 5d94  ].jn...].jp...].
+000054e0: 6a72 0300 005d 946a 7403 0000 5d94 756a  jr...].jt...].uj
+000054f0: 6203 0000 6ad3 0300 006a 5503 0000 6ac5  b...j....jU...j.
+00005500: 0500 0075 626a c903 0000 2981 947d 9428  ...ubj....)..}.(
+00005510: 6a4c 0300 0068 6c6a 4d03 0000 5d94 6ad2  jL...hljM...].j.
+00005520: 0300 008c 0774 6f63 7472 6565 9493 9429  .....toctree...)
+00005530: 8194 7d94 286a 4c03 0000 686c 6a4d 0300  ..}.(jL...hljM..
+00005540: 005d 946a 5603 0000 7d94 286a 6c03 0000  .].jV...}.(jl...
+00005550: 5d94 6a6e 0300 005d 946a 7003 0000 5d94  ].jn...].jp...].
+00005560: 6a72 0300 005d 946a 7403 0000 5d94 8c06  jr...].jt...]...
+00005570: 7061 7265 6e74 946a e702 0000 8c07 656e  parent.j......en
+00005580: 7472 6965 7394 5d94 284e 8c0a 6275 7461  tries.].(N..buta
+00005590: 6e65 5f50 4d46 9486 944e 8c0d 6469 616c  ne_PMF...N..dial
+000055a0: 616e 696e 655f 504d 4694 8694 658c 0c69  anine_PMF...e..i
+000055b0: 6e63 6c75 6465 6669 6c65 7394 5d94 286a  ncludefiles.].(j
+000055c0: f305 0000 6af5 0500 0065 8c08 6d61 7864  ....j....e..maxd
+000055d0: 6570 7468 944b 018c 0763 6170 7469 6f6e  epth.K...caption
+000055e0: 944e 8c04 676c 6f62 9489 8c06 6869 6464  .N..glob....hidd
+000055f0: 656e 9489 8c0d 696e 636c 7564 6568 6964  en....includehid
+00005600: 6465 6e94 898c 086e 756d 6265 7265 6494  den....numbered.
+00005610: 4b00 8c0a 7469 746c 6573 6f6e 6c79 9489  K...titlesonly..
+00005620: 8c0a 7261 7765 6e74 7269 6573 945d 9475  ..rawentries.].u
+00005630: 6a62 0300 006a e505 0000 8c06 736f 7572  jb...j......sour
+00005640: 6365 948c 682f 5573 6572 732f 6469 6e67  ce..h/Users/ding
+00005650: 7871 2f4c 6962 7261 7279 2f43 6c6f 7564  xq/Library/Cloud
+00005660: 5374 6f72 6167 652f 426f 782d 426f 782f  Storage/Box-Box/
+00005670: 5265 7365 6172 6368 2f50 726f 6a65 6374  Research/Project
+00005680: 735f 6f6e 5f47 6974 6875 622f 4661 7374  s_on_Github/Fast
+00005690: 4d42 4152 2f64 6f63 732f 736f 7572 6365  MBAR/docs/source
+000056a0: 2f65 7861 6d70 6c65 732e 7273 7494 8c04  /examples.rst...
+000056b0: 6c69 6e65 944b 2e6a 5503 0000 6ae2 0500  line.K.jU...j...
+000056c0: 0075 6261 6a56 0300 007d 9428 6a6c 0300  .ubajV...}.(jl..
+000056d0: 005d 946a 6e03 0000 5d94 6a70 0300 005d  .].jn...].jp...]
+000056e0: 946a 7203 0000 5d94 6a74 0300 005d 9475  .jr...].jt...].u
+000056f0: 6a62 0300 006a c803 0000 6a55 0300 006a  jb...j....jU...j
+00005700: c505 0000 7562 656a 5603 0000 7d94 286a  ....ubejV...}.(j
+00005710: 6c03 0000 5d94 6a6e 0300 005d 946a 7003  l...].jn...].jp.
+00005720: 0000 5d94 6a72 0300 005d 946a 7403 0000  ..].jr...].jt...
+00005730: 5d94 756a 6203 0000 6acd 0300 006a 5503  ].ujb...j....jU.
+00005740: 0000 6a9f 0500 0075 6265 6a56 0300 007d  ..j....ubejV...}
+00005750: 9428 6a6c 0300 005d 946a 6e03 0000 5d94  .(jl...].jn...].
+00005760: 6a70 0300 005d 946a 7203 0000 5d94 6a74  jp...].jr...].jt
+00005770: 0300 005d 9475 6a62 0300 006a c803 0000  ...].ujb...j....
+00005780: 6a55 0300 006a 8305 0000 7562 656a 5603  jU...j....ubejV.
+00005790: 0000 7d94 286a 6c03 0000 5d94 6a6e 0300  ..}.(jl...].jn..
+000057a0: 005d 946a 7003 0000 5d94 6a72 0300 005d  .].jp...].jr...]
+000057b0: 946a 7403 0000 5d94 756a 6203 0000 6acd  .jt...].ujb...j.
+000057c0: 0300 006a 5503 0000 6a80 0500 0075 6261  ...jU...j....uba
+000057d0: 6a56 0300 007d 9428 6a6c 0300 005d 946a  jV...}.(jl...].j
+000057e0: 6e03 0000 5d94 6a70 0300 005d 946a 7203  n...].jp...].jr.
+000057f0: 0000 5d94 6a74 0300 005d 9475 6a62 0300  ..].jt...].ujb..
+00005800: 006a c803 0000 7562 6ae8 0200 006a c903  .j....ubj....j..
+00005810: 0000 2981 947d 9428 6a4c 0300 0068 6c6a  ..)..}.(jL...hlj
+00005820: 4d03 0000 5d94 6ace 0300 0029 8194 7d94  M...].j....)..}.
+00005830: 286a 4c03 0000 686c 6a4d 0300 005d 9428  (jL...hljM...].(
+00005840: 6ad4 0300 0029 8194 7d94 286a 4c03 0000  j....)..}.(jL...
+00005850: 686c 6a4d 0300 005d 946a d903 0000 2981  hljM...].j....).
+00005860: 947d 9428 6a4c 0300 0068 6c6a 4d03 0000  .}.(jL...hljM...
+00005870: 5d94 6a50 0300 008c 1457 656c 636f 6d65  ].jP.....Welcome
+00005880: 2074 6f20 4661 7374 4d42 4152 2194 8594   to FastMBAR!...
+00005890: 8194 7d94 6a55 0300 006a 2c06 0000 7362  ..}.jU...j,...sb
+000058a0: 616a 5603 0000 7d94 286a 6c03 0000 5d94  ajV...}.(jl...].
+000058b0: 6a6e 0300 005d 946a 7003 0000 5d94 6a72  jn...].jp...].jr
+000058c0: 0300 005d 946a 7403 0000 5d94 8c08 696e  ...].jt...]...in
+000058d0: 7465 726e 616c 9488 8c06 7265 6675 7269  ternal....refuri
+000058e0: 946a e802 0000 8c0a 616e 6368 6f72 6e61  .j......anchorna
+000058f0: 6d65 9468 6c75 6a62 0300 006a d803 0000  me.hlujb...j....
+00005900: 6a55 0300 006a 2906 0000 7562 616a 5603  jU...j)...ubajV.
+00005910: 0000 7d94 286a 6c03 0000 5d94 6a6e 0300  ..}.(jl...].jn..
+00005920: 005d 946a 7003 0000 5d94 6a72 0300 005d  .].jp...].jr...]
+00005930: 946a 7403 0000 5d94 756a 6203 0000 6ad3  .jt...].ujb...j.
+00005940: 0300 006a 5503 0000 6a26 0600 0075 626a  ...jU...j&...ubj
+00005950: c903 0000 2981 947d 9428 6a4c 0300 0068  ....)..}.(jL...h
+00005960: 6c6a 4d03 0000 5d94 286a ce03 0000 2981  ljM...].(j....).
+00005970: 947d 9428 6a4c 0300 0068 6c6a 4d03 0000  .}.(jL...hljM...
+00005980: 5d94 6ad4 0300 0029 8194 7d94 286a 4c03  ].j....)..}.(jL.
+00005990: 0000 686c 6a4d 0300 005d 946a d903 0000  ..hljM...].j....
+000059a0: 2981 947d 9428 6a4c 0300 0068 6c6a 4d03  )..}.(jL...hljM.
+000059b0: 0000 5d94 6a50 0300 008c 1157 6861 7420  ..].jP.....What 
+000059c0: 6973 2046 6173 744d 4241 523f 9485 9481  is FastMBAR?....
+000059d0: 947d 946a 5503 0000 6a4b 0600 0073 6261  .}.jU...jK...sba
+000059e0: 6a56 0300 007d 9428 6a6c 0300 005d 946a  jV...}.(jl...].j
+000059f0: 6e03 0000 5d94 6a70 0300 005d 946a 7203  n...].jp...].jr.
+00005a00: 0000 5d94 6a74 0300 005d 948c 0869 6e74  ..].jt...]...int
+00005a10: 6572 6e61 6c94 888c 0672 6566 7572 6994  ernal....refuri.
+00005a20: 6ae8 0200 008c 0a61 6e63 686f 726e 616d  j......anchornam
+00005a30: 6594 8c11 2377 6861 742d 6973 2d66 6173  e...#what-is-fas
+00005a40: 746d 6261 7294 756a 6203 0000 6ad8 0300  tmbar.ujb...j...
+00005a50: 006a 5503 0000 6a48 0600 0075 6261 6a56  .jU...jH...ubajV
+00005a60: 0300 007d 9428 6a6c 0300 005d 946a 6e03  ...}.(jl...].jn.
+00005a70: 0000 5d94 6a70 0300 005d 946a 7203 0000  ..].jp...].jr...
+00005a80: 5d94 6a74 0300 005d 9475 6a62 0300 006a  ].jt...].ujb...j
+00005a90: d303 0000 6a55 0300 006a 4506 0000 7562  ....jU...jE...ub
+00005aa0: 616a 5603 0000 7d94 286a 6c03 0000 5d94  ajV...}.(jl...].
+00005ab0: 6a6e 0300 005d 946a 7003 0000 5d94 6a72  jn...].jp...].jr
+00005ac0: 0300 005d 946a 7403 0000 5d94 756a 6203  ...].jt...].ujb.
+00005ad0: 0000 6acd 0300 006a 5503 0000 6a42 0600  ..j....jU...jB..
+00005ae0: 0075 626a ce03 0000 2981 947d 9428 6a4c  .ubj....)..}.(jL
+00005af0: 0300 0068 6c6a 4d03 0000 5d94 6ad4 0300  ...hljM...].j...
+00005b00: 0029 8194 7d94 286a 4c03 0000 686c 6a4d  .)..}.(jL...hljM
 00005b10: 0300 005d 946a d903 0000 2981 947d 9428  ...].j....)..}.(
-00005b20: 6a51 0300 0068 6c6a 5203 0000 5d94 6ade  jQ...hljR...].j.
-00005b30: 0300 0029 8194 7d94 286a 5103 0000 686c  ...)..}.(jQ...hl
-00005b40: 6a52 0300 005d 946a 5503 0000 8c0d 5768  jR...].jU.....Wh
-00005b50: 7920 4661 7374 4d42 4152 3f94 8594 8194  y FastMBAR?.....
-00005b60: 7d94 6a5a 0300 006a 7406 0000 7362 616a  }.jZ...jt...sbaj
-00005b70: 5b03 0000 7d94 286a 5d03 0000 5d94 6a5f  [...}.(j]...].j_
-00005b80: 0300 005d 946a 6103 0000 5d94 6a63 0300  ...].ja...].jc..
-00005b90: 005d 946a 6503 0000 5d94 8c08 696e 7465  .].je...]...inte
-00005ba0: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
-00005bb0: 2003 0000 8c0a 616e 6368 6f72 6e61 6d65   .....anchorname
-00005bc0: 948c 0d23 7768 792d 6661 7374 6d62 6172  ...#why-fastmbar
-00005bd0: 9475 6a67 0300 006a ef03 0000 6a5a 0300  .ujg...j....jZ..
-00005be0: 006a 7106 0000 7562 616a 5b03 0000 7d94  .jq...ubaj[...}.
-00005bf0: 286a 5d03 0000 5d94 6a5f 0300 005d 946a  (j]...].j_...].j
-00005c00: 6103 0000 5d94 6a63 0300 005d 946a 6503  a...].jc...].je.
-00005c10: 0000 5d94 756a 6703 0000 6af6 0300 006a  ..].ujg...j....j
-00005c20: 5a03 0000 6a6e 0600 0075 6261 6a5b 0300  Z...jn...ubaj[..
-00005c30: 007d 9428 6a5d 0300 005d 946a 5f03 0000  .}.(j]...].j_...
-00005c40: 5d94 6a61 0300 005d 946a 6303 0000 5d94  ].ja...].jc...].
-00005c50: 6a65 0300 005d 9475 6a67 0300 006a fd03  je...].ujg...j..
-00005c60: 0000 6a5a 0300 006a 4806 0000 7562 6ad3  ..jZ...jH...ubj.
-00005c70: 0300 0029 8194 7d94 286a 5103 0000 686c  ...)..}.(jQ...hl
-00005c80: 6a52 0300 005d 9428 6ad9 0300 0029 8194  jR...].(j....)..
-00005c90: 7d94 286a 5103 0000 686c 6a52 0300 005d  }.(jQ...hljR...]
-00005ca0: 946a de03 0000 2981 947d 9428 6a51 0300  .j....)..}.(jQ..
-00005cb0: 0068 6c6a 5203 0000 5d94 6a55 0300 008c  .hljR...].jU....
-00005cc0: 1448 6f77 2074 6f20 7573 6520 4661 7374  .How to use Fast
-00005cd0: 4d42 4152 3f94 8594 8194 7d94 6a5a 0300  MBAR?.....}.jZ..
-00005ce0: 006a 9706 0000 7362 616a 5b03 0000 7d94  .j....sbaj[...}.
-00005cf0: 286a 5d03 0000 5d94 6a5f 0300 005d 946a  (j]...].j_...].j
-00005d00: 6103 0000 5d94 6a63 0300 005d 946a 6503  a...].jc...].je.
-00005d10: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
-00005d20: 8c06 7265 6675 7269 946a 2003 0000 8c0a  ..refuri.j .....
-00005d30: 616e 6368 6f72 6e61 6d65 948c 1423 686f  anchorname...#ho
-00005d40: 772d 746f 2d75 7365 2d66 6173 746d 6261  w-to-use-fastmba
-00005d50: 7294 756a 6703 0000 6aef 0300 006a 5a03  r.ujg...j....jZ.
-00005d60: 0000 6a94 0600 0075 6261 6a5b 0300 007d  ..j....ubaj[...}
-00005d70: 9428 6a5d 0300 005d 946a 5f03 0000 5d94  .(j]...].j_...].
-00005d80: 6a61 0300 005d 946a 6303 0000 5d94 6a65  ja...].jc...].je
-00005d90: 0300 005d 9475 6a67 0300 006a f603 0000  ...].ujg...j....
-00005da0: 6a5a 0300 006a 9106 0000 7562 6ace 0300  jZ...j....ubj...
-00005db0: 0029 8194 7d94 286a 5103 0000 686c 6a52  .)..}.(jQ...hljR
-00005dc0: 0300 005d 946a eb05 0000 2981 947d 9428  ...].j....)..}.(
-00005dd0: 6a51 0300 0068 6c6a 5203 0000 5d94 6a5b  jQ...hljR...].j[
-00005de0: 0300 007d 9428 6a5d 0300 005d 946a 5f03  ...}.(j]...].j_.
-00005df0: 0000 5d94 6a61 0300 005d 946a 6303 0000  ..].ja...].jc...
-00005e00: 5d94 6a65 0300 005d 948c 0670 6172 656e  ].je...]...paren
-00005e10: 7494 6a20 0300 008c 0765 6e74 7269 6573  t.j .....entries
-00005e20: 945d 9428 4e8c 0c69 6e73 7461 6c6c 6174  .].(N..installat
-00005e30: 696f 6e94 8694 4e8c 0575 7361 6765 9486  ion...N..usage..
-00005e40: 944e 8c03 4150 4994 8694 4e8c 0865 7861  .N..API...N..exa
-00005e50: 6d70 6c65 7394 8694 4e8c 0a72 6566 6572  mples...N..refer
-00005e60: 656e 6365 7394 8694 658c 0c69 6e63 6c75  ences...e..inclu
-00005e70: 6465 6669 6c65 7394 5d94 286a bd06 0000  defiles.].(j....
-00005e80: 6abf 0600 006a c106 0000 6ac3 0600 006a  j....j....j....j
-00005e90: c506 0000 658c 086d 6178 6465 7074 6894  ....e..maxdepth.
-00005ea0: 4b02 8c07 6361 7074 696f 6e94 4e8c 0467  K...caption.N..g
-00005eb0: 6c6f 6294 898c 0668 6964 6465 6e94 898c  lob....hidden...
-00005ec0: 0d69 6e63 6c75 6465 6869 6464 656e 9489  .includehidden..
-00005ed0: 8c08 6e75 6d62 6572 6564 944b 008c 0a74  ..numbered.K...t
-00005ee0: 6974 6c65 736f 6e6c 7994 898c 0a72 6177  itlesonly....raw
-00005ef0: 656e 7472 6965 7394 5d94 756a 6703 0000  entries.].ujg...
-00005f00: 6a07 0600 006a 0806 0000 8c65 2f55 7365  j....j.....e/Use
-00005f10: 7273 2f64 696e 6778 712f 4c69 6272 6172  rs/dingxq/Librar
-00005f20: 792f 436c 6f75 6453 746f 7261 6765 2f42  y/CloudStorage/B
-00005f30: 6f78 2d42 6f78 2f52 6573 6561 7263 682f  ox-Box/Research/
-00005f40: 5072 6f6a 6563 7473 5f6f 6e5f 4769 7468  Projects_on_Gith
-00005f50: 7562 2f46 6173 744d 4241 522f 646f 6373  ub/FastMBAR/docs
-00005f60: 2f73 6f75 7263 652f 696e 6465 782e 7273  /source/index.rs
-00005f70: 7494 6a0a 0600 004b 206a 5a03 0000 6aae  t.j....K jZ...j.
-00005f80: 0600 0075 6261 6a5b 0300 007d 9428 6a5d  ...ubaj[...}.(j]
-00005f90: 0300 005d 946a 5f03 0000 5d94 6a61 0300  ...].j_...].ja..
-00005fa0: 005d 946a 6303 0000 5d94 6a65 0300 005d  .].jc...].je...]
-00005fb0: 9475 6a67 0300 006a 0404 0000 6a5a 0300  .ujg...j....jZ..
-00005fc0: 006a 9106 0000 7562 656a 5b03 0000 7d94  .j....ubej[...}.
-00005fd0: 286a 5d03 0000 5d94 6a5f 0300 005d 946a  (j]...].j_...].j
-00005fe0: 6103 0000 5d94 6a63 0300 005d 946a 6503  a...].jc...].je.
-00005ff0: 0000 5d94 756a 6703 0000 6afd 0300 006a  ..].ujg...j....j
-00006000: 5a03 0000 6a48 0600 0075 6265 6a5b 0300  Z...jH...ubej[..
-00006010: 007d 9428 6a5d 0300 005d 946a 5f03 0000  .}.(j]...].j_...
-00006020: 5d94 6a61 0300 005d 946a 6303 0000 5d94  ].ja...].jc...].
-00006030: 6a65 0300 005d 9475 6a67 0300 006a 0404  je...].ujg...j..
-00006040: 0000 6a5a 0300 006a 2c06 0000 7562 656a  ..jZ...j,...ubej
-00006050: 5b03 0000 7d94 286a 5d03 0000 5d94 6a5f  [...}.(j]...].j_
-00006060: 0300 005d 946a 6103 0000 5d94 6a63 0300  ...].ja...].jc..
-00006070: 005d 946a 6503 0000 5d94 756a 6703 0000  .].je...].ujg...
-00006080: 6afd 0300 006a 5a03 0000 6a29 0600 0075  j....jZ...j)...u
-00006090: 6261 6a5b 0300 007d 9428 6a5d 0300 005d  baj[...}.(j]...]
-000060a0: 946a 5f03 0000 5d94 6a61 0300 005d 946a  .j_...].ja...].j
-000060b0: 6303 0000 5d94 6a65 0300 005d 9475 6a67  c...].je...].ujg
-000060c0: 0300 006a 0404 0000 7562 6a21 0300 006a  ...j....ubj!...j
-000060d0: ce03 0000 2981 947d 9428 6a51 0300 0068  ....)..}.(jQ...h
-000060e0: 6c6a 5203 0000 5d94 6ad3 0300 0029 8194  ljR...].j....)..
-000060f0: 7d94 286a 5103 0000 686c 6a52 0300 005d  }.(jQ...hljR...]
-00006100: 946a d903 0000 2981 947d 9428 6a51 0300  .j....)..}.(jQ..
-00006110: 0068 6c6a 5203 0000 5d94 6ade 0300 0029  .hljR...].j....)
-00006120: 8194 7d94 286a 5103 0000 686c 6a52 0300  ..}.(jQ...hljR..
-00006130: 005d 946a 5503 0000 8c0a 5265 6665 7265  .].jU.....Refere
-00006140: 6e63 6573 9485 9481 947d 946a 5a03 0000  nces.....}.jZ...
-00006150: 6afa 0600 0073 6261 6a5b 0300 007d 9428  j....sbaj[...}.(
-00006160: 6a5d 0300 005d 946a 5f03 0000 5d94 6a61  j]...].j_...].ja
-00006170: 0300 005d 946a 6303 0000 5d94 6a65 0300  ...].jc...].je..
-00006180: 005d 948c 0869 6e74 6572 6e61 6c94 888c  .]...internal...
-00006190: 0672 6566 7572 6994 6a21 0300 008c 0a61  .refuri.j!.....a
-000061a0: 6e63 686f 726e 616d 6594 686c 756a 6703  nchorname.hlujg.
-000061b0: 0000 6aef 0300 006a 5a03 0000 6af7 0600  ..j....jZ...j...
-000061c0: 0075 6261 6a5b 0300 007d 9428 6a5d 0300  .ubaj[...}.(j]..
-000061d0: 005d 946a 5f03 0000 5d94 6a61 0300 005d  .].j_...].ja...]
-000061e0: 946a 6303 0000 5d94 6a65 0300 005d 9475  .jc...].je...].u
-000061f0: 6a67 0300 006a f603 0000 6a5a 0300 006a  jg...j....jZ...j
-00006200: f406 0000 7562 616a 5b03 0000 7d94 286a  ....ubaj[...}.(j
-00006210: 5d03 0000 5d94 6a5f 0300 005d 946a 6103  ]...].j_...].ja.
-00006220: 0000 5d94 6a63 0300 005d 946a 6503 0000  ..].jc...].je...
-00006230: 5d94 756a 6703 0000 6afd 0300 006a 5a03  ].ujg...j....jZ.
-00006240: 0000 6af1 0600 0075 6261 6a5b 0300 007d  ..j....ubaj[...}
-00006250: 9428 6a5d 0300 005d 946a 5f03 0000 5d94  .(j]...].j_...].
-00006260: 6a61 0300 005d 946a 6303 0000 5d94 6a65  ja...].jc...].je
-00006270: 0300 005d 9475 6a67 0300 006a 0404 0000  ...].ujg...j....
-00006280: 7562 6a22 0300 006a ce03 0000 2981 947d  ubj"...j....)..}
-00006290: 9428 6a51 0300 0068 6c6a 5203 0000 5d94  .(jQ...hljR...].
-000062a0: 6ad3 0300 0029 8194 7d94 286a 5103 0000  j....)..}.(jQ...
-000062b0: 686c 6a52 0300 005d 9428 6ad9 0300 0029  hljR...].(j....)
-000062c0: 8194 7d94 286a 5103 0000 686c 6a52 0300  ..}.(jQ...hljR..
-000062d0: 005d 946a de03 0000 2981 947d 9428 6a51  .].j....)..}.(jQ
-000062e0: 0300 0068 6c6a 5203 0000 5d94 6a55 0300  ...hljR...].jU..
-000062f0: 008c 0555 7361 6765 9485 9481 947d 946a  ...Usage.....}.j
-00006300: 5a03 0000 6a25 0700 0073 6261 6a5b 0300  Z...j%...sbaj[..
-00006310: 007d 9428 6a5d 0300 005d 946a 5f03 0000  .}.(j]...].j_...
-00006320: 5d94 6a61 0300 005d 946a 6303 0000 5d94  ].ja...].jc...].
-00006330: 6a65 0300 005d 948c 0869 6e74 6572 6e61  je...]...interna
-00006340: 6c94 888c 0672 6566 7572 6994 6a22 0300  l....refuri.j"..
-00006350: 008c 0a61 6e63 686f 726e 616d 6594 686c  ...anchorname.hl
-00006360: 756a 6703 0000 6aef 0300 006a 5a03 0000  ujg...j....jZ...
-00006370: 6a22 0700 0075 6261 6a5b 0300 007d 9428  j"...ubaj[...}.(
-00006380: 6a5d 0300 005d 946a 5f03 0000 5d94 6a61  j]...].j_...].ja
-00006390: 0300 005d 946a 6303 0000 5d94 6a65 0300  ...].jc...].je..
-000063a0: 005d 9475 6a67 0300 006a f603 0000 6a5a  .].ujg...j....jZ
-000063b0: 0300 006a 1f07 0000 7562 6ace 0300 0029  ...j....ubj....)
-000063c0: 8194 7d94 286a 5103 0000 686c 6a52 0300  ..}.(jQ...hljR..
-000063d0: 005d 9428 6ad3 0300 0029 8194 7d94 286a  .].(j....)..}.(j
-000063e0: 5103 0000 686c 6a52 0300 005d 946a d903  Q...hljR...].j..
-000063f0: 0000 2981 947d 9428 6a51 0300 0068 6c6a  ..)..}.(jQ...hlj
-00006400: 5203 0000 5d94 6ade 0300 0029 8194 7d94  R...].j....)..}.
-00006410: 286a 5103 0000 686c 6a52 0300 005d 946a  (jQ...hljR...].j
-00006420: 5503 0000 8c1e 312e 2057 6865 6e20 746f  U.....1. When to
-00006430: 2075 7365 204d 4241 5220 6571 7561 7469   use MBAR equati
-00006440: 6f6e 733f 9485 9481 947d 946a 5a03 0000  ons?.....}.jZ...
-00006450: 6a44 0700 0073 6261 6a5b 0300 007d 9428  jD...sbaj[...}.(
-00006460: 6a5d 0300 005d 946a 5f03 0000 5d94 6a61  j]...].j_...].ja
-00006470: 0300 005d 946a 6303 0000 5d94 6a65 0300  ...].jc...].je..
-00006480: 005d 948c 0869 6e74 6572 6e61 6c94 888c  .]...internal...
-00006490: 0672 6566 7572 6994 6a22 0300 008c 0a61  .refuri.j".....a
-000064a0: 6e63 686f 726e 616d 6594 8c1b 2377 6865  nchorname...#whe
-000064b0: 6e2d 746f 2d75 7365 2d6d 6261 722d 6571  n-to-use-mbar-eq
-000064c0: 7561 7469 6f6e 7394 756a 6703 0000 6aef  uations.ujg...j.
-000064d0: 0300 006a 5a03 0000 6a41 0700 0075 6261  ...jZ...jA...uba
-000064e0: 6a5b 0300 007d 9428 6a5d 0300 005d 946a  j[...}.(j]...].j
-000064f0: 5f03 0000 5d94 6a61 0300 005d 946a 6303  _...].ja...].jc.
-00006500: 0000 5d94 6a65 0300 005d 9475 6a67 0300  ..].je...].ujg..
-00006510: 006a f603 0000 6a5a 0300 006a 3e07 0000  .j....jZ...j>...
-00006520: 7562 616a 5b03 0000 7d94 286a 5d03 0000  ubaj[...}.(j]...
-00006530: 5d94 6a5f 0300 005d 946a 6103 0000 5d94  ].j_...].ja...].
-00006540: 6a63 0300 005d 946a 6503 0000 5d94 756a  jc...].je...].uj
-00006550: 6703 0000 6afd 0300 006a 5a03 0000 6a3b  g...j....jZ...j;
-00006560: 0700 0075 626a d303 0000 2981 947d 9428  ...ubj....)..}.(
-00006570: 6a51 0300 0068 6c6a 5203 0000 5d94 6ad9  jQ...hljR...].j.
-00006580: 0300 0029 8194 7d94 286a 5103 0000 686c  ...)..}.(jQ...hl
-00006590: 6a52 0300 005d 946a de03 0000 2981 947d  jR...].j....)..}
-000065a0: 9428 6a51 0300 0068 6c6a 5203 0000 5d94  .(jQ...hljR...].
-000065b0: 6a55 0300 008c 1732 2e20 486f 7720 746f  jU.....2. How to
-000065c0: 2075 7365 2046 6173 744d 4241 523f 9485   use FastMBAR?..
-000065d0: 9481 947d 946a 5a03 0000 6a67 0700 0073  ...}.jZ...jg...s
-000065e0: 6261 6a5b 0300 007d 9428 6a5d 0300 005d  baj[...}.(j]...]
-000065f0: 946a 5f03 0000 5d94 6a61 0300 005d 946a  .j_...].ja...].j
-00006600: 6303 0000 5d94 6a65 0300 005d 948c 0869  c...].je...]...i
-00006610: 6e74 6572 6e61 6c94 888c 0672 6566 7572  nternal....refur
-00006620: 6994 6a22 0300 008c 0a61 6e63 686f 726e  i.j".....anchorn
-00006630: 616d 6594 8c14 2368 6f77 2d74 6f2d 7573  ame...#how-to-us
-00006640: 652d 6661 7374 6d62 6172 9475 6a67 0300  e-fastmbar.ujg..
-00006650: 006a ef03 0000 6a5a 0300 006a 6407 0000  .j....jZ...jd...
-00006660: 7562 616a 5b03 0000 7d94 286a 5d03 0000  ubaj[...}.(j]...
-00006670: 5d94 6a5f 0300 005d 946a 6103 0000 5d94  ].j_...].ja...].
-00006680: 6a63 0300 005d 946a 6503 0000 5d94 756a  jc...].je...].uj
-00006690: 6703 0000 6af6 0300 006a 5a03 0000 6a61  g...j....jZ...ja
-000066a0: 0700 0075 6261 6a5b 0300 007d 9428 6a5d  ...ubaj[...}.(j]
-000066b0: 0300 005d 946a 5f03 0000 5d94 6a61 0300  ...].j_...].ja..
-000066c0: 005d 946a 6303 0000 5d94 6a65 0300 005d  .].jc...].je...]
-000066d0: 9475 6a67 0300 006a fd03 0000 6a5a 0300  .ujg...j....jZ..
-000066e0: 006a 3b07 0000 7562 656a 5b03 0000 7d94  .j;...ubej[...}.
-000066f0: 286a 5d03 0000 5d94 6a5f 0300 005d 946a  (j]...].j_...].j
-00006700: 6103 0000 5d94 6a63 0300 005d 946a 6503  a...].jc...].je.
-00006710: 0000 5d94 756a 6703 0000 6a04 0400 006a  ..].ujg...j....j
-00006720: 5a03 0000 6a1f 0700 0075 6265 6a5b 0300  Z...j....ubej[..
-00006730: 007d 9428 6a5d 0300 005d 946a 5f03 0000  .}.(j]...].j_...
-00006740: 5d94 6a61 0300 005d 946a 6303 0000 5d94  ].ja...].jc...].
-00006750: 6a65 0300 005d 9475 6a67 0300 006a fd03  je...].ujg...j..
-00006760: 0000 6a5a 0300 006a 1c07 0000 7562 616a  ..jZ...j....ubaj
-00006770: 5b03 0000 7d94 286a 5d03 0000 5d94 6a5f  [...}.(j]...].j_
-00006780: 0300 005d 946a 6103 0000 5d94 6a63 0300  ...].ja...].jc..
-00006790: 005d 946a 6503 0000 5d94 756a 6703 0000  .].je...].ujg...
-000067a0: 6a04 0400 0075 626a e702 0000 6ace 0300  j....ubj....j...
-000067b0: 0029 8194 7d94 286a 5103 0000 686c 6a52  .)..}.(jQ...hljR
-000067c0: 0300 005d 946a d303 0000 2981 947d 9428  ...].j....)..}.(
-000067d0: 6a51 0300 0068 6c6a 5203 0000 5d94 286a  jQ...hljR...].(j
-000067e0: d903 0000 2981 947d 9428 6a51 0300 0068  ....)..}.(jQ...h
-000067f0: 6c6a 5203 0000 5d94 6ade 0300 0029 8194  ljR...].j....)..
-00006800: 7d94 286a 5103 0000 686c 6a52 0300 005d  }.(jQ...hljR...]
-00006810: 946a 5503 0000 8c0c 496e 7374 616c 6c61  .jU.....Installa
-00006820: 7469 6f6e 9485 9481 947d 946a 5a03 0000  tion.....}.jZ...
-00006830: 6a9f 0700 0073 6261 6a5b 0300 007d 9428  j....sbaj[...}.(
-00006840: 6abf 0300 005d 946a c103 0000 5d94 6ac3  j....].j....].j.
-00006850: 0300 005d 946a c503 0000 5d94 6ac7 0300  ...].j....].j...
-00006860: 005d 948c 0869 6e74 6572 6e61 6c94 888c  .]...internal...
-00006870: 0672 6566 7572 6994 6ae7 0200 008c 0a61  .refuri.j......a
-00006880: 6e63 686f 726e 616d 6594 686c 756a 6703  nchorname.hlujg.
-00006890: 0000 6add 0300 006a 5a03 0000 6a9c 0700  ..j....jZ...j...
-000068a0: 0075 6261 6a5b 0300 007d 9428 6abf 0300  .ubaj[...}.(j...
-000068b0: 005d 946a c103 0000 5d94 6ac3 0300 005d  .].j....].j....]
-000068c0: 946a c503 0000 5d94 6ac7 0300 005d 9475  .j....].j....].u
-000068d0: 6a67 0300 006a d803 0000 6a5a 0300 006a  jg...j....jZ...j
-000068e0: 9907 0000 7562 6ace 0300 0029 8194 7d94  ....ubj....)..}.
-000068f0: 286a 5103 0000 686c 6a52 0300 005d 9428  (jQ...hljR...].(
-00006900: 6ad3 0300 0029 8194 7d94 286a 5103 0000  j....)..}.(jQ...
-00006910: 686c 6a52 0300 005d 946a d903 0000 2981  hljR...].j....).
-00006920: 947d 9428 6a51 0300 0068 6c6a 5203 0000  .}.(jQ...hljR...
-00006930: 5d94 6ade 0300 0029 8194 7d94 286a 5103  ].j....)..}.(jQ.
-00006940: 0000 686c 6a52 0300 005d 946a 5503 0000  ..hljR...].jU...
-00006950: 8c1d 312e 204e 6577 2074 6f20 5079 7468  ..1. New to Pyth
-00006960: 6f6e 206f 7220 416e 6163 6f6e 6461 3f94  on or Anaconda?.
-00006970: 8594 8194 7d94 6a5a 0300 006a be07 0000  ....}.jZ...j....
-00006980: 7362 616a 5b03 0000 7d94 286a bf03 0000  sbaj[...}.(j....
-00006990: 5d94 6ac1 0300 005d 946a c303 0000 5d94  ].j....].j....].
-000069a0: 6ac5 0300 005d 946a c703 0000 5d94 8c08  j....].j....]...
-000069b0: 696e 7465 726e 616c 9488 8c06 7265 6675  internal....refu
-000069c0: 7269 946a e702 0000 8c0a 616e 6368 6f72  ri.j......anchor
-000069d0: 6e61 6d65 948c 1a23 6e65 772d 746f 2d70  name...#new-to-p
-000069e0: 7974 686f 6e2d 6f72 2d61 6e61 636f 6e64  ython-or-anacond
-000069f0: 6194 756a 6703 0000 6add 0300 006a 5a03  a.ujg...j....jZ.
-00006a00: 0000 6abb 0700 0075 6261 6a5b 0300 007d  ..j....ubaj[...}
-00006a10: 9428 6abf 0300 005d 946a c103 0000 5d94  .(j....].j....].
-00006a20: 6ac3 0300 005d 946a c503 0000 5d94 6ac7  j....].j....].j.
-00006a30: 0300 005d 9475 6a67 0300 006a d803 0000  ...].ujg...j....
-00006a40: 6a5a 0300 006a b807 0000 7562 616a 5b03  jZ...j....ubaj[.
-00006a50: 0000 7d94 286a bf03 0000 5d94 6ac1 0300  ..}.(j....].j...
-00006a60: 005d 946a c303 0000 5d94 6ac5 0300 005d  .].j....].j....]
-00006a70: 946a c703 0000 5d94 756a 6703 0000 6ad2  .j....].ujg...j.
-00006a80: 0300 006a 5a03 0000 6ab5 0700 0075 626a  ...jZ...j....ubj
-00006a90: d303 0000 2981 947d 9428 6a51 0300 0068  ....)..}.(jQ...h
-00006aa0: 6c6a 5203 0000 5d94 6ad9 0300 0029 8194  ljR...].j....)..
-00006ab0: 7d94 286a 5103 0000 686c 6a52 0300 005d  }.(jQ...hljR...]
-00006ac0: 946a de03 0000 2981 947d 9428 6a51 0300  .j....)..}.(jQ..
-00006ad0: 0068 6c6a 5203 0000 5d94 6a55 0300 008c  .hljR...].jU....
-00006ae0: 1c32 2e20 496e 7374 616c 6c20 4661 7374  .2. Install Fast
-00006af0: 4d42 4152 2077 6974 6820 7069 7094 8594  MBAR with pip...
-00006b00: 8194 7d94 6a5a 0300 006a e107 0000 7362  ..}.jZ...j....sb
-00006b10: 616a 5b03 0000 7d94 286a bf03 0000 5d94  aj[...}.(j....].
-00006b20: 6ac1 0300 005d 946a c303 0000 5d94 6ac5  j....].j....].j.
-00006b30: 0300 005d 946a c703 0000 5d94 8c08 696e  ...].j....]...in
-00006b40: 7465 726e 616c 9488 8c06 7265 6675 7269  ternal....refuri
-00006b50: 946a e702 0000 8c0a 616e 6368 6f72 6e61  .j......anchorna
-00006b60: 6d65 948c 1a23 696e 7374 616c 6c2d 6661  me...#install-fa
-00006b70: 7374 6d62 6172 2d77 6974 682d 7069 7094  stmbar-with-pip.
-00006b80: 756a 6703 0000 6add 0300 006a 5a03 0000  ujg...j....jZ...
-00006b90: 6ade 0700 0075 6261 6a5b 0300 007d 9428  j....ubaj[...}.(
-00006ba0: 6abf 0300 005d 946a c103 0000 5d94 6ac3  j....].j....].j.
-00006bb0: 0300 005d 946a c503 0000 5d94 6ac7 0300  ...].j....].j...
-00006bc0: 005d 9475 6a67 0300 006a d803 0000 6a5a  .].ujg...j....jZ
-00006bd0: 0300 006a db07 0000 7562 616a 5b03 0000  ...j....ubaj[...
-00006be0: 7d94 286a bf03 0000 5d94 6ac1 0300 005d  }.(j....].j....]
-00006bf0: 946a c303 0000 5d94 6ac5 0300 005d 946a  .j....].j....].j
-00006c00: c703 0000 5d94 756a 6703 0000 6ad2 0300  ....].ujg...j...
-00006c10: 006a 5a03 0000 6ab5 0700 0075 626a d303  .jZ...j....ubj..
-00006c20: 0000 2981 947d 9428 6a51 0300 0068 6c6a  ..)..}.(jQ...hlj
-00006c30: 5203 0000 5d94 6ad9 0300 0029 8194 7d94  R...].j....)..}.
-00006c40: 286a 5103 0000 686c 6a52 0300 005d 946a  (jQ...hljR...].j
-00006c50: de03 0000 2981 947d 9428 6a51 0300 0068  ....)..}.(jQ...h
-00006c60: 6c6a 5203 0000 5d94 6a55 0300 008c 2433  ljR...].jU....$3
-00006c70: 2e20 5465 7374 2074 6865 2049 6e73 7461  . Test the Insta
-00006c80: 6c6c 6174 696f 6e20 6f66 2046 6173 744d  llation of FastM
-00006c90: 4241 5294 8594 8194 7d94 6a5a 0300 006a  BAR.....}.jZ...j
-00006ca0: 0408 0000 7362 616a 5b03 0000 7d94 286a  ....sbaj[...}.(j
-00006cb0: bf03 0000 5d94 6ac1 0300 005d 946a c303  ....].j....].j..
-00006cc0: 0000 5d94 6ac5 0300 005d 946a c703 0000  ..].j....].j....
-00006cd0: 5d94 8c08 696e 7465 726e 616c 9488 8c06  ]...internal....
-00006ce0: 7265 6675 7269 946a e702 0000 8c0a 616e  refuri.j......an
-00006cf0: 6368 6f72 6e61 6d65 948c 2223 7465 7374  chorname.."#test
-00006d00: 2d74 6865 2d69 6e73 7461 6c6c 6174 696f  -the-installatio
-00006d10: 6e2d 6f66 2d66 6173 746d 6261 7294 756a  n-of-fastmbar.uj
-00006d20: 6703 0000 6add 0300 006a 5a03 0000 6a01  g...j....jZ...j.
-00006d30: 0800 0075 6261 6a5b 0300 007d 9428 6abf  ...ubaj[...}.(j.
-00006d40: 0300 005d 946a c103 0000 5d94 6ac3 0300  ...].j....].j...
-00006d50: 005d 946a c503 0000 5d94 6ac7 0300 005d  .].j....].j....]
-00006d60: 9475 6a67 0300 006a d803 0000 6a5a 0300  .ujg...j....jZ..
-00006d70: 006a fe07 0000 7562 616a 5b03 0000 7d94  .j....ubaj[...}.
-00006d80: 286a bf03 0000 5d94 6ac1 0300 005d 946a  (j....].j....].j
-00006d90: c303 0000 5d94 6ac5 0300 005d 946a c703  ....].j....].j..
-00006da0: 0000 5d94 756a 6703 0000 6ad2 0300 006a  ..].ujg...j....j
-00006db0: 5a03 0000 6ab5 0700 0075 6265 6a5b 0300  Z...j....ubej[..
-00006dc0: 007d 9428 6abf 0300 005d 946a c103 0000  .}.(j....].j....
-00006dd0: 5d94 6ac3 0300 005d 946a c503 0000 5d94  ].j....].j....].
-00006de0: 6ac7 0300 005d 9475 6a67 0300 006a cd03  j....].ujg...j..
-00006df0: 0000 6a5a 0300 006a 9907 0000 7562 656a  ..jZ...j....ubej
-00006e00: 5b03 0000 7d94 286a bf03 0000 5d94 6ac1  [...}.(j....].j.
-00006e10: 0300 005d 946a c303 0000 5d94 6ac5 0300  ...].j....].j...
-00006e20: 005d 946a c703 0000 5d94 756a 6703 0000  .].j....].ujg...
-00006e30: 6ad2 0300 006a 5a03 0000 6a96 0700 0075  j....jZ...j....u
-00006e40: 6261 6a5b 0300 007d 9428 6abf 0300 005d  baj[...}.(j....]
-00006e50: 946a c103 0000 5d94 6ac3 0300 005d 946a  .j....].j....].j
-00006e60: c503 0000 5d94 6ac7 0300 005d 9475 6a67  ....].j....].ujg
-00006e70: 0300 006a cd03 0000 7562 758c 0f74 6f63  ...j....ubu..toc
-00006e80: 5f6e 756d 5f65 6e74 7269 6573 947d 9428  _num_entries.}.(
-00006e90: 6a1c 0300 004b 016a 1d03 0000 4b05 6a1e  j....K.j....K.j.
-00006ea0: 0300 004b 056a 1f03 0000 4b03 6a20 0300  ...K.j....K.j ..
-00006eb0: 004b 046a 2103 0000 4b01 6a22 0300 004b  .K.j!...K.j"...K
-00006ec0: 036a e702 0000 4b04 758c 0e74 6f63 5f73  .j....K.u..toc_s
-00006ed0: 6563 6e75 6d62 6572 7394 7d94 8c0e 746f  ecnumbers.}...to
-00006ee0: 635f 6669 676e 756d 6265 7273 947d 948c  c_fignumbers.}..
-00006ef0: 1074 6f63 7472 6565 5f69 6e63 6c75 6465  .toctree_include
-00006f00: 7394 7d94 286a 1f03 0000 5d94 286a f805  s.}.(j....].(j..
-00006f10: 0000 6afa 0500 0065 6a20 0300 005d 9428  ..j....ej ...].(
-00006f20: 6abd 0600 006a bf06 0000 6ac1 0600 006a  j....j....j....j
-00006f30: c306 0000 6ac5 0600 0065 758c 1066 696c  ....j....eu..fil
-00006f40: 6573 5f74 6f5f 7265 6275 696c 6494 7d94  es_to_rebuild.}.
-00006f50: 286a f805 0000 8f94 286a 1f03 0000 906a  (j......(j.....j
-00006f60: fa05 0000 8f94 286a 1f03 0000 906a bd06  ......(j.....j..
-00006f70: 0000 8f94 286a 2003 0000 906a bf06 0000  ....(j ....j....
-00006f80: 8f94 286a 2003 0000 906a c106 0000 8f94  ..(j ....j......
-00006f90: 286a 2003 0000 906a c306 0000 8f94 286a  (j ....j......(j
-00006fa0: 2003 0000 906a c506 0000 8f94 286a 2003   ....j......(j .
-00006fb0: 0000 9075 8c0d 676c 6f62 5f74 6f63 7472  ...u..glob_toctr
-00006fc0: 6565 7394 8f94 8c11 6e75 6d62 6572 6564  ees.....numbered
-00006fd0: 5f74 6f63 7472 6565 7394 8f94 8c0a 646f  _toctrees.....do
-00006fe0: 6d61 696e 6461 7461 947d 9428 8c01 6394  maindata.}.(..c.
-00006ff0: 7d94 288c 0b72 6f6f 745f 7379 6d62 6f6c  }.(..root_symbol
-00007000: 946a f102 0000 8c06 5379 6d62 6f6c 9493  .j......Symbol..
-00007010: 9429 8194 7d94 286a 5a03 0000 4e8c 0c73  .)..}.(jZ...N..s
-00007020: 6962 6c69 6e67 4162 6f76 6594 4e8c 0c73  iblingAbove.N..s
-00007030: 6962 6c69 6e67 4265 6c6f 7794 4e8c 0569  iblingBelow.N..i
-00007040: 6465 6e74 944e 8c0b 6465 636c 6172 6174  dent.N..declarat
-00007050: 696f 6e94 4e8c 0764 6f63 6e61 6d65 944e  ion.N..docname.N
-00007060: 6a0a 0600 004e 8c0f 6973 5265 6465 636c  j....N..isRedecl
-00007070: 6172 6174 696f 6e94 898c 095f 6368 696c  aration...._chil
-00007080: 6472 656e 945d 948c 0d5f 616e 6f6e 4368  dren.]..._anonCh
-00007090: 696c 6472 656e 945d 9475 628c 076f 626a  ildren.].ub..obj
-000070a0: 6563 7473 947d 946a ef02 0000 4b00 758c  ects.}.j....K.u.
-000070b0: 0963 6861 6e67 6573 6574 947d 9428 8c07  .changeset.}.(..
-000070c0: 6368 616e 6765 7394 7d94 6aef 0200 004b  changes.}.j....K
-000070d0: 0075 8c08 6369 7461 7469 6f6e 947d 9428  .u..citation.}.(
-000070e0: 6aef 0200 004b 008c 0963 6974 6174 696f  j....K...citatio
-000070f0: 6e73 947d 948c 0d63 6974 6174 696f 6e5f  ns.}...citation_
-00007100: 7265 6673 947d 9475 8c03 6370 7094 7d94  refs.}.u..cpp.}.
-00007110: 286a 4e08 0000 6af4 0200 006a 4f08 0000  (jN...j....jO...
-00007120: 9394 2981 947d 9428 6a5a 0300 004e 6a53  ..)..}.(jZ...NjS
-00007130: 0800 004e 6a54 0800 004e 8c09 6964 656e  ...NjT...N..iden
-00007140: 744f 724f 7094 4e8c 0e74 656d 706c 6174  tOrOp.N..templat
-00007150: 6550 6172 616d 7394 4e8c 0c74 656d 706c  eParams.N..templ
-00007160: 6174 6541 7267 7394 4e6a 5608 0000 4e6a  ateArgs.NjV...Nj
-00007170: 5708 0000 4e6a 0a06 0000 4e6a 5808 0000  W...Nj....NjX...
-00007180: 896a 5908 0000 5d94 6a5b 0800 005d 9475  .jY...].j[...].u
-00007190: 626a 6103 0000 7d94 6aef 0200 004b 0075  bja...}.j....K.u
-000071a0: 8c05 696e 6465 7894 7d94 286a ef02 0000  ..index.}.(j....
-000071b0: 4b00 8c07 656e 7472 6965 7394 7d94 286a  K...entries.}.(j
-000071c0: 1c03 0000 5d94 2828 8c06 7369 6e67 6c65  ....].((..single
-000071d0: 948c 1c46 6173 744d 4241 5220 2863 6c61  ...FastMBAR (cla
-000071e0: 7373 2069 6e20 4661 7374 4d42 4152 2994  ss in FastMBAR).
-000071f0: 8c11 4661 7374 4d42 4152 2e46 6173 744d  ..FastMBAR.FastM
-00007200: 4241 5294 686c 4e74 9428 6a79 0800 008c  BAR.hlNt.(jy....
-00007210: 255f 5f69 6e69 745f 5f28 2920 2846 6173  %__init__() (Fas
-00007220: 744d 4241 522e 4661 7374 4d42 4152 206d  tMBAR.FastMBAR m
-00007230: 6574 686f 6429 948c 1a46 6173 744d 4241  ethod)...FastMBA
-00007240: 522e 4661 7374 4d42 4152 2e5f 5f69 6e69  R.FastMBAR.__ini
-00007250: 745f 5f94 686c 4e74 9428 6a79 0800 008c  t__.hlNt.(jy....
-00007260: 1e46 2028 4661 7374 4d42 4152 2e46 6173  .F (FastMBAR.Fas
-00007270: 744d 4241 5220 7072 6f70 6572 7479 2994  tMBAR property).
-00007280: 8c13 4661 7374 4d42 4152 2e46 6173 744d  ..FastMBAR.FastM
-00007290: 4241 522e 4694 686c 4e74 9428 6a79 0800  BAR.F.hlNt.(jy..
-000072a0: 008c 2246 5f73 7464 2028 4661 7374 4d42  .."F_std (FastMB
-000072b0: 4152 2e46 6173 744d 4241 5220 7072 6f70  AR.FastMBAR prop
-000072c0: 6572 7479 2994 8c17 4661 7374 4d42 4152  erty)...FastMBAR
-000072d0: 2e46 6173 744d 4241 522e 465f 7374 6494  .FastMBAR.F_std.
-000072e0: 686c 4e74 9428 6a79 0800 008c 2246 5f63  hlNt.(jy...."F_c
-000072f0: 6f76 2028 4661 7374 4d42 4152 2e46 6173  ov (FastMBAR.Fas
-00007300: 744d 4241 5220 7072 6f70 6572 7479 2994  tMBAR property).
-00007310: 8c17 4661 7374 4d42 4152 2e46 6173 744d  ..FastMBAR.FastM
-00007320: 4241 522e 465f 636f 7694 686c 4e74 9428  BAR.F_cov.hlNt.(
-00007330: 6a79 0800 008c 2344 656c 7461 4620 2846  jy....#DeltaF (F
-00007340: 6173 744d 4241 522e 4661 7374 4d42 4152  astMBAR.FastMBAR
-00007350: 2070 726f 7065 7274 7929 948c 1846 6173   property)...Fas
-00007360: 744d 4241 522e 4661 7374 4d42 4152 2e44  tMBAR.FastMBAR.D
-00007370: 656c 7461 4694 686c 4e74 9428 6a79 0800  eltaF.hlNt.(jy..
-00007380: 008c 2744 656c 7461 465f 7374 6420 2846  ..'DeltaF_std (F
-00007390: 6173 744d 4241 522e 4661 7374 4d42 4152  astMBAR.FastMBAR
-000073a0: 2070 726f 7065 7274 7929 948c 1c46 6173   property)...Fas
-000073b0: 744d 4241 522e 4661 7374 4d42 4152 2e44  tMBAR.FastMBAR.D
-000073c0: 656c 7461 465f 7374 6494 686c 4e74 9428  eltaF_std.hlNt.(
-000073d0: 6a79 0800 008c 296c 6f67 5f70 726f 625f  jy....)log_prob_
-000073e0: 6d69 7820 2846 6173 744d 4241 522e 4661  mix (FastMBAR.Fa
-000073f0: 7374 4d42 4152 2070 726f 7065 7274 7929  stMBAR property)
-00007400: 948c 1e46 6173 744d 4241 522e 4661 7374  ...FastMBAR.Fast
-00007410: 4d42 4152 2e6c 6f67 5f70 726f 625f 6d69  MBAR.log_prob_mi
-00007420: 7894 686c 4e74 9428 6a79 0800 008c 4863  x.hlNt.(jy....Hc
-00007430: 616c 6375 6c61 7465 5f66 7265 655f 656e  alculate_free_en
-00007440: 6572 6769 6573 5f6f 665f 7065 7274 7572  ergies_of_pertur
-00007450: 6265 645f 7374 6174 6573 2829 2028 4661  bed_states() (Fa
-00007460: 7374 4d42 4152 2e46 6173 744d 4241 5220  stMBAR.FastMBAR 
-00007470: 6d65 7468 6f64 2994 8c3d 4661 7374 4d42  method)..=FastMB
-00007480: 4152 2e46 6173 744d 4241 522e 6361 6c63  AR.FastMBAR.calc
-00007490: 756c 6174 655f 6672 6565 5f65 6e65 7267  ulate_free_energ
-000074a0: 6965 735f 6f66 5f70 6572 7475 7262 6564  ies_of_perturbed
-000074b0: 5f73 7461 7465 7394 686c 4e74 9465 6a1d  _states.hlNt.ej.
-000074c0: 0300 005d 946a 1e03 0000 5d94 6a1f 0300  ...].j....].j...
-000074d0: 005d 946a 2003 0000 5d94 6a21 0300 005d  .].j ...].j!...]
-000074e0: 946a 2203 0000 5d94 6ae7 0200 005d 9475  .j"...].j....].u
-000074f0: 758c 026a 7394 7d94 286a 5d08 0000 7d94  u..js.}.(j]...}.
-00007500: 8c07 6d6f 6475 6c65 7394 7d94 6aef 0200  ..modules.}.j...
-00007510: 004b 0075 8c04 6d61 7468 947d 9428 6a5d  .K.u..math.}.(j]
-00007520: 0800 007d 948c 0d68 6173 5f65 7175 6174  ...}...has_equat
-00007530: 696f 6e73 947d 9428 6a1c 0300 0088 6a1d  ions.}.(j.....j.
-00007540: 0300 0088 6a1e 0300 0088 6a1f 0300 0089  ....j.....j.....
-00007550: 6a20 0300 0089 6a21 0300 0089 6a22 0300  j ....j!....j"..
-00007560: 0088 6ae7 0200 0089 756a ef02 0000 4b00  ..j.....uj....K.
-00007570: 758c 0270 7994 7d94 286a 5d08 0000 7d94  u..py.}.(j]...}.
-00007580: 288c 1146 6173 744d 4241 522e 4661 7374  (..FastMBAR.Fast
-00007590: 4d42 4152 948c 1573 7068 696e 782e 646f  MBAR...sphinx.do
-000075a0: 6d61 696e 732e 7079 7468 6f6e 948c 0b4f  mains.python...O
-000075b0: 626a 6563 7445 6e74 7279 9493 9428 6a1c  bjectEntry...(j.
-000075c0: 0300 006a 7b08 0000 8c05 636c 6173 7394  ...j{.....class.
-000075d0: 8974 9481 948c 1a46 6173 744d 4241 522e  .t.....FastMBAR.
-000075e0: 6661 7374 6d62 6172 2e46 6173 744d 4241  fastmbar.FastMBA
-000075f0: 5294 6aac 0800 0028 6a1c 0300 006a 7b08  R.j....(j....j{.
-00007600: 0000 6aad 0800 0088 7494 8194 8c1a 4661  ..j.....t.....Fa
-00007610: 7374 4d42 4152 2e46 6173 744d 4241 522e  stMBAR.FastMBAR.
-00007620: 5f5f 696e 6974 5f5f 946a ac08 0000 286a  __init__.j....(j
-00007630: 1c03 0000 6a7e 0800 008c 066d 6574 686f  ....j~.....metho
-00007640: 6494 8974 9481 948c 1346 6173 744d 4241  d..t.....FastMBA
-00007650: 522e 4661 7374 4d42 4152 2e46 946a ac08  R.FastMBAR.F.j..
-00007660: 0000 286a 1c03 0000 6a81 0800 008c 0870  ..(j....j......p
-00007670: 726f 7065 7274 7994 8974 9481 948c 1746  roperty..t.....F
-00007680: 6173 744d 4241 522e 4661 7374 4d42 4152  astMBAR.FastMBAR
-00007690: 2e46 5f73 7464 946a ac08 0000 286a 1c03  .F_std.j....(j..
-000076a0: 0000 6a84 0800 008c 0870 726f 7065 7274  ..j......propert
-000076b0: 7994 8974 9481 948c 1746 6173 744d 4241  y..t.....FastMBA
-000076c0: 522e 4661 7374 4d42 4152 2e46 5f63 6f76  R.FastMBAR.F_cov
-000076d0: 946a ac08 0000 286a 1c03 0000 6a87 0800  .j....(j....j...
-000076e0: 008c 0870 726f 7065 7274 7994 8974 9481  ...property..t..
-000076f0: 948c 1846 6173 744d 4241 522e 4661 7374  ...FastMBAR.Fast
-00007700: 4d42 4152 2e44 656c 7461 4694 6aac 0800  MBAR.DeltaF.j...
-00007710: 0028 6a1c 0300 006a 8a08 0000 8c08 7072  .(j....j......pr
-00007720: 6f70 6572 7479 9489 7494 8194 8c1c 4661  operty..t.....Fa
-00007730: 7374 4d42 4152 2e46 6173 744d 4241 522e  stMBAR.FastMBAR.
-00007740: 4465 6c74 6146 5f73 7464 946a ac08 0000  DeltaF_std.j....
-00007750: 286a 1c03 0000 6a8d 0800 008c 0870 726f  (j....j......pro
-00007760: 7065 7274 7994 8974 9481 948c 1e46 6173  perty..t.....Fas
-00007770: 744d 4241 522e 4661 7374 4d42 4152 2e6c  tMBAR.FastMBAR.l
-00007780: 6f67 5f70 726f 625f 6d69 7894 6aac 0800  og_prob_mix.j...
-00007790: 0028 6a1c 0300 006a 9008 0000 8c08 7072  .(j....j......pr
-000077a0: 6f70 6572 7479 9489 7494 8194 8c3d 4661  operty..t....=Fa
-000077b0: 7374 4d42 4152 2e46 6173 744d 4241 522e  stMBAR.FastMBAR.
-000077c0: 6361 6c63 756c 6174 655f 6672 6565 5f65  calculate_free_e
-000077d0: 6e65 7267 6965 735f 6f66 5f70 6572 7475  nergies_of_pertu
-000077e0: 7262 6564 5f73 7461 7465 7394 6aac 0800  rbed_states.j...
-000077f0: 0028 6a1c 0300 006a 9308 0000 8c06 6d65  .(j....j......me
-00007800: 7468 6f64 9489 7494 8194 756a 9f08 0000  thod..t...uj....
-00007810: 7d94 6aef 0200 004b 0075 8c03 7273 7494  }.j....K.u..rst.
-00007820: 7d94 286a 5d08 0000 7d94 6aef 0200 004b  }.(j]...}.j....K
-00007830: 0075 8c03 7374 6494 7d94 288c 0b70 726f  .u..std.}.(..pro
-00007840: 676f 7074 696f 6e73 947d 946a 5d08 0000  goptions.}.j]...
-00007850: 7d94 8c06 6c61 6265 6c73 947d 9428 8c08  }...labels.}.(..
-00007860: 6765 6e69 6e64 6578 946a de08 0000 686c  genindex.j....hl
-00007870: 8c0d 7370 6869 6e78 2e6c 6f63 616c 6594  ..sphinx.locale.
-00007880: 8c11 5f54 7261 6e73 6c61 7469 6f6e 5072  .._TranslationPr
-00007890: 6f78 7994 9394 286a df08 0000 8c0f 5f6c  oxy...(j......_l
-000078a0: 617a 795f 7472 616e 736c 6174 6594 9394  azy_translate...
-000078b0: 8c06 7370 6869 6e78 948c 0767 656e 6572  ..sphinx...gener
-000078c0: 616c 948c 0549 6e64 6578 9474 9481 946a  al...Index.t...j
-000078d0: e308 0000 6ae4 0800 006a e508 0000 6ae6  ....j....j....j.
-000078e0: 0800 0087 9486 9462 8794 8c08 6d6f 6469  .......b....modi
-000078f0: 6e64 6578 948c 0b70 792d 6d6f 6469 6e64  ndex...py-modind
-00007900: 6578 9468 6c6a e108 0000 286a e308 0000  ex.hlj....(j....
-00007910: 6ae4 0800 006a e508 0000 8c0c 4d6f 6475  j....j......Modu
-00007920: 6c65 2049 6e64 6578 9474 9481 946a e308  le Index.t...j..
-00007930: 0000 6ae4 0800 006a e508 0000 6aee 0800  ..j....j....j...
-00007940: 0087 9486 9462 8794 8c06 7365 6172 6368  .....b....search
-00007950: 946a f408 0000 686c 6ae1 0800 0028 6ae3  .j....hlj....(j.
-00007960: 0800 006a e408 0000 6ae5 0800 008c 0b53  ...j....j......S
-00007970: 6561 7263 6820 5061 6765 9474 9481 946a  earch Page.t...j
-00007980: e308 0000 6ae4 0800 006a e508 0000 6af5  ....j....j....j.
-00007990: 0800 0087 9486 9462 8794 8c0b 7079 2d6d  .......b....py-m
-000079a0: 6f64 696e 6465 7894 8c0b 7079 2d6d 6f64  odindex...py-mod
-000079b0: 696e 6465 7894 686c 8c13 5079 7468 6f6e  index.hl..Python
-000079c0: 204d 6f64 756c 6520 496e 6465 7894 8794   Module Index...
-000079d0: 8c08 6578 616d 706c 6573 946a 1f03 0000  ..examples.j....
-000079e0: 8c08 6578 616d 706c 6573 948c 0845 7861  ..examples...Exa
-000079f0: 6d70 6c65 7394 8794 758c 0a61 6e6f 6e6c  mples...u..anonl
-00007a00: 6162 656c 7394 7d94 286a de08 0000 6ade  abels.}.(j....j.
-00007a10: 0800 0068 6c86 946a ec08 0000 6aed 0800  ...hl..j....j...
-00007a20: 0068 6c86 946a f408 0000 6af4 0800 0068  .hl..j....j....h
-00007a30: 6c86 946a fb08 0000 6afc 0800 0068 6c86  l..j....j....hl.
-00007a40: 946a ff08 0000 6a1f 0300 006a 0009 0000  .j....j....j....
-00007a50: 8694 756a ef02 0000 4b00 8c05 7465 726d  ..uj....K...term
-00007a60: 7394 7d94 7575 8c06 696d 6167 6573 948c  s.}.uu..images..
-00007a70: 0b73 7068 696e 782e 7574 696c 948c 1046  .sphinx.util...F
-00007a80: 696c 656e 616d 6555 6e69 7144 6963 7494  ilenameUniqDict.
-00007a90: 9394 2981 9428 6a2e 0300 008f 9428 6a1d  ..)..(j......(j.
-00007aa0: 0300 0090 8c09 4669 675f 312e 706e 6794  ......Fig_1.png.
-00007ab0: 8694 6a31 0300 008f 9428 6a1d 0300 0090  ..j1.....(j.....
-00007ac0: 8c09 4669 675f 322e 706e 6794 8694 6a30  ..Fig_2.png...j0
-00007ad0: 0300 008f 9428 6a1d 0300 0090 8c07 504d  .....(j.......PM
-00007ae0: 462e 706e 6794 8694 6a36 0300 008f 9428  F.png...j6.....(
-00007af0: 6a1e 0300 0090 8c0a 4669 675f 3131 2e70  j.......Fig_11.p
-00007b00: 6e67 9486 946a 3503 0000 8f94 286a 1e03  ng...j5.....(j..
-00007b10: 0000 908c 0a46 6967 5f32 312e 706e 6794  .....Fig_21.png.
-00007b20: 8694 6a34 0300 008f 9428 6a1e 0300 0090  ..j4.....(j.....
-00007b30: 8c08 504d 4631 2e70 6e67 9486 946a 3f03  ..PMF1.png...j?.
-00007b40: 0000 8f94 286a 2203 0000 908c 1165 6e65  ....(j"......ene
-00007b50: 7267 795f 6d61 7472 6978 2e70 6e67 9486  rgy_matrix.png..
-00007b60: 9475 8f94 286a 1509 0000 6a21 0900 006a  .u..(j....j!...j
-00007b70: 1809 0000 6a24 0900 006a 1209 0000 6a1b  ....j$...j....j.
-00007b80: 0900 006a 1e09 0000 9062 8c07 646c 6669  ...j.....b..dlfi
-00007b90: 6c65 7394 6a0d 0900 008c 0d44 6f77 6e6c  les.j......Downl
-00007ba0: 6f61 6446 696c 6573 9493 9429 8194 8c12  oadFiles...)....
-00007bb0: 6f72 6967 696e 616c 5f69 6d61 6765 5f75  original_image_u
-00007bc0: 7269 947d 948c 0974 656d 705f 6461 7461  ri.}...temp_data
-00007bd0: 947d 948c 0b72 6566 5f63 6f6e 7465 7874  .}...ref_context
-00007be0: 947d 948c 115f 7669 6577 636f 6465 5f6d  .}..._viewcode_m
-00007bf0: 6f64 756c 6573 947d 948c 1146 6173 744d  odules.}...FastM
-00007c00: 4241 522e 6661 7374 6d62 6172 9428 58c6  BAR.fastmbar.(X.
-00007c10: 7100 0066 726f 6d20 7479 7069 6e67 2069  q..from typing i
-00007c20: 6d70 6f72 7420 556e 696f 6e0a 696d 706f  mport Union.impo
-00007c30: 7274 2074 6f72 6368 0a69 6d70 6f72 7420  rt torch.import 
-00007c40: 6e75 6d70 7920 6173 206e 700a 696d 706f  numpy as np.impo
-00007c50: 7274 2073 6369 7079 2e6f 7074 696d 697a  rt scipy.optimiz
-00007c60: 6520 6173 206f 7074 696d 697a 650a 696d  e as optimize.im
-00007c70: 706f 7274 206d 6174 680a 0a0a 636c 6173  port math...clas
-00007c80: 7320 4661 7374 4d42 4152 3a0a 2020 2020  s FastMBAR:.    
-00007c90: 2222 220a 2020 2020 5468 6520 4661 7374  """.    The Fast
-00007ca0: 4d42 4152 2063 6c61 7373 2069 7320 696e  MBAR class is in
-00007cb0: 6974 6961 6c69 7a65 6420 7769 7468 2061  itialized with a
-00007cc0: 6e20 656e 6572 6779 206d 6174 7269 7820  n energy matrix 
-00007cd0: 616e 6420 616e 2061 7272 6179 0a20 2020  and an array.   
-00007ce0: 206f 6620 6e75 6d20 6f66 2063 6f6e 666f   of num of confo
-00007cf0: 726d 6174 696f 6e73 2e20 5468 6520 636f  rmations. The co
-00007d00: 7272 6573 706f 6e64 696e 6720 4d42 4152  rresponding MBAR
-00007d10: 2065 7175 6174 696f 6e20 6973 2073 6f6c   equation is sol
-00007d20: 7665 640a 2020 2020 696e 2074 6865 2063  ved.    in the c
-00007d30: 6f6e 7374 7275 6374 6f72 2e20 5468 6572  onstructor. Ther
-00007d40: 6566 6f72 652c 2074 6865 2072 656c 6174  efore, the relat
-00007d50: 6976 6520 6672 6565 2065 6e65 7267 6965  ive free energie
-00007d60: 7320 6f66 2073 7461 7465 730a 2020 2020  s of states.    
-00007d70: 7573 6564 2069 6e20 7468 6520 656e 6572  used in the ener
-00007d80: 6779 206d 6174 7269 7820 6973 2063 616c  gy matrix is cal
-00007d90: 6375 6c61 7465 6420 696e 2074 6865 2063  culated in the c
-00007da0: 6f6e 7374 7275 6374 6f72 2e20 5468 650a  onstructor. The.
-00007db0: 2020 2020 6d65 7468 6f64 202a 2a63 616c      method **cal
-00007dc0: 6375 6c61 7465 5f66 7265 655f 656e 6572  culate_free_ener
-00007dd0: 6769 6573 5f66 6f72 5f70 6572 7475 7262  gies_for_perturb
-00007de0: 6564 5f73 7461 7465 732a 2a0a 2020 2020  ed_states**.    
-00007df0: 6361 6e20 6265 2075 7365 6420 746f 2063  can be used to c
-00007e00: 616c 6375 6c61 7465 6420 7468 6520 7265  alculated the re
-00007e10: 6c61 7469 7665 2066 7265 6520 656e 6572  lative free ener
-00007e20: 6769 6573 206f 6620 7065 7274 7572 6265  gies of perturbe
-00007e30: 6420 7374 6174 6573 2e0a 2020 2020 2222  d states..    ""
-00007e40: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
-00007e50: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00007e60: 662c 0a20 2020 2020 2020 2065 6e65 7267  f,.        energ
-00007e70: 793a 2055 6e69 6f6e 5b6e 702e 6e64 6172  y: Union[np.ndar
-00007e80: 7261 792c 2074 6f72 6368 2e54 656e 736f  ray, torch.Tenso
-00007e90: 725d 2c0a 2020 2020 2020 2020 6e75 6d5f  r],.        num_
-00007ea0: 636f 6e66 3a20 556e 696f 6e5b 6e70 2e6e  conf: Union[np.n
-00007eb0: 6461 7272 6179 2c20 746f 7263 682e 5465  darray, torch.Te
-00007ec0: 6e73 6f72 5d2c 0a20 2020 2020 2020 2063  nsor],.        c
-00007ed0: 7564 613a 2062 6f6f 6c20 3d20 4661 6c73  uda: bool = Fals
-00007ee0: 652c 0a20 2020 2020 2020 2063 7564 615f  e,.        cuda_
-00007ef0: 6261 7463 685f 6d6f 6465 3a20 556e 696f  batch_mode: Unio
-00007f00: 6e5b 626f 6f6c 2c20 4e6f 6e65 5d20 3d20  n[bool, None] = 
-00007f10: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
-00007f20: 6f74 7374 7261 703a 2062 6f6f 6c20 3d20  otstrap: bool = 
-00007f30: 4661 6c73 652c 0a20 2020 2020 2020 2062  False,.        b
-00007f40: 6f6f 7473 7472 6170 5f62 6c6f 636b 5f73  ootstrap_block_s
-00007f50: 697a 653a 2069 6e74 203d 2033 2c0a 2020  ize: int = 3,.  
-00007f60: 2020 2020 2020 626f 6f74 7374 7261 705f        bootstrap_
-00007f70: 6e75 6d5f 7265 703a 2069 6e74 203d 2031  num_rep: int = 1
-00007f80: 3030 2c0a 2020 2020 2020 2020 7665 7262  00,.        verb
-00007f90: 6f73 653a 2062 6f6f 6c20 3d20 4661 6c73  ose: bool = Fals
-00007fa0: 652c 0a20 2020 2020 2020 206d 6574 686f  e,.        metho
-00007fb0: 643a 2073 7472 203d 2022 4e65 7774 6f6e  d: str = "Newton
-00007fc0: 222c 0a20 2020 2029 202d 3e20 4e6f 6e65  ",.    ) -> None
-00007fd0: 3a0a 2020 2020 2020 2020 2222 2249 6e69  :.        """Ini
-00007fe0: 7469 616c 697a 6572 2066 6f72 2074 6865  tializer for the
-00007ff0: 2063 6c61 7373 2046 6173 744d 4241 520a   class FastMBAR.
-00008000: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00008010: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00008020: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2065  ------.        e
-00008030: 6e65 7267 7920 3a20 3244 206e 6461 7272  nergy : 2D ndarr
-00008040: 6179 206f 7220 3244 2074 656e 736f 720a  ay or 2D tensor.
-00008050: 2020 2020 2020 2020 2020 2020 4974 2068              It h
-00008060: 6173 2061 2073 697a 6520 6f66 2028 4d20  as a size of (M 
-00008070: 7820 4e29 2c20 7768 6572 6520 4d20 6973  x N), where M is
-00008080: 2074 6865 206e 756d 6265 7220 6f66 2073   the number of s
-00008090: 7461 7465 730a 2020 2020 2020 2020 2020  tates.          
-000080a0: 2020 616e 6420 4e20 6973 2074 6865 2074    and N is the t
-000080b0: 6f74 616c 206e 756d 6265 7220 6f66 2063  otal number of c
-000080c0: 6f6e 666f 726d 6174 696f 6e73 2e20 5468  onformations. Th
-000080d0: 6520 656e 7472 7920 656e 6572 6779 5b69  e entry energy[i
-000080e0: 2c6a 5d0a 2020 2020 2020 2020 2020 2020  ,j].            
-000080f0: 6973 2074 6865 2072 6564 7563 6564 2028  is the reduced (
-00008100: 756e 6974 6c65 7373 2920 656e 6572 6779  unitless) energy
-00008110: 206f 6620 636f 6e66 6f72 6d61 7469 6f6e   of conformation
-00008120: 206a 2069 6e20 7374 6174 6520 692e 0a20   j in state i.. 
-00008130: 2020 2020 2020 2020 2020 2049 6620 626f             If bo
-00008140: 6f74 7374 7261 7070 696e 6720 6973 2075  otstrapping is u
-00008150: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
-00008160: 2074 6865 2075 6e63 6572 7461 696e 7479   the uncertainty
-00008170: 2c20 7468 6520 6f72 6465 720a 2020 2020  , the order.    
-00008180: 2020 2020 2020 2020 6f66 2063 6f6e 666f          of confo
-00008190: 726d 6174 696f 6e73 206d 6174 7465 7273  rmations matters
-000081a0: 2e20 436f 6e66 6f72 6d61 7469 6f6e 7320  . Conformations 
-000081b0: 7361 6d70 6c65 6420 6672 6f6d 206f 6e65  sampled from one
-000081c0: 2073 7461 7465 0a20 2020 2020 2020 2020   state.         
-000081d0: 2020 206e 6565 6420 746f 206f 6363 7079     need to occpy
-000081e0: 2061 2063 6f6e 7469 6e75 6f75 7320 6368   a continuous ch
-000081f0: 756e 6b20 6f66 2063 6f6c 6c75 6d6e 732e  unk of collumns.
-00008200: 2043 6f6e 666f 726d 6174 696f 6e73 2073   Conformations s
-00008210: 616d 706c 6564 0a20 2020 2020 2020 2020  ampled.         
-00008220: 2020 2066 726f 6d20 7374 6174 6520 6b20     from state k 
-00008230: 6e65 6564 2074 6f20 6f63 6375 7079 2063  need to occupy c
-00008240: 6f6c 6c75 6d6e 7320 746f 2074 6865 206c  ollumns to the l
-00008250: 6566 7420 6f66 2063 6f6e 666f 726d 6174  eft of conformat
-00008260: 696f 6e73 0a20 2020 2020 2020 2020 2020  ions.           
-00008270: 2073 616d 706c 6564 2066 726f 6d20 7374   sampled from st
-00008280: 6174 6520 6c20 6966 206b 203c 206c 2e20  ate l if k < l. 
-00008290: 4966 2062 6f6f 7473 7472 6170 7069 6e67  If bootstrapping
-000082a0: 2069 7320 6e6f 7420 7573 6564 2c20 7468   is not used, th
-000082b0: 656e 0a20 2020 2020 2020 2020 2020 2074  en.            t
-000082c0: 6865 206f 7264 6572 206f 6620 636f 6e66  he order of conf
-000082d0: 6f72 6d61 7469 6f6e 2064 6f65 7320 6e6f  ormation does no
-000082e0: 7420 6d61 7474 6572 2e0a 2020 2020 2020  t matter..      
-000082f0: 2020 6e75 6d5f 636f 6e66 3a20 3144 2069    num_conf: 1D i
-00008300: 6e74 206e 6461 7272 6179 206f 7220 3144  nt ndarray or 1D
-00008310: 2074 656e 736f 720a 2020 2020 2020 2020   tensor.        
-00008320: 2020 2020 4974 2073 686f 756c 6420 6861      It should ha
-00008330: 7665 2061 2073 697a 6520 6f66 204d 2c20  ve a size of M, 
-00008340: 7768 6572 6520 6e75 6d5f 636f 6e66 5b69  where num_conf[i
-00008350: 5d20 6973 2074 6865 206e 756d 206f 660a  ] is the num of.
-00008360: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-00008370: 6f72 6d61 7469 6f6e 7320 7361 6d70 6c65  ormations sample
-00008380: 6420 6672 6f6d 2073 7461 7465 2069 2e20  d from state i. 
-00008390: 5468 6572 6566 6f72 652c 206e 702e 7375  Therefore, np.su
-000083a0: 6d28 6e75 6d5f 636f 6e66 290a 2020 2020  m(num_conf).    
-000083b0: 2020 2020 2020 2020 6861 7320 746f 2062          has to b
-000083c0: 6520 6571 7561 6c20 746f 204e 2e20 416c  e equal to N. Al
-000083d0: 6c20 656e 7472 6965 7320 696e 206e 756d  l entries in num
-000083e0: 5f63 6f6e 6620 6861 7665 2074 6f20 6265  _conf have to be
-000083f0: 2073 7472 6963 746c 790a 2020 2020 2020   strictly.      
-00008400: 2020 2020 2020 6772 6561 7465 7220 7468        greater th
-00008410: 616e 2030 2e0a 2020 2020 2020 2020 6375  an 0..        cu
-00008420: 6461 3a20 626f 6f6c 2c20 6f70 7469 6f6e  da: bool, option
-00008430: 616c 2028 6465 6661 756c 743d 4661 6c73  al (default=Fals
-00008440: 6529 0a20 2020 2020 2020 2020 2020 2049  e).            I
-00008450: 6620 6974 2069 7320 7365 7420 746f 2062  f it is set to b
-00008460: 6520 5472 7565 2c20 7468 656e 2074 6865  e True, then the
-00008470: 2063 616c 6375 6c61 7469 6f6e 2077 696c   calculation wil
-00008480: 6c20 6265 2072 756e 206f 6e0a 2020 2020  l be run on.    
-00008490: 2020 2020 2020 2020 6120 6772 6170 6869          a graphi
-000084a0: 6361 6c20 7072 6f63 6573 7369 6e67 2075  cal processing u
-000084b0: 6e69 7420 2847 5055 2920 7573 696e 6720  nit (GPU) using 
-000084c0: 4355 4441 2e0a 2020 2020 2020 2020 6375  CUDA..        cu
-000084d0: 6461 5f62 6174 6368 5f6d 6f64 653a 2062  da_batch_mode: b
-000084e0: 6f6f 6c2c 206f 7074 696f 6e61 6c20 2864  ool, optional (d
-000084f0: 6566 6175 6c74 3d4e 6f6e 6529 0a20 2020  efault=None).   
-00008500: 2020 2020 2020 2020 2054 6865 2062 6174           The bat
-00008510: 6368 206d 6f64 6520 6973 2074 7572 6e65  ch mode is turne
-00008520: 6420 6f6e 2077 6865 6e20 7468 6520 7369  d on when the si
-00008530: 7a65 206f 6620 7468 6520 656e 6572 6779  ze of the energy
-00008540: 206d 6174 7269 7820 6973 0a20 2020 2020   matrix is.     
-00008550: 2020 2020 2020 2074 6f6f 206c 6172 6765         too large
-00008560: 2066 6f72 2074 6865 206d 656d 6f72 7920   for the memory 
-00008570: 6f66 2061 2047 5055 2e20 5768 656e 2063  of a GPU. When c
-00008580: 7564 615f 6261 7463 685f 6d6f 6465 2069  uda_batch_mode i
-00008590: 7320 5472 7565 2c0a 2020 2020 2020 2020  s True,.        
-000085a0: 2020 2020 7468 6520 656e 6572 6779 206d      the energy m
-000085b0: 6174 7269 7820 7769 6c6c 2062 6520 7370  atrix will be sp
-000085c0: 6c69 7420 696e 746f 206d 756c 7469 706c  lit into multipl
-000085d0: 6520 6261 7463 6865 7320 7768 6963 6820  e batches which 
-000085e0: 6172 6520 7573 6564 0a20 2020 2020 2020  are used.       
-000085f0: 2020 2020 2073 6571 7565 6e74 6961 6c6c       sequentiall
-00008600: 792e 2049 6620 6375 6461 5f62 6174 6368  y. If cuda_batch
-00008610: 5f6d 6f64 6520 3d20 4e6f 6e65 2c20 6974  _mode = None, it
-00008620: 2077 696c 6c20 6265 2073 6574 2061 7574   will be set aut
-00008630: 6f6d 6174 6963 616c 6c79 0a20 2020 2020  omatically.     
-00008640: 2020 2020 2020 2062 6173 6564 206f 6e20         based on 
-00008650: 7468 6520 7369 7a65 206f 6620 656e 6572  the size of ener
-00008660: 6779 2061 6e64 2074 6865 206d 656d 6f72  gy and the memor
-00008670: 7920 6f66 2074 6865 2061 7661 6962 6c65  y of the avaible
-00008680: 2047 5055 2064 6576 6963 652e 0a20 2020   GPU device..   
-00008690: 2020 2020 2062 6f6f 7473 7472 6170 3a20       bootstrap: 
-000086a0: 626f 6f6c 2c20 6f70 7469 6f6e 616c 2028  bool, optional (
-000086b0: 6465 6661 756c 743d 4661 6c73 6529 0a20  default=False). 
-000086c0: 2020 2020 2020 2020 2020 2049 6620 626f             If bo
-000086d0: 6f74 7374 7261 7020 6973 2054 7275 652c  otstrap is True,
-000086e0: 2074 6865 2075 6e63 6572 7461 696e 7479   the uncertainty
-000086f0: 206f 6620 7468 6520 6361 6c63 756c 6174   of the calculat
-00008700: 6564 2066 7265 6520 656e 6572 6769 6573  ed free energies
-00008710: 0a20 2020 2020 2020 2020 2020 2077 696c  .            wil
-00008720: 6c20 6265 2065 7374 696d 6174 6520 7573  l be estimate us
-00008730: 696e 6720 626c 6f63 6b20 626f 6f74 7374  ing block bootst
-00008740: 7261 7069 6e67 2e0a 2020 2020 2020 2020  raping..        
-00008750: 626f 6f74 7374 7261 705f 626c 6f63 6b5f  bootstrap_block_
-00008760: 7369 7a65 3a20 696e 742c 206f 7074 696f  size: int, optio
-00008770: 6e61 6c20 2864 6566 6175 6c74 3d33 290a  nal (default=3).
-00008780: 2020 2020 2020 2020 2020 2020 626c 6f63              bloc
-00008790: 6b20 7369 7a65 2075 7365 6420 696e 2062  k size used in b
-000087a0: 6c6f 636b 2062 6f6f 7473 7472 6170 7069  lock bootstrappi
-000087b0: 6e67 0a20 2020 2020 2020 2062 6f6f 7473  ng.        boots
-000087c0: 7472 6170 5f6e 756d 5f72 6570 3a20 696e  trap_num_rep: in
-000087d0: 742c 206f 7074 696f 6e61 6c20 2864 6566  t, optional (def
-000087e0: 6175 6c74 3d31 3030 290a 2020 2020 2020  ault=100).      
-000087f0: 2020 2020 2020 6e75 6d62 6572 206f 6620        number of 
-00008800: 7265 7072 6561 7473 2069 6e20 626c 6f63  repreats in bloc
-00008810: 6b20 626f 6f74 7374 7261 7070 696e 670a  k bootstrapping.
-00008820: 2020 2020 2020 2020 7665 7262 6f73 653a          verbose:
-00008830: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c20   bool, optional 
-00008840: 2864 6566 6175 6c74 3d46 616c 7365 290a  (default=False).
-00008850: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-00008860: 6572 626f 7365 2069 7320 7472 7565 2c20  erbose is true, 
-00008870: 7468 6520 6465 7461 696c 6564 2069 6e66  the detailed inf
-00008880: 6f72 6d61 7469 6f6e 206f 6620 736f 6c76  ormation of solv
-00008890: 696e 6720 4d42 4152 2065 7175 6174 696f  ing MBAR equatio
-000088a0: 6e73 0a20 2020 2020 2020 2020 2020 2069  ns.            i
-000088b0: 7320 7072 696e 7465 642e 0a20 2020 2020  s printed..     
-000088c0: 2020 206d 6574 686f 643a 2073 7472 2c20     method: str, 
-000088d0: 6f70 7469 6f6e 616c 2028 6465 6661 756c  optional (defaul
-000088e0: 743d 224e 6577 746f 6e22 290a 2020 2020  t="Newton").    
-000088f0: 2020 2020 2020 2020 7468 6520 6d65 7468          the meth
-00008900: 6f64 2075 7365 6420 746f 2073 6f6c 7665  od used to solve
-00008910: 2074 6865 204d 4241 5220 6571 7561 7469   the MBAR equati
-00008920: 6f6e 2e20 5468 6520 6465 6661 756c 7420  on. The default 
-00008930: 6973 204e 6577 746f 6e27 7320 6d65 7468  is Newton's meth
-00008940: 6f64 2e0a 2020 2020 2020 2020 2222 220a  od..        """.
-00008950: 0a20 2020 2020 2020 2023 2323 2320 6368  .        #### ch
-00008960: 6563 6b20 7468 6520 7061 7261 6d65 7465  eck the paramete
-00008970: 7273 3a20 656e 6572 6779 2061 6e64 206e  rs: energy and n
-00008980: 756d 5f63 6f6e 660a 2020 2020 2020 2020  um_conf.        
-00008990: 2323 204e 6f74 6520 7468 6174 2062 6f74  ## Note that bot
-000089a0: 6820 7365 6c66 2e65 6e65 7267 7920 616e  h self.energy an
-000089b0: 6420 7365 6c66 2e63 6f6e 6620 7769 6c6c  d self.conf will
-000089c0: 2062 6520 6f6e 2043 5055 7320 6e6f 206d   be on CPUs no m
-000089d0: 6174 7465 720a 2020 2020 2020 2020 2323  atter.        ##
-000089e0: 2069 6620 6375 6461 2069 7320 5472 7565   if cuda is True
-000089f0: 206f 7220 4661 6c73 652e 0a0a 2020 2020   or False...    
-00008a00: 2020 2020 2323 2065 6e65 7267 7920 6e65      ## energy ne
-00008a10: 6564 7320 746f 2062 6520 6120 322d 4420  eds to be a 2-D 
-00008a20: 6e64 6172 7261 7920 6f72 2061 2032 2d44  ndarray or a 2-D
-00008a30: 2074 656e 736f 722e 0a20 2020 2020 2020   tensor..       
-00008a40: 2023 2320 636f 6e76 6572 7420 6974 2069   ## convert it i
-00008a50: 6e74 6f20 646f 7562 6c65 2070 7265 6369  nto double preci
-00008a60: 7369 6f6e 2069 6620 6e6f 740a 2020 2020  sion if not.    
-00008a70: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00008a80: 6528 656e 6572 6779 2c20 6e70 2e6e 6461  e(energy, np.nda
-00008a90: 7272 6179 293a 0a20 2020 2020 2020 2020  rray):.         
-00008aa0: 2020 2065 6e65 7267 7920 3d20 656e 6572     energy = ener
-00008ab0: 6779 2e61 7374 7970 6528 6e70 2e66 6c6f  gy.astype(np.flo
-00008ac0: 6174 3634 290a 2020 2020 2020 2020 2020  at64).          
-00008ad0: 2020 7365 6c66 2e65 6e65 7267 7920 3d20    self.energy = 
-00008ae0: 746f 7263 682e 6672 6f6d 5f6e 756d 7079  torch.from_numpy
-00008af0: 2865 6e65 7267 7929 0a20 2020 2020 2020  (energy).       
-00008b00: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-00008b10: 2865 6e65 7267 792c 2074 6f72 6368 2e54  (energy, torch.T
-00008b20: 656e 736f 7229 3a0a 2020 2020 2020 2020  ensor):.        
-00008b30: 2020 2020 7365 6c66 2e65 6e65 7267 7920      self.energy 
-00008b40: 3d20 656e 6572 6779 2e64 6f75 626c 6528  = energy.double(
-00008b50: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00008b60: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00008b70: 6520 5479 7065 4572 726f 7228 2265 6e65  e TypeError("ene
-00008b80: 7267 7920 6861 7320 746f 2062 6520 6120  rgy has to be a 
-00008b90: 322d 4420 6e64 6172 7261 7920 6f72 2061  2-D ndarray or a
-00008ba0: 2032 2d44 2074 656e 736f 722e 2229 0a0a   2-D tensor.")..
-00008bb0: 2020 2020 2020 2020 2323 206e 756d 5f63          ## num_c
-00008bc0: 6f6e 6620 6e65 6564 7320 746f 2062 6520  onf needs to be 
-00008bd0: 6120 312d 4420 6e64 6172 7261 7920 6f72  a 1-D ndarray or
-00008be0: 2061 2031 2d44 2074 656e 736f 722e 0a20   a 1-D tensor.. 
-00008bf0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00008c00: 616e 6365 286e 756d 5f63 6f6e 662c 206e  ance(num_conf, n
-00008c10: 702e 6e64 6172 7261 7929 3a0a 2020 2020  p.ndarray):.    
-00008c20: 2020 2020 2020 2020 6e75 6d5f 636f 6e66          num_conf
-00008c30: 203d 206e 756d 5f63 6f6e 662e 6173 7479   = num_conf.asty
-00008c40: 7065 286e 702e 666c 6f61 7436 3429 0a20  pe(np.float64). 
-00008c50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008c60: 6e75 6d5f 636f 6e66 203d 2074 6f72 6368  num_conf = torch
-00008c70: 2e66 726f 6d5f 6e75 6d70 7928 6e75 6d5f  .from_numpy(num_
-00008c80: 636f 6e66 290a 2020 2020 2020 2020 656c  conf).        el
-00008c90: 6966 2069 7369 6e73 7461 6e63 6528 6e75  if isinstance(nu
-00008ca0: 6d5f 636f 6e66 2c20 746f 7263 682e 5465  m_conf, torch.Te
-00008cb0: 6e73 6f72 293a 0a20 2020 2020 2020 2020  nsor):.         
-00008cc0: 2020 2073 656c 662e 6e75 6d5f 636f 6e66     self.num_conf
-00008cd0: 203d 206e 756d 5f63 6f6e 662e 646f 7562   = num_conf.doub
-00008ce0: 6c65 2829 0a20 2020 2020 2020 2065 6c73  le().        els
-00008cf0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00008d00: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
-00008d10: 6e75 6d5f 636f 6e66 2068 6173 2074 6f20  num_conf has to 
-00008d20: 6265 2061 2031 2d44 206e 6461 7272 6179  be a 1-D ndarray
-00008d30: 206f 7220 6120 312d 4420 7465 6e73 6f72   or a 1-D tensor
-00008d40: 2e22 290a 0a20 2020 2020 2020 2023 2320  .")..        ## 
-00008d50: 6368 6563 6b20 7468 6520 7368 6170 6520  check the shape 
-00008d60: 6f66 2065 6e65 7267 7920 616e 6420 6e75  of energy and nu
-00008d70: 6d5f 636f 6e66 0a20 2020 2020 2020 2069  m_conf.        i
-00008d80: 6620 656e 6572 6779 2e6e 6469 6d20 213d  f energy.ndim !=
-00008d90: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-00008da0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00008db0: 2822 656e 6572 6779 2068 6173 2074 6f20  ("energy has to 
-00008dc0: 6265 2061 2032 2d44 206e 6461 7272 6179  be a 2-D ndarray
-00008dd0: 206f 7220 6120 322d 4420 7465 6e73 6f72   or a 2-D tensor
-00008de0: 2e22 290a 2020 2020 2020 2020 6966 206e  .").        if n
-00008df0: 756d 5f63 6f6e 662e 6e64 696d 2021 3d20  um_conf.ndim != 
-00008e00: 313a 0a20 2020 2020 2020 2020 2020 2072  1:.            r
-00008e10: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00008e20: 226e 756d 5f63 6f6e 6620 6861 7320 746f  "num_conf has to
-00008e30: 2062 6520 6120 312d 4420 6e64 6172 7261   be a 1-D ndarra
-00008e40: 7920 6f72 2061 2031 2d44 2074 656e 736f  y or a 1-D tenso
-00008e50: 722e 2229 0a20 2020 2020 2020 2069 6620  r.").        if 
-00008e60: 656e 6572 6779 2e73 6861 7065 5b30 5d20  energy.shape[0] 
-00008e70: 213d 206e 756d 5f63 6f6e 662e 7368 6170  != num_conf.shap
-00008e80: 655b 305d 3a0a 2020 2020 2020 2020 2020  e[0]:.          
-00008e90: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00008ea0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-00008eb0: 2020 2020 2274 6865 206e 756d 6265 7220      "the number 
-00008ec0: 6f66 2072 6f77 7320 696e 2065 6e65 7267  of rows in energ
-00008ed0: 7920 6861 7320 746f 2062 6520 6571 7561  y has to be equa
-00008ee0: 6c20 746f 2074 6865 206c 656e 6774 6820  l to the length 
-00008ef0: 6f66 206e 756d 5f63 6f6e 662e 220a 2020  of num_conf.".  
-00008f00: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00008f10: 2020 2020 2023 2320 6368 6563 6b20 6966       ## check if
-00008f20: 2074 6865 206e 756d 6265 7220 6f66 2063   the number of c
-00008f30: 6f6e 666f 726d 6174 696f 6e73 2073 616d  onformations sam
-00008f40: 706c 6564 2066 726f 6d20 6561 6368 2073  pled from each s
-00008f50: 7461 7465 2069 7320 6772 6561 7465 7220  tate is greater 
-00008f60: 7468 616e 2030 0a20 2020 2020 2020 2069  than 0.        i
-00008f70: 6620 746f 7263 682e 7375 6d28 7365 6c66  f torch.sum(self
-00008f80: 2e6e 756d 5f63 6f6e 6620 3c3d 2030 2920  .num_conf <= 0) 
-00008f90: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
-00008fa0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00008fb0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00008fc0: 2020 2022 616c 6c20 656e 7472 6965 7320     "all entries 
-00008fd0: 696e 206e 756d 5f63 6f6e 6620 6861 7665  in num_conf have
-00008fe0: 2074 6f20 6265 2073 7472 6963 746c 7920   to be strictly 
-00008ff0: 6772 6561 7465 7220 7468 616e 2030 2e22  greater than 0."
-00009000: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00009010: 2020 2020 2020 2020 2323 2063 6865 636b          ## check
-00009020: 2069 6620 7468 6520 746f 7461 6c20 6e75   if the total nu
-00009030: 6d62 6572 206f 6620 636f 6e66 6f72 6d61  mber of conforma
-00009040: 7469 6f6e 7320 6973 2065 7175 616c 2074  tions is equal t
-00009050: 6f20 7468 6520 6e75 6d62 6572 206f 6620  o the number of 
-00009060: 636f 6c75 6d6e 7320 696e 2065 6e65 7267  columns in energ
-00009070: 790a 2020 2020 2020 2020 6966 2074 6f72  y.        if tor
-00009080: 6368 2e73 756d 2873 656c 662e 6e75 6d5f  ch.sum(self.num_
-00009090: 636f 6e66 2920 213d 2073 656c 662e 656e  conf) != self.en
-000090a0: 6572 6779 2e73 6861 7065 5b31 5d3a 0a20  ergy.shape[1]:. 
-000090b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000090c0: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
-000090d0: 2020 2020 2020 2020 2020 2020 2022 7468               "th
-000090e0: 6520 7375 6d20 6f66 206e 756d 5f63 6f6e  e sum of num_con
-000090f0: 6620 6861 7320 746f 2062 6520 6571 7561  f has to be equa
-00009100: 6c20 746f 2074 6865 206e 756d 6265 7220  l to the number 
-00009110: 6f66 2063 6f6c 756d 6e73 2069 6e20 656e  of columns in en
-00009120: 6572 6779 2e22 0a20 2020 2020 2020 2020  ergy.".         
-00009130: 2020 2029 0a0a 2020 2020 2020 2020 7365     )..        se
-00009140: 6c66 2e4d 203d 2073 656c 662e 656e 6572  lf.M = self.ener
-00009150: 6779 2e73 6861 7065 5b30 5d0a 2020 2020  gy.shape[0].    
-00009160: 2020 2020 7365 6c66 2e4e 203d 2073 656c      self.N = sel
-00009170: 662e 656e 6572 6779 2e73 6861 7065 5b31  f.energy.shape[1
-00009180: 5d0a 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
-00009190: 6375 6461 203d 2063 7564 610a 2020 2020  cuda = cuda.    
-000091a0: 2020 2020 6966 2073 656c 662e 6375 6461      if self.cuda
-000091b0: 2069 7320 5472 7565 3a0a 2020 2020 2020   is True:.      
-000091c0: 2020 2020 2020 7365 6c66 2e64 6576 6963        self.devic
-000091d0: 6520 3d20 746f 7263 682e 6465 7669 6365  e = torch.device
-000091e0: 2822 6375 6461 2229 0a20 2020 2020 2020  ("cuda").       
-000091f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00009200: 2020 2073 656c 662e 6465 7669 6365 203d     self.device =
-00009210: 2074 6f72 6368 2e64 6576 6963 6528 2263   torch.device("c
-00009220: 7075 2229 0a0a 2020 2020 2020 2020 6966  pu")..        if
-00009230: 2073 656c 662e 6375 6461 3a0a 2020 2020   self.cuda:.    
-00009240: 2020 2020 2020 2020 2323 2063 6865 636b          ## check
-00009250: 2069 6620 7468 6520 4750 5520 6465 7669   if the GPU devi
-00009260: 6365 2068 6173 2065 6e6f 7567 6820 6d65  ce has enough me
-00009270: 6d6f 7279 2e20 4966 206e 6f74 2c20 6375  mory. If not, cu
-00009280: 6461 5f62 6174 6368 5f6d 6f64 6520 6973  da_batch_mode is
-00009290: 2074 7572 6e65 6420 6f6e 0a0a 2020 2020   turned on..    
-000092a0: 2020 2020 2020 2020 2323 2061 7574 6f6d          ## autom
-000092b0: 6174 6963 616c 6c79 2064 6574 6572 6d69  atically determi
-000092c0: 6e65 2069 6620 6375 6461 5f62 6174 6368  ne if cuda_batch
-000092d0: 5f6d 6f64 6520 6973 206f 6e20 6f72 206f  _mode is on or o
-000092e0: 6666 0a20 2020 2020 2020 2020 2020 2073  ff.            s
-000092f0: 656c 662e 5f74 6f74 616c 5f47 5055 5f6d  elf._total_GPU_m
-00009300: 656d 6f72 7920 3d20 746f 7263 682e 6375  emory = torch.cu
-00009310: 6461 2e67 6574 5f64 6576 6963 655f 7072  da.get_device_pr
-00009320: 6f70 6572 7469 6573 2830 292e 746f 7461  operties(0).tota
-00009330: 6c5f 6d65 6d6f 7279 0a20 2020 2020 2020  l_memory.       
-00009340: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-00009350: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-00009360: 6e65 7267 792e 6e75 6d65 6c28 2920 2a20  nergy.numel() * 
-00009370: 7365 6c66 2e65 6e65 7267 792e 656c 656d  self.energy.elem
-00009380: 656e 745f 7369 7a65 2829 0a20 2020 2020  ent_size().     
-00009390: 2020 2020 2020 2020 2020 203c 2073 656c             < sel
-000093a0: 662e 5f74 6f74 616c 5f47 5055 5f6d 656d  f._total_GPU_mem
-000093b0: 6f72 7920 2f20 3130 0a20 2020 2020 2020  ory / 10.       
-000093c0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-000093d0: 2020 2020 2020 2020 7365 6c66 2e63 7564          self.cud
-000093e0: 615f 6261 7463 685f 6d6f 6465 203d 2046  a_batch_mode = F
-000093f0: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-00009400: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00009410: 2020 2020 2020 2073 656c 662e 6375 6461         self.cuda
-00009420: 5f62 6174 6368 5f6d 6f64 6520 3d20 5472  _batch_mode = Tr
-00009430: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
-00009440: 2323 2063 7564 615f 6261 7463 685f 6d6f  ## cuda_batch_mo
-00009450: 6465 2063 616e 2062 6520 656e 666f 7263  de can be enforc
-00009460: 6564 2062 7920 7061 7373 696e 6720 7468  ed by passing th
-00009470: 6520 6172 6775 6d65 6e74 2063 7564 615f  e argument cuda_
-00009480: 6261 7463 685f 6d6f 6465 0a20 2020 2020  batch_mode.     
-00009490: 2020 2020 2020 2069 6620 6375 6461 5f62         if cuda_b
-000094a0: 6174 6368 5f6d 6f64 6520 6973 206e 6f74  atch_mode is not
-000094b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000094c0: 2020 2020 2020 2073 656c 662e 6375 6461         self.cuda
-000094d0: 5f62 6174 6368 5f6d 6f64 6520 3d20 6375  _batch_mode = cu
-000094e0: 6461 5f62 6174 6368 5f6d 6f64 650a 0a20  da_batch_mode.. 
-000094f0: 2020 2020 2020 2023 2320 7768 656e 2063         ## when c
-00009500: 7564 615f 6261 7463 685f 6d6f 6465 2069  uda_batch_mode i
-00009510: 7320 7573 6564 2c20 7765 206e 6565 6420  s used, we need 
-00009520: 746f 2064 6563 6964 6520 6f6e 2074 6865  to decide on the
-00009530: 2062 6174 6368 5f73 697a 6520 6261 7365   batch_size base
-00009540: 6420 6f6e 0a20 2020 2020 2020 2023 2320  d on.        ## 
-00009550: 626f 7468 2074 6865 206d 656d 6f72 7920  both the memory 
-00009560: 6f66 2074 6865 2047 5055 2064 6576 6963  of the GPU devic
-00009570: 6520 616e 6420 7468 6520 7369 7a65 206f  e and the size o
-00009580: 6620 656e 6572 6779 206d 6174 7269 780a  f energy matrix.
-00009590: 2020 2020 2020 2020 7365 6c66 2e5f 6261          self._ba
-000095a0: 7463 685f 7369 7a65 203d 204e 6f6e 650a  tch_size = None.
-000095b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000095c0: 6375 6461 2061 6e64 2073 656c 662e 6375  cuda and self.cu
-000095d0: 6461 5f62 6174 6368 5f6d 6f64 653a 0a20  da_batch_mode:. 
-000095e0: 2020 2020 2020 2020 2020 2023 2320 6261             ## ba
-000095f0: 7463 6820 7369 7a65 2066 6f72 2073 6570  tch size for sep
-00009600: 6572 6174 696e 6720 636f 6e66 6f72 6d61  erating conforma
-00009610: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
-00009620: 2020 7365 6c66 2e5f 6261 7463 685f 7369    self._batch_si
-00009630: 7a65 203d 2069 6e74 280a 2020 2020 2020  ze = int(.      
-00009640: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00009650: 746f 7461 6c5f 4750 555f 6d65 6d6f 7279  total_GPU_memory
-00009660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009670: 202f 2032 300a 2020 2020 2020 2020 2020   / 20.          
-00009680: 2020 2020 2020 2f20 7365 6c66 2e65 6e65        / self.ene
-00009690: 7267 792e 7368 6170 655b 305d 0a20 2020  rgy.shape[0].   
-000096a0: 2020 2020 2020 2020 2020 2020 202f 2073               / s
-000096b0: 656c 662e 656e 6572 6779 2e65 6c65 6d65  elf.energy.eleme
-000096c0: 6e74 5f73 697a 6528 290a 2020 2020 2020  nt_size().      
-000096d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000096e0: 2020 2020 7365 6c66 2e5f 6261 7463 685f      self._batch_
-000096f0: 7369 7a65 203d 206d 696e 2831 3032 342c  size = min(1024,
-00009700: 2073 656c 662e 5f62 6174 6368 5f73 697a   self._batch_siz
-00009710: 6529 0a0a 2020 2020 2020 2020 2323 2077  e)..        ## w
-00009720: 6865 7468 6572 2074 6f20 7573 6520 626f  hether to use bo
-00009730: 6f74 7374 7261 7020 746f 2065 7374 696d  otstrap to estim
-00009740: 6174 6520 7468 6520 756e 6365 7274 6169  ate the uncertai
-00009750: 6e74 7920 6f66 2074 6865 2063 616c 6375  nty of the calcu
-00009760: 6c61 7465 6420 6672 6565 2065 6e65 7267  lated free energ
-00009770: 6965 730a 2020 2020 2020 2020 2323 2062  ies.        ## b
-00009780: 6f6f 7473 7472 6170 206e 6565 6473 2074  ootstrap needs t
-00009790: 6f20 6265 2061 2062 6f6f 6c65 616e 0a20  o be a boolean. 
-000097a0: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-000097b0: 696e 7374 616e 6365 2862 6f6f 7473 7472  instance(bootstr
-000097c0: 6170 2c20 626f 6f6c 293a 0a20 2020 2020  ap, bool):.     
-000097d0: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
-000097e0: 6545 7272 6f72 2822 626f 6f74 7374 7261  eError("bootstra
-000097f0: 7020 6861 7320 746f 2062 6520 6120 626f  p has to be a bo
-00009800: 6f6c 6561 6e2e 2229 0a20 2020 2020 2020  olean.").       
-00009810: 2073 656c 662e 626f 6f74 7374 7261 7020   self.bootstrap 
-00009820: 3d20 626f 6f74 7374 7261 700a 0a20 2020  = bootstrap..   
-00009830: 2020 2020 2023 2320 626c 6f63 6b20 7369       ## block si
-00009840: 7a65 2075 7365 6420 696e 2062 6c6f 636b  ze used in block
-00009850: 2062 6f6f 7473 7472 6170 7069 6e67 0a20   bootstrapping. 
-00009860: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-00009870: 696e 7374 616e 6365 2862 6f6f 7473 7472  instance(bootstr
-00009880: 6170 5f62 6c6f 636b 5f73 697a 652c 2069  ap_block_size, i
-00009890: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-000098a0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-000098b0: 2822 626f 6f74 7374 7261 705f 626c 6f63  ("bootstrap_bloc
-000098c0: 6b5f 7369 7a65 2068 6173 2074 6f20 6265  k_size has to be
-000098d0: 2061 6e20 696e 7465 6765 722e 2229 0a20   an integer."). 
-000098e0: 2020 2020 2020 2073 656c 662e 626f 6f74         self.boot
-000098f0: 7374 7261 705f 626c 6f63 6b5f 7369 7a65  strap_block_size
-00009900: 203d 2062 6f6f 7473 7472 6170 5f62 6c6f   = bootstrap_blo
-00009910: 636b 5f73 697a 650a 0a20 2020 2020 2020  ck_size..       
-00009920: 2023 2320 6e75 6d62 6572 206f 6620 7265   ## number of re
-00009930: 7065 6174 7320 696e 2062 6c6f 636b 2062  peats in block b
-00009940: 6f6f 7473 7472 6170 7069 6e67 0a20 2020  ootstrapping.   
-00009950: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
-00009960: 7374 616e 6365 2862 6f6f 7473 7472 6170  stance(bootstrap
-00009970: 5f6e 756d 5f72 6570 2c20 696e 7429 3a0a  _num_rep, int):.
-00009980: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00009990: 6520 5479 7065 4572 726f 7228 2262 6f6f  e TypeError("boo
-000099a0: 7473 7472 6170 5f6e 756d 5f72 6570 2068  tstrap_num_rep h
-000099b0: 6173 2074 6f20 6265 2061 6e20 696e 7465  as to be an inte
-000099c0: 6765 722e 2229 0a20 2020 2020 2020 2073  ger.").        s
-000099d0: 656c 662e 626f 6f74 7374 7261 705f 6e75  elf.bootstrap_nu
-000099e0: 6d5f 7265 7020 3d20 626f 6f74 7374 7261  m_rep = bootstra
-000099f0: 705f 6e75 6d5f 7265 700a 0a20 2020 2020  p_num_rep..     
-00009a00: 2020 2023 2320 7768 6574 6865 7220 746f     ## whether to
-00009a10: 2070 7269 6e74 2074 6865 2064 6574 6169   print the detai
-00009a20: 6c65 6420 696e 666f 726d 6174 696f 6e20  led information 
-00009a30: 6f66 2073 6f6c 7669 6e67 204d 4241 5220  of solving MBAR 
-00009a40: 6571 7561 7469 6f6e 730a 2020 2020 2020  equations.      
-00009a50: 2020 2323 2076 6572 626f 7365 206e 6565    ## verbose nee
-00009a60: 6473 2074 6f20 6265 2061 2062 6f6f 6c65  ds to be a boole
-00009a70: 616e 0a20 2020 2020 2020 2069 6620 6e6f  an.        if no
-00009a80: 7420 6973 696e 7374 616e 6365 2876 6572  t isinstance(ver
-00009a90: 626f 7365 2c20 626f 6f6c 293a 0a20 2020  bose, bool):.   
-00009aa0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-00009ab0: 7970 6545 7272 6f72 2822 7665 7262 6f73  ypeError("verbos
-00009ac0: 6520 6861 7320 746f 2062 6520 6120 626f  e has to be a bo
-00009ad0: 6f6c 6561 6e2e 2229 0a20 2020 2020 2020  olean.").       
-00009ae0: 2073 656c 662e 7665 7262 6f73 6520 3d20   self.verbose = 
-00009af0: 7665 7262 6f73 650a 0a20 2020 2020 2020  verbose..       
-00009b00: 2023 2320 6d65 7468 6f64 2075 7365 6420   ## method used 
-00009b10: 746f 2073 6f6c 7665 2074 6865 204d 4241  to solve the MBA
-00009b20: 5220 6571 7561 7469 6f6e 0a20 2020 2020  R equation.     
-00009b30: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-00009b40: 616e 6365 286d 6574 686f 642c 2073 7472  ance(method, str
-00009b50: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00009b60: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
-00009b70: 6d65 7468 6f64 2068 6173 2074 6f20 6265  method has to be
-00009b80: 2061 2073 7472 696e 672e 2229 0a20 2020   a string.").   
-00009b90: 2020 2020 2069 6620 6d65 7468 6f64 206e       if method n
-00009ba0: 6f74 2069 6e20 5b22 4e65 7774 6f6e 222c  ot in ["Newton",
-00009bb0: 2022 4c2d 4246 4753 2d42 225d 3a0a 2020   "L-BFGS-B"]:.  
-00009bc0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00009bd0: 5661 6c75 6545 7272 6f72 2822 6d65 7468  ValueError("meth
-00009be0: 6f64 2068 6173 2074 6f20 6265 204e 6577  od has to be New
-00009bf0: 746f 6e20 6f72 204c 2d42 4647 532d 422e  ton or L-BFGS-B.
-00009c00: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00009c10: 6d65 7468 6f64 203d 206d 6574 686f 640a  method = method.
-00009c20: 0a20 2020 2020 2020 2023 2320 736f 6c76  .        ## solv
-00009c30: 6520 7468 6520 4d42 4152 2065 7175 6174  e the MBAR equat
-00009c40: 696f 6e0a 2020 2020 2020 2020 6966 2073  ion.        if s
-00009c50: 656c 662e 626f 6f74 7374 7261 7020 6973  elf.bootstrap is
-00009c60: 2046 616c 7365 3a0a 2020 2020 2020 2020   False:.        
-00009c70: 2020 2020 6446 5f69 6e69 7420 3d20 7365      dF_init = se
-00009c80: 6c66 2e65 6e65 7267 792e 6e65 775f 7a65  lf.energy.new_ze
-00009c90: 726f 7328 7365 6c66 2e4d 202d 2031 290a  ros(self.M - 1).
-00009ca0: 2020 2020 2020 2020 2020 2020 6446 203d              dF =
-00009cb0: 205f 736f 6c76 655f 6d62 6172 280a 2020   _solve_mbar(.  
-00009cc0: 2020 2020 2020 2020 2020 2020 2020 6446                dF
-00009cd0: 5f69 6e69 742e 746f 2873 656c 662e 6465  _init.to(self.de
-00009ce0: 7669 6365 292c 0a20 2020 2020 2020 2020  vice),.         
-00009cf0: 2020 2020 2020 2073 656c 662e 656e 6572         self.ener
-00009d00: 6779 2e74 6f28 7365 6c66 2e64 6576 6963  gy.to(self.devic
-00009d10: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00009d20: 2020 2020 7365 6c66 2e6e 756d 5f63 6f6e      self.num_con
-00009d30: 662e 746f 2873 656c 662e 6465 7669 6365  f.to(self.device
-00009d40: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00009d50: 2020 2073 656c 662e 6d65 7468 6f64 2c0a     self.method,.
-00009d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d70: 7365 6c66 2e5f 6261 7463 685f 7369 7a65  self._batch_size
-00009d80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00009d90: 2020 7665 7262 6f73 653d 7365 6c66 2e76    verbose=self.v
-00009da0: 6572 626f 7365 2c0a 2020 2020 2020 2020  erbose,.        
-00009db0: 2020 2020 292e 6370 7528 290a 0a20 2020      ).cpu()..   
-00009dc0: 2020 2020 2020 2020 2023 2320 7368 6966           ## shif
-00009dd0: 7420 7365 6c66 2e5f 4620 7375 6368 2074  t self._F such t
-00009de0: 6861 7420 5c73 756d 5f69 2046 5b69 5d2a  hat \sum_i F[i]*
-00009df0: 6e75 6d5f 636f 6e66 5b69 5d20 3d20 300a  num_conf[i] = 0.
-00009e00: 2020 2020 2020 2020 2020 2020 4620 3d20              F = 
-00009e10: 746f 7263 682e 6361 7428 5b64 462e 6e65  torch.cat([dF.ne
-00009e20: 775f 7a65 726f 7328 3129 2c20 6446 5d29  w_zeros(1), dF])
-00009e30: 0a20 2020 2020 2020 2020 2020 2070 6920  .            pi 
-00009e40: 3d20 7365 6c66 2e6e 756d 5f63 6f6e 6620  = self.num_conf 
-00009e50: 2f20 7365 6c66 2e4e 0a20 2020 2020 2020  / self.N.       
-00009e60: 2020 2020 2073 656c 662e 5f46 203d 2046       self._F = F
-00009e70: 202d 2074 6f72 6368 2e73 756d 2870 6920   - torch.sum(pi 
-00009e80: 2a20 4629 0a0a 2020 2020 2020 2020 2020  * F)..          
-00009e90: 2020 6220 3d20 2d73 656c 662e 5f46 202d    b = -self._F -
-00009ea0: 2074 6f72 6368 2e6c 6f67 2873 656c 662e   torch.log(self.
-00009eb0: 6e75 6d5f 636f 6e66 290a 2020 2020 2020  num_conf).      
-00009ec0: 2020 2020 2020 7365 6c66 2e5f 6c6f 675f        self._log_
-00009ed0: 7072 6f62 5f6d 6978 203d 2074 6f72 6368  prob_mix = torch
-00009ee0: 2e6c 6f67 7375 6d65 7870 282d 2873 656c  .logsumexp(-(sel
-00009ef0: 662e 656e 6572 6779 202b 2062 5b3a 2c20  f.energy + b[:, 
-00009f00: 4e6f 6e65 5d29 2c20 6469 6d3d 3029 0a20  None]), dim=0). 
-00009f10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009f20: 5f6c 6f67 5f6d 7520 3d20 2d73 656c 662e  _log_mu = -self.
-00009f30: 6c6f 675f 7072 6f62 5f6d 6978 0a0a 2020  log_prob_mix..  
-00009f40: 2020 2020 2020 2020 2020 2323 2043 6f6d            ## Com
-00009f50: 7075 7465 2073 656c 662e 5f46 5f63 6f76  pute self._F_cov
-00009f60: 2075 6e64 6572 2074 6865 2063 6f6e 7374   under the const
-00009f70: 7261 696e 7420 7468 6174 205c 7375 6d5f  raint that \sum_
-00009f80: 6920 465b 695d 2a6e 756d 5f63 6f6e 665b  i F[i]*num_conf[
-00009f90: 695d 203d 2030 0a0a 2020 2020 2020 2020  i] = 0..        
-00009fa0: 2020 2020 2323 2054 6865 7265 2061 7265      ## There are
-00009fb0: 2074 776f 2077 6179 7320 746f 2063 6f6d   two ways to com
-00009fc0: 7075 7465 2074 6865 2063 6f76 6172 6961  pute the covaria
-00009fd0: 6e63 6520 6d61 7472 6978 206f 6620 7365  nce matrix of se
-00009fe0: 6c66 2e5f 460a 2020 2020 2020 2020 2020  lf._F.          
-00009ff0: 2020 2323 2053 6565 2065 7175 6174 696f    ## See equatio
-0000a000: 6e20 342e 3220 616e 6420 362e 3420 696e  n 4.2 and 6.4 in
-0000a010: 2074 6865 2066 6f6c 6c6f 7769 6e67 2070   the following p
-0000a020: 6170 6572 2066 6f72 2064 6574 6169 6c73  aper for details
-0000a030: 0a20 2020 2020 2020 2020 2020 2023 2320  .            ## 
-0000a040: 224b 6f6e 672c 2041 2e2c 2065 7420 616c  "Kong, A., et al
-0000a050: 2e20 2241 2074 6865 6f72 7920 6f66 2073  . "A theory of s
-0000a060: 7461 7469 7374 6963 616c 206d 6f64 656c  tatistical model
-0000a070: 7320 666f 7220 4d6f 6e74 6520 4361 726c  s for Monte Carl
-0000a080: 6f20 696e 7465 6772 6174 696f 6e2e 220a  o integration.".
-0000a090: 2020 2020 2020 2020 2020 2020 2323 204a              ## J
-0000a0a0: 6f75 726e 616c 206f 6620 7468 6520 526f  ournal of the Ro
-0000a0b0: 7961 6c20 5374 6174 6973 7469 6361 6c20  yal Statistical 
-0000a0c0: 536f 6369 6574 7920 5365 7269 6573 2042  Society Series B
-0000a0d0: 3a20 5374 6174 6973 7469 6361 6c20 4d65  : Statistical Me
-0000a0e0: 7468 6f64 6f6c 6f67 7920 3635 2e33 0a20  thodology 65.3. 
-0000a0f0: 2020 2020 2020 2020 2020 2023 2320 2832             ## (2
-0000a100: 3030 3329 3a20 3538 352d 3630 342e 2220  003): 585-604." 
-0000a110: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
-0000a120: 3130 2e31 3131 312f 3134 3637 2d39 3836  10.1111/1467-986
-0000a130: 382e 3030 3430 340a 0a20 2020 2020 2020  8.00404..       
-0000a140: 2020 2020 2023 2320 5468 6520 6669 7273       ## The firs
-0000a150: 7420 7761 7920 6173 2073 686f 776e 2069  t way as shown i
-0000a160: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
-0000a170: 7573 6573 2065 7175 6174 696f 6e20 342e  uses equation 4.
-0000a180: 320a 2020 2020 2020 2020 2020 2020 2323  2.            ##
-0000a190: 2074 6869 7320 6d65 7468 6f64 2069 7320   this method is 
-0000a1a0: 6d6f 7265 2067 656e 6572 616c 2074 6861  more general tha
-0000a1b0: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
-0000a1c0: 6d65 7468 6f64 2c20 6d65 616e 696e 6720  method, meaning 
-0000a1d0: 7468 6174 0a20 2020 2020 2020 2020 2020  that.           
-0000a1e0: 2023 2320 6974 2063 616e 2061 6c73 6f20   ## it can also 
-0000a1f0: 6265 2075 7365 6420 746f 2063 6f6d 7075  be used to compu
-0000a200: 7465 2063 6f76 6172 6961 6e63 6520 6d61  te covariance ma
-0000a210: 7472 6978 2066 6f72 2070 6572 7475 7262  trix for perturb
-0000a220: 6564 2073 7461 7465 732e 0a20 2020 2020  ed states..     
-0000a230: 2020 2020 2020 2023 2320 5468 6572 6566         ## Theref
-0000a240: 6f72 6520 6974 2069 7320 7573 6564 2068  ore it is used h
-0000a250: 6572 652e 0a20 2020 2020 2020 2020 2020  ere..           
-0000a260: 2073 656c 662e 5020 3d20 746f 7263 682e   self.P = torch.
-0000a270: 6578 7028 0a20 2020 2020 2020 2020 2020  exp(.           
-0000a280: 2020 2020 202d 2873 656c 662e 656e 6572       -(self.ener
-0000a290: 6779 202d 2073 656c 662e 5f46 5b3a 2c20  gy - self._F[:, 
-0000a2a0: 4e6f 6e65 5d20 2b20 7365 6c66 2e5f 6c6f  None] + self._lo
-0000a2b0: 675f 7072 6f62 5f6d 6978 290a 2020 2020  g_prob_mix).    
-0000a2c0: 2020 2020 2020 2020 292e 7428 290a 2020          ).t().  
-0000a2d0: 2020 2020 2020 2020 2020 5720 3d20 746f            W = to
-0000a2e0: 7263 682e 6469 6167 2873 656c 662e 6e75  rch.diag(self.nu
-0000a2f0: 6d5f 636f 6e66 290a 2020 2020 2020 2020  m_conf).        
-0000a300: 2020 2020 512c 2052 203d 2074 6f72 6368      Q, R = torch
-0000a310: 2e6c 696e 616c 672e 7172 2873 656c 662e  .linalg.qr(self.
-0000a320: 5029 0a20 2020 2020 2020 2020 2020 2041  P).            A
-0000a330: 203d 2074 6f72 6368 2e65 7965 2873 656c   = torch.eye(sel
-0000a340: 662e 4d2c 2064 6576 6963 653d 572e 6465  f.M, device=W.de
-0000a350: 7669 6365 2920 2d20 5220 4020 5720 4020  vice) - R @ W @ 
-0000a360: 522e 540a 2020 2020 2020 2020 2020 2020  R.T.            
-0000a370: 7365 6c66 2e5f 465f 636f 7620 3d20 522e  self._F_cov = R.
-0000a380: 5420 4020 746f 7263 682e 6c69 6e61 6c67  T @ torch.linalg
-0000a390: 2e70 696e 7628 412c 2068 6572 6d69 7469  .pinv(A, hermiti
-0000a3a0: 616e 3d54 7275 652c 2072 746f 6c3d 3165  an=True, rtol=1e
-0000a3b0: 2d38 2920 4020 520a 0a20 2020 2020 2020  -8) @ R..       
-0000a3c0: 2020 2020 2023 2023 2054 6865 2073 6563       # # The sec
-0000a3d0: 6f6e 6420 7761 7920 7573 6573 2065 7175  ond way uses equ
-0000a3e0: 6174 696f 6e20 362e 340a 2020 2020 2020  ation 6.4.      
-0000a3f0: 2020 2020 2020 2320 6966 2073 656c 662e        # if self.
-0000a400: 5f62 6174 6368 5f73 697a 6520 6973 204e  _batch_size is N
-0000a410: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000a420: 2023 2020 2020 2048 203d 205f 636f 6d70   #     H = _comp
-0000a430: 7574 655f 6865 7373 6961 6e5f 6c6f 675f  ute_hessian_log_
-0000a440: 6c69 6b65 6c69 686f 6f64 5f6f 665f 4628  likelihood_of_F(
-0000a450: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-0000a460: 2020 2020 2020 2073 656c 662e 5f46 2c20         self._F, 
-0000a470: 7365 6c66 2e65 6e65 7267 792c 2073 656c  self.energy, sel
-0000a480: 662e 6e75 6d5f 636f 6e66 0a20 2020 2020  f.num_conf.     
-0000a490: 2020 2020 2020 2023 2020 2020 2029 0a20         #     ). 
-0000a4a0: 2020 2020 2020 2020 2020 2023 2065 6c73             # els
-0000a4b0: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
-0000a4c0: 2020 2020 2048 203d 205f 636f 6d70 7574       H = _comput
-0000a4d0: 655f 6865 7373 6961 6e5f 6c6f 675f 6c69  e_hessian_log_li
-0000a4e0: 6b65 6c69 686f 6f64 5f6f 665f 465f 696e  kelihood_of_F_in
-0000a4f0: 5f62 6174 6368 280a 2020 2020 2020 2020  _batch(.        
-0000a500: 2020 2020 2320 2020 2020 2020 2020 7365      #         se
-0000a510: 6c66 2e5f 462c 2073 656c 662e 656e 6572  lf._F, self.ener
-0000a520: 6779 2c20 7365 6c66 2e6e 756d 5f63 6f6e  gy, self.num_con
-0000a530: 662c 2073 656c 662e 5f62 6174 6368 5f73  f, self._batch_s
-0000a540: 697a 650a 2020 2020 2020 2020 2020 2020  ize.            
-0000a550: 2320 2020 2020 290a 2020 2020 2020 2020  #     ).        
-0000a560: 2020 2020 2320 4870 203d 2048 2e6e 6577      # Hp = H.new
-0000a570: 5f7a 6572 6f73 2828 7365 6c66 2e4d 202b  _zeros((self.M +
-0000a580: 2031 2c20 7365 6c66 2e4d 202b 2031 2929   1, self.M + 1))
-0000a590: 2e63 7075 2829 0a20 2020 2020 2020 2020  .cpu().         
-0000a5a0: 2020 2023 2048 705b 3020 3a20 7365 6c66     # Hp[0 : self
-0000a5b0: 2e4d 2c20 3020 3a20 7365 6c66 2e4d 5d20  .M, 0 : self.M] 
-0000a5c0: 3d20 480a 2020 2020 2020 2020 2020 2020  = H.            
-0000a5d0: 2320 4870 5b73 656c 662e 4d2c 2030 203a  # Hp[self.M, 0 :
-0000a5e0: 2073 656c 662e 4d5d 203d 202d 7365 6c66   self.M] = -self
-0000a5f0: 2e6e 756d 5f63 6f6e 660a 2020 2020 2020  .num_conf.      
-0000a600: 2020 2020 2020 2320 4870 5b30 203a 2073        # Hp[0 : s
-0000a610: 656c 662e 4d2c 2073 656c 662e 4d5d 203d  elf.M, self.M] =
-0000a620: 202d 7365 6c66 2e6e 756d 5f63 6f6e 660a   -self.num_conf.
-0000a630: 2020 2020 2020 2020 2020 2020 2320 4870              # Hp
-0000a640: 5b73 656c 662e 4d2c 2073 656c 662e 4d5d  [self.M, self.M]
-0000a650: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
-0000a660: 2023 2073 656c 662e 5f46 5f63 6f76 203d   # self._F_cov =
-0000a670: 2074 6f72 6368 2e6c 696e 616c 672e 696e   torch.linalg.in
-0000a680: 7628 2d48 7029 5b30 203a 2073 656c 662e  v(-Hp)[0 : self.
-0000a690: 4d2c 2030 203a 2073 656c 662e 4d5d 0a20  M, 0 : self.M]. 
-0000a6a0: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
-0000a6b0: 662e 5f46 5f63 6f76 203d 2073 656c 662e  f._F_cov = self.
-0000a6c0: 5f46 5f63 6f76 202d 2074 6f72 6368 2e64  _F_cov - torch.d
-0000a6d0: 6961 6728 3120 2f20 7365 6c66 2e6e 756d  iag(1 / self.num
-0000a6e0: 5f63 6f6e 6629 202b 2031 202f 2073 656c  _conf) + 1 / sel
-0000a6f0: 662e 4e0a 0a20 2020 2020 2020 2020 2020  f.N..           
-0000a700: 2073 656c 662e 5f46 5f73 7464 203d 2073   self._F_std = s
-0000a710: 656c 662e 5f46 5f63 6f76 2e64 6961 676f  elf._F_cov.diago
-0000a720: 6e61 6c28 292e 7371 7274 2829 0a0a 2020  nal().sqrt()..  
-0000a730: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000a740: 4465 6c74 6146 203d 2073 656c 662e 5f46  DeltaF = self._F
-0000a750: 5b4e 6f6e 652c 203a 5d20 2d20 7365 6c66  [None, :] - self
-0000a760: 2e5f 465b 3a2c 204e 6f6e 655d 0a20 2020  ._F[:, None].   
-0000a770: 2020 2020 2020 2020 2073 656c 662e 5f44           self._D
-0000a780: 656c 7461 465f 636f 7620 3d20 280a 2020  eltaF_cov = (.  
-0000a790: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000a7a0: 6c66 2e5f 465f 636f 762e 6469 6167 2829  lf._F_cov.diag()
-0000a7b0: 5b3a 2c20 4e6f 6e65 5d0a 2020 2020 2020  [:, None].      
-0000a7c0: 2020 2020 2020 2020 2020 2b20 7365 6c66            + self
-0000a7d0: 2e5f 465f 636f 762e 6469 6167 2829 5b4e  ._F_cov.diag()[N
-0000a7e0: 6f6e 652c 203a 5d0a 2020 2020 2020 2020  one, :].        
-0000a7f0: 2020 2020 2020 2020 2d20 3220 2a20 7365          - 2 * se
-0000a800: 6c66 2e5f 465f 636f 760a 2020 2020 2020  lf._F_cov.      
-0000a810: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000a820: 2020 2020 7365 6c66 2e5f 4465 6c74 6146      self._DeltaF
-0000a830: 5f73 7464 203d 2073 656c 662e 5f44 656c  _std = self._Del
-0000a840: 7461 465f 636f 762e 7371 7274 2829 0a0a  taF_cov.sqrt()..
-0000a850: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
-0000a860: 662e 626f 6f74 7374 7261 7020 6973 2054  f.bootstrap is T
-0000a870: 7275 653a 0a20 2020 2020 2020 2020 2020  rue:.           
-0000a880: 2064 4673 203d 205b 5d0a 2020 2020 2020   dFs = [].      
-0000a890: 2020 2020 2020 6c6f 675f 7072 6f62 5f6d        log_prob_m
-0000a8a0: 6978 203d 205b 5d0a 2020 2020 2020 2020  ix = [].        
-0000a8b0: 2020 2020 6446 5f69 6e69 7420 3d20 7365      dF_init = se
-0000a8c0: 6c66 2e65 6e65 7267 792e 6e65 775f 7a65  lf.energy.new_ze
-0000a8d0: 726f 7328 7365 6c66 2e4d 202d 2031 290a  ros(self.M - 1).
-0000a8e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a8f0: 2e5f 636f 6e66 5f69 6478 203d 205b 5d0a  ._conf_idx = [].
-0000a900: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000a910: 5f20 696e 2072 616e 6765 2873 656c 662e  _ in range(self.
-0000a920: 626f 6f74 7374 7261 705f 6e75 6d5f 7265  bootstrap_num_re
-0000a930: 7029 3a0a 2020 2020 2020 2020 2020 2020  p):.            
-0000a940: 2020 2020 636f 6e66 5f69 6478 203d 205f      conf_idx = _
-0000a950: 626f 6f74 7374 7261 705f 636f 6e66 5f69  bootstrap_conf_i
-0000a960: 6478 280a 2020 2020 2020 2020 2020 2020  dx(.            
-0000a970: 2020 2020 2020 2020 7365 6c66 2e6e 756d          self.num
-0000a980: 5f63 6f6e 662e 746f 2874 6f72 6368 2e69  _conf.to(torch.i
-0000a990: 6e74 3634 292c 2073 656c 662e 626f 6f74  nt64), self.boot
-0000a9a0: 7374 7261 705f 626c 6f63 6b5f 7369 7a65  strap_block_size
-0000a9b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a9c0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000a9d0: 2020 2064 4620 3d20 5f73 6f6c 7665 5f6d     dF = _solve_m
-0000a9e0: 6261 7228 0a20 2020 2020 2020 2020 2020  bar(.           
-0000a9f0: 2020 2020 2020 2020 2064 465f 696e 6974           dF_init
-0000aa00: 2e74 6f28 7365 6c66 2e64 6576 6963 6529  .to(self.device)
-0000aa10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000aa20: 2020 2020 2020 7365 6c66 2e65 6e65 7267        self.energ
-0000aa30: 795b 3a2c 2063 6f6e 665f 6964 785d 2e74  y[:, conf_idx].t
-0000aa40: 6f28 7365 6c66 2e64 6576 6963 6529 2c0a  o(self.device),.
-0000aa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa60: 2020 2020 7365 6c66 2e6e 756d 5f63 6f6e      self.num_con
-0000aa70: 662e 746f 2873 656c 662e 6465 7669 6365  f.to(self.device
-0000aa80: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000aa90: 2020 2020 2020 2073 656c 662e 6d65 7468         self.meth
-0000aaa0: 6f64 2c0a 2020 2020 2020 2020 2020 2020  od,.            
-0000aab0: 2020 2020 2020 2020 7365 6c66 2e5f 6261          self._ba
-0000aac0: 7463 685f 7369 7a65 2c0a 2020 2020 2020  tch_size,.      
-0000aad0: 2020 2020 2020 2020 2020 2020 2020 7665                ve
-0000aae0: 7262 6f73 653d 7365 6c66 2e76 6572 626f  rbose=self.verbo
-0000aaf0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-0000ab00: 2020 2020 292e 6370 7528 290a 2020 2020      ).cpu().    
-0000ab10: 2020 2020 2020 2020 2020 2020 6446 5f69              dF_i
-0000ab20: 6e69 7420 3d20 6446 0a20 2020 2020 2020  nit = dF.       
-0000ab30: 2020 2020 2020 2020 2064 4673 2e61 7070           dFs.app
-0000ab40: 656e 6428 6446 2e63 6c6f 6e65 2829 290a  end(dF.clone()).
-0000ab50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ab60: 2046 203d 2074 6f72 6368 2e63 6174 285b   F = torch.cat([
-0000ab70: 6446 2e6e 6577 5f7a 6572 6f73 2831 292c  dF.new_zeros(1),
-0000ab80: 2064 465d 290a 2020 2020 2020 2020 2020   dF]).          
-0000ab90: 2020 2020 2020 2323 2073 6869 6674 2046        ## shift F
-0000aba0: 2073 7563 6820 7468 6174 205c 7375 6d5f   such that \sum_
-0000abb0: 6920 465b 695d 2a6e 756d 5f63 6f6e 665b  i F[i]*num_conf[
-0000abc0: 695d 203d 2030 0a20 2020 2020 2020 2020  i] = 0.         
-0000abd0: 2020 2020 2020 2070 6920 3d20 7365 6c66         pi = self
-0000abe0: 2e6e 756d 5f63 6f6e 6620 2f20 7365 6c66  .num_conf / self
-0000abf0: 2e4e 0a20 2020 2020 2020 2020 2020 2020  .N.             
-0000ac00: 2020 2046 203d 2046 202d 2074 6f72 6368     F = F - torch
-0000ac10: 2e73 756d 2870 6920 2a20 4629 0a0a 2020  .sum(pi * F)..  
-0000ac20: 2020 2020 2020 2020 2020 2020 2020 6220                b 
-0000ac30: 3d20 2d46 202d 2074 6f72 6368 2e6c 6f67  = -F - torch.log
-0000ac40: 2873 656c 662e 6e75 6d5f 636f 6e66 202f  (self.num_conf /
-0000ac50: 2073 656c 662e 4e29 0a20 2020 2020 2020   self.N).       
-0000ac60: 2020 2020 2020 2020 206c 6f67 5f70 726f           log_pro
-0000ac70: 625f 6d69 782e 6170 7065 6e64 280a 2020  b_mix.append(.  
-0000ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac90: 2020 746f 7263 682e 6c6f 6773 756d 6578    torch.logsumex
-0000aca0: 7028 2d28 7365 6c66 2e65 6e65 7267 795b  p(-(self.energy[
-0000acb0: 3a2c 2063 6f6e 665f 6964 785d 202b 2062  :, conf_idx] + b
-0000acc0: 5b3a 2c20 4e6f 6e65 5d29 2c20 6469 6d3d  [:, None]), dim=
-0000acd0: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
-0000ace0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000acf0: 2020 2020 2073 656c 662e 5f63 6f6e 665f       self._conf_
-0000ad00: 6964 782e 6170 7065 6e64 2863 6f6e 665f  idx.append(conf_
-0000ad10: 6964 7829 0a0a 2020 2020 2020 2020 2020  idx)..          
-0000ad20: 2020 6446 203d 2074 6f72 6368 2e73 7461    dF = torch.sta
-0000ad30: 636b 2864 4673 2c20 6469 6d3d 3129 0a20  ck(dFs, dim=1). 
-0000ad40: 2020 2020 2020 2020 2020 2046 203d 2074             F = t
-0000ad50: 6f72 6368 2e63 6174 285b 6446 2e6e 6577  orch.cat([dF.new
-0000ad60: 5f7a 6572 6f73 2831 2c20 6446 2e73 6861  _zeros(1, dF.sha
-0000ad70: 7065 5b31 5d29 2c20 6446 5d2c 2064 696d  pe[1]), dF], dim
-0000ad80: 3d30 290a 0a20 2020 2020 2020 2020 2020  =0)..           
-0000ad90: 2023 2320 7368 6966 7420 4620 7375 6368   ## shift F such
-0000ada0: 2074 6861 7420 5c73 756d 5f69 2046 5b69   that \sum_i F[i
-0000adb0: 5d2a 6e75 6d5f 636f 6e66 5b69 5d20 3d20  ]*num_conf[i] = 
-0000adc0: 300a 2020 2020 2020 2020 2020 2020 7069  0.            pi
-0000add0: 203d 2073 656c 662e 6e75 6d5f 636f 6e66   = self.num_conf
-0000ade0: 202f 2073 656c 662e 4e0a 2020 2020 2020   / self.N.      
-0000adf0: 2020 2020 2020 7365 6c66 2e5f 465f 626f        self._F_bo
-0000ae00: 6f74 7374 7261 7020 3d20 4620 2d20 746f  otstrap = F - to
-0000ae10: 7263 682e 7375 6d28 7069 5b3a 2c20 4e6f  rch.sum(pi[:, No
-0000ae20: 6e65 5d20 2a20 462c 2064 696d 3d30 290a  ne] * F, dim=0).
-0000ae30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000ae40: 662e 5f46 203d 2074 6f72 6368 2e6d 6561  f._F = torch.mea
-0000ae50: 6e28 7365 6c66 2e5f 465f 626f 6f74 7374  n(self._F_bootst
-0000ae60: 7261 702c 2064 696d 3d31 290a 2020 2020  rap, dim=1).    
-0000ae70: 2020 2020 2020 2020 7365 6c66 2e5f 465f          self._F_
-0000ae80: 7374 6420 3d20 746f 7263 682e 7374 6428  std = torch.std(
-0000ae90: 7365 6c66 2e5f 465f 626f 6f74 7374 7261  self._F_bootstra
-0000aea0: 702c 2064 696d 3d31 290a 2020 2020 2020  p, dim=1).      
-0000aeb0: 2020 2020 2020 7365 6c66 2e5f 465f 636f        self._F_co
-0000aec0: 7620 3d20 746f 7263 682e 636f 7628 7365  v = torch.cov(se
-0000aed0: 6c66 2e5f 465f 626f 6f74 7374 7261 7029  lf._F_bootstrap)
-0000aee0: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000aef0: 6c66 2e5f 6c6f 675f 7072 6f62 5f6d 6978  lf._log_prob_mix
-0000af00: 203d 2074 6f72 6368 2e73 7461 636b 286c   = torch.stack(l
-0000af10: 6f67 5f70 726f 625f 6d69 782c 2064 696d  og_prob_mix, dim
-0000af20: 3d30 290a 2020 2020 2020 2020 2020 2020  =0).            
-0000af30: 4465 6c74 6146 203d 2064 465b 4e6f 6e65  DeltaF = dF[None
-0000af40: 2c20 3a2c 203a 5d20 2d20 6446 5b3a 2c20  , :, :] - dF[:, 
-0000af50: 4e6f 6e65 2c20 3a5d 0a20 2020 2020 2020  None, :].       
-0000af60: 2020 2020 2073 656c 662e 5f44 656c 7461       self._Delta
-0000af70: 4620 3d20 746f 7263 682e 6d65 616e 2844  F = torch.mean(D
-0000af80: 656c 7461 462c 2064 696d 3d32 290a 2020  eltaF, dim=2).  
-0000af90: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000afa0: 4465 6c74 6146 5f73 7464 203d 2074 6f72  DeltaF_std = tor
-0000afb0: 6368 2e73 7464 2844 656c 7461 462c 2064  ch.std(DeltaF, d
-0000afc0: 696d 3d32 290a 0a20 2020 2040 7072 6f70  im=2)..    @prop
-0000afd0: 6572 7479 0a20 2020 2064 6566 2046 2873  erty.    def F(s
-0000afe0: 656c 6629 202d 3e20 6e70 2e6e 6461 7272  elf) -> np.ndarr
-0000aff0: 6179 3a0a 2020 2020 2020 2020 2222 2246  ay:.        """F
-0000b000: 7265 6520 656e 6572 6769 6573 206f 6620  ree energies of 
-0000b010: 7468 6520 7374 6174 6573 2075 6e64 6572  the states under
-0000b020: 2074 6865 2063 6f6e 7374 7261 696e 7420   the constraint 
-0000b030: 3a6d 6174 683a 605c 7375 6d5f 7b6b 3d31  :math:`\sum_{k=1
-0000b040: 7d5e 7b4d 7d20 4e5f 6b20 2a20 465f 6b20  }^{M} N_k * F_k 
-0000b050: 3d20 3060 2c0a 2020 2020 2020 2020 7768  = 0`,.        wh
-0000b060: 6572 6520 3a6d 6174 683a 604e 5f6b 6020  ere :math:`N_k` 
-0000b070: 6973 2074 6865 206e 756d 6265 7220 6f66  is the number of
-0000b080: 2063 6f6e 666f 726d 6174 696f 6e73 2073   conformations s
-0000b090: 616d 706c 6564 2066 726f 6d20 7374 6174  ampled from stat
-0000b0a0: 6520 6b2e 0a20 2020 2020 2020 2022 2222  e k..        """
-0000b0b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000b0c0: 7365 6c66 2e5f 462e 6370 7528 292e 6e75  self._F.cpu().nu
-0000b0d0: 6d70 7928 290a 0a20 2020 2040 7072 6f70  mpy()..    @prop
-0000b0e0: 6572 7479 0a20 2020 2064 6566 2046 5f73  erty.    def F_s
-0000b0f0: 7464 2873 656c 6629 202d 3e20 6e70 2e6e  td(self) -> np.n
-0000b100: 6461 7272 6179 3a0a 2020 2020 2020 2020  darray:.        
-0000b110: 2222 2253 7461 6e64 6172 6420 6465 7669  """Standard devi
-0000b120: 6174 696f 6e20 6f66 2074 6865 2066 7265  ation of the fre
-0000b130: 6520 656e 6572 6769 6573 206f 6620 7468  e energies of th
-0000b140: 6520 7374 6174 6573 2075 6e64 6572 2074  e states under t
-0000b150: 6865 2063 6f6e 7374 7261 696e 740a 2020  he constraint.  
-0000b160: 2020 2020 2020 3a6d 6174 683a 605c 7375        :math:`\su
-0000b170: 6d5f 7b6b 3d31 7d5e 7b4d 7d20 4e5f 6b20  m_{k=1}^{M} N_k 
-0000b180: 2a20 465f 6b20 3d20 3060 2c0a 2020 2020  * F_k = 0`,.    
-0000b190: 2020 2020 7768 6572 6520 3a6d 6174 683a      where :math:
-0000b1a0: 604e 5f6b 6020 6973 2074 6865 206e 756d  `N_k` is the num
-0000b1b0: 6265 7220 6f66 2063 6f6e 666f 726d 6174  ber of conformat
-0000b1c0: 696f 6e73 2073 616d 706c 6564 2066 726f  ions sampled fro
-0000b1d0: 6d20 7374 6174 6520 6b2e 0a20 2020 2020  m state k..     
-0000b1e0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-0000b1f0: 6574 7572 6e20 7365 6c66 2e5f 465f 7374  eturn self._F_st
-0000b200: 642e 6370 7528 292e 6e75 6d70 7928 290a  d.cpu().numpy().
-0000b210: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000b220: 2020 2064 6566 2046 5f63 6f76 2873 656c     def F_cov(sel
-0000b230: 6629 202d 3e20 6e70 2e6e 6461 7272 6179  f) -> np.ndarray
-0000b240: 3a0a 2020 2020 2020 2020 2222 2243 6f76  :.        """Cov
-0000b250: 6172 6961 6e63 6520 6d61 7472 6978 206f  ariance matrix o
-0000b260: 6620 7468 6520 6672 6565 2065 6e65 7267  f the free energ
-0000b270: 6965 7320 6f66 2074 6865 2073 7461 7465  ies of the state
-0000b280: 7320 756e 6465 7220 7468 6520 636f 6e73  s under the cons
-0000b290: 7472 6169 6e74 0a20 2020 2020 2020 203a  traint.        :
-0000b2a0: 6d61 7468 3a60 5c73 756d 5f7b 6b3d 317d  math:`\sum_{k=1}
-0000b2b0: 5e7b 4d7d 204e 5f6b 202a 2046 5f6b 203d  ^{M} N_k * F_k =
-0000b2c0: 2030 602c 0a20 2020 2020 2020 2077 6865   0`,.        whe
-0000b2d0: 7265 203a 6d61 7468 3a60 4e5f 6b60 2069  re :math:`N_k` i
-0000b2e0: 7320 7468 6520 6e75 6d62 6572 206f 6620  s the number of 
-0000b2f0: 636f 6e66 6f72 6d61 7469 6f6e 7320 7361  conformations sa
-0000b300: 6d70 6c65 6420 6672 6f6d 2073 7461 7465  mpled from state
-0000b310: 206b 2e0a 2020 2020 2020 2020 2222 220a   k..        """.
-0000b320: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000b330: 656c 662e 5f46 5f63 6f76 2e63 7075 2829  elf._F_cov.cpu()
-0000b340: 2e6e 756d 7079 2829 0a0a 2020 2020 4070  .numpy()..    @p
-0000b350: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000b360: 4465 6c74 6146 2873 656c 6629 202d 3e20  DeltaF(self) -> 
-0000b370: 6e70 2e6e 6461 7272 6179 3a0a 2020 2020  np.ndarray:.    
-0000b380: 2020 2020 2222 2246 7265 6520 656e 6572      """Free ener
-0000b390: 6779 2064 6966 6665 7265 6e63 6520 6265  gy difference be
-0000b3a0: 7477 6565 6e20 7374 6174 6573 2e0a 2020  tween states..  
-0000b3b0: 2020 2020 2020 3a6d 6174 683a 605c 6d61        :math:`\ma
-0000b3c0: 7468 726d 7b44 656c 7461 467d 5b69 2c6a  thrm{DeltaF}[i,j
-0000b3d0: 5d60 2069 7320 7468 6520 6672 6565 2065  ]` is the free e
-0000b3e0: 6e65 7267 7920 6469 6666 6572 656e 6365  nergy difference
-0000b3f0: 2062 6574 7765 656e 2073 7461 7465 206a   between state j
-0000b400: 2061 6e64 2073 7461 7465 2069 2c0a 2020   and state i,.  
-0000b410: 2020 2020 2020 692e 652e 2c20 3a6d 6174        i.e., :mat
-0000b420: 683a 605c 6d61 7468 726d 7b44 656c 7461  h:`\mathrm{Delta
-0000b430: 467d 5b69 2c6a 5d20 3d20 465b 6a5d 202d  F}[i,j] = F[j] -
-0000b440: 2046 5b69 5d60 202e 0a20 2020 2020 2020   F[i]` ..       
-0000b450: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-0000b460: 7572 6e20 7365 6c66 2e5f 4465 6c74 6146  urn self._DeltaF
-0000b470: 2e63 7075 2829 2e6e 756d 7079 2829 0a0a  .cpu().numpy()..
-0000b480: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000b490: 2020 6465 6620 4465 6c74 6146 5f73 7464    def DeltaF_std
-0000b4a0: 2873 656c 6629 202d 3e20 6e70 2e6e 6461  (self) -> np.nda
-0000b4b0: 7272 6179 3a0a 2020 2020 2020 2020 2222  rray:.        ""
-0000b4c0: 2253 7461 6e64 6172 6420 6465 7669 6174  "Standard deviat
-0000b4d0: 696f 6e20 6f66 2074 6865 2066 7265 6520  ion of the free 
-0000b4e0: 656e 6572 6779 2064 6966 6665 7265 6e63  energy differenc
-0000b4f0: 6520 6265 7477 6565 6e20 7374 6174 6573  e between states
-0000b500: 2e0a 2020 2020 2020 2020 3a6d 6174 683a  ..        :math:
-0000b510: 605c 6d61 7468 726d 7b44 656c 7461 465f  `\mathrm{DeltaF_
-0000b520: 7374 647d 5b69 2c6a 5d60 2069 7320 7468  std}[i,j]` is th
-0000b530: 6520 7374 616e 6461 7264 2064 6576 6961  e standard devia
-0000b540: 7469 6f6e 206f 6620 7468 6520 6672 6565  tion of the free
-0000b550: 2065 6e65 7267 790a 2020 2020 2020 2020   energy.        
-0000b560: 6469 6666 6572 656e 6365 203a 6d61 7468  difference :math
-0000b570: 3a60 5c6d 6174 6872 6d7b 4465 6c74 6146  :`\mathrm{DeltaF
-0000b580: 7d5b 692c 6a5d 602e 0a20 2020 2020 2020  }[i,j]`..       
-0000b590: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-0000b5a0: 7572 6e20 7365 6c66 2e5f 4465 6c74 6146  urn self._DeltaF
-0000b5b0: 5f73 7464 2e63 7075 2829 2e6e 756d 7079  _std.cpu().numpy
-0000b5c0: 2829 0a0a 2020 2020 4070 726f 7065 7274  ()..    @propert
-0000b5d0: 790a 2020 2020 6465 6620 6c6f 675f 7072  y.    def log_pr
-0000b5e0: 6f62 5f6d 6978 2873 656c 6629 202d 3e20  ob_mix(self) -> 
-0000b5f0: 6e70 2e6e 6461 7272 6179 3a0a 2020 2020  np.ndarray:.    
-0000b600: 2020 2020 2222 2274 6865 206c 6f67 2070      """the log p
-0000b610: 726f 6261 6269 6c69 7479 2064 656e 7369  robability densi
-0000b620: 7479 206f 6620 636f 6e66 6f72 6d61 7469  ty of conformati
-0000b630: 6f6e 7320 696e 2074 6865 206d 6978 7475  ons in the mixtu
-0000b640: 7265 2064 6973 7472 6962 7574 696f 6e2e  re distribution.
-0000b650: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-0000b660: 726e 2073 656c 662e 5f6c 6f67 5f70 726f  rn self._log_pro
-0000b670: 625f 6d69 782e 6370 7528 292e 6e75 6d70  b_mix.cpu().nump
-0000b680: 7928 290a 0a20 2020 2064 6566 2063 616c  y()..    def cal
-0000b690: 6375 6c61 7465 5f66 7265 655f 656e 6572  culate_free_ener
-0000b6a0: 6769 6573 5f6f 665f 7065 7274 7572 6265  gies_of_perturbe
-0000b6b0: 645f 7374 6174 6573 2873 656c 662c 2065  d_states(self, e
-0000b6c0: 6e65 7267 795f 7065 7274 7572 6265 6429  nergy_perturbed)
-0000b6d0: 3a0a 2020 2020 2020 2020 2222 2263 616c  :.        """cal
-0000b6e0: 6375 6c61 7465 2066 7265 6520 656e 6572  culate free ener
-0000b6f0: 6769 6573 2066 6f72 2070 6572 7475 7262  gies for perturb
-0000b700: 6564 2073 7461 7465 732e 0a0a 2020 2020  ed states...    
-0000b710: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0000b720: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0000b730: 2d2d 0a20 2020 2020 2020 2065 6e65 7267  --.        energ
-0000b740: 795f 7065 7274 7572 6265 643a 2032 2d44  y_perturbed: 2-D
-0000b750: 2066 6c6f 6174 206e 6461 7272 6179 2077   float ndarray w
-0000b760: 6974 6820 7369 7a65 206f 6620 284c 2c4e  ith size of (L,N
-0000b770: 290a 2020 2020 2020 2020 2020 2020 6561  ).            ea
-0000b780: 6368 2072 6f77 206f 6620 7468 6520 656e  ch row of the en
-0000b790: 6572 6779 5f70 6572 7475 7262 6564 206d  ergy_perturbed m
-0000b7a0: 6174 7269 7820 7265 7072 6573 656e 7473  atrix represents
-0000b7b0: 2061 2073 7461 7465 2061 6e64 0a20 2020   a state and.   
-0000b7c0: 2020 2020 2020 2020 2074 6865 2076 616c           the val
-0000b7d0: 7565 2065 6e65 7267 795f 7065 7274 7572  ue energy_pertur
-0000b7e0: 6265 645b 6c2c 6e5d 2072 6570 7265 7365  bed[l,n] represe
-0000b7f0: 6e74 7320 7468 6520 7265 6475 6365 6420  nts the reduced 
-0000b800: 656e 6572 6779 0a20 2020 2020 2020 2020  energy.         
-0000b810: 2020 206f 6620 7468 6520 6e27 7468 2063     of the n'th c
-0000b820: 6f6e 666f 726d 6174 696f 6e20 696e 2074  onformation in t
-0000b830: 6865 206c 2774 6820 7065 7274 7572 6265  he l'th perturbe
-0000b840: 6420 7374 6174 652e 0a0a 2020 2020 2020  d state...      
-0000b850: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-0000b860: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-0000b870: 2020 7265 7375 6c74 733a 2064 6963 740a    results: dict.
-0000b880: 2020 2020 2020 2020 2020 2020 6120 6469              a di
-0000b890: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
-0000b8a0: 696e 6720 7468 6520 666f 6c6c 6f77 696e  ing the followin
-0000b8b0: 6720 6b65 7973 3a0a 0a20 2020 2020 2020  g keys:..       
-0000b8c0: 2020 2020 202a 2a46 2a2a 202d 2074 6865       **F** - the
-0000b8d0: 2066 7265 6520 656e 6572 6779 206f 6620   free energy of 
-0000b8e0: 7468 6520 7065 7274 7572 6265 6420 7374  the perturbed st
-0000b8f0: 6174 6573 2e0a 0a20 2020 2020 2020 2020  ates...         
-0000b900: 2020 202a 2a46 5f73 7464 2a2a 202d 2074     **F_std** - t
-0000b910: 6865 2073 7461 6e64 6172 6420 6465 7669  he standard devi
-0000b920: 6174 696f 6e20 6f66 2074 6865 2066 7265  ation of the fre
-0000b930: 6520 656e 6572 6779 206f 6620 7468 6520  e energy of the 
-0000b940: 7065 7274 7572 6265 6420 7374 6174 6573  perturbed states
-0000b950: 2e20 0a0a 2020 2020 2020 2020 2020 2020  . ..            
-0000b960: 2a2a 465f 636f 762a 2a20 2d20 7468 6520  **F_cov** - the 
-0000b970: 636f 7661 7269 616e 6365 2062 6574 7765  covariance betwe
-0000b980: 656e 2074 6865 2066 7265 6520 656e 6572  en the free ener
-0000b990: 6769 6573 206f 6620 7468 6520 7065 7274  gies of the pert
-0000b9a0: 7572 6265 6420 7374 6174 6573 2e0a 0a20  urbed states... 
-0000b9b0: 2020 2020 2020 2020 2020 202a 2a44 656c             **Del
-0000b9c0: 7461 462a 2a20 2d20 3a6d 6174 683a 605c  taF** - :math:`\
-0000b9d0: 6d61 7468 726d 7b44 656c 7461 467d 5b6b  mathrm{DeltaF}[k
-0000b9e0: 2c6c 5d60 2069 7320 7468 6520 6672 6565  ,l]` is the free
-0000b9f0: 2065 6e65 7267 7920 6469 6666 6572 656e   energy differen
-0000ba00: 6365 2062 6574 7765 656e 2073 7461 7465  ce between state
-0000ba10: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-0000ba20: 2020 2020 2020 2020 203a 6d61 7468 3a60           :math:`
-0000ba30: 6b60 2061 6e64 2073 7461 7465 203a 6d61  k` and state :ma
-0000ba40: 7468 3a60 6c60 2c20 692e 652e 2c20 3a6d  th:`l`, i.e., :m
-0000ba50: 6174 683a 605c 6d61 7468 726d 7b44 656c  ath:`\mathrm{Del
-0000ba60: 7461 467d 5b6b 2c6c 5d20 3d20 465b 6c5d  taF}[k,l] = F[l]
-0000ba70: 202d 2046 5b6b 5d60 202e 0a0a 2020 2020   - F[k]` ...    
-0000ba80: 2020 2020 2020 2020 2a2a 4465 6c74 6146          **DeltaF
-0000ba90: 5f73 7464 2a2a 202d 2074 6865 2073 7461  _std** - the sta
-0000baa0: 6e64 6172 6420 6465 7669 6174 696f 6e20  ndard deviation 
-0000bab0: 6f66 2074 6865 2066 7265 6520 656e 6572  of the free ener
-0000bac0: 6779 2064 6966 6665 7265 6e63 652e 0a20  gy difference.. 
-0000bad0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-0000bae0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-0000baf0: 6528 656e 6572 6779 5f70 6572 7475 7262  e(energy_perturb
-0000bb00: 6564 2c20 6e70 2e6e 6461 7272 6179 293a  ed, np.ndarray):
-0000bb10: 0a20 2020 2020 2020 2020 2020 2065 6e65  .            ene
-0000bb20: 7267 795f 7065 7274 7572 6265 6420 3d20  rgy_perturbed = 
-0000bb30: 656e 6572 6779 5f70 6572 7475 7262 6564  energy_perturbed
-0000bb40: 2e61 7374 7970 6528 6e70 2e66 6c6f 6174  .astype(np.float
-0000bb50: 3634 290a 2020 2020 2020 2020 2020 2020  64).            
-0000bb60: 656e 6572 6779 5f70 6572 7475 7262 6564  energy_perturbed
-0000bb70: 203d 2074 6f72 6368 2e66 726f 6d5f 6e75   = torch.from_nu
-0000bb80: 6d70 7928 656e 6572 6779 5f70 6572 7475  mpy(energy_pertu
-0000bb90: 7262 6564 290a 2020 2020 2020 2020 656c  rbed).        el
-0000bba0: 6966 2069 7369 6e73 7461 6e63 6528 656e  if isinstance(en
-0000bbb0: 6572 6779 5f70 6572 7475 7262 6564 2c20  ergy_perturbed, 
-0000bbc0: 746f 7263 682e 5465 6e73 6f72 293a 0a20  torch.Tensor):. 
-0000bbd0: 2020 2020 2020 2020 2020 2065 6e65 7267             energ
-0000bbe0: 795f 7065 7274 7572 6265 6420 3d20 656e  y_perturbed = en
-0000bbf0: 6572 6779 5f70 6572 7475 7262 6564 2e64  ergy_perturbed.d
-0000bc00: 6f75 626c 6528 290a 2020 2020 2020 2020  ouble().        
-0000bc10: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000bc20: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-0000bc30: 7228 2265 6e65 7267 795f 7065 7274 7572  r("energy_pertur
-0000bc40: 6265 6420 6861 7320 746f 2062 6520 6120  bed has to be a 
-0000bc50: 322d 4420 6e64 6172 7261 7920 6f72 2061  2-D ndarray or a
-0000bc60: 2032 2d44 2074 656e 736f 722e 2229 0a0a   2-D tensor.")..
-0000bc70: 2020 2020 2020 2020 6966 2065 6e65 7267          if energ
-0000bc80: 795f 7065 7274 7572 6265 642e 6e64 696d  y_perturbed.ndim
-0000bc90: 2021 3d20 323a 0a20 2020 2020 2020 2020   != 2:.         
-0000bca0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0000bcb0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-0000bcc0: 2020 2020 2022 656e 6572 6779 5f70 6572       "energy_per
-0000bcd0: 7475 7262 6564 2068 6173 2074 6f20 6265  turbed has to be
-0000bce0: 2061 2032 2d44 206e 6461 7272 6179 206f   a 2-D ndarray o
-0000bcf0: 7220 6120 322d 4420 7465 6e73 6f72 2e22  r a 2-D tensor."
-0000bd00: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000bd10: 2020 2020 2020 2069 6620 656e 6572 6779         if energy
-0000bd20: 5f70 6572 7475 7262 6564 2e73 6861 7065  _perturbed.shape
-0000bd30: 5b31 5d20 213d 2073 656c 662e 656e 6572  [1] != self.ener
-0000bd40: 6779 2e73 6861 7065 5b31 5d3a 0a20 2020  gy.shape[1]:.   
-0000bd50: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-0000bd60: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
-0000bd70: 2020 2020 2020 2020 2020 2022 7468 6520             "the 
-0000bd80: 6e75 6d62 6572 206f 6620 636f 6c75 6d6e  number of column
-0000bd90: 7320 696e 2065 6e65 7267 795f 7065 7274  s in energy_pert
-0000bda0: 7572 6265 6420 6861 7320 746f 2062 6520  urbed has to be 
-0000bdb0: 6571 7561 6c20 746f 2074 6865 206e 756d  equal to the num
-0000bdc0: 6265 7220 6f66 2063 6f6c 756d 6e73 2069  ber of columns i
-0000bdd0: 6e20 656e 6572 6779 2e22 0a20 2020 2020  n energy.".     
-0000bde0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000bdf0: 2020 4c20 3d20 656e 6572 6779 5f70 6572    L = energy_per
-0000be00: 7475 7262 6564 2e73 6861 7065 5b30 5d0a  turbed.shape[0].
-0000be10: 0a20 2020 2020 2020 2046 203d 204e 6f6e  .        F = Non
-0000be20: 650a 2020 2020 2020 2020 465f 636f 7620  e.        F_cov 
-0000be30: 3d20 4e6f 6e65 0a20 2020 2020 2020 2046  = None.        F
-0000be40: 5f73 7464 203d 204e 6f6e 650a 0a20 2020  _std = None..   
-0000be50: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-0000be60: 2e62 6f6f 7473 7472 6170 3a0a 2020 2020  .bootstrap:.    
-0000be70: 2020 2020 2020 2020 6475 203d 2065 6e65          du = ene
-0000be80: 7267 795f 7065 7274 7572 6265 6420 2b20  rgy_perturbed + 
-0000be90: 7365 6c66 2e5f 6c6f 675f 7072 6f62 5f6d  self._log_prob_m
-0000bea0: 6978 0a20 2020 2020 2020 2020 2020 2046  ix.            F
-0000beb0: 203d 202d 746f 7263 682e 6c6f 6773 756d   = -torch.logsum
-0000bec0: 6578 7028 2d64 752c 2064 696d 3d31 290a  exp(-du, dim=1).
-0000bed0: 0a20 2020 2020 2020 2020 2020 2046 5f65  .            F_e
-0000bee0: 7874 203d 2074 6f72 6368 2e63 6174 285b  xt = torch.cat([
-0000bef0: 7365 6c66 2e5f 462c 2046 5d29 0a20 2020  self._F, F]).   
-0000bf00: 2020 2020 2020 2020 2055 203d 2074 6f72           U = tor
-0000bf10: 6368 2e63 6174 285b 7365 6c66 2e65 6e65  ch.cat([self.ene
-0000bf20: 7267 792c 2065 6e65 7267 795f 7065 7274  rgy, energy_pert
-0000bf30: 7572 6265 645d 2c20 6469 6d3d 3029 2e74  urbed], dim=0).t
-0000bf40: 2829 0a20 2020 2020 2020 2020 2020 2050  ().            P
-0000bf50: 203d 2074 6f72 6368 2e65 7870 282d 2855   = torch.exp(-(U
-0000bf60: 202d 2046 5f65 7874 202b 2073 656c 662e   - F_ext + self.
-0000bf70: 5f6c 6f67 5f70 726f 625f 6d69 785b 3a2c  _log_prob_mix[:,
-0000bf80: 204e 6f6e 655d 2929 0a0a 2020 2020 2020   None]))..      
-0000bf90: 2020 2020 2020 5720 3d20 746f 7263 682e        W = torch.
-0000bfa0: 6469 6167 2874 6f72 6368 2e63 6174 285b  diag(torch.cat([
-0000bfb0: 7365 6c66 2e6e 756d 5f63 6f6e 662c 2073  self.num_conf, s
-0000bfc0: 656c 662e 6e75 6d5f 636f 6e66 2e6e 6577  elf.num_conf.new
-0000bfd0: 5f7a 6572 6f73 284c 295d 2929 0a20 2020  _zeros(L)])).   
-0000bfe0: 2020 2020 2020 2020 2051 2c20 5220 3d20           Q, R = 
-0000bff0: 746f 7263 682e 6c69 6e61 6c67 2e71 7228  torch.linalg.qr(
-0000c000: 5029 0a20 2020 2020 2020 2020 2020 2041  P).            A
-0000c010: 203d 2074 6f72 6368 2e65 7965 2873 656c   = torch.eye(sel
-0000c020: 662e 4d20 2b20 4c2c 2064 6576 6963 653d  f.M + L, device=
-0000c030: 572e 6465 7669 6365 2920 2d20 5220 4020  W.device) - R @ 
-0000c040: 5720 4020 522e 540a 2020 2020 2020 2020  W @ R.T.        
-0000c050: 2020 2020 465f 636f 7620 3d20 522e 5420      F_cov = R.T 
-0000c060: 4020 746f 7263 682e 6c69 6e61 6c67 2e70  @ torch.linalg.p
-0000c070: 696e 7628 412c 2068 6572 6d69 7469 616e  inv(A, hermitian
-0000c080: 3d54 7275 652c 2072 746f 6c3d 3165 2d38  =True, rtol=1e-8
-0000c090: 2920 4020 520a 0a20 2020 2020 2020 2020  ) @ R..         
-0000c0a0: 2020 2046 5f63 6f76 203d 2046 5f63 6f76     F_cov = F_cov
-0000c0b0: 5b73 656c 662e 4d20 3a2c 2073 656c 662e  [self.M :, self.
-0000c0c0: 4d20 3a5d 0a20 2020 2020 2020 2020 2020  M :].           
-0000c0d0: 2046 5f73 7464 203d 2046 5f63 6f76 2e64   F_std = F_cov.d
-0000c0e0: 6961 676f 6e61 6c28 292e 7371 7274 2829  iagonal().sqrt()
-0000c0f0: 0a0a 2020 2020 2020 2020 2020 2020 4465  ..            De
-0000c100: 6c74 6146 203d 2046 5b4e 6f6e 652c 203a  ltaF = F[None, :
-0000c110: 5d20 2d20 465b 3a2c 204e 6f6e 655d 0a20  ] - F[:, None]. 
-0000c120: 2020 2020 2020 2020 2020 2044 656c 7461             Delta
-0000c130: 465f 636f 7620 3d20 465f 636f 762e 6469  F_cov = F_cov.di
-0000c140: 6167 2829 5b3a 2c20 4e6f 6e65 5d20 2b20  ag()[:, None] + 
-0000c150: 465f 636f 762e 6469 6167 2829 5b4e 6f6e  F_cov.diag()[Non
-0000c160: 652c 203a 5d20 2d20 3220 2a20 465f 636f  e, :] - 2 * F_co
-0000c170: 760a 2020 2020 2020 2020 2020 2020 4465  v.            De
-0000c180: 6c74 6146 5f73 7464 203d 2044 656c 7461  ltaF_std = Delta
-0000c190: 465f 636f 762e 7371 7274 2829 0a20 2020  F_cov.sqrt().   
-0000c1a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000c1b0: 2020 2020 2020 2046 5f6c 6973 7420 3d20         F_list = 
-0000c1c0: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
-0000c1d0: 6f72 206b 2069 6e20 7261 6e67 6528 7365  or k in range(se
-0000c1e0: 6c66 2e62 6f6f 7473 7472 6170 5f6e 756d  lf.bootstrap_num
-0000c1f0: 5f72 6570 293a 0a20 2020 2020 2020 2020  _rep):.         
-0000c200: 2020 2020 2020 2064 7520 3d20 656e 6572         du = ener
-0000c210: 6779 5f70 6572 7475 7262 6564 5b3a 2c20  gy_perturbed[:, 
-0000c220: 7365 6c66 2e5f 636f 6e66 5f69 6478 5b6b  self._conf_idx[k
-0000c230: 5d5d 202b 2073 656c 662e 5f6c 6f67 5f70  ]] + self._log_p
-0000c240: 726f 625f 6d69 785b 6b5d 0a20 2020 2020  rob_mix[k].     
-0000c250: 2020 2020 2020 2020 2020 2046 203d 202d             F = -
-0000c260: 746f 7263 682e 6c6f 6773 756d 6578 7028  torch.logsumexp(
-0000c270: 2d64 752c 2064 696d 3d31 290a 2020 2020  -du, dim=1).    
-0000c280: 2020 2020 2020 2020 2020 2020 465f 6c69              F_li
-0000c290: 7374 2e61 7070 656e 6428 4629 0a20 2020  st.append(F).   
-0000c2a0: 2020 2020 2020 2020 2046 5f6c 6973 7420           F_list 
-0000c2b0: 3d20 746f 7263 682e 7374 6163 6b28 465f  = torch.stack(F_
-0000c2c0: 6c69 7374 2c20 6469 6d3d 3129 0a20 2020  list, dim=1).   
-0000c2d0: 2020 2020 2020 2020 2046 203d 2074 6f72           F = tor
-0000c2e0: 6368 2e6d 6561 6e28 465f 6c69 7374 2c20  ch.mean(F_list, 
-0000c2f0: 6469 6d3d 3129 0a20 2020 2020 2020 2020  dim=1).         
-0000c300: 2020 2046 5f73 7464 203d 2074 6f72 6368     F_std = torch
-0000c310: 2e73 7464 2846 5f6c 6973 742c 2064 696d  .std(F_list, dim
-0000c320: 3d31 290a 2020 2020 2020 2020 2020 2020  =1).            
-0000c330: 465f 636f 7620 3d20 746f 7263 682e 636f  F_cov = torch.co
-0000c340: 7628 465f 6c69 7374 290a 0a20 2020 2020  v(F_list)..     
-0000c350: 2020 2020 2020 2044 656c 7461 4620 3d20         DeltaF = 
-0000c360: 465b 4e6f 6e65 2c20 3a5d 202d 2046 5b3a  F[None, :] - F[:
-0000c370: 2c20 4e6f 6e65 5d0a 2020 2020 2020 2020  , None].        
-0000c380: 2020 2020 4465 6c74 6146 5f73 7464 203d      DeltaF_std =
-0000c390: 2074 6f72 6368 2e73 7464 2846 5f6c 6973   torch.std(F_lis
-0000c3a0: 745b 3a2c 203a 2c20 4e6f 6e65 5d20 2d20  t[:, :, None] - 
-0000c3b0: 465f 6c69 7374 5b3a 2c20 4e6f 6e65 2c20  F_list[:, None, 
-0000c3c0: 3a5d 2c20 6469 6d3d 3129 0a0a 2020 2020  :], dim=1)..    
-0000c3d0: 2020 2020 7265 7375 6c74 7320 3d20 7b0a      results = {.
-0000c3e0: 2020 2020 2020 2020 2020 2020 2246 223a              "F":
-0000c3f0: 2046 2e6e 756d 7079 2829 2c0a 2020 2020   F.numpy(),.    
-0000c400: 2020 2020 2020 2020 2246 5f73 7464 223a          "F_std":
-0000c410: 2046 5f73 7464 2e6e 756d 7079 2829 2c0a   F_std.numpy(),.
-0000c420: 2020 2020 2020 2020 2020 2020 2246 5f63              "F_c
-0000c430: 6f76 223a 2046 5f63 6f76 2e6e 756d 7079  ov": F_cov.numpy
-0000c440: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-0000c450: 2244 656c 7461 4622 3a20 4465 6c74 6146  "DeltaF": DeltaF
-0000c460: 2e6e 756d 7079 2829 2c0a 2020 2020 2020  .numpy(),.      
-0000c470: 2020 2020 2020 2244 656c 7461 465f 7374        "DeltaF_st
-0000c480: 6422 3a20 4465 6c74 6146 5f73 7464 2e6e  d": DeltaF_std.n
-0000c490: 756d 7079 2829 2c0a 2020 2020 2020 2020  umpy(),.        
-0000c4a0: 7d0a 0a20 2020 2020 2020 2072 6574 7572  }..        retur
-0000c4b0: 6e20 7265 7375 6c74 730a 0a64 6566 205f  n results..def _
-0000c4c0: 636f 6d70 7574 655f 6c6f 6770 5f6f 665f  compute_logp_of_
-0000c4d0: 4628 462c 2065 6e65 7267 792c 206e 756d  F(F, energy, num
-0000c4e0: 5f63 6f6e 6629 3a0a 2020 2020 6c6f 6770  _conf):.    logp
-0000c4f0: 203d 2028 0a20 2020 2020 2020 2074 6f72   = (.        tor
-0000c500: 6368 2e73 756d 286e 756d 5f63 6f6e 6620  ch.sum(num_conf 
-0000c510: 2a20 4629 0a20 2020 2020 2020 202d 2074  * F).        - t
-0000c520: 6f72 6368 2e6c 6f67 7375 6d65 7870 282d  orch.logsumexp(-
-0000c530: 2865 6e65 7267 792e 5420 2d20 746f 7263  (energy.T - torc
-0000c540: 682e 6c6f 6728 6e75 6d5f 636f 6e66 2920  h.log(num_conf) 
-0000c550: 2d20 4629 2c20 6469 6d3d 3129 2e73 756d  - F), dim=1).sum
-0000c560: 2829 0a20 2020 2029 0a20 2020 2072 6574  ().    ).    ret
-0000c570: 7572 6e20 6c6f 6770 0a0a 0a64 6566 205f  urn logp...def _
-0000c580: 636f 6d70 7574 655f 6c6f 7373 5f61 6e64  compute_loss_and
-0000c590: 5f67 7261 645f 6f66 5f64 4628 6446 2c20  _grad_of_dF(dF, 
-0000c5a0: 656e 6572 6779 2c20 6e75 6d5f 636f 6e66  energy, num_conf
-0000c5b0: 293a 0a20 2020 2022 2222 436f 6d70 7574  ):.    """Comput
-0000c5c0: 6520 7468 6520 6c6f 7373 2066 756e 6374  e the loss funct
-0000c5d0: 696f 6e20 616e 6420 7468 6520 6772 6164  ion and the grad
-0000c5e0: 6965 6e74 206f 6620 6446 2067 6976 656e  ient of dF given
-0000c5f0: 2065 6e65 7267 7920 616e 6420 6e75 6d5f   energy and num_
-0000c600: 636f 6e66 2e0a 2020 2020 5061 7261 6d65  conf..    Parame
-0000c610: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0000c620: 2d2d 2d0a 2020 2020 6446 3a20 312d 4420  ---.    dF: 1-D 
-0000c630: 666c 6f61 7420 7465 6e73 6f72 2077 6974  float tensor wit
-0000c640: 6820 7369 7a65 2028 4d2d 3129 0a20 2020  h size (M-1).   
-0000c650: 2020 2020 2054 6865 2066 7265 6520 656e       The free en
-0000c660: 6572 6779 2064 6966 6665 7265 6e63 6520  ergy difference 
-0000c670: 6265 7477 6565 6e20 7374 6174 6520 3020  between state 0 
-0000c680: 616e 6420 6f74 6865 7220 7374 6174 6573  and other states
-0000c690: 2e20 5468 6520 656e 7472 790a 2020 2020  . The entry.    
-0000c6a0: 2020 2020 6446 5b69 5d20 6973 2074 6865      dF[i] is the
-0000c6b0: 2066 7265 6520 656e 6572 6779 2064 6966   free energy dif
-0000c6c0: 6665 7265 6e63 6520 6265 7477 6565 6e20  ference between 
-0000c6d0: 7374 6174 6520 3020 616e 6420 7374 6174  state 0 and stat
-0000c6e0: 6520 692b 312e 0a20 2020 2065 6e65 7267  e i+1..    energ
-0000c6f0: 793a 2032 2d44 2066 6c6f 6174 2074 656e  y: 2-D float ten
-0000c700: 736f 7220 7769 7468 2073 697a 6520 284d  sor with size (M
-0000c710: 2078 204e 290a 2020 2020 2020 2020 4120   x N).        A 
-0000c720: 322d 4420 7465 6e73 6f72 2077 6974 6820  2-D tensor with 
-0000c730: 7369 7a65 206f 6620 4d20 7820 4e2c 2077  size of M x N, w
-0000c740: 6865 7265 204d 2069 7320 7468 6520 6e75  here M is the nu
-0000c750: 6d62 6572 206f 6620 7374 6174 730a 2020  mber of stats.  
-0000c760: 2020 2020 2020 616e 6420 4e20 6973 2074        and N is t
-0000c770: 6865 2074 6f74 616c 206e 756d 6265 7220  he total number 
-0000c780: 6f66 2063 6f6e 666f 726d 6174 696f 6e73  of conformations
-0000c790: 2e20 5468 6520 656e 7472 7920 656e 6572  . The entry ener
-0000c7a0: 6779 5b69 2c6a 5d0a 2020 2020 6e75 6d5f  gy[i,j].    num_
-0000c7b0: 636f 6e66 3a20 312d 4420 696e 7420 7465  conf: 1-D int te
-0000c7c0: 6e73 6f72 2077 6974 6820 7369 7a65 2028  nsor with size (
-0000c7d0: 4d29 0a20 2020 2020 2020 2041 2031 2d44  M).        A 1-D
-0000c7e0: 2074 656e 736f 7220 7769 7468 2073 697a   tensor with siz
-0000c7f0: 6520 6f66 204d 2c20 7768 6572 6520 6e75  e of M, where nu
-0000c800: 6d5f 636f 6e66 5b69 5d20 6973 2074 6865  m_conf[i] is the
-0000c810: 206e 756d 206f 660a 2020 2020 2020 2020   num of.        
-0000c820: 636f 6e66 6f72 6d61 7469 6f6e 7320 7361  conformations sa
-0000c830: 6d70 6c65 6420 6672 6f6d 2073 7461 7465  mpled from state
-0000c840: 2069 2e20 5468 6572 6566 6f72 652c 2074   i. Therefore, t
-0000c850: 6f72 6368 2e73 756d 286e 756d 5f63 6f6e  orch.sum(num_con
-0000c860: 6629 0a20 2020 2020 2020 2068 6173 2074  f).        has t
-0000c870: 6f20 6265 2065 7175 616c 2074 6f20 4e2e  o be equal to N.
-0000c880: 2041 6c6c 2065 6e74 7269 6573 2069 6e20   All entries in 
-0000c890: 6e75 6d5f 636f 6e66 2068 6176 6520 746f  num_conf have to
-0000c8a0: 2062 6520 7374 7269 6374 6c79 0a20 2020   be strictly.   
-0000c8b0: 2020 2020 2067 7265 6174 6572 2074 6861       greater tha
-0000c8c0: 6e20 302e 0a20 2020 2022 2222 0a0a 2020  n 0..    """..  
-0000c8d0: 2020 2320 636f 6d70 7574 6520 7468 6520    # compute the 
-0000c8e0: 6c6f 7373 2066 756e 6374 696f 6e0a 2020  loss function.  
-0000c8f0: 2020 4620 3d20 746f 7263 682e 6361 7428    F = torch.cat(
-0000c900: 5b64 462e 6e65 775f 7a65 726f 7328 3129  [dF.new_zeros(1)
-0000c910: 2c20 6446 5d29 0a20 2020 206c 6f67 7020  , dF]).    logp 
-0000c920: 3d20 5f63 6f6d 7075 7465 5f6c 6f67 705f  = _compute_logp_
-0000c930: 6f66 5f46 2846 2c20 656e 6572 6779 2c20  of_F(F, energy, 
-0000c940: 6e75 6d5f 636f 6e66 290a 2020 2020 6c6f  num_conf).    lo
-0000c950: 7373 203d 202d 6c6f 6770 202f 206e 756d  ss = -logp / num
-0000c960: 5f63 6f6e 662e 7375 6d28 290a 2020 2020  _conf.sum().    
-0000c970: 7520 3d20 656e 6572 6779 202d 2046 5b3a  u = energy - F[:
-0000c980: 2c20 4e6f 6e65 5d20 2d20 746f 7263 682e  , None] - torch.
-0000c990: 6c6f 6728 6e75 6d5f 636f 6e66 295b 3a2c  log(num_conf)[:,
-0000c9a0: 204e 6f6e 655d 0a0a 2020 2020 2320 636f   None]..    # co
-0000c9b0: 6d70 7574 6520 7468 6520 6772 6164 6965  mpute the gradie
-0000c9c0: 6e74 206f 6620 7468 6520 6c6f 7373 2066  nt of the loss f
-0000c9d0: 756e 6374 696f 6e0a 2020 2020 7020 3d20  unction.    p = 
-0000c9e0: 746f 7263 682e 736f 6674 6d61 7828 2d75  torch.softmax(-u
-0000c9f0: 2c20 6469 6d3d 3029 0a20 2020 2067 7261  , dim=0).    gra
-0000ca00: 6420 3d20 746f 7263 682e 6d65 616e 2870  d = torch.mean(p
-0000ca10: 2c20 6469 6d3d 3129 202d 206e 756d 5f63  , dim=1) - num_c
-0000ca20: 6f6e 6620 2f20 6e75 6d5f 636f 6e66 2e73  onf / num_conf.s
-0000ca30: 756d 2829 0a20 2020 2067 7261 6420 3d20  um().    grad = 
-0000ca40: 6772 6164 5b31 3a5d 0a0a 2020 2020 7265  grad[1:]..    re
-0000ca50: 7475 726e 206c 6f73 732c 2067 7261 640a  turn loss, grad.
-0000ca60: 0a0a 6465 6620 5f63 6f6d 7075 7465 5f6c  ..def _compute_l
-0000ca70: 6f73 735f 616e 645f 6772 6164 5f6f 665f  oss_and_grad_of_
-0000ca80: 6446 5f69 6e5f 6261 7463 6828 6446 2c20  dF_in_batch(dF, 
-0000ca90: 656e 6572 6779 2c20 6e75 6d5f 636f 6e66  energy, num_conf
-0000caa0: 2c20 6261 7463 685f 7369 7a65 3a20 696e  , batch_size: in
-0000cab0: 7429 3a0a 2020 2020 2222 2254 6869 7320  t):.    """This 
-0000cac0: 6973 2074 6865 2062 6174 6368 2076 6572  is the batch ver
-0000cad0: 7369 6f6e 206f 6620 5f63 6f6d 7075 7465  sion of _compute
-0000cae0: 5f6c 6f73 735f 616e 645f 6772 6164 5f6f  _loss_and_grad_o
-0000caf0: 665f 6446 2e0a 2020 2020 5468 6520 6261  f_dF..    The ba
-0000cb00: 7463 6820 7665 7273 696f 6e20 6973 2075  tch version is u
-0000cb10: 7365 6420 7768 656e 2074 6865 2073 697a  sed when the siz
-0000cb20: 6520 6f66 2065 6e65 7267 7920 6973 2074  e of energy is t
-0000cb30: 6f6f 206c 6172 6765 2074 6f20 6669 7420  oo large to fit 
-0000cb40: 696e 746f 2074 6865 0a20 2020 206d 656d  into the.    mem
-0000cb50: 6f72 7920 6f66 2061 2047 5055 2e20 5468  ory of a GPU. Th
-0000cb60: 6520 656e 6572 6779 206d 6174 7269 7820  e energy matrix 
-0000cb70: 6973 2073 706c 6974 2069 6e74 6f20 6d75  is split into mu
-0000cb80: 6c74 6970 6c65 2062 6174 6368 6573 2061  ltiple batches a
-0000cb90: 6e64 2074 6865 0a20 2020 2063 616c 6375  nd the.    calcu
-0000cba0: 6c61 7469 6f6e 2069 7320 646f 6e65 2073  lation is done s
-0000cbb0: 6571 7565 6e74 6961 6c6c 792e 0a0a 2020  equentially...  
-0000cbc0: 2020 5468 6520 7061 7261 6d65 7465 7273    The parameters
-0000cbd0: 2061 7265 2074 6865 2073 616d 6520 6173   are the same as
-0000cbe0: 205f 636f 6d70 7574 655f 6c6f 7373 5f61   _compute_loss_a
-0000cbf0: 6e64 5f67 7261 645f 6f66 5f64 462e 0a20  nd_grad_of_dF.. 
-0000cc00: 2020 2022 2222 0a0a 2020 2020 6e20 3d20     """..    n = 
-0000cc10: 6e75 6d5f 636f 6e66 0a20 2020 204e 203d  num_conf.    N =
-0000cc20: 2074 6f72 6368 2e73 756d 286e 290a 2020   torch.sum(n).  
-0000cc30: 2020 6e5f 6f76 6572 5f4e 203d 206e 202f    n_over_N = n /
-0000cc40: 204e 0a0a 2020 2020 6966 2065 6e65 7267   N..    if energ
-0000cc50: 792e 7368 6170 655b 315d 2025 2062 6174  y.shape[1] % bat
-0000cc60: 6368 5f73 697a 6520 3d3d 2030 3a0a 2020  ch_size == 0:.  
-0000cc70: 2020 2020 2020 6e75 6d5f 6261 7463 6820        num_batch 
-0000cc80: 3d20 656e 6572 6779 2e73 6861 7065 5b31  = energy.shape[1
-0000cc90: 5d20 2f2f 2062 6174 6368 5f73 697a 650a  ] // batch_size.
-0000cca0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000ccb0: 2020 6e75 6d5f 6261 7463 6820 3d20 656e    num_batch = en
-0000ccc0: 6572 6779 2e73 6861 7065 5b31 5d20 2f2f  ergy.shape[1] //
-0000ccd0: 2062 6174 6368 5f73 697a 6520 2b20 310a   batch_size + 1.
-0000cce0: 0a20 2020 2046 203d 2074 6f72 6368 2e63  .    F = torch.c
-0000ccf0: 6174 285b 6446 2e6e 6577 5f7a 6572 6f73  at([dF.new_zeros
-0000cd00: 2831 292c 2064 465d 290a 2020 2020 6c6f  (1), dF]).    lo
-0000cd10: 7373 203d 202d 746f 7263 682e 7375 6d28  ss = -torch.sum(
-0000cd20: 6e75 6d5f 636f 6e66 202a 2046 290a 2020  num_conf * F).  
-0000cd30: 2020 6772 6164 203d 202d 6e75 6d5f 636f    grad = -num_co
-0000cd40: 6e66 0a0a 2020 2020 666f 7220 6920 696e  nf..    for i in
-0000cd50: 2072 616e 6765 286e 756d 5f62 6174 6368   range(num_batch
-0000cd60: 293a 0a20 2020 2020 2020 2065 6e65 7267  ):.        energ
-0000cd70: 795f 6261 7463 6820 3d20 656e 6572 6779  y_batch = energy
-0000cd80: 5b3a 2c20 6920 2a20 6261 7463 685f 7369  [:, i * batch_si
-0000cd90: 7a65 203a 2028 6920 2b20 3129 202a 2062  ze : (i + 1) * b
-0000cda0: 6174 6368 5f73 697a 655d 0a20 2020 2020  atch_size].     
-0000cdb0: 2020 2075 203d 2065 6e65 7267 795f 6261     u = energy_ba
-0000cdc0: 7463 682e 6375 6461 2829 202d 2074 6f72  tch.cuda() - tor
-0000cdd0: 6368 2e6c 6f67 286e 756d 5f63 6f6e 6629  ch.log(num_conf)
-0000cde0: 5b3a 2c20 4e6f 6e65 5d20 2d20 465b 3a2c  [:, None] - F[:,
-0000cdf0: 204e 6f6e 655d 0a20 2020 2020 2020 206c   None].        l
-0000ce00: 6f73 7320 2b3d 2074 6f72 6368 2e6c 6f67  oss += torch.log
-0000ce10: 7375 6d65 7870 282d 752c 2064 696d 3d30  sumexp(-u, dim=0
-0000ce20: 292e 7375 6d28 290a 0a20 2020 2020 2020  ).sum()..       
-0000ce30: 2070 203d 2074 6f72 6368 2e73 6f66 746d   p = torch.softm
-0000ce40: 6178 282d 752c 2064 696d 3d30 290a 2020  ax(-u, dim=0).  
-0000ce50: 2020 2020 2020 6772 6164 202b 3d20 746f        grad += to
-0000ce60: 7263 682e 7375 6d28 702c 2064 696d 3d31  rch.sum(p, dim=1
-0000ce70: 290a 0a20 2020 206c 6f73 7320 3d20 6c6f  )..    loss = lo
-0000ce80: 7373 202f 204e 0a20 2020 2067 7261 6420  ss / N.    grad 
-0000ce90: 3d20 6772 6164 202f 204e 0a20 2020 2067  = grad / N.    g
-0000cea0: 7261 6420 3d20 6772 6164 5b31 3a5d 0a20  rad = grad[1:]. 
-0000ceb0: 2020 2072 6574 7572 6e20 6c6f 7373 2c20     return loss, 
-0000cec0: 6772 6164 0a0a 0a64 6566 205f 636f 6d70  grad...def _comp
-0000ced0: 7574 655f 6865 7373 6961 6e5f 6c6f 675f  ute_hessian_log_
-0000cee0: 6c69 6b65 6c69 686f 6f64 5f6f 665f 4628  likelihood_of_F(
-0000cef0: 462c 2065 6e65 7267 792c 206e 756d 5f63  F, energy, num_c
-0000cf00: 6f6e 6629 3a0a 2020 2020 7520 3d20 656e  onf):.    u = en
-0000cf10: 6572 6779 202d 2046 5b3a 2c20 4e6f 6e65  ergy - F[:, None
-0000cf20: 5d20 2d20 746f 7263 682e 6c6f 6728 6e75  ] - torch.log(nu
-0000cf30: 6d5f 636f 6e66 295b 3a2c 204e 6f6e 655d  m_conf)[:, None]
-0000cf40: 0a20 2020 2070 203d 2074 6f72 6368 2e73  .    p = torch.s
-0000cf50: 6f66 746d 6178 282d 752c 2064 696d 3d30  oftmax(-u, dim=0
-0000cf60: 290a 2020 2020 7070 203d 2074 6f72 6368  ).    pp = torch
-0000cf70: 2e6d 6174 6d75 6c28 702c 2070 2e54 290a  .matmul(p, p.T).
-0000cf80: 2020 2020 4820 3d20 7070 202d 2074 6f72      H = pp - tor
-0000cf90: 6368 2e64 6961 6728 746f 7263 682e 7375  ch.diag(torch.su
-0000cfa0: 6d28 702c 2031 2929 0a20 2020 2072 6574  m(p, 1)).    ret
-0000cfb0: 7572 6e20 480a 0a0a 6465 6620 5f63 6f6d  urn H...def _com
-0000cfc0: 7075 7465 5f68 6573 7369 616e 5f6c 6f67  pute_hessian_log
-0000cfd0: 5f6c 696b 656c 6968 6f6f 645f 6f66 5f46  _likelihood_of_F
-0000cfe0: 5f69 6e5f 6261 7463 6828 462c 2065 6e65  _in_batch(F, ene
-0000cff0: 7267 792c 206e 756d 5f63 6f6e 662c 2062  rgy, num_conf, b
-0000d000: 6174 6368 5f73 697a 653a 2069 6e74 293a  atch_size: int):
-0000d010: 0a20 2020 2069 6620 656e 6572 6779 2e73  .    if energy.s
-0000d020: 6861 7065 5b31 5d20 2520 6261 7463 685f  hape[1] % batch_
-0000d030: 7369 7a65 203d 3d20 303a 0a20 2020 2020  size == 0:.     
-0000d040: 2020 206e 756d 5f62 6174 6368 203d 2065     num_batch = e
-0000d050: 6e65 7267 792e 7368 6170 655b 315d 202f  nergy.shape[1] /
-0000d060: 2f20 6261 7463 685f 7369 7a65 0a20 2020  / batch_size.   
-0000d070: 2065 6c73 653a 0a20 2020 2020 2020 206e   else:.        n
-0000d080: 756d 5f62 6174 6368 203d 2065 6e65 7267  um_batch = energ
-0000d090: 792e 7368 6170 655b 315d 202f 2f20 6261  y.shape[1] // ba
-0000d0a0: 7463 685f 7369 7a65 202b 2031 0a0a 2020  tch_size + 1..  
-0000d0b0: 2020 4820 3d20 462e 6e65 775f 7a65 726f    H = F.new_zero
-0000d0c0: 7328 2846 2e73 6861 7065 5b30 5d2c 2046  s((F.shape[0], F
-0000d0d0: 2e73 6861 7065 5b30 5d29 292e 6375 6461  .shape[0])).cuda
-0000d0e0: 2829 0a20 2020 2066 6f72 2069 2069 6e20  ().    for i in 
-0000d0f0: 7261 6e67 6528 6e75 6d5f 6261 7463 6829  range(num_batch)
-0000d100: 3a0a 2020 2020 2020 2020 656e 6572 6779  :.        energy
-0000d110: 5f62 6174 6368 203d 2065 6e65 7267 795b  _batch = energy[
-0000d120: 3a2c 2069 202a 2062 6174 6368 5f73 697a  :, i * batch_siz
-0000d130: 6520 3a20 2869 202b 2031 2920 2a20 6261  e : (i + 1) * ba
-0000d140: 7463 685f 7369 7a65 5d0a 2020 2020 2020  tch_size].      
-0000d150: 2020 7520 3d20 656e 6572 6779 5f62 6174    u = energy_bat
-0000d160: 6368 2e63 7564 6128 2920 2d20 465b 3a2c  ch.cuda() - F[:,
-0000d170: 204e 6f6e 655d 202d 2074 6f72 6368 2e6c   None] - torch.l
-0000d180: 6f67 286e 756d 5f63 6f6e 6629 5b3a 2c20  og(num_conf)[:, 
-0000d190: 4e6f 6e65 5d0a 0a20 2020 2020 2020 2070  None]..        p
-0000d1a0: 203d 2074 6f72 6368 2e73 6f66 746d 6178   = torch.softmax
-0000d1b0: 282d 752c 2064 696d 3d30 290a 2020 2020  (-u, dim=0).    
-0000d1c0: 2020 2020 7070 203d 2074 6f72 6368 2e6d      pp = torch.m
-0000d1d0: 6174 6d75 6c28 702c 2070 2e54 290a 2020  atmul(p, p.T).  
-0000d1e0: 2020 2020 2020 4820 2b3d 2070 7020 2d20        H += pp - 
-0000d1f0: 746f 7263 682e 6469 6167 2874 6f72 6368  torch.diag(torch
-0000d200: 2e73 756d 2870 2c20 3129 290a 0a20 2020  .sum(p, 1))..   
-0000d210: 2072 6574 7572 6e20 480a 0a0a 6465 6620   return H...def 
-0000d220: 5f63 6f6d 7075 7465 5f68 6573 7369 616e  _compute_hessian
-0000d230: 5f6c 6f73 735f 6f66 5f64 4628 6446 2c20  _loss_of_dF(dF, 
-0000d240: 656e 6572 6779 2c20 6e75 6d5f 636f 6e66  energy, num_conf
-0000d250: 293a 0a20 2020 204e 203d 2074 6f72 6368  ):.    N = torch
-0000d260: 2e73 756d 286e 756d 5f63 6f6e 6629 0a20  .sum(num_conf). 
-0000d270: 2020 2046 203d 2074 6f72 6368 2e63 6174     F = torch.cat
-0000d280: 285b 6446 2e6e 6577 5f7a 6572 6f73 2831  ([dF.new_zeros(1
-0000d290: 292c 2064 465d 290a 2020 2020 4820 3d20  ), dF]).    H = 
-0000d2a0: 5f63 6f6d 7075 7465 5f68 6573 7369 616e  _compute_hessian
-0000d2b0: 5f6c 6f67 5f6c 696b 656c 6968 6f6f 645f  _log_likelihood_
-0000d2c0: 6f66 5f46 2846 2c20 656e 6572 6779 2c20  of_F(F, energy, 
-0000d2d0: 6e75 6d5f 636f 6e66 290a 2020 2020 4820  num_conf).    H 
-0000d2e0: 3d20 2d48 5b31 3a2c 2031 3a5d 202f 204e  = -H[1:, 1:] / N
-0000d2f0: 0a20 2020 2072 6574 7572 6e20 480a 0a0a  .    return H...
-0000d300: 6465 6620 5f63 6f6d 7075 7465 5f68 6573  def _compute_hes
-0000d310: 7369 616e 5f6c 6f73 735f 6f66 5f64 465f  sian_loss_of_dF_
-0000d320: 696e 5f62 6174 6368 2864 462c 2065 6e65  in_batch(dF, ene
-0000d330: 7267 792c 206e 756d 5f63 6f6e 662c 2062  rgy, num_conf, b
-0000d340: 6174 6368 5f73 697a 653a 2069 6e74 293a  atch_size: int):
-0000d350: 0a20 2020 204e 203d 2074 6f72 6368 2e73  .    N = torch.s
-0000d360: 756d 286e 756d 5f63 6f6e 6629 0a20 2020  um(num_conf).   
-0000d370: 2046 203d 2074 6f72 6368 2e63 6174 285b   F = torch.cat([
-0000d380: 6446 2e6e 6577 5f7a 6572 6f73 2831 292c  dF.new_zeros(1),
-0000d390: 2064 465d 290a 2020 2020 4820 3d20 5f63   dF]).    H = _c
-0000d3a0: 6f6d 7075 7465 5f68 6573 7369 616e 5f6c  ompute_hessian_l
-0000d3b0: 6f67 5f6c 696b 656c 6968 6f6f 645f 6f66  og_likelihood_of
-0000d3c0: 5f46 5f69 6e5f 6261 7463 6828 462c 2065  _F_in_batch(F, e
-0000d3d0: 6e65 7267 792c 206e 756d 5f63 6f6e 662c  nergy, num_conf,
-0000d3e0: 2062 6174 6368 5f73 697a 6529 0a20 2020   batch_size).   
-0000d3f0: 2048 203d 202d 485b 313a 2c20 313a 5d20   H = -H[1:, 1:] 
-0000d400: 2f20 4e0a 2020 2020 7265 7475 726e 2048  / N.    return H
-0000d410: 0a0a 0a64 6566 205f 736f 6c76 655f 6d62  ...def _solve_mb
-0000d420: 6172 2864 465f 696e 6974 2c20 656e 6572  ar(dF_init, ener
-0000d430: 6779 2c20 6e75 6d5f 636f 6e66 2c20 6d65  gy, num_conf, me
-0000d440: 7468 6f64 2c20 6261 7463 685f 7369 7a65  thod, batch_size
-0000d450: 3d4e 6f6e 652c 2076 6572 626f 7365 3d46  =None, verbose=F
-0000d460: 616c 7365 293a 0a20 2020 2069 6620 6261  alse):.    if ba
-0000d470: 7463 685f 7369 7a65 2069 7320 6e6f 7420  tch_size is not 
-0000d480: 4e6f 6e65 3a0a 2020 2020 2020 2020 6966  None:.        if
-0000d490: 206d 6574 686f 6420 3d3d 2022 4e65 7774   method == "Newt
-0000d4a0: 6f6e 223a 0a20 2020 2020 2020 2020 2020  on":.           
-0000d4b0: 2072 6573 756c 7473 203d 2066 6d69 6e5f   results = fmin_
-0000d4c0: 6e65 7774 6f6e 280a 2020 2020 2020 2020  newton(.        
-0000d4d0: 2020 2020 2020 2020 663d 5f63 6f6d 7075          f=_compu
-0000d4e0: 7465 5f6c 6f73 735f 616e 645f 6772 6164  te_loss_and_grad
-0000d4f0: 5f6f 665f 6446 5f69 6e5f 6261 7463 682c  _of_dF_in_batch,
-0000d500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d510: 2068 6573 733d 5f63 6f6d 7075 7465 5f68   hess=_compute_h
-0000d520: 6573 7369 616e 5f6c 6f73 735f 6f66 5f64  essian_loss_of_d
-0000d530: 465f 696e 5f62 6174 6368 2c0a 2020 2020  F_in_batch,.    
-0000d540: 2020 2020 2020 2020 2020 2020 785f 696e              x_in
-0000d550: 6974 3d64 465f 696e 6974 2c0a 2020 2020  it=dF_init,.    
-0000d560: 2020 2020 2020 2020 2020 2020 6172 6773              args
-0000d570: 3d28 656e 6572 6779 2c20 6e75 6d5f 636f  =(energy, num_co
-0000d580: 6e66 2c20 6261 7463 685f 7369 7a65 292c  nf, batch_size),
-0000d590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d5a0: 2076 6572 626f 7365 3d76 6572 626f 7365   verbose=verbose
-0000d5b0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0000d5c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000d5d0: 726e 2072 6573 756c 7473 5b22 7822 5d0a  rn results["x"].
-0000d5e0: 0a20 2020 2020 2020 2065 6c69 6620 6d65  .        elif me
-0000d5f0: 7468 6f64 203d 3d20 224c 2d42 4647 532d  thod == "L-BFGS-
-0000d600: 4222 3a0a 2020 2020 2020 2020 2020 2020  B":.            
-0000d610: 6f70 7469 6f6e 7320 3d20 7b22 6469 7370  options = {"disp
-0000d620: 223a 2076 6572 626f 7365 2c20 2267 746f  ": verbose, "gto
-0000d630: 6c22 3a20 3165 2d38 7d0a 2020 2020 2020  l": 1e-8}.      
-0000d640: 2020 2020 2020 7265 7375 6c74 7320 3d20        results = 
-0000d650: 6f70 7469 6d69 7a65 2e6d 696e 696d 697a  optimize.minimiz
-0000d660: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-0000d670: 2020 206c 616d 6264 6120 783a 205b 0a20     lambda x: [. 
-0000d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d690: 2020 2072 2e63 7075 2829 2e6e 756d 7079     r.cpu().numpy
-0000d6a0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0000d6b0: 2020 2020 2020 2066 6f72 2072 2069 6e20         for r in 
-0000d6c0: 5f63 6f6d 7075 7465 5f6c 6f73 735f 616e  _compute_loss_an
-0000d6d0: 645f 6772 6164 5f6f 665f 6446 5f69 6e5f  d_grad_of_dF_in_
-0000d6e0: 6261 7463 6828 0a20 2020 2020 2020 2020  batch(.         
-0000d6f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000d700: 6e65 7267 792e 6e65 775f 7465 6e73 6f72  nergy.new_tensor
-0000d710: 2878 292c 2065 6e65 7267 792c 206e 756d  (x), energy, num
-0000d720: 5f63 6f6e 662c 2062 6174 6368 5f73 697a  _conf, batch_siz
-0000d730: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000d740: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000d750: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-0000d760: 2020 2020 2020 2020 2020 2064 465f 696e             dF_in
-0000d770: 6974 2e63 7075 2829 2e6e 756d 7079 2829  it.cpu().numpy()
-0000d780: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d790: 2020 6a61 633d 5472 7565 2c0a 2020 2020    jac=True,.    
-0000d7a0: 2020 2020 2020 2020 2020 2020 6d65 7468              meth
-0000d7b0: 6f64 3d22 4c2d 4246 4753 2d42 222c 0a20  od="L-BFGS-B",. 
-0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000d7d0: 6f6c 3d31 652d 3132 2c0a 2020 2020 2020  ol=1e-12,.      
-0000d7e0: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
-0000d7f0: 733d 6f70 7469 6f6e 732c 0a20 2020 2020  s=options,.     
-0000d800: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000d810: 2020 2020 2072 6574 7572 6e20 746f 7263       return torc
-0000d820: 682e 6672 6f6d 5f6e 756d 7079 2872 6573  h.from_numpy(res
-0000d830: 756c 7473 5b22 7822 5d29 0a20 2020 2065  ults["x"]).    e
-0000d840: 6c73 653a 0a20 2020 2020 2020 2069 6620  lse:.        if 
-0000d850: 6d65 7468 6f64 203d 3d20 224e 6577 746f  method == "Newto
-0000d860: 6e22 3a0a 2020 2020 2020 2020 2020 2020  n":.            
-0000d870: 7265 7375 6c74 7320 3d20 666d 696e 5f6e  results = fmin_n
-0000d880: 6577 746f 6e28 0a20 2020 2020 2020 2020  ewton(.         
-0000d890: 2020 2020 2020 2066 3d5f 636f 6d70 7574         f=_comput
-0000d8a0: 655f 6c6f 7373 5f61 6e64 5f67 7261 645f  e_loss_and_grad_
-0000d8b0: 6f66 5f64 462c 0a20 2020 2020 2020 2020  of_dF,.         
-0000d8c0: 2020 2020 2020 2068 6573 733d 5f63 6f6d         hess=_com
-0000d8d0: 7075 7465 5f68 6573 7369 616e 5f6c 6f73  pute_hessian_los
-0000d8e0: 735f 6f66 5f64 462c 0a20 2020 2020 2020  s_of_dF,.       
-0000d8f0: 2020 2020 2020 2020 2078 5f69 6e69 743d           x_init=
-0000d900: 6446 5f69 6e69 742c 0a20 2020 2020 2020  dF_init,.       
-0000d910: 2020 2020 2020 2020 2061 7267 733d 2865           args=(e
-0000d920: 6e65 7267 792c 206e 756d 5f63 6f6e 6629  nergy, num_conf)
-0000d930: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d940: 2020 7665 7262 6f73 653d 7665 7262 6f73    verbose=verbos
-0000d950: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
-0000d960: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000d970: 7572 6e20 7265 7375 6c74 735b 2278 225d  urn results["x"]
-0000d980: 0a20 2020 2020 2020 2065 6c69 6620 6d65  .        elif me
-0000d990: 7468 6f64 203d 3d20 224c 2d42 4647 532d  thod == "L-BFGS-
-0000d9a0: 4222 3a0a 2020 2020 2020 2020 2020 2020  B":.            
-0000d9b0: 6f70 7469 6f6e 7320 3d20 7b22 6469 7370  options = {"disp
-0000d9c0: 223a 2076 6572 626f 7365 2c20 2267 746f  ": verbose, "gto
-0000d9d0: 6c22 3a20 3165 2d38 7d0a 2020 2020 2020  l": 1e-8}.      
-0000d9e0: 2020 2020 2020 7265 7375 6c74 7320 3d20        results = 
-0000d9f0: 6f70 7469 6d69 7a65 2e6d 696e 696d 697a  optimize.minimiz
-0000da00: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-0000da10: 2020 206c 616d 6264 6120 783a 205b 0a20     lambda x: [. 
-0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da30: 2020 2072 2e63 7075 2829 2e6e 756d 7079     r.cpu().numpy
-0000da40: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0000da50: 2020 2020 2020 2066 6f72 2072 2069 6e20         for r in 
-0000da60: 5f63 6f6d 7075 7465 5f6c 6f73 735f 616e  _compute_loss_an
-0000da70: 645f 6772 6164 5f6f 665f 6446 280a 2020  d_grad_of_dF(.  
-0000da80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da90: 2020 2020 2020 656e 6572 6779 2e6e 6577        energy.new
-0000daa0: 5f74 656e 736f 7228 7829 2c20 656e 6572  _tensor(x), ener
-0000dab0: 6779 2c20 6e75 6d5f 636f 6e66 0a20 2020  gy, num_conf.   
-0000dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dad0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000dae0: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
-0000daf0: 2020 2020 2020 6446 5f69 6e69 742e 6370        dF_init.cp
-0000db00: 7528 292e 6e75 6d70 7928 292c 0a20 2020  u().numpy(),.   
-0000db10: 2020 2020 2020 2020 2020 2020 206a 6163               jac
-0000db20: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-0000db30: 2020 2020 2020 206d 6574 686f 643d 224c         method="L
-0000db40: 2d42 4647 532d 4222 2c0a 2020 2020 2020  -BFGS-B",.      
-0000db50: 2020 2020 2020 2020 2020 746f 6c3d 3165            tol=1e
-0000db60: 2d31 322c 0a20 2020 2020 2020 2020 2020  -12,.           
-0000db70: 2020 2020 206f 7074 696f 6e73 3d6f 7074       options=opt
-0000db80: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-0000db90: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000dba0: 7265 7475 726e 2074 6f72 6368 2e66 726f  return torch.fro
-0000dbb0: 6d5f 6e75 6d70 7928 7265 7375 6c74 735b  m_numpy(results[
-0000dbc0: 2278 225d 290a 0a0a 6465 6620 5f62 6f6f  "x"])...def _boo
-0000dbd0: 7473 7472 6170 5f63 6f6e 665f 6964 7828  tstrap_conf_idx(
-0000dbe0: 6e75 6d5f 636f 6e66 2c20 626f 6f74 7374  num_conf, bootst
-0000dbf0: 7261 705f 626c 6f63 6b5f 7369 7a65 293a  rap_block_size):
-0000dc00: 0a20 2020 206e 756d 5f63 6f6e 665f 6375  .    num_conf_cu
-0000dc10: 6d73 756d 203d 2074 6f72 6368 2e63 756d  msum = torch.cum
-0000dc20: 7375 6d28 6e75 6d5f 636f 6e66 2c20 6469  sum(num_conf, di
-0000dc30: 6d3d 3029 2e74 6f6c 6973 7428 290a 2020  m=0).tolist().  
-0000dc40: 2020 6e75 6d5f 636f 6e66 5f63 756d 7375    num_conf_cumsu
-0000dc50: 6d2e 706f 7028 2d31 290a 2020 2020 6e75  m.pop(-1).    nu
-0000dc60: 6d5f 636f 6e66 5f63 756d 7375 6d20 3d20  m_conf_cumsum = 
-0000dc70: 5b30 5d20 2b20 6e75 6d5f 636f 6e66 5f63  [0] + num_conf_c
-0000dc80: 756d 7375 6d0a 2020 2020 636f 6e66 5f69  umsum.    conf_i
-0000dc90: 6478 203d 205b 5d0a 2020 2020 666f 7220  dx = [].    for 
-0000dca0: 6920 696e 2072 616e 6765 286c 656e 286e  i in range(len(n
-0000dcb0: 756d 5f63 6f6e 6629 293a 0a20 2020 2020  um_conf)):.     
-0000dcc0: 2020 206c 656e 5f73 6571 203d 2069 6e74     len_seq = int
-0000dcd0: 286e 756d 5f63 6f6e 665b 695d 2920 2023  (num_conf[i])  #
-0000dce0: 2320 7573 696e 6720 6369 7263 756c 6172  # using circular
-0000dcf0: 2062 6c6f 636b 2062 6f6f 7473 7472 6170   block bootstrap
-0000dd00: 0a20 2020 2020 2020 206e 756d 5f73 616d  .        num_sam
-0000dd10: 706c 655f 626c 6f63 6b20 3d20 696e 7428  ple_block = int(
-0000dd20: 6e70 2e63 6569 6c28 6c65 6e5f 7365 7120  np.ceil(len_seq 
-0000dd30: 2f20 626f 6f74 7374 7261 705f 626c 6f63  / bootstrap_bloc
-0000dd40: 6b5f 7369 7a65 2929 0a20 2020 2020 2020  k_size)).       
-0000dd50: 2069 6478 7320 3d20 746f 7263 682e 7261   idxs = torch.ra
-0000dd60: 6e64 696e 7428 302c 206c 656e 5f73 6571  ndint(0, len_seq
-0000dd70: 2c20 286e 756d 5f73 616d 706c 655f 626c  , (num_sample_bl
-0000dd80: 6f63 6b2c 2929 0a20 2020 2020 2020 2073  ock,)).        s
-0000dd90: 616d 706c 655f 6964 7820 3d20 746f 7263  ample_idx = torc
-0000dda0: 682e 6361 7428 0a20 2020 2020 2020 2020  h.cat(.         
-0000ddb0: 2020 205b 746f 7263 682e 6172 616e 6765     [torch.arange
-0000ddc0: 2869 6478 2c20 6964 7820 2b20 626f 6f74  (idx, idx + boot
-0000ddd0: 7374 7261 705f 626c 6f63 6b5f 7369 7a65  strap_block_size
-0000dde0: 2920 666f 7220 6964 7820 696e 2069 6478  ) for idx in idx
-0000ddf0: 735d 0a20 2020 2020 2020 2029 0a20 2020  s].        ).   
-0000de00: 2020 2020 2073 616d 706c 655f 6964 7820       sample_idx 
-0000de10: 3d20 746f 7263 682e 7265 6d61 696e 6465  = torch.remainde
-0000de20: 7228 7361 6d70 6c65 5f69 6478 2c20 6c65  r(sample_idx, le
-0000de30: 6e5f 7365 7129 0a20 2020 2020 2020 2073  n_seq).        s
-0000de40: 616d 706c 655f 6964 7820 3d20 7361 6d70  ample_idx = samp
-0000de50: 6c65 5f69 6478 5b30 3a6c 656e 5f73 6571  le_idx[0:len_seq
-0000de60: 5d0a 2020 2020 2020 2020 7361 6d70 6c65  ].        sample
-0000de70: 5f69 6478 203d 2073 616d 706c 655f 6964  _idx = sample_id
-0000de80: 7820 2b20 6e75 6d5f 636f 6e66 5f63 756d  x + num_conf_cum
-0000de90: 7375 6d5b 695d 0a20 2020 2020 2020 2063  sum[i].        c
-0000dea0: 6f6e 665f 6964 782e 6170 7065 6e64 2873  onf_idx.append(s
-0000deb0: 616d 706c 655f 6964 7829 0a20 2020 2063  ample_idx).    c
-0000dec0: 6f6e 665f 6964 7820 3d20 746f 7263 682e  onf_idx = torch.
-0000ded0: 6361 7428 636f 6e66 5f69 6478 290a 2020  cat(conf_idx).  
-0000dee0: 2020 7265 7475 726e 2063 6f6e 665f 6964    return conf_id
-0000def0: 780a 0a0a 6465 6620 666d 696e 5f6e 6577  x...def fmin_new
-0000df00: 746f 6e28 662c 2068 6573 732c 2078 5f69  ton(f, hess, x_i
-0000df10: 6e69 742c 2061 7267 733d 2829 2c20 7665  nit, args=(), ve
-0000df20: 7262 6f73 653d 5472 7565 2c20 6570 733d  rbose=True, eps=
-0000df30: 3165 2d31 322c 206d 6178 5f69 7465 723d  1e-12, max_iter=
-0000df40: 3330 3029 3a0a 2020 2020 2222 224d 696e  300):.    """Min
-0000df50: 696d 697a 6520 6120 6675 6e63 7469 6f6e  imize a function
-0000df60: 2077 6974 6820 7468 6520 4e65 7774 6f6e   with the Newton
-0000df70: 2773 206d 6574 686f 642e 0a0a 2020 2020  's method...    
-0000df80: 466f 7220 6465 7461 696c 7320 6f66 2074  For details of t
-0000df90: 6865 204e 6577 746f 6e27 7320 6d65 7468  he Newton's meth
-0000dfa0: 6f64 2c20 7365 6520 4368 6170 7465 7220  od, see Chapter 
-0000dfb0: 392e 3520 6f66 2050 726f 662e 2042 6f79  9.5 of Prof. Boy
-0000dfc0: 6427 7320 626f 6f6b 0a20 2020 2060 436f  d's book.    `Co
-0000dfd0: 6e76 6578 204f 7074 696d 697a 6174 696f  nvex Optimizatio
-0000dfe0: 6e20 3c68 7474 7073 3a2f 2f77 6562 2e73  n <https://web.s
-0000dff0: 7461 6e66 6f72 642e 6564 752f 7e62 6f79  tanford.edu/~boy
-0000e000: 642f 6376 7862 6f6f 6b2f 3e60 5f2e 0a0a  d/cvxbook/>`_...
-0000e010: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000e020: 2020 6620 2863 616c 6c61 626c 6529 3a20    f (callable): 
-0000e030: 7468 6520 6f62 6a65 6374 6976 6520 6675  the objective fu
-0000e040: 6e63 7469 6f6e 2074 6f20 6265 206d 696e  nction to be min
-0000e050: 696d 697a 6564 2e0a 2020 2020 2020 2020  imized..        
-0000e060: 2020 2020 6628 783a 5465 6e73 6f72 2c20      f(x:Tensor, 
-0000e070: 2a61 7267 7329 202d 3e20 2028 793a 5465  *args) ->  (y:Te
-0000e080: 6e73 6f72 2c20 6772 6164 3a54 656e 736f  nsor, grad:Tenso
-0000e090: 7229 2c20 7768 6572 650a 2020 2020 2020  r), where.      
-0000e0a0: 2020 2020 2020 7920 6973 2074 6865 2066        y is the f
-0000e0b0: 756e 6374 696f 6e20 7661 6c75 6520 616e  unction value an
-0000e0c0: 6420 6772 6164 2069 7320 7468 6520 6772  d grad is the gr
-0000e0d0: 6164 6965 6e74 2e0a 2020 2020 2020 2020  adient..        
-0000e0e0: 6865 7373 2028 6361 6c6c 6162 6c65 293a  hess (callable):
-0000e0f0: 2074 6865 2066 756e 6374 696f 6e20 746f   the function to
-0000e100: 2063 6f6d 7075 7465 2074 6865 2048 6573   compute the Hes
-0000e110: 7369 616e 206d 6174 7269 782e 0a20 2020  sian matrix..   
-0000e120: 2020 2020 2020 2020 2068 6573 7328 783a           hess(x:
-0000e130: 5465 6e73 6f72 2c20 2a61 7267 7329 202d  Tensor, *args) -
-0000e140: 3e20 6120 7477 6f20 6469 6d65 6e73 696f  > a two dimensio
-0000e150: 6e61 6c20 7465 6e73 6f72 2e0a 2020 2020  nal tensor..    
-0000e160: 2020 2020 785f 696e 6974 2028 5465 6e73      x_init (Tens
-0000e170: 6f72 293a 2074 6865 2069 6e69 7469 616c  or): the initial
-0000e180: 2076 616c 7565 2e0a 2020 2020 2020 2020   value..        
-0000e190: 6172 6773 2028 7475 706c 6529 3a20 6578  args (tuple): ex
-0000e1a0: 7472 6120 7061 7261 6d65 7465 7273 2066  tra parameters f
-0000e1b0: 6f72 2066 2061 6e64 2068 6573 732e 0a20  or f and hess.. 
-0000e1c0: 2020 2020 2020 2076 6572 626f 7365 2028         verbose (
-0000e1d0: 626f 6f6c 293a 2077 6865 7468 6572 2074  bool): whether t
-0000e1e0: 6f20 7072 696e 7420 6d69 6e69 6d69 7a69  o print minimizi
-0000e1f0: 6e67 206c 6f67 2069 6e66 6f72 6d61 7469  ng log informati
-0000e200: 6f6e 2e0a 2020 2020 2020 2020 6570 7320  on..        eps 
-0000e210: 2866 6c6f 6174 293a 2074 6f6c 6572 616e  (float): toleran
-0000e220: 6365 2066 6f72 2073 746f 7070 696e 670a  ce for stopping.
-0000e230: 2020 2020 2020 2020 6d61 785f 6974 6572          max_iter
-0000e240: 2028 696e 7429 3a20 6d61 7869 6d75 6d20   (int): maximum 
-0000e250: 6e75 6d62 6572 206f 6620 6974 6572 6174  number of iterat
-0000e260: 696f 6e73 2e0a 2020 2020 2222 220a 0a20  ions..    """.. 
-0000e270: 2020 2023 2320 636f 6e73 7461 6e74 7320     ## constants 
-0000e280: 7573 6564 2069 6e20 6261 636b 7472 6163  used in backtrac
-0000e290: 6b69 6e67 206c 696e 6520 7365 6172 6368  king line search
-0000e2a0: 0a20 2020 2061 6c70 6861 2c20 6265 7461  .    alpha, beta
-0000e2b0: 203d 2030 2e30 312c 2030 2e32 0a0a 2020   = 0.01, 0.2..  
-0000e2c0: 2020 2323 204e 6577 746f 6e27 7320 6d65    ## Newton's me
-0000e2d0: 7468 6f64 2066 6f72 206d 696e 696d 697a  thod for minimiz
-0000e2e0: 696e 6720 7468 6520 6675 6e63 7469 6f6e  ing the function
-0000e2f0: 0a20 2020 2069 6e64 785f 6974 6572 203d  .    indx_iter =
-0000e300: 2030 0a0a 2020 2020 4e5f 6675 6e63 203d   0..    N_func =
-0000e310: 2030 0a0a 2020 2020 6966 2076 6572 626f   0..    if verbo
-0000e320: 7365 3a0a 2020 2020 2020 2020 7072 696e  se:.        prin
-0000e330: 7428 223d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  t("=============
+00005b20: 6a4c 0300 0068 6c6a 4d03 0000 5d94 6a50  jL...hljM...].jP
+00005b30: 0300 008c 0d57 6879 2046 6173 744d 4241  .....Why FastMBA
+00005b40: 523f 9485 9481 947d 946a 5503 0000 6a6e  R?.....}.jU...jn
+00005b50: 0600 0073 6261 6a56 0300 007d 9428 6a6c  ...sbajV...}.(jl
+00005b60: 0300 005d 946a 6e03 0000 5d94 6a70 0300  ...].jn...].jp..
+00005b70: 005d 946a 7203 0000 5d94 6a74 0300 005d  .].jr...].jt...]
+00005b80: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
+00005b90: 6566 7572 6994 6ae8 0200 008c 0a61 6e63  efuri.j......anc
+00005ba0: 686f 726e 616d 6594 8c0d 2377 6879 2d66  horname...#why-f
+00005bb0: 6173 746d 6261 7294 756a 6203 0000 6ad8  astmbar.ujb...j.
+00005bc0: 0300 006a 5503 0000 6a6b 0600 0075 6261  ...jU...jk...uba
+00005bd0: 6a56 0300 007d 9428 6a6c 0300 005d 946a  jV...}.(jl...].j
+00005be0: 6e03 0000 5d94 6a70 0300 005d 946a 7203  n...].jp...].jr.
+00005bf0: 0000 5d94 6a74 0300 005d 9475 6a62 0300  ..].jt...].ujb..
+00005c00: 006a d303 0000 6a55 0300 006a 6806 0000  .j....jU...jh...
+00005c10: 7562 616a 5603 0000 7d94 286a 6c03 0000  ubajV...}.(jl...
+00005c20: 5d94 6a6e 0300 005d 946a 7003 0000 5d94  ].jn...].jp...].
+00005c30: 6a72 0300 005d 946a 7403 0000 5d94 756a  jr...].jt...].uj
+00005c40: 6203 0000 6acd 0300 006a 5503 0000 6a42  b...j....jU...jB
+00005c50: 0600 0075 626a ce03 0000 2981 947d 9428  ...ubj....)..}.(
+00005c60: 6a4c 0300 0068 6c6a 4d03 0000 5d94 286a  jL...hljM...].(j
+00005c70: d403 0000 2981 947d 9428 6a4c 0300 0068  ....)..}.(jL...h
+00005c80: 6c6a 4d03 0000 5d94 6ad9 0300 0029 8194  ljM...].j....)..
+00005c90: 7d94 286a 4c03 0000 686c 6a4d 0300 005d  }.(jL...hljM...]
+00005ca0: 946a 5003 0000 8c14 486f 7720 746f 2075  .jP.....How to u
+00005cb0: 7365 2046 6173 744d 4241 523f 9485 9481  se FastMBAR?....
+00005cc0: 947d 946a 5503 0000 6a91 0600 0073 6261  .}.jU...j....sba
+00005cd0: 6a56 0300 007d 9428 6a6c 0300 005d 946a  jV...}.(jl...].j
+00005ce0: 6e03 0000 5d94 6a70 0300 005d 946a 7203  n...].jp...].jr.
+00005cf0: 0000 5d94 6a74 0300 005d 948c 0869 6e74  ..].jt...]...int
+00005d00: 6572 6e61 6c94 888c 0672 6566 7572 6994  ernal....refuri.
+00005d10: 6ae8 0200 008c 0a61 6e63 686f 726e 616d  j......anchornam
+00005d20: 6594 8c14 2368 6f77 2d74 6f2d 7573 652d  e...#how-to-use-
+00005d30: 6661 7374 6d62 6172 9475 6a62 0300 006a  fastmbar.ujb...j
+00005d40: d803 0000 6a55 0300 006a 8e06 0000 7562  ....jU...j....ub
+00005d50: 616a 5603 0000 7d94 286a 6c03 0000 5d94  ajV...}.(jl...].
+00005d60: 6a6e 0300 005d 946a 7003 0000 5d94 6a72  jn...].jp...].jr
+00005d70: 0300 005d 946a 7403 0000 5d94 756a 6203  ...].jt...].ujb.
+00005d80: 0000 6ad3 0300 006a 5503 0000 6a8b 0600  ..j....jU...j...
+00005d90: 0075 626a c903 0000 2981 947d 9428 6a4c  .ubj....)..}.(jL
+00005da0: 0300 0068 6c6a 4d03 0000 5d94 6ae6 0500  ...hljM...].j...
+00005db0: 0029 8194 7d94 286a 4c03 0000 686c 6a4d  .)..}.(jL...hljM
+00005dc0: 0300 005d 946a 5603 0000 7d94 286a 6c03  ...].jV...}.(jl.
+00005dd0: 0000 5d94 6a6e 0300 005d 946a 7003 0000  ..].jn...].jp...
+00005de0: 5d94 6a72 0300 005d 946a 7403 0000 5d94  ].jr...].jt...].
+00005df0: 8c06 7061 7265 6e74 946a e802 0000 8c07  ..parent.j......
+00005e00: 656e 7472 6965 7394 5d94 284e 8c0c 696e  entries.].(N..in
+00005e10: 7374 616c 6c61 7469 6f6e 9486 944e 8c05  stallation...N..
+00005e20: 7573 6167 6594 8694 4e8c 0341 5049 9486  usage...N..API..
+00005e30: 944e 8c08 6578 616d 706c 6573 9486 944e  .N..examples...N
+00005e40: 8c0a 7265 6665 7265 6e63 6573 9486 9465  ..references...e
+00005e50: 8c0c 696e 636c 7564 6566 696c 6573 945d  ..includefiles.]
+00005e60: 9428 6ab7 0600 006a b906 0000 6abb 0600  .(j....j....j...
+00005e70: 006a bd06 0000 6abf 0600 0065 8c08 6d61  .j....j....e..ma
+00005e80: 7864 6570 7468 944b 028c 0763 6170 7469  xdepth.K...capti
+00005e90: 6f6e 944e 8c04 676c 6f62 9489 8c06 6869  on.N..glob....hi
+00005ea0: 6464 656e 9489 8c0d 696e 636c 7564 6568  dden....includeh
+00005eb0: 6964 6465 6e94 898c 086e 756d 6265 7265  idden....numbere
+00005ec0: 6494 4b00 8c0a 7469 746c 6573 6f6e 6c79  d.K...titlesonly
+00005ed0: 9489 8c0a 7261 7765 6e74 7269 6573 945d  ....rawentries.]
+00005ee0: 9475 6a62 0300 006a e505 0000 6a02 0600  .ujb...j....j...
+00005ef0: 008c 652f 5573 6572 732f 6469 6e67 7871  ..e/Users/dingxq
+00005f00: 2f4c 6962 7261 7279 2f43 6c6f 7564 5374  /Library/CloudSt
+00005f10: 6f72 6167 652f 426f 782d 426f 782f 5265  orage/Box-Box/Re
+00005f20: 7365 6172 6368 2f50 726f 6a65 6374 735f  search/Projects_
+00005f30: 6f6e 5f47 6974 6875 622f 4661 7374 4d42  on_Github/FastMB
+00005f40: 4152 2f64 6f63 732f 736f 7572 6365 2f69  AR/docs/source/i
+00005f50: 6e64 6578 2e72 7374 946a 0406 0000 4b20  ndex.rst.j....K 
+00005f60: 6a55 0300 006a a806 0000 7562 616a 5603  jU...j....ubajV.
+00005f70: 0000 7d94 286a 6c03 0000 5d94 6a6e 0300  ..}.(jl...].jn..
+00005f80: 005d 946a 7003 0000 5d94 6a72 0300 005d  .].jp...].jr...]
+00005f90: 946a 7403 0000 5d94 756a 6203 0000 6ac8  .jt...].ujb...j.
+00005fa0: 0300 006a 5503 0000 6a8b 0600 0075 6265  ...jU...j....ube
+00005fb0: 6a56 0300 007d 9428 6a6c 0300 005d 946a  jV...}.(jl...].j
+00005fc0: 6e03 0000 5d94 6a70 0300 005d 946a 7203  n...].jp...].jr.
+00005fd0: 0000 5d94 6a74 0300 005d 9475 6a62 0300  ..].jt...].ujb..
+00005fe0: 006a cd03 0000 6a55 0300 006a 4206 0000  .j....jU...jB...
+00005ff0: 7562 656a 5603 0000 7d94 286a 6c03 0000  ubejV...}.(jl...
+00006000: 5d94 6a6e 0300 005d 946a 7003 0000 5d94  ].jn...].jp...].
+00006010: 6a72 0300 005d 946a 7403 0000 5d94 756a  jr...].jt...].uj
+00006020: 6203 0000 6ac8 0300 006a 5503 0000 6a26  b...j....jU...j&
+00006030: 0600 0075 6265 6a56 0300 007d 9428 6a6c  ...ubejV...}.(jl
+00006040: 0300 005d 946a 6e03 0000 5d94 6a70 0300  ...].jn...].jp..
+00006050: 005d 946a 7203 0000 5d94 6a74 0300 005d  .].jr...].jt...]
+00006060: 9475 6a62 0300 006a cd03 0000 6a55 0300  .ujb...j....jU..
+00006070: 006a 2306 0000 7562 616a 5603 0000 7d94  .j#...ubajV...}.
+00006080: 286a 6c03 0000 5d94 6a6e 0300 005d 946a  (jl...].jn...].j
+00006090: 7003 0000 5d94 6a72 0300 005d 946a 7403  p...].jr...].jt.
+000060a0: 0000 5d94 756a 6203 0000 6ac8 0300 0075  ..].ujb...j....u
+000060b0: 626a ec02 0000 6ac9 0300 0029 8194 7d94  bj....j....)..}.
+000060c0: 286a 4c03 0000 686c 6a4d 0300 005d 946a  (jL...hljM...].j
+000060d0: ce03 0000 2981 947d 9428 6a4c 0300 0068  ....)..}.(jL...h
+000060e0: 6c6a 4d03 0000 5d94 286a d403 0000 2981  ljM...].(j....).
+000060f0: 947d 9428 6a4c 0300 0068 6c6a 4d03 0000  .}.(jL...hljM...
+00006100: 5d94 6ad9 0300 0029 8194 7d94 286a 4c03  ].j....)..}.(jL.
+00006110: 0000 686c 6a4d 0300 005d 946a 5003 0000  ..hljM...].jP...
+00006120: 8c0c 496e 7374 616c 6c61 7469 6f6e 9485  ..Installation..
+00006130: 9481 947d 946a 5503 0000 6af4 0600 0073  ...}.jU...j....s
+00006140: 6261 6a56 0300 007d 9428 6a6c 0300 005d  bajV...}.(jl...]
+00006150: 946a 6e03 0000 5d94 6a70 0300 005d 946a  .jn...].jp...].j
+00006160: 7203 0000 5d94 6a74 0300 005d 948c 0869  r...].jt...]...i
+00006170: 6e74 6572 6e61 6c94 888c 0672 6566 7572  nternal....refur
+00006180: 6994 6aec 0200 008c 0a61 6e63 686f 726e  i.j......anchorn
+00006190: 616d 6594 686c 756a 6203 0000 6ad8 0300  ame.hlujb...j...
+000061a0: 006a 5503 0000 6af1 0600 0075 6261 6a56  .jU...j....ubajV
+000061b0: 0300 007d 9428 6a6c 0300 005d 946a 6e03  ...}.(jl...].jn.
+000061c0: 0000 5d94 6a70 0300 005d 946a 7203 0000  ..].jp...].jr...
+000061d0: 5d94 6a74 0300 005d 9475 6a62 0300 006a  ].jt...].ujb...j
+000061e0: d303 0000 6a55 0300 006a ee06 0000 7562  ....jU...j....ub
+000061f0: 6ac9 0300 0029 8194 7d94 286a 4c03 0000  j....)..}.(jL...
+00006200: 686c 6a4d 0300 005d 9428 6ace 0300 0029  hljM...].(j....)
+00006210: 8194 7d94 286a 4c03 0000 686c 6a4d 0300  ..}.(jL...hljM..
+00006220: 005d 946a d403 0000 2981 947d 9428 6a4c  .].j....)..}.(jL
+00006230: 0300 0068 6c6a 4d03 0000 5d94 6ad9 0300  ...hljM...].j...
+00006240: 0029 8194 7d94 286a 4c03 0000 686c 6a4d  .)..}.(jL...hljM
+00006250: 0300 005d 946a 5003 0000 8c1d 312e 204e  ...].jP.....1. N
+00006260: 6577 2074 6f20 5079 7468 6f6e 206f 7220  ew to Python or 
+00006270: 416e 6163 6f6e 6461 3f94 8594 8194 7d94  Anaconda?.....}.
+00006280: 6a55 0300 006a 1307 0000 7362 616a 5603  jU...j....sbajV.
+00006290: 0000 7d94 286a 6c03 0000 5d94 6a6e 0300  ..}.(jl...].jn..
+000062a0: 005d 946a 7003 0000 5d94 6a72 0300 005d  .].jp...].jr...]
+000062b0: 946a 7403 0000 5d94 8c08 696e 7465 726e  .jt...]...intern
+000062c0: 616c 9488 8c06 7265 6675 7269 946a ec02  al....refuri.j..
+000062d0: 0000 8c0a 616e 6368 6f72 6e61 6d65 948c  ....anchorname..
+000062e0: 1a23 6e65 772d 746f 2d70 7974 686f 6e2d  .#new-to-python-
+000062f0: 6f72 2d61 6e61 636f 6e64 6194 756a 6203  or-anaconda.ujb.
+00006300: 0000 6ad8 0300 006a 5503 0000 6a10 0700  ..j....jU...j...
+00006310: 0075 6261 6a56 0300 007d 9428 6a6c 0300  .ubajV...}.(jl..
+00006320: 005d 946a 6e03 0000 5d94 6a70 0300 005d  .].jn...].jp...]
+00006330: 946a 7203 0000 5d94 6a74 0300 005d 9475  .jr...].jt...].u
+00006340: 6a62 0300 006a d303 0000 6a55 0300 006a  jb...j....jU...j
+00006350: 0d07 0000 7562 616a 5603 0000 7d94 286a  ....ubajV...}.(j
+00006360: 6c03 0000 5d94 6a6e 0300 005d 946a 7003  l...].jn...].jp.
+00006370: 0000 5d94 6a72 0300 005d 946a 7403 0000  ..].jr...].jt...
+00006380: 5d94 756a 6203 0000 6acd 0300 006a 5503  ].ujb...j....jU.
+00006390: 0000 6a0a 0700 0075 626a ce03 0000 2981  ..j....ubj....).
+000063a0: 947d 9428 6a4c 0300 0068 6c6a 4d03 0000  .}.(jL...hljM...
+000063b0: 5d94 6ad4 0300 0029 8194 7d94 286a 4c03  ].j....)..}.(jL.
+000063c0: 0000 686c 6a4d 0300 005d 946a d903 0000  ..hljM...].j....
+000063d0: 2981 947d 9428 6a4c 0300 0068 6c6a 4d03  )..}.(jL...hljM.
+000063e0: 0000 5d94 6a50 0300 008c 1c32 2e20 496e  ..].jP.....2. In
+000063f0: 7374 616c 6c20 4661 7374 4d42 4152 2077  stall FastMBAR w
+00006400: 6974 6820 7069 7094 8594 8194 7d94 6a55  ith pip.....}.jU
+00006410: 0300 006a 3607 0000 7362 616a 5603 0000  ...j6...sbajV...
+00006420: 7d94 286a 6c03 0000 5d94 6a6e 0300 005d  }.(jl...].jn...]
+00006430: 946a 7003 0000 5d94 6a72 0300 005d 946a  .jp...].jr...].j
+00006440: 7403 0000 5d94 8c08 696e 7465 726e 616c  t...]...internal
+00006450: 9488 8c06 7265 6675 7269 946a ec02 0000  ....refuri.j....
+00006460: 8c0a 616e 6368 6f72 6e61 6d65 948c 1a23  ..anchorname...#
+00006470: 696e 7374 616c 6c2d 6661 7374 6d62 6172  install-fastmbar
+00006480: 2d77 6974 682d 7069 7094 756a 6203 0000  -with-pip.ujb...
+00006490: 6ad8 0300 006a 5503 0000 6a33 0700 0075  j....jU...j3...u
+000064a0: 6261 6a56 0300 007d 9428 6a6c 0300 005d  bajV...}.(jl...]
+000064b0: 946a 6e03 0000 5d94 6a70 0300 005d 946a  .jn...].jp...].j
+000064c0: 7203 0000 5d94 6a74 0300 005d 9475 6a62  r...].jt...].ujb
+000064d0: 0300 006a d303 0000 6a55 0300 006a 3007  ...j....jU...j0.
+000064e0: 0000 7562 616a 5603 0000 7d94 286a 6c03  ..ubajV...}.(jl.
+000064f0: 0000 5d94 6a6e 0300 005d 946a 7003 0000  ..].jn...].jp...
+00006500: 5d94 6a72 0300 005d 946a 7403 0000 5d94  ].jr...].jt...].
+00006510: 756a 6203 0000 6acd 0300 006a 5503 0000  ujb...j....jU...
+00006520: 6a0a 0700 0075 626a ce03 0000 2981 947d  j....ubj....)..}
+00006530: 9428 6a4c 0300 0068 6c6a 4d03 0000 5d94  .(jL...hljM...].
+00006540: 6ad4 0300 0029 8194 7d94 286a 4c03 0000  j....)..}.(jL...
+00006550: 686c 6a4d 0300 005d 946a d903 0000 2981  hljM...].j....).
+00006560: 947d 9428 6a4c 0300 0068 6c6a 4d03 0000  .}.(jL...hljM...
+00006570: 5d94 6a50 0300 008c 2433 2e20 5465 7374  ].jP....$3. Test
+00006580: 2074 6865 2049 6e73 7461 6c6c 6174 696f   the Installatio
+00006590: 6e20 6f66 2046 6173 744d 4241 5294 8594  n of FastMBAR...
+000065a0: 8194 7d94 6a55 0300 006a 5907 0000 7362  ..}.jU...jY...sb
+000065b0: 616a 5603 0000 7d94 286a 6c03 0000 5d94  ajV...}.(jl...].
+000065c0: 6a6e 0300 005d 946a 7003 0000 5d94 6a72  jn...].jp...].jr
+000065d0: 0300 005d 946a 7403 0000 5d94 8c08 696e  ...].jt...]...in
+000065e0: 7465 726e 616c 9488 8c06 7265 6675 7269  ternal....refuri
+000065f0: 946a ec02 0000 8c0a 616e 6368 6f72 6e61  .j......anchorna
+00006600: 6d65 948c 2223 7465 7374 2d74 6865 2d69  me.."#test-the-i
+00006610: 6e73 7461 6c6c 6174 696f 6e2d 6f66 2d66  nstallation-of-f
+00006620: 6173 746d 6261 7294 756a 6203 0000 6ad8  astmbar.ujb...j.
+00006630: 0300 006a 5503 0000 6a56 0700 0075 6261  ...jU...jV...uba
+00006640: 6a56 0300 007d 9428 6a6c 0300 005d 946a  jV...}.(jl...].j
+00006650: 6e03 0000 5d94 6a70 0300 005d 946a 7203  n...].jp...].jr.
+00006660: 0000 5d94 6a74 0300 005d 9475 6a62 0300  ..].jt...].ujb..
+00006670: 006a d303 0000 6a55 0300 006a 5307 0000  .j....jU...jS...
+00006680: 7562 616a 5603 0000 7d94 286a 6c03 0000  ubajV...}.(jl...
+00006690: 5d94 6a6e 0300 005d 946a 7003 0000 5d94  ].jn...].jp...].
+000066a0: 6a72 0300 005d 946a 7403 0000 5d94 756a  jr...].jt...].uj
+000066b0: 6203 0000 6acd 0300 006a 5503 0000 6a0a  b...j....jU...j.
+000066c0: 0700 0075 6265 6a56 0300 007d 9428 6a6c  ...ubejV...}.(jl
+000066d0: 0300 005d 946a 6e03 0000 5d94 6a70 0300  ...].jn...].jp..
+000066e0: 005d 946a 7203 0000 5d94 6a74 0300 005d  .].jr...].jt...]
+000066f0: 9475 6a62 0300 006a c803 0000 6a55 0300  .ujb...j....jU..
+00006700: 006a ee06 0000 7562 656a 5603 0000 7d94  .j....ubejV...}.
+00006710: 286a 6c03 0000 5d94 6a6e 0300 005d 946a  (jl...].jn...].j
+00006720: 7003 0000 5d94 6a72 0300 005d 946a 7403  p...].jr...].jt.
+00006730: 0000 5d94 756a 6203 0000 6acd 0300 006a  ..].ujb...j....j
+00006740: 5503 0000 6aeb 0600 0075 6261 6a56 0300  U...j....ubajV..
+00006750: 007d 9428 6a6c 0300 005d 946a 6e03 0000  .}.(jl...].jn...
+00006760: 5d94 6a70 0300 005d 946a 7203 0000 5d94  ].jp...].jr...].
+00006770: 6a74 0300 005d 9475 6a62 0300 006a c803  jt...].ujb...j..
+00006780: 0000 7562 6aea 0200 006a c903 0000 2981  ..ubj....j....).
+00006790: 947d 9428 6a4c 0300 0068 6c6a 4d03 0000  .}.(jL...hljM...
+000067a0: 5d94 6ace 0300 0029 8194 7d94 286a 4c03  ].j....)..}.(jL.
+000067b0: 0000 686c 6a4d 0300 005d 946a d403 0000  ..hljM...].j....
+000067c0: 2981 947d 9428 6a4c 0300 0068 6c6a 4d03  )..}.(jL...hljM.
+000067d0: 0000 5d94 6ad9 0300 0029 8194 7d94 286a  ..].j....)..}.(j
+000067e0: 4c03 0000 686c 6a4d 0300 005d 946a 5003  L...hljM...].jP.
+000067f0: 0000 8c0a 5265 6665 7265 6e63 6573 9485  ....References..
+00006800: 9481 947d 946a 5503 0000 6a91 0700 0073  ...}.jU...j....s
+00006810: 6261 6a56 0300 007d 9428 6a6c 0300 005d  bajV...}.(jl...]
+00006820: 946a 6e03 0000 5d94 6a70 0300 005d 946a  .jn...].jp...].j
+00006830: 7203 0000 5d94 6a74 0300 005d 948c 0869  r...].jt...]...i
+00006840: 6e74 6572 6e61 6c94 888c 0672 6566 7572  nternal....refur
+00006850: 6994 6aea 0200 008c 0a61 6e63 686f 726e  i.j......anchorn
+00006860: 616d 6594 686c 756a 6203 0000 6ad8 0300  ame.hlujb...j...
+00006870: 006a 5503 0000 6a8e 0700 0075 6261 6a56  .jU...j....ubajV
+00006880: 0300 007d 9428 6a6c 0300 005d 946a 6e03  ...}.(jl...].jn.
+00006890: 0000 5d94 6a70 0300 005d 946a 7203 0000  ..].jp...].jr...
+000068a0: 5d94 6a74 0300 005d 9475 6a62 0300 006a  ].jt...].ujb...j
+000068b0: d303 0000 6a55 0300 006a 8b07 0000 7562  ....jU...j....ub
+000068c0: 616a 5603 0000 7d94 286a 6c03 0000 5d94  ajV...}.(jl...].
+000068d0: 6a6e 0300 005d 946a 7003 0000 5d94 6a72  jn...].jp...].jr
+000068e0: 0300 005d 946a 7403 0000 5d94 756a 6203  ...].jt...].ujb.
+000068f0: 0000 6acd 0300 006a 5503 0000 6a88 0700  ..j....jU...j...
+00006900: 0075 6261 6a56 0300 007d 9428 6a6c 0300  .ubajV...}.(jl..
+00006910: 005d 946a 6e03 0000 5d94 6a70 0300 005d  .].jn...].jp...]
+00006920: 946a 7203 0000 5d94 6a74 0300 005d 9475  .jr...].jt...].u
+00006930: 6a62 0300 006a c803 0000 7562 6aed 0200  jb...j....ubj...
+00006940: 006a c903 0000 2981 947d 9428 6a4c 0300  .j....)..}.(jL..
+00006950: 0068 6c6a 4d03 0000 5d94 6ace 0300 0029  .hljM...].j....)
+00006960: 8194 7d94 286a 4c03 0000 686c 6a4d 0300  ..}.(jL...hljM..
+00006970: 005d 9428 6ad4 0300 0029 8194 7d94 286a  .].(j....)..}.(j
+00006980: 4c03 0000 686c 6a4d 0300 005d 946a d903  L...hljM...].j..
+00006990: 0000 2981 947d 9428 6a4c 0300 0068 6c6a  ..)..}.(jL...hlj
+000069a0: 4d03 0000 5d94 6a50 0300 008c 0555 7361  M...].jP.....Usa
+000069b0: 6765 9485 9481 947d 946a 5503 0000 6abc  ge.....}.jU...j.
+000069c0: 0700 0073 6261 6a56 0300 007d 9428 6a6c  ...sbajV...}.(jl
+000069d0: 0300 005d 946a 6e03 0000 5d94 6a70 0300  ...].jn...].jp..
+000069e0: 005d 946a 7203 0000 5d94 6a74 0300 005d  .].jr...].jt...]
+000069f0: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
+00006a00: 6566 7572 6994 6aed 0200 008c 0a61 6e63  efuri.j......anc
+00006a10: 686f 726e 616d 6594 686c 756a 6203 0000  horname.hlujb...
+00006a20: 6ad8 0300 006a 5503 0000 6ab9 0700 0075  j....jU...j....u
+00006a30: 6261 6a56 0300 007d 9428 6a6c 0300 005d  bajV...}.(jl...]
+00006a40: 946a 6e03 0000 5d94 6a70 0300 005d 946a  .jn...].jp...].j
+00006a50: 7203 0000 5d94 6a74 0300 005d 9475 6a62  r...].jt...].ujb
+00006a60: 0300 006a d303 0000 6a55 0300 006a b607  ...j....jU...j..
+00006a70: 0000 7562 6ac9 0300 0029 8194 7d94 286a  ..ubj....)..}.(j
+00006a80: 4c03 0000 686c 6a4d 0300 005d 9428 6ace  L...hljM...].(j.
+00006a90: 0300 0029 8194 7d94 286a 4c03 0000 686c  ...)..}.(jL...hl
+00006aa0: 6a4d 0300 005d 946a d403 0000 2981 947d  jM...].j....)..}
+00006ab0: 9428 6a4c 0300 0068 6c6a 4d03 0000 5d94  .(jL...hljM...].
+00006ac0: 6ad9 0300 0029 8194 7d94 286a 4c03 0000  j....)..}.(jL...
+00006ad0: 686c 6a4d 0300 005d 946a 5003 0000 8c1e  hljM...].jP.....
+00006ae0: 312e 2057 6865 6e20 746f 2075 7365 204d  1. When to use M
+00006af0: 4241 5220 6571 7561 7469 6f6e 733f 9485  BAR equations?..
+00006b00: 9481 947d 946a 5503 0000 6adb 0700 0073  ...}.jU...j....s
+00006b10: 6261 6a56 0300 007d 9428 6a6c 0300 005d  bajV...}.(jl...]
+00006b20: 946a 6e03 0000 5d94 6a70 0300 005d 946a  .jn...].jp...].j
+00006b30: 7203 0000 5d94 6a74 0300 005d 948c 0869  r...].jt...]...i
+00006b40: 6e74 6572 6e61 6c94 888c 0672 6566 7572  nternal....refur
+00006b50: 6994 6aed 0200 008c 0a61 6e63 686f 726e  i.j......anchorn
+00006b60: 616d 6594 8c1b 2377 6865 6e2d 746f 2d75  ame...#when-to-u
+00006b70: 7365 2d6d 6261 722d 6571 7561 7469 6f6e  se-mbar-equation
+00006b80: 7394 756a 6203 0000 6ad8 0300 006a 5503  s.ujb...j....jU.
+00006b90: 0000 6ad8 0700 0075 6261 6a56 0300 007d  ..j....ubajV...}
+00006ba0: 9428 6a6c 0300 005d 946a 6e03 0000 5d94  .(jl...].jn...].
+00006bb0: 6a70 0300 005d 946a 7203 0000 5d94 6a74  jp...].jr...].jt
+00006bc0: 0300 005d 9475 6a62 0300 006a d303 0000  ...].ujb...j....
+00006bd0: 6a55 0300 006a d507 0000 7562 616a 5603  jU...j....ubajV.
+00006be0: 0000 7d94 286a 6c03 0000 5d94 6a6e 0300  ..}.(jl...].jn..
+00006bf0: 005d 946a 7003 0000 5d94 6a72 0300 005d  .].jp...].jr...]
+00006c00: 946a 7403 0000 5d94 756a 6203 0000 6acd  .jt...].ujb...j.
+00006c10: 0300 006a 5503 0000 6ad2 0700 0075 626a  ...jU...j....ubj
+00006c20: ce03 0000 2981 947d 9428 6a4c 0300 0068  ....)..}.(jL...h
+00006c30: 6c6a 4d03 0000 5d94 6ad4 0300 0029 8194  ljM...].j....)..
+00006c40: 7d94 286a 4c03 0000 686c 6a4d 0300 005d  }.(jL...hljM...]
+00006c50: 946a d903 0000 2981 947d 9428 6a4c 0300  .j....)..}.(jL..
+00006c60: 0068 6c6a 4d03 0000 5d94 6a50 0300 008c  .hljM...].jP....
+00006c70: 1732 2e20 486f 7720 746f 2075 7365 2046  .2. How to use F
+00006c80: 6173 744d 4241 523f 9485 9481 947d 946a  astMBAR?.....}.j
+00006c90: 5503 0000 6afe 0700 0073 6261 6a56 0300  U...j....sbajV..
+00006ca0: 007d 9428 6a6c 0300 005d 946a 6e03 0000  .}.(jl...].jn...
+00006cb0: 5d94 6a70 0300 005d 946a 7203 0000 5d94  ].jp...].jr...].
+00006cc0: 6a74 0300 005d 948c 0869 6e74 6572 6e61  jt...]...interna
+00006cd0: 6c94 888c 0672 6566 7572 6994 6aed 0200  l....refuri.j...
+00006ce0: 008c 0a61 6e63 686f 726e 616d 6594 8c14  ...anchorname...
+00006cf0: 2368 6f77 2d74 6f2d 7573 652d 6661 7374  #how-to-use-fast
+00006d00: 6d62 6172 9475 6a62 0300 006a d803 0000  mbar.ujb...j....
+00006d10: 6a55 0300 006a fb07 0000 7562 616a 5603  jU...j....ubajV.
+00006d20: 0000 7d94 286a 6c03 0000 5d94 6a6e 0300  ..}.(jl...].jn..
+00006d30: 005d 946a 7003 0000 5d94 6a72 0300 005d  .].jp...].jr...]
+00006d40: 946a 7403 0000 5d94 756a 6203 0000 6ad3  .jt...].ujb...j.
+00006d50: 0300 006a 5503 0000 6af8 0700 0075 6261  ...jU...j....uba
+00006d60: 6a56 0300 007d 9428 6a6c 0300 005d 946a  jV...}.(jl...].j
+00006d70: 6e03 0000 5d94 6a70 0300 005d 946a 7203  n...].jp...].jr.
+00006d80: 0000 5d94 6a74 0300 005d 9475 6a62 0300  ..].jt...].ujb..
+00006d90: 006a cd03 0000 6a55 0300 006a d207 0000  .j....jU...j....
+00006da0: 7562 656a 5603 0000 7d94 286a 6c03 0000  ubejV...}.(jl...
+00006db0: 5d94 6a6e 0300 005d 946a 7003 0000 5d94  ].jn...].jp...].
+00006dc0: 6a72 0300 005d 946a 7403 0000 5d94 756a  jr...].jt...].uj
+00006dd0: 6203 0000 6ac8 0300 006a 5503 0000 6ab6  b...j....jU...j.
+00006de0: 0700 0075 6265 6a56 0300 007d 9428 6a6c  ...ubejV...}.(jl
+00006df0: 0300 005d 946a 6e03 0000 5d94 6a70 0300  ...].jn...].jp..
+00006e00: 005d 946a 7203 0000 5d94 6a74 0300 005d  .].jr...].jt...]
+00006e10: 9475 6a62 0300 006a cd03 0000 6a55 0300  .ujb...j....jU..
+00006e20: 006a b307 0000 7562 616a 5603 0000 7d94  .j....ubajV...}.
+00006e30: 286a 6c03 0000 5d94 6a6e 0300 005d 946a  (jl...].jn...].j
+00006e40: 7003 0000 5d94 6a72 0300 005d 946a 7403  p...].jr...].jt.
+00006e50: 0000 5d94 756a 6203 0000 6ac8 0300 0075  ..].ujb...j....u
+00006e60: 6275 8c0f 746f 635f 6e75 6d5f 656e 7472  bu..toc_num_entr
+00006e70: 6965 7394 7d94 286a 1c03 0000 4b05 6ae9  ies.}.(j....K.j.
+00006e80: 0200 004b 016a ee02 0000 4b05 6ae7 0200  ...K.j....K.j...
+00006e90: 004b 036a e802 0000 4b04 6aec 0200 004b  .K.j....K.j....K
+00006ea0: 046a ea02 0000 4b01 6aed 0200 004b 0375  .j....K.j....K.u
+00006eb0: 8c0e 746f 635f 7365 636e 756d 6265 7273  ..toc_secnumbers
+00006ec0: 947d 948c 0e74 6f63 5f66 6967 6e75 6d62  .}...toc_fignumb
+00006ed0: 6572 7394 7d94 8c10 746f 6374 7265 655f  ers.}...toctree_
+00006ee0: 696e 636c 7564 6573 947d 9428 6ae7 0200  includes.}.(j...
+00006ef0: 005d 9428 6af3 0500 006a f505 0000 656a  .].(j....j....ej
+00006f00: e802 0000 5d94 286a b706 0000 6ab9 0600  ....].(j....j...
+00006f10: 006a bb06 0000 6abd 0600 006a bf06 0000  .j....j....j....
+00006f20: 6575 8c10 6669 6c65 735f 746f 5f72 6562  eu..files_to_reb
+00006f30: 7569 6c64 947d 9428 6af3 0500 008f 9428  uild.}.(j......(
+00006f40: 6ae7 0200 0090 6af5 0500 008f 9428 6ae7  j.....j......(j.
+00006f50: 0200 0090 6ab7 0600 008f 9428 6ae8 0200  ....j......(j...
+00006f60: 0090 6ab9 0600 008f 9428 6ae8 0200 0090  ..j......(j.....
+00006f70: 6abb 0600 008f 9428 6ae8 0200 0090 6abd  j......(j.....j.
+00006f80: 0600 008f 9428 6ae8 0200 0090 6abf 0600  .....(j.....j...
+00006f90: 008f 9428 6ae8 0200 0090 758c 0d67 6c6f  ...(j.....u..glo
+00006fa0: 625f 746f 6374 7265 6573 948f 948c 116e  b_toctrees.....n
+00006fb0: 756d 6265 7265 645f 746f 6374 7265 6573  umbered_toctrees
+00006fc0: 948f 948c 0a64 6f6d 6169 6e64 6174 6194  .....domaindata.
+00006fd0: 7d94 288c 0163 947d 9428 8c0b 726f 6f74  }.(..c.}.(..root
+00006fe0: 5f73 796d 626f 6c94 6af1 0200 008c 0653  _symbol.j......S
+00006ff0: 796d 626f 6c94 9394 2981 947d 9428 6a55  ymbol...)..}.(jU
+00007000: 0300 004e 8c0c 7369 626c 696e 6741 626f  ...N..siblingAbo
+00007010: 7665 944e 8c0c 7369 626c 696e 6742 656c  ve.N..siblingBel
+00007020: 6f77 944e 8c05 6964 656e 7494 4e8c 0b64  ow.N..ident.N..d
+00007030: 6563 6c61 7261 7469 6f6e 944e 8c07 646f  eclaration.N..do
+00007040: 636e 616d 6594 4e6a 0406 0000 4e8c 0f69  cname.Nj....N..i
+00007050: 7352 6564 6563 6c61 7261 7469 6f6e 9489  sRedeclaration..
+00007060: 8c09 5f63 6869 6c64 7265 6e94 5d94 8c0d  .._children.]...
+00007070: 5f61 6e6f 6e43 6869 6c64 7265 6e94 5d94  _anonChildren.].
+00007080: 7562 8c07 6f62 6a65 6374 7394 7d94 6aef  ub..objects.}.j.
+00007090: 0200 004b 0075 8c09 6368 616e 6765 7365  ...K.u..changese
+000070a0: 7494 7d94 288c 0763 6861 6e67 6573 947d  t.}.(..changes.}
+000070b0: 946a ef02 0000 4b00 758c 0863 6974 6174  .j....K.u..citat
+000070c0: 696f 6e94 7d94 286a ef02 0000 4b00 8c09  ion.}.(j....K...
+000070d0: 6369 7461 7469 6f6e 7394 7d94 8c0d 6369  citations.}...ci
+000070e0: 7461 7469 6f6e 5f72 6566 7394 7d94 758c  tation_refs.}.u.
+000070f0: 0363 7070 947d 9428 6a48 0800 006a f402  .cpp.}.(jH...j..
+00007100: 0000 6a49 0800 0093 9429 8194 7d94 286a  ..jI.....)..}.(j
+00007110: 5503 0000 4e6a 4d08 0000 4e6a 4e08 0000  U...NjM...NjN...
+00007120: 4e8c 0969 6465 6e74 4f72 4f70 944e 8c0e  N..identOrOp.N..
+00007130: 7465 6d70 6c61 7465 5061 7261 6d73 944e  templateParams.N
+00007140: 8c0c 7465 6d70 6c61 7465 4172 6773 944e  ..templateArgs.N
+00007150: 6a50 0800 004e 6a51 0800 004e 6a04 0600  jP...NjQ...Nj...
+00007160: 004e 6a52 0800 0089 6a53 0800 005d 946a  .NjR....jS...].j
+00007170: 5508 0000 5d94 7562 8c05 6e61 6d65 7394  U...].ub..names.
+00007180: 7d94 6aef 0200 004b 0075 8c05 696e 6465  }.j....K.u..inde
+00007190: 7894 7d94 286a ef02 0000 4b00 8c07 656e  x.}.(j....K...en
+000071a0: 7472 6965 7394 7d94 286a 1c03 0000 5d94  tries.}.(j....].
+000071b0: 6ae9 0200 005d 9428 288c 0673 696e 676c  j....].((..singl
+000071c0: 6594 8c1c 4661 7374 4d42 4152 2028 636c  e...FastMBAR (cl
+000071d0: 6173 7320 696e 2046 6173 744d 4241 5229  ass in FastMBAR)
+000071e0: 948c 1146 6173 744d 4241 522e 4661 7374  ...FastMBAR.Fast
+000071f0: 4d42 4152 9468 6c4e 7494 286a 7508 0000  MBAR.hlNt.(ju...
+00007200: 8c25 5f5f 696e 6974 5f5f 2829 2028 4661  .%__init__() (Fa
+00007210: 7374 4d42 4152 2e46 6173 744d 4241 5220  stMBAR.FastMBAR 
+00007220: 6d65 7468 6f64 2994 8c1a 4661 7374 4d42  method)...FastMB
+00007230: 4152 2e46 6173 744d 4241 522e 5f5f 696e  AR.FastMBAR.__in
+00007240: 6974 5f5f 9468 6c4e 7494 286a 7508 0000  it__.hlNt.(ju...
+00007250: 8c1e 4620 2846 6173 744d 4241 522e 4661  ..F (FastMBAR.Fa
+00007260: 7374 4d42 4152 2070 726f 7065 7274 7929  stMBAR property)
+00007270: 948c 1346 6173 744d 4241 522e 4661 7374  ...FastMBAR.Fast
+00007280: 4d42 4152 2e46 9468 6c4e 7494 286a 7508  MBAR.F.hlNt.(ju.
+00007290: 0000 8c22 465f 7374 6420 2846 6173 744d  ..."F_std (FastM
+000072a0: 4241 522e 4661 7374 4d42 4152 2070 726f  BAR.FastMBAR pro
+000072b0: 7065 7274 7929 948c 1746 6173 744d 4241  perty)...FastMBA
+000072c0: 522e 4661 7374 4d42 4152 2e46 5f73 7464  R.FastMBAR.F_std
+000072d0: 9468 6c4e 7494 286a 7508 0000 8c22 465f  .hlNt.(ju...."F_
+000072e0: 636f 7620 2846 6173 744d 4241 522e 4661  cov (FastMBAR.Fa
+000072f0: 7374 4d42 4152 2070 726f 7065 7274 7929  stMBAR property)
+00007300: 948c 1746 6173 744d 4241 522e 4661 7374  ...FastMBAR.Fast
+00007310: 4d42 4152 2e46 5f63 6f76 9468 6c4e 7494  MBAR.F_cov.hlNt.
+00007320: 286a 7508 0000 8c23 4465 6c74 6146 2028  (ju....#DeltaF (
+00007330: 4661 7374 4d42 4152 2e46 6173 744d 4241  FastMBAR.FastMBA
+00007340: 5220 7072 6f70 6572 7479 2994 8c18 4661  R property)...Fa
+00007350: 7374 4d42 4152 2e46 6173 744d 4241 522e  stMBAR.FastMBAR.
+00007360: 4465 6c74 6146 9468 6c4e 7494 286a 7508  DeltaF.hlNt.(ju.
+00007370: 0000 8c27 4465 6c74 6146 5f73 7464 2028  ...'DeltaF_std (
+00007380: 4661 7374 4d42 4152 2e46 6173 744d 4241  FastMBAR.FastMBA
+00007390: 5220 7072 6f70 6572 7479 2994 8c1c 4661  R property)...Fa
+000073a0: 7374 4d42 4152 2e46 6173 744d 4241 522e  stMBAR.FastMBAR.
+000073b0: 4465 6c74 6146 5f73 7464 9468 6c4e 7494  DeltaF_std.hlNt.
+000073c0: 286a 7508 0000 8c29 6c6f 675f 7072 6f62  (ju....)log_prob
+000073d0: 5f6d 6978 2028 4661 7374 4d42 4152 2e46  _mix (FastMBAR.F
+000073e0: 6173 744d 4241 5220 7072 6f70 6572 7479  astMBAR property
+000073f0: 2994 8c1e 4661 7374 4d42 4152 2e46 6173  )...FastMBAR.Fas
+00007400: 744d 4241 522e 6c6f 675f 7072 6f62 5f6d  tMBAR.log_prob_m
+00007410: 6978 9468 6c4e 7494 286a 7508 0000 8c48  ix.hlNt.(ju....H
+00007420: 6361 6c63 756c 6174 655f 6672 6565 5f65  calculate_free_e
+00007430: 6e65 7267 6965 735f 6f66 5f70 6572 7475  nergies_of_pertu
+00007440: 7262 6564 5f73 7461 7465 7328 2920 2846  rbed_states() (F
+00007450: 6173 744d 4241 522e 4661 7374 4d42 4152  astMBAR.FastMBAR
+00007460: 206d 6574 686f 6429 948c 3d46 6173 744d   method)..=FastM
+00007470: 4241 522e 4661 7374 4d42 4152 2e63 616c  BAR.FastMBAR.cal
+00007480: 6375 6c61 7465 5f66 7265 655f 656e 6572  culate_free_ener
+00007490: 6769 6573 5f6f 665f 7065 7274 7572 6265  gies_of_perturbe
+000074a0: 645f 7374 6174 6573 9468 6c4e 7494 656a  d_states.hlNt.ej
+000074b0: ee02 0000 5d94 6ae7 0200 005d 946a e802  ....].j....].j..
+000074c0: 0000 5d94 6aec 0200 005d 946a ea02 0000  ..].j....].j....
+000074d0: 5d94 6aed 0200 005d 9475 758c 026a 7394  ].j....].uu..js.
+000074e0: 7d94 286a 5708 0000 7d94 8c07 6d6f 6475  }.(jW...}...modu
+000074f0: 6c65 7394 7d94 6aef 0200 004b 0075 8c04  les.}.j....K.u..
+00007500: 6d61 7468 947d 9428 6a57 0800 007d 948c  math.}.(jW...}..
+00007510: 0d68 6173 5f65 7175 6174 696f 6e73 947d  .has_equations.}
+00007520: 9428 6a1c 0300 0088 6ae9 0200 0088 6aee  .(j.....j.....j.
+00007530: 0200 0088 6ae7 0200 0089 6ae8 0200 0089  ....j.....j.....
+00007540: 6aec 0200 0089 6aea 0200 0089 6aed 0200  j.....j.....j...
+00007550: 0088 756a ef02 0000 4b00 758c 0270 7994  ..uj....K.u..py.
+00007560: 7d94 286a 5708 0000 7d94 288c 1146 6173  }.(jW...}.(..Fas
+00007570: 744d 4241 522e 4661 7374 4d42 4152 948c  tMBAR.FastMBAR..
+00007580: 1573 7068 696e 782e 646f 6d61 696e 732e  .sphinx.domains.
+00007590: 7079 7468 6f6e 948c 0b4f 626a 6563 7445  python...ObjectE
+000075a0: 6e74 7279 9493 9428 6ae9 0200 006a 7708  ntry...(j....jw.
+000075b0: 0000 8c05 636c 6173 7394 8974 9481 948c  ....class..t....
+000075c0: 1a46 6173 744d 4241 522e 6661 7374 6d62  .FastMBAR.fastmb
+000075d0: 6172 2e46 6173 744d 4241 5294 6aa7 0800  ar.FastMBAR.j...
+000075e0: 0028 6ae9 0200 006a 7708 0000 6aa8 0800  .(j....jw...j...
+000075f0: 0088 7494 8194 8c1a 4661 7374 4d42 4152  ..t.....FastMBAR
+00007600: 2e46 6173 744d 4241 522e 5f5f 696e 6974  .FastMBAR.__init
+00007610: 5f5f 946a a708 0000 286a e902 0000 6a7a  __.j....(j....jz
+00007620: 0800 008c 066d 6574 686f 6494 8974 9481  .....method..t..
+00007630: 948c 1346 6173 744d 4241 522e 4661 7374  ...FastMBAR.Fast
+00007640: 4d42 4152 2e46 946a a708 0000 286a e902  MBAR.F.j....(j..
+00007650: 0000 6a7d 0800 008c 0870 726f 7065 7274  ..j}.....propert
+00007660: 7994 8974 9481 948c 1746 6173 744d 4241  y..t.....FastMBA
+00007670: 522e 4661 7374 4d42 4152 2e46 5f73 7464  R.FastMBAR.F_std
+00007680: 946a a708 0000 286a e902 0000 6a80 0800  .j....(j....j...
+00007690: 008c 0870 726f 7065 7274 7994 8974 9481  ...property..t..
+000076a0: 948c 1746 6173 744d 4241 522e 4661 7374  ...FastMBAR.Fast
+000076b0: 4d42 4152 2e46 5f63 6f76 946a a708 0000  MBAR.F_cov.j....
+000076c0: 286a e902 0000 6a83 0800 008c 0870 726f  (j....j......pro
+000076d0: 7065 7274 7994 8974 9481 948c 1846 6173  perty..t.....Fas
+000076e0: 744d 4241 522e 4661 7374 4d42 4152 2e44  tMBAR.FastMBAR.D
+000076f0: 656c 7461 4694 6aa7 0800 0028 6ae9 0200  eltaF.j....(j...
+00007700: 006a 8608 0000 8c08 7072 6f70 6572 7479  .j......property
+00007710: 9489 7494 8194 8c1c 4661 7374 4d42 4152  ..t.....FastMBAR
+00007720: 2e46 6173 744d 4241 522e 4465 6c74 6146  .FastMBAR.DeltaF
+00007730: 5f73 7464 946a a708 0000 286a e902 0000  _std.j....(j....
+00007740: 6a89 0800 008c 0870 726f 7065 7274 7994  j......property.
+00007750: 8974 9481 948c 1e46 6173 744d 4241 522e  .t.....FastMBAR.
+00007760: 4661 7374 4d42 4152 2e6c 6f67 5f70 726f  FastMBAR.log_pro
+00007770: 625f 6d69 7894 6aa7 0800 0028 6ae9 0200  b_mix.j....(j...
+00007780: 006a 8c08 0000 8c08 7072 6f70 6572 7479  .j......property
+00007790: 9489 7494 8194 8c3d 4661 7374 4d42 4152  ..t....=FastMBAR
+000077a0: 2e46 6173 744d 4241 522e 6361 6c63 756c  .FastMBAR.calcul
+000077b0: 6174 655f 6672 6565 5f65 6e65 7267 6965  ate_free_energie
+000077c0: 735f 6f66 5f70 6572 7475 7262 6564 5f73  s_of_perturbed_s
+000077d0: 7461 7465 7394 6aa7 0800 0028 6ae9 0200  tates.j....(j...
+000077e0: 006a 8f08 0000 8c06 6d65 7468 6f64 9489  .j......method..
+000077f0: 7494 8194 756a 9a08 0000 7d94 6aef 0200  t...uj....}.j...
+00007800: 004b 0075 8c03 7273 7494 7d94 286a 5708  .K.u..rst.}.(jW.
+00007810: 0000 7d94 6aef 0200 004b 0075 8c03 7374  ..}.j....K.u..st
+00007820: 6494 7d94 288c 0b70 726f 676f 7074 696f  d.}.(..progoptio
+00007830: 6e73 947d 946a 5708 0000 7d94 8c06 6c61  ns.}.jW...}...la
+00007840: 6265 6c73 947d 9428 8c08 6765 6e69 6e64  bels.}.(..genind
+00007850: 6578 946a d908 0000 686c 8c0d 7370 6869  ex.j....hl..sphi
+00007860: 6e78 2e6c 6f63 616c 6594 8c11 5f54 7261  nx.locale..._Tra
+00007870: 6e73 6c61 7469 6f6e 5072 6f78 7994 9394  nslationProxy...
+00007880: 286a da08 0000 8c0f 5f6c 617a 795f 7472  (j......_lazy_tr
+00007890: 616e 736c 6174 6594 9394 8c06 7370 6869  anslate.....sphi
+000078a0: 6e78 948c 0767 656e 6572 616c 948c 0549  nx...general...I
+000078b0: 6e64 6578 9474 9481 946a de08 0000 6adf  ndex.t...j....j.
+000078c0: 0800 006a e008 0000 6ae1 0800 0087 9486  ...j....j.......
+000078d0: 9462 8794 8c08 6d6f 6469 6e64 6578 948c  .b....modindex..
+000078e0: 0b70 792d 6d6f 6469 6e64 6578 9468 6c6a  .py-modindex.hlj
+000078f0: dc08 0000 286a de08 0000 6adf 0800 006a  ....(j....j....j
+00007900: e008 0000 8c0c 4d6f 6475 6c65 2049 6e64  ......Module Ind
+00007910: 6578 9474 9481 946a de08 0000 6adf 0800  ex.t...j....j...
+00007920: 006a e008 0000 6ae9 0800 0087 9486 9462  .j....j........b
+00007930: 8794 8c06 7365 6172 6368 946a ef08 0000  ....search.j....
+00007940: 686c 6adc 0800 0028 6ade 0800 006a df08  hlj....(j....j..
+00007950: 0000 6ae0 0800 008c 0b53 6561 7263 6820  ..j......Search 
+00007960: 5061 6765 9474 9481 946a de08 0000 6adf  Page.t...j....j.
+00007970: 0800 006a e008 0000 6af0 0800 0087 9486  ...j....j.......
+00007980: 9462 8794 8c0b 7079 2d6d 6f64 696e 6465  .b....py-modinde
+00007990: 7894 8c0b 7079 2d6d 6f64 696e 6465 7894  x...py-modindex.
+000079a0: 686c 8c13 5079 7468 6f6e 204d 6f64 756c  hl..Python Modul
+000079b0: 6520 496e 6465 7894 8794 8c08 6578 616d  e Index.....exam
+000079c0: 706c 6573 946a e702 0000 8c08 6578 616d  ples.j......exam
+000079d0: 706c 6573 948c 0845 7861 6d70 6c65 7394  ples...Examples.
+000079e0: 8794 758c 0a61 6e6f 6e6c 6162 656c 7394  ..u..anonlabels.
+000079f0: 7d94 286a d908 0000 6ad9 0800 0068 6c86  }.(j....j....hl.
+00007a00: 946a e708 0000 6ae8 0800 0068 6c86 946a  .j....j....hl..j
+00007a10: ef08 0000 6aef 0800 0068 6c86 946a f608  ....j....hl..j..
+00007a20: 0000 6af7 0800 0068 6c86 946a fa08 0000  ..j....hl..j....
+00007a30: 6ae7 0200 006a fb08 0000 8694 756a ef02  j....j......uj..
+00007a40: 0000 4b00 8c05 7465 726d 7394 7d94 7575  ..K...terms.}.uu
+00007a50: 8c06 696d 6167 6573 948c 0b73 7068 696e  ..images...sphin
+00007a60: 782e 7574 696c 948c 1046 696c 656e 616d  x.util...Filenam
+00007a70: 6555 6e69 7144 6963 7494 9394 2981 9428  eUniqDict...)..(
+00007a80: 6a27 0300 008f 9428 6a1c 0300 0090 8c0a  j'.....(j.......
+00007a90: 4669 675f 3131 2e70 6e67 9486 946a 2803  Fig_11.png...j(.
+00007aa0: 0000 8f94 286a 1c03 0000 908c 0a46 6967  ....(j.......Fig
+00007ab0: 5f32 312e 706e 6794 8694 6a26 0300 008f  _21.png...j&....
+00007ac0: 9428 6a1c 0300 0090 8c08 504d 4631 2e70  .(j.......PMF1.p
+00007ad0: 6e67 9486 946a 2c03 0000 8f94 286a ee02  ng...j,.....(j..
+00007ae0: 0000 908c 0946 6967 5f31 2e70 6e67 9486  .....Fig_1.png..
+00007af0: 946a 2f03 0000 8f94 286a ee02 0000 908c  .j/.....(j......
+00007b00: 0946 6967 5f32 2e70 6e67 9486 946a 2d03  .Fig_2.png...j-.
+00007b10: 0000 8f94 286a ee02 0000 908c 0750 4d46  ....(j.......PMF
+00007b20: 2e70 6e67 9486 946a 3903 0000 8f94 286a  .png...j9.....(j
+00007b30: ed02 0000 908c 1165 6e65 7267 795f 6d61  .......energy_ma
+00007b40: 7472 6978 2e70 6e67 9486 9475 8f94 286a  trix.png...u..(j
+00007b50: 1009 0000 6a1c 0900 006a 1609 0000 6a19  ....j....j....j.
+00007b60: 0900 006a 1309 0000 6a1f 0900 006a 0d09  ...j....j....j..
+00007b70: 0000 9062 8c07 646c 6669 6c65 7394 6a08  ...b..dlfiles.j.
+00007b80: 0900 008c 0d44 6f77 6e6c 6f61 6446 696c  .....DownloadFil
+00007b90: 6573 9493 9429 8194 8c12 6f72 6967 696e  es...)....origin
+00007ba0: 616c 5f69 6d61 6765 5f75 7269 947d 948c  al_image_uri.}..
+00007bb0: 0974 656d 705f 6461 7461 947d 948c 0b72  .temp_data.}...r
+00007bc0: 6566 5f63 6f6e 7465 7874 947d 948c 115f  ef_context.}..._
+00007bd0: 7669 6577 636f 6465 5f6d 6f64 756c 6573  viewcode_modules
+00007be0: 947d 948c 1146 6173 744d 4241 522e 6661  .}...FastMBAR.fa
+00007bf0: 7374 6d62 6172 9428 58c6 7100 0066 726f  stmbar.(X.q..fro
+00007c00: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+00007c10: 556e 696f 6e0a 696d 706f 7274 2074 6f72  Union.import tor
+00007c20: 6368 0a69 6d70 6f72 7420 6e75 6d70 7920  ch.import numpy 
+00007c30: 6173 206e 700a 696d 706f 7274 2073 6369  as np.import sci
+00007c40: 7079 2e6f 7074 696d 697a 6520 6173 206f  py.optimize as o
+00007c50: 7074 696d 697a 650a 696d 706f 7274 206d  ptimize.import m
+00007c60: 6174 680a 0a0a 636c 6173 7320 4661 7374  ath...class Fast
+00007c70: 4d42 4152 3a0a 2020 2020 2222 220a 2020  MBAR:.    """.  
+00007c80: 2020 5468 6520 4661 7374 4d42 4152 2063    The FastMBAR c
+00007c90: 6c61 7373 2069 7320 696e 6974 6961 6c69  lass is initiali
+00007ca0: 7a65 6420 7769 7468 2061 6e20 656e 6572  zed with an ener
+00007cb0: 6779 206d 6174 7269 7820 616e 6420 616e  gy matrix and an
+00007cc0: 2061 7272 6179 0a20 2020 206f 6620 6e75   array.    of nu
+00007cd0: 6d20 6f66 2063 6f6e 666f 726d 6174 696f  m of conformatio
+00007ce0: 6e73 2e20 5468 6520 636f 7272 6573 706f  ns. The correspo
+00007cf0: 6e64 696e 6720 4d42 4152 2065 7175 6174  nding MBAR equat
+00007d00: 696f 6e20 6973 2073 6f6c 7665 640a 2020  ion is solved.  
+00007d10: 2020 696e 2074 6865 2063 6f6e 7374 7275    in the constru
+00007d20: 6374 6f72 2e20 5468 6572 6566 6f72 652c  ctor. Therefore,
+00007d30: 2074 6865 2072 656c 6174 6976 6520 6672   the relative fr
+00007d40: 6565 2065 6e65 7267 6965 7320 6f66 2073  ee energies of s
+00007d50: 7461 7465 730a 2020 2020 7573 6564 2069  tates.    used i
+00007d60: 6e20 7468 6520 656e 6572 6779 206d 6174  n the energy mat
+00007d70: 7269 7820 6973 2063 616c 6375 6c61 7465  rix is calculate
+00007d80: 6420 696e 2074 6865 2063 6f6e 7374 7275  d in the constru
+00007d90: 6374 6f72 2e20 5468 650a 2020 2020 6d65  ctor. The.    me
+00007da0: 7468 6f64 202a 2a63 616c 6375 6c61 7465  thod **calculate
+00007db0: 5f66 7265 655f 656e 6572 6769 6573 5f66  _free_energies_f
+00007dc0: 6f72 5f70 6572 7475 7262 6564 5f73 7461  or_perturbed_sta
+00007dd0: 7465 732a 2a0a 2020 2020 6361 6e20 6265  tes**.    can be
+00007de0: 2075 7365 6420 746f 2063 616c 6375 6c61   used to calcula
+00007df0: 7465 6420 7468 6520 7265 6c61 7469 7665  ted the relative
+00007e00: 2066 7265 6520 656e 6572 6769 6573 206f   free energies o
+00007e10: 6620 7065 7274 7572 6265 6420 7374 6174  f perturbed stat
+00007e20: 6573 2e0a 2020 2020 2222 220a 0a20 2020  es..    """..   
+00007e30: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00007e40: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00007e50: 2020 2020 2065 6e65 7267 793a 2055 6e69       energy: Uni
+00007e60: 6f6e 5b6e 702e 6e64 6172 7261 792c 2074  on[np.ndarray, t
+00007e70: 6f72 6368 2e54 656e 736f 725d 2c0a 2020  orch.Tensor],.  
+00007e80: 2020 2020 2020 6e75 6d5f 636f 6e66 3a20        num_conf: 
+00007e90: 556e 696f 6e5b 6e70 2e6e 6461 7272 6179  Union[np.ndarray
+00007ea0: 2c20 746f 7263 682e 5465 6e73 6f72 5d2c  , torch.Tensor],
+00007eb0: 0a20 2020 2020 2020 2063 7564 613a 2062  .        cuda: b
+00007ec0: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+00007ed0: 2020 2020 2063 7564 615f 6261 7463 685f       cuda_batch_
+00007ee0: 6d6f 6465 3a20 556e 696f 6e5b 626f 6f6c  mode: Union[bool
+00007ef0: 2c20 4e6f 6e65 5d20 3d20 4e6f 6e65 2c0a  , None] = None,.
+00007f00: 2020 2020 2020 2020 626f 6f74 7374 7261          bootstra
+00007f10: 703a 2062 6f6f 6c20 3d20 4661 6c73 652c  p: bool = False,
+00007f20: 0a20 2020 2020 2020 2062 6f6f 7473 7472  .        bootstr
+00007f30: 6170 5f62 6c6f 636b 5f73 697a 653a 2069  ap_block_size: i
+00007f40: 6e74 203d 2033 2c0a 2020 2020 2020 2020  nt = 3,.        
+00007f50: 626f 6f74 7374 7261 705f 6e75 6d5f 7265  bootstrap_num_re
+00007f60: 703a 2069 6e74 203d 2031 3030 2c0a 2020  p: int = 100,.  
+00007f70: 2020 2020 2020 7665 7262 6f73 653a 2062        verbose: b
+00007f80: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+00007f90: 2020 2020 206d 6574 686f 643a 2073 7472       method: str
+00007fa0: 203d 2022 4e65 7774 6f6e 222c 0a20 2020   = "Newton",.   
+00007fb0: 2029 202d 3e20 4e6f 6e65 3a0a 2020 2020   ) -> None:.    
+00007fc0: 2020 2020 2222 2249 6e69 7469 616c 697a      """Initializ
+00007fd0: 6572 2066 6f72 2074 6865 2063 6c61 7373  er for the class
+00007fe0: 2046 6173 744d 4241 520a 0a20 2020 2020   FastMBAR..     
+00007ff0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00008000: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00008010: 0a20 2020 2020 2020 2065 6e65 7267 7920  .        energy 
+00008020: 3a20 3244 206e 6461 7272 6179 206f 7220  : 2D ndarray or 
+00008030: 3244 2074 656e 736f 720a 2020 2020 2020  2D tensor.      
+00008040: 2020 2020 2020 4974 2068 6173 2061 2073        It has a s
+00008050: 697a 6520 6f66 2028 4d20 7820 4e29 2c20  ize of (M x N), 
+00008060: 7768 6572 6520 4d20 6973 2074 6865 206e  where M is the n
+00008070: 756d 6265 7220 6f66 2073 7461 7465 730a  umber of states.
+00008080: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00008090: 4e20 6973 2074 6865 2074 6f74 616c 206e  N is the total n
+000080a0: 756d 6265 7220 6f66 2063 6f6e 666f 726d  umber of conform
+000080b0: 6174 696f 6e73 2e20 5468 6520 656e 7472  ations. The entr
+000080c0: 7920 656e 6572 6779 5b69 2c6a 5d0a 2020  y energy[i,j].  
+000080d0: 2020 2020 2020 2020 2020 6973 2074 6865            is the
+000080e0: 2072 6564 7563 6564 2028 756e 6974 6c65   reduced (unitle
+000080f0: 7373 2920 656e 6572 6779 206f 6620 636f  ss) energy of co
+00008100: 6e66 6f72 6d61 7469 6f6e 206a 2069 6e20  nformation j in 
+00008110: 7374 6174 6520 692e 0a20 2020 2020 2020  state i..       
+00008120: 2020 2020 2049 6620 626f 6f74 7374 7261       If bootstra
+00008130: 7070 696e 6720 6973 2075 7365 6420 746f  pping is used to
+00008140: 2063 616c 6375 6c61 7465 2074 6865 2075   calculate the u
+00008150: 6e63 6572 7461 696e 7479 2c20 7468 6520  ncertainty, the 
+00008160: 6f72 6465 720a 2020 2020 2020 2020 2020  order.          
+00008170: 2020 6f66 2063 6f6e 666f 726d 6174 696f    of conformatio
+00008180: 6e73 206d 6174 7465 7273 2e20 436f 6e66  ns matters. Conf
+00008190: 6f72 6d61 7469 6f6e 7320 7361 6d70 6c65  ormations sample
+000081a0: 6420 6672 6f6d 206f 6e65 2073 7461 7465  d from one state
+000081b0: 0a20 2020 2020 2020 2020 2020 206e 6565  .            nee
+000081c0: 6420 746f 206f 6363 7079 2061 2063 6f6e  d to occpy a con
+000081d0: 7469 6e75 6f75 7320 6368 756e 6b20 6f66  tinuous chunk of
+000081e0: 2063 6f6c 6c75 6d6e 732e 2043 6f6e 666f   collumns. Confo
+000081f0: 726d 6174 696f 6e73 2073 616d 706c 6564  rmations sampled
+00008200: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
+00008210: 6d20 7374 6174 6520 6b20 6e65 6564 2074  m state k need t
+00008220: 6f20 6f63 6375 7079 2063 6f6c 6c75 6d6e  o occupy collumn
+00008230: 7320 746f 2074 6865 206c 6566 7420 6f66  s to the left of
+00008240: 2063 6f6e 666f 726d 6174 696f 6e73 0a20   conformations. 
+00008250: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
+00008260: 6564 2066 726f 6d20 7374 6174 6520 6c20  ed from state l 
+00008270: 6966 206b 203c 206c 2e20 4966 2062 6f6f  if k < l. If boo
+00008280: 7473 7472 6170 7069 6e67 2069 7320 6e6f  tstrapping is no
+00008290: 7420 7573 6564 2c20 7468 656e 0a20 2020  t used, then.   
+000082a0: 2020 2020 2020 2020 2074 6865 206f 7264           the ord
+000082b0: 6572 206f 6620 636f 6e66 6f72 6d61 7469  er of conformati
+000082c0: 6f6e 2064 6f65 7320 6e6f 7420 6d61 7474  on does not matt
+000082d0: 6572 2e0a 2020 2020 2020 2020 6e75 6d5f  er..        num_
+000082e0: 636f 6e66 3a20 3144 2069 6e74 206e 6461  conf: 1D int nda
+000082f0: 7272 6179 206f 7220 3144 2074 656e 736f  rray or 1D tenso
+00008300: 720a 2020 2020 2020 2020 2020 2020 4974  r.            It
+00008310: 2073 686f 756c 6420 6861 7665 2061 2073   should have a s
+00008320: 697a 6520 6f66 204d 2c20 7768 6572 6520  ize of M, where 
+00008330: 6e75 6d5f 636f 6e66 5b69 5d20 6973 2074  num_conf[i] is t
+00008340: 6865 206e 756d 206f 660a 2020 2020 2020  he num of.      
+00008350: 2020 2020 2020 636f 6e66 6f72 6d61 7469        conformati
+00008360: 6f6e 7320 7361 6d70 6c65 6420 6672 6f6d  ons sampled from
+00008370: 2073 7461 7465 2069 2e20 5468 6572 6566   state i. Theref
+00008380: 6f72 652c 206e 702e 7375 6d28 6e75 6d5f  ore, np.sum(num_
+00008390: 636f 6e66 290a 2020 2020 2020 2020 2020  conf).          
+000083a0: 2020 6861 7320 746f 2062 6520 6571 7561    has to be equa
+000083b0: 6c20 746f 204e 2e20 416c 6c20 656e 7472  l to N. All entr
+000083c0: 6965 7320 696e 206e 756d 5f63 6f6e 6620  ies in num_conf 
+000083d0: 6861 7665 2074 6f20 6265 2073 7472 6963  have to be stric
+000083e0: 746c 790a 2020 2020 2020 2020 2020 2020  tly.            
+000083f0: 6772 6561 7465 7220 7468 616e 2030 2e0a  greater than 0..
+00008400: 2020 2020 2020 2020 6375 6461 3a20 626f          cuda: bo
+00008410: 6f6c 2c20 6f70 7469 6f6e 616c 2028 6465  ol, optional (de
+00008420: 6661 756c 743d 4661 6c73 6529 0a20 2020  fault=False).   
+00008430: 2020 2020 2020 2020 2049 6620 6974 2069           If it i
+00008440: 7320 7365 7420 746f 2062 6520 5472 7565  s set to be True
+00008450: 2c20 7468 656e 2074 6865 2063 616c 6375  , then the calcu
+00008460: 6c61 7469 6f6e 2077 696c 6c20 6265 2072  lation will be r
+00008470: 756e 206f 6e0a 2020 2020 2020 2020 2020  un on.          
+00008480: 2020 6120 6772 6170 6869 6361 6c20 7072    a graphical pr
+00008490: 6f63 6573 7369 6e67 2075 6e69 7420 2847  ocessing unit (G
+000084a0: 5055 2920 7573 696e 6720 4355 4441 2e0a  PU) using CUDA..
+000084b0: 2020 2020 2020 2020 6375 6461 5f62 6174          cuda_bat
+000084c0: 6368 5f6d 6f64 653a 2062 6f6f 6c2c 206f  ch_mode: bool, o
+000084d0: 7074 696f 6e61 6c20 2864 6566 6175 6c74  ptional (default
+000084e0: 3d4e 6f6e 6529 0a20 2020 2020 2020 2020  =None).         
+000084f0: 2020 2054 6865 2062 6174 6368 206d 6f64     The batch mod
+00008500: 6520 6973 2074 7572 6e65 6420 6f6e 2077  e is turned on w
+00008510: 6865 6e20 7468 6520 7369 7a65 206f 6620  hen the size of 
+00008520: 7468 6520 656e 6572 6779 206d 6174 7269  the energy matri
+00008530: 7820 6973 0a20 2020 2020 2020 2020 2020  x is.           
+00008540: 2074 6f6f 206c 6172 6765 2066 6f72 2074   too large for t
+00008550: 6865 206d 656d 6f72 7920 6f66 2061 2047  he memory of a G
+00008560: 5055 2e20 5768 656e 2063 7564 615f 6261  PU. When cuda_ba
+00008570: 7463 685f 6d6f 6465 2069 7320 5472 7565  tch_mode is True
+00008580: 2c0a 2020 2020 2020 2020 2020 2020 7468  ,.            th
+00008590: 6520 656e 6572 6779 206d 6174 7269 7820  e energy matrix 
+000085a0: 7769 6c6c 2062 6520 7370 6c69 7420 696e  will be split in
+000085b0: 746f 206d 756c 7469 706c 6520 6261 7463  to multiple batc
+000085c0: 6865 7320 7768 6963 6820 6172 6520 7573  hes which are us
+000085d0: 6564 0a20 2020 2020 2020 2020 2020 2073  ed.            s
+000085e0: 6571 7565 6e74 6961 6c6c 792e 2049 6620  equentially. If 
+000085f0: 6375 6461 5f62 6174 6368 5f6d 6f64 6520  cuda_batch_mode 
+00008600: 3d20 4e6f 6e65 2c20 6974 2077 696c 6c20  = None, it will 
+00008610: 6265 2073 6574 2061 7574 6f6d 6174 6963  be set automatic
+00008620: 616c 6c79 0a20 2020 2020 2020 2020 2020  ally.           
+00008630: 2062 6173 6564 206f 6e20 7468 6520 7369   based on the si
+00008640: 7a65 206f 6620 656e 6572 6779 2061 6e64  ze of energy and
+00008650: 2074 6865 206d 656d 6f72 7920 6f66 2074   the memory of t
+00008660: 6865 2061 7661 6962 6c65 2047 5055 2064  he avaible GPU d
+00008670: 6576 6963 652e 0a20 2020 2020 2020 2062  evice..        b
+00008680: 6f6f 7473 7472 6170 3a20 626f 6f6c 2c20  ootstrap: bool, 
+00008690: 6f70 7469 6f6e 616c 2028 6465 6661 756c  optional (defaul
+000086a0: 743d 4661 6c73 6529 0a20 2020 2020 2020  t=False).       
+000086b0: 2020 2020 2049 6620 626f 6f74 7374 7261       If bootstra
+000086c0: 7020 6973 2054 7275 652c 2074 6865 2075  p is True, the u
+000086d0: 6e63 6572 7461 696e 7479 206f 6620 7468  ncertainty of th
+000086e0: 6520 6361 6c63 756c 6174 6564 2066 7265  e calculated fre
+000086f0: 6520 656e 6572 6769 6573 0a20 2020 2020  e energies.     
+00008700: 2020 2020 2020 2077 696c 6c20 6265 2065         will be e
+00008710: 7374 696d 6174 6520 7573 696e 6720 626c  stimate using bl
+00008720: 6f63 6b20 626f 6f74 7374 7261 7069 6e67  ock bootstraping
+00008730: 2e0a 2020 2020 2020 2020 626f 6f74 7374  ..        bootst
+00008740: 7261 705f 626c 6f63 6b5f 7369 7a65 3a20  rap_block_size: 
+00008750: 696e 742c 206f 7074 696f 6e61 6c20 2864  int, optional (d
+00008760: 6566 6175 6c74 3d33 290a 2020 2020 2020  efault=3).      
+00008770: 2020 2020 2020 626c 6f63 6b20 7369 7a65        block size
+00008780: 2075 7365 6420 696e 2062 6c6f 636b 2062   used in block b
+00008790: 6f6f 7473 7472 6170 7069 6e67 0a20 2020  ootstrapping.   
+000087a0: 2020 2020 2062 6f6f 7473 7472 6170 5f6e       bootstrap_n
+000087b0: 756d 5f72 6570 3a20 696e 742c 206f 7074  um_rep: int, opt
+000087c0: 696f 6e61 6c20 2864 6566 6175 6c74 3d31  ional (default=1
+000087d0: 3030 290a 2020 2020 2020 2020 2020 2020  00).            
+000087e0: 6e75 6d62 6572 206f 6620 7265 7072 6561  number of reprea
+000087f0: 7473 2069 6e20 626c 6f63 6b20 626f 6f74  ts in block boot
+00008800: 7374 7261 7070 696e 670a 2020 2020 2020  strapping.      
+00008810: 2020 7665 7262 6f73 653a 2062 6f6f 6c2c    verbose: bool,
+00008820: 206f 7074 696f 6e61 6c20 2864 6566 6175   optional (defau
+00008830: 6c74 3d46 616c 7365 290a 2020 2020 2020  lt=False).      
+00008840: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
+00008850: 2069 7320 7472 7565 2c20 7468 6520 6465   is true, the de
+00008860: 7461 696c 6564 2069 6e66 6f72 6d61 7469  tailed informati
+00008870: 6f6e 206f 6620 736f 6c76 696e 6720 4d42  on of solving MB
+00008880: 4152 2065 7175 6174 696f 6e73 0a20 2020  AR equations.   
+00008890: 2020 2020 2020 2020 2069 7320 7072 696e           is prin
+000088a0: 7465 642e 0a20 2020 2020 2020 206d 6574  ted..        met
+000088b0: 686f 643a 2073 7472 2c20 6f70 7469 6f6e  hod: str, option
+000088c0: 616c 2028 6465 6661 756c 743d 224e 6577  al (default="New
+000088d0: 746f 6e22 290a 2020 2020 2020 2020 2020  ton").          
+000088e0: 2020 7468 6520 6d65 7468 6f64 2075 7365    the method use
+000088f0: 6420 746f 2073 6f6c 7665 2074 6865 204d  d to solve the M
+00008900: 4241 5220 6571 7561 7469 6f6e 2e20 5468  BAR equation. Th
+00008910: 6520 6465 6661 756c 7420 6973 204e 6577  e default is New
+00008920: 746f 6e27 7320 6d65 7468 6f64 2e0a 2020  ton's method..  
+00008930: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00008940: 2020 2023 2323 2320 6368 6563 6b20 7468     #### check th
+00008950: 6520 7061 7261 6d65 7465 7273 3a20 656e  e parameters: en
+00008960: 6572 6779 2061 6e64 206e 756d 5f63 6f6e  ergy and num_con
+00008970: 660a 2020 2020 2020 2020 2323 204e 6f74  f.        ## Not
+00008980: 6520 7468 6174 2062 6f74 6820 7365 6c66  e that both self
+00008990: 2e65 6e65 7267 7920 616e 6420 7365 6c66  .energy and self
+000089a0: 2e63 6f6e 6620 7769 6c6c 2062 6520 6f6e  .conf will be on
+000089b0: 2043 5055 7320 6e6f 206d 6174 7465 720a   CPUs no matter.
+000089c0: 2020 2020 2020 2020 2323 2069 6620 6375          ## if cu
+000089d0: 6461 2069 7320 5472 7565 206f 7220 4661  da is True or Fa
+000089e0: 6c73 652e 0a0a 2020 2020 2020 2020 2323  lse...        ##
+000089f0: 2065 6e65 7267 7920 6e65 6564 7320 746f   energy needs to
+00008a00: 2062 6520 6120 322d 4420 6e64 6172 7261   be a 2-D ndarra
+00008a10: 7920 6f72 2061 2032 2d44 2074 656e 736f  y or a 2-D tenso
+00008a20: 722e 0a20 2020 2020 2020 2023 2320 636f  r..        ## co
+00008a30: 6e76 6572 7420 6974 2069 6e74 6f20 646f  nvert it into do
+00008a40: 7562 6c65 2070 7265 6369 7369 6f6e 2069  uble precision i
+00008a50: 6620 6e6f 740a 2020 2020 2020 2020 6966  f not.        if
+00008a60: 2069 7369 6e73 7461 6e63 6528 656e 6572   isinstance(ener
+00008a70: 6779 2c20 6e70 2e6e 6461 7272 6179 293a  gy, np.ndarray):
+00008a80: 0a20 2020 2020 2020 2020 2020 2065 6e65  .            ene
+00008a90: 7267 7920 3d20 656e 6572 6779 2e61 7374  rgy = energy.ast
+00008aa0: 7970 6528 6e70 2e66 6c6f 6174 3634 290a  ype(np.float64).
+00008ab0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008ac0: 2e65 6e65 7267 7920 3d20 746f 7263 682e  .energy = torch.
+00008ad0: 6672 6f6d 5f6e 756d 7079 2865 6e65 7267  from_numpy(energ
+00008ae0: 7929 0a20 2020 2020 2020 2065 6c69 6620  y).        elif 
+00008af0: 6973 696e 7374 616e 6365 2865 6e65 7267  isinstance(energ
+00008b00: 792c 2074 6f72 6368 2e54 656e 736f 7229  y, torch.Tensor)
+00008b10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00008b20: 6c66 2e65 6e65 7267 7920 3d20 656e 6572  lf.energy = ener
+00008b30: 6779 2e64 6f75 626c 6528 290a 2020 2020  gy.double().    
+00008b40: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008b50: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
+00008b60: 4572 726f 7228 2265 6e65 7267 7920 6861  Error("energy ha
+00008b70: 7320 746f 2062 6520 6120 322d 4420 6e64  s to be a 2-D nd
+00008b80: 6172 7261 7920 6f72 2061 2032 2d44 2074  array or a 2-D t
+00008b90: 656e 736f 722e 2229 0a0a 2020 2020 2020  ensor.")..      
+00008ba0: 2020 2323 206e 756d 5f63 6f6e 6620 6e65    ## num_conf ne
+00008bb0: 6564 7320 746f 2062 6520 6120 312d 4420  eds to be a 1-D 
+00008bc0: 6e64 6172 7261 7920 6f72 2061 2031 2d44  ndarray or a 1-D
+00008bd0: 2074 656e 736f 722e 0a20 2020 2020 2020   tensor..       
+00008be0: 2069 6620 6973 696e 7374 616e 6365 286e   if isinstance(n
+00008bf0: 756d 5f63 6f6e 662c 206e 702e 6e64 6172  um_conf, np.ndar
+00008c00: 7261 7929 3a0a 2020 2020 2020 2020 2020  ray):.          
+00008c10: 2020 6e75 6d5f 636f 6e66 203d 206e 756d    num_conf = num
+00008c20: 5f63 6f6e 662e 6173 7479 7065 286e 702e  _conf.astype(np.
+00008c30: 666c 6f61 7436 3429 0a20 2020 2020 2020  float64).       
+00008c40: 2020 2020 2073 656c 662e 6e75 6d5f 636f       self.num_co
+00008c50: 6e66 203d 2074 6f72 6368 2e66 726f 6d5f  nf = torch.from_
+00008c60: 6e75 6d70 7928 6e75 6d5f 636f 6e66 290a  numpy(num_conf).
+00008c70: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+00008c80: 6e73 7461 6e63 6528 6e75 6d5f 636f 6e66  nstance(num_conf
+00008c90: 2c20 746f 7263 682e 5465 6e73 6f72 293a  , torch.Tensor):
+00008ca0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00008cb0: 662e 6e75 6d5f 636f 6e66 203d 206e 756d  f.num_conf = num
+00008cc0: 5f63 6f6e 662e 646f 7562 6c65 2829 0a20  _conf.double(). 
+00008cd0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00008ce0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+00008cf0: 7970 6545 7272 6f72 2822 6e75 6d5f 636f  ypeError("num_co
+00008d00: 6e66 2068 6173 2074 6f20 6265 2061 2031  nf has to be a 1
+00008d10: 2d44 206e 6461 7272 6179 206f 7220 6120  -D ndarray or a 
+00008d20: 312d 4420 7465 6e73 6f72 2e22 290a 0a20  1-D tensor.").. 
+00008d30: 2020 2020 2020 2023 2320 6368 6563 6b20         ## check 
+00008d40: 7468 6520 7368 6170 6520 6f66 2065 6e65  the shape of ene
+00008d50: 7267 7920 616e 6420 6e75 6d5f 636f 6e66  rgy and num_conf
+00008d60: 0a20 2020 2020 2020 2069 6620 656e 6572  .        if ener
+00008d70: 6779 2e6e 6469 6d20 213d 2032 3a0a 2020  gy.ndim != 2:.  
+00008d80: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00008d90: 5661 6c75 6545 7272 6f72 2822 656e 6572  ValueError("ener
+00008da0: 6779 2068 6173 2074 6f20 6265 2061 2032  gy has to be a 2
+00008db0: 2d44 206e 6461 7272 6179 206f 7220 6120  -D ndarray or a 
+00008dc0: 322d 4420 7465 6e73 6f72 2e22 290a 2020  2-D tensor.").  
+00008dd0: 2020 2020 2020 6966 206e 756d 5f63 6f6e        if num_con
+00008de0: 662e 6e64 696d 2021 3d20 313a 0a20 2020  f.ndim != 1:.   
+00008df0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00008e00: 616c 7565 4572 726f 7228 226e 756d 5f63  alueError("num_c
+00008e10: 6f6e 6620 6861 7320 746f 2062 6520 6120  onf has to be a 
+00008e20: 312d 4420 6e64 6172 7261 7920 6f72 2061  1-D ndarray or a
+00008e30: 2031 2d44 2074 656e 736f 722e 2229 0a20   1-D tensor."). 
+00008e40: 2020 2020 2020 2069 6620 656e 6572 6779         if energy
+00008e50: 2e73 6861 7065 5b30 5d20 213d 206e 756d  .shape[0] != num
+00008e60: 5f63 6f6e 662e 7368 6170 655b 305d 3a0a  _conf.shape[0]:.
+00008e70: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00008e80: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+00008e90: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00008ea0: 6865 206e 756d 6265 7220 6f66 2072 6f77  he number of row
+00008eb0: 7320 696e 2065 6e65 7267 7920 6861 7320  s in energy has 
+00008ec0: 746f 2062 6520 6571 7561 6c20 746f 2074  to be equal to t
+00008ed0: 6865 206c 656e 6774 6820 6f66 206e 756d  he length of num
+00008ee0: 5f63 6f6e 662e 220a 2020 2020 2020 2020  _conf.".        
+00008ef0: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
+00008f00: 2320 6368 6563 6b20 6966 2074 6865 206e  # check if the n
+00008f10: 756d 6265 7220 6f66 2063 6f6e 666f 726d  umber of conform
+00008f20: 6174 696f 6e73 2073 616d 706c 6564 2066  ations sampled f
+00008f30: 726f 6d20 6561 6368 2073 7461 7465 2069  rom each state i
+00008f40: 7320 6772 6561 7465 7220 7468 616e 2030  s greater than 0
+00008f50: 0a20 2020 2020 2020 2069 6620 746f 7263  .        if torc
+00008f60: 682e 7375 6d28 7365 6c66 2e6e 756d 5f63  h.sum(self.num_c
+00008f70: 6f6e 6620 3c3d 2030 2920 3e20 303a 0a20  onf <= 0) > 0:. 
+00008f80: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00008f90: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+00008fa0: 2020 2020 2020 2020 2020 2020 2022 616c               "al
+00008fb0: 6c20 656e 7472 6965 7320 696e 206e 756d  l entries in num
+00008fc0: 5f63 6f6e 6620 6861 7665 2074 6f20 6265  _conf have to be
+00008fd0: 2073 7472 6963 746c 7920 6772 6561 7465   strictly greate
+00008fe0: 7220 7468 616e 2030 2e22 0a20 2020 2020  r than 0.".     
+00008ff0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00009000: 2020 2323 2063 6865 636b 2069 6620 7468    ## check if th
+00009010: 6520 746f 7461 6c20 6e75 6d62 6572 206f  e total number o
+00009020: 6620 636f 6e66 6f72 6d61 7469 6f6e 7320  f conformations 
+00009030: 6973 2065 7175 616c 2074 6f20 7468 6520  is equal to the 
+00009040: 6e75 6d62 6572 206f 6620 636f 6c75 6d6e  number of column
+00009050: 7320 696e 2065 6e65 7267 790a 2020 2020  s in energy.    
+00009060: 2020 2020 6966 2074 6f72 6368 2e73 756d      if torch.sum
+00009070: 2873 656c 662e 6e75 6d5f 636f 6e66 2920  (self.num_conf) 
+00009080: 213d 2073 656c 662e 656e 6572 6779 2e73  != self.energy.s
+00009090: 6861 7065 5b31 5d3a 0a20 2020 2020 2020  hape[1]:.       
+000090a0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+000090b0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+000090c0: 2020 2020 2020 2022 7468 6520 7375 6d20         "the sum 
+000090d0: 6f66 206e 756d 5f63 6f6e 6620 6861 7320  of num_conf has 
+000090e0: 746f 2062 6520 6571 7561 6c20 746f 2074  to be equal to t
+000090f0: 6865 206e 756d 6265 7220 6f66 2063 6f6c  he number of col
+00009100: 756d 6e73 2069 6e20 656e 6572 6779 2e22  umns in energy."
+00009110: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00009120: 2020 2020 2020 2020 7365 6c66 2e4d 203d          self.M =
+00009130: 2073 656c 662e 656e 6572 6779 2e73 6861   self.energy.sha
+00009140: 7065 5b30 5d0a 2020 2020 2020 2020 7365  pe[0].        se
+00009150: 6c66 2e4e 203d 2073 656c 662e 656e 6572  lf.N = self.ener
+00009160: 6779 2e73 6861 7065 5b31 5d0a 0a20 2020  gy.shape[1]..   
+00009170: 2020 2020 2073 656c 662e 6375 6461 203d       self.cuda =
+00009180: 2063 7564 610a 2020 2020 2020 2020 6966   cuda.        if
+00009190: 2073 656c 662e 6375 6461 2069 7320 5472   self.cuda is Tr
+000091a0: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
+000091b0: 7365 6c66 2e64 6576 6963 6520 3d20 746f  self.device = to
+000091c0: 7263 682e 6465 7669 6365 2822 6375 6461  rch.device("cuda
+000091d0: 2229 0a20 2020 2020 2020 2065 6c73 653a  ").        else:
+000091e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000091f0: 662e 6465 7669 6365 203d 2074 6f72 6368  f.device = torch
+00009200: 2e64 6576 6963 6528 2263 7075 2229 0a0a  .device("cpu")..
+00009210: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00009220: 6375 6461 3a0a 2020 2020 2020 2020 2020  cuda:.          
+00009230: 2020 2323 2063 6865 636b 2069 6620 7468    ## check if th
+00009240: 6520 4750 5520 6465 7669 6365 2068 6173  e GPU device has
+00009250: 2065 6e6f 7567 6820 6d65 6d6f 7279 2e20   enough memory. 
+00009260: 4966 206e 6f74 2c20 6375 6461 5f62 6174  If not, cuda_bat
+00009270: 6368 5f6d 6f64 6520 6973 2074 7572 6e65  ch_mode is turne
+00009280: 6420 6f6e 0a0a 2020 2020 2020 2020 2020  d on..          
+00009290: 2020 2323 2061 7574 6f6d 6174 6963 616c    ## automatical
+000092a0: 6c79 2064 6574 6572 6d69 6e65 2069 6620  ly determine if 
+000092b0: 6375 6461 5f62 6174 6368 5f6d 6f64 6520  cuda_batch_mode 
+000092c0: 6973 206f 6e20 6f72 206f 6666 0a20 2020  is on or off.   
+000092d0: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
+000092e0: 6f74 616c 5f47 5055 5f6d 656d 6f72 7920  otal_GPU_memory 
+000092f0: 3d20 746f 7263 682e 6375 6461 2e67 6574  = torch.cuda.get
+00009300: 5f64 6576 6963 655f 7072 6f70 6572 7469  _device_properti
+00009310: 6573 2830 292e 746f 7461 6c5f 6d65 6d6f  es(0).total_memo
+00009320: 7279 0a20 2020 2020 2020 2020 2020 2069  ry.            i
+00009330: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00009340: 2020 2020 7365 6c66 2e65 6e65 7267 792e      self.energy.
+00009350: 6e75 6d65 6c28 2920 2a20 7365 6c66 2e65  numel() * self.e
+00009360: 6e65 7267 792e 656c 656d 656e 745f 7369  nergy.element_si
+00009370: 7a65 2829 0a20 2020 2020 2020 2020 2020  ze().           
+00009380: 2020 2020 203c 2073 656c 662e 5f74 6f74       < self._tot
+00009390: 616c 5f47 5055 5f6d 656d 6f72 7920 2f20  al_GPU_memory / 
+000093a0: 3130 0a20 2020 2020 2020 2020 2020 2029  10.            )
+000093b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000093c0: 2020 7365 6c66 2e63 7564 615f 6261 7463    self.cuda_batc
+000093d0: 685f 6d6f 6465 203d 2046 616c 7365 0a20  h_mode = False. 
+000093e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000093f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009400: 2073 656c 662e 6375 6461 5f62 6174 6368   self.cuda_batch
+00009410: 5f6d 6f64 6520 3d20 5472 7565 0a0a 2020  _mode = True..  
+00009420: 2020 2020 2020 2020 2020 2323 2063 7564            ## cud
+00009430: 615f 6261 7463 685f 6d6f 6465 2063 616e  a_batch_mode can
+00009440: 2062 6520 656e 666f 7263 6564 2062 7920   be enforced by 
+00009450: 7061 7373 696e 6720 7468 6520 6172 6775  passing the argu
+00009460: 6d65 6e74 2063 7564 615f 6261 7463 685f  ment cuda_batch_
+00009470: 6d6f 6465 0a20 2020 2020 2020 2020 2020  mode.           
+00009480: 2069 6620 6375 6461 5f62 6174 6368 5f6d   if cuda_batch_m
+00009490: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
+000094a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000094b0: 2073 656c 662e 6375 6461 5f62 6174 6368   self.cuda_batch
+000094c0: 5f6d 6f64 6520 3d20 6375 6461 5f62 6174  _mode = cuda_bat
+000094d0: 6368 5f6d 6f64 650a 0a20 2020 2020 2020  ch_mode..       
+000094e0: 2023 2320 7768 656e 2063 7564 615f 6261   ## when cuda_ba
+000094f0: 7463 685f 6d6f 6465 2069 7320 7573 6564  tch_mode is used
+00009500: 2c20 7765 206e 6565 6420 746f 2064 6563  , we need to dec
+00009510: 6964 6520 6f6e 2074 6865 2062 6174 6368  ide on the batch
+00009520: 5f73 697a 6520 6261 7365 6420 6f6e 0a20  _size based on. 
+00009530: 2020 2020 2020 2023 2320 626f 7468 2074         ## both t
+00009540: 6865 206d 656d 6f72 7920 6f66 2074 6865  he memory of the
+00009550: 2047 5055 2064 6576 6963 6520 616e 6420   GPU device and 
+00009560: 7468 6520 7369 7a65 206f 6620 656e 6572  the size of ener
+00009570: 6779 206d 6174 7269 780a 2020 2020 2020  gy matrix.      
+00009580: 2020 7365 6c66 2e5f 6261 7463 685f 7369    self._batch_si
+00009590: 7a65 203d 204e 6f6e 650a 2020 2020 2020  ze = None.      
+000095a0: 2020 6966 2073 656c 662e 6375 6461 2061    if self.cuda a
+000095b0: 6e64 2073 656c 662e 6375 6461 5f62 6174  nd self.cuda_bat
+000095c0: 6368 5f6d 6f64 653a 0a20 2020 2020 2020  ch_mode:.       
+000095d0: 2020 2020 2023 2320 6261 7463 6820 7369       ## batch si
+000095e0: 7a65 2066 6f72 2073 6570 6572 6174 696e  ze for seperatin
+000095f0: 6720 636f 6e66 6f72 6d61 7469 6f6e 730a  g conformations.
+00009600: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009610: 2e5f 6261 7463 685f 7369 7a65 203d 2069  ._batch_size = i
+00009620: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
+00009630: 2020 2020 7365 6c66 2e5f 746f 7461 6c5f      self._total_
+00009640: 4750 555f 6d65 6d6f 7279 0a20 2020 2020  GPU_memory.     
+00009650: 2020 2020 2020 2020 2020 202f 2032 300a             / 20.
+00009660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009670: 2f20 7365 6c66 2e65 6e65 7267 792e 7368  / self.energy.sh
+00009680: 6170 655b 305d 0a20 2020 2020 2020 2020  ape[0].         
+00009690: 2020 2020 2020 202f 2073 656c 662e 656e         / self.en
+000096a0: 6572 6779 2e65 6c65 6d65 6e74 5f73 697a  ergy.element_siz
+000096b0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+000096c0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000096d0: 6c66 2e5f 6261 7463 685f 7369 7a65 203d  lf._batch_size =
+000096e0: 206d 696e 2831 3032 342c 2073 656c 662e   min(1024, self.
+000096f0: 5f62 6174 6368 5f73 697a 6529 0a0a 2020  _batch_size)..  
+00009700: 2020 2020 2020 2323 2077 6865 7468 6572        ## whether
+00009710: 2074 6f20 7573 6520 626f 6f74 7374 7261   to use bootstra
+00009720: 7020 746f 2065 7374 696d 6174 6520 7468  p to estimate th
+00009730: 6520 756e 6365 7274 6169 6e74 7920 6f66  e uncertainty of
+00009740: 2074 6865 2063 616c 6375 6c61 7465 6420   the calculated 
+00009750: 6672 6565 2065 6e65 7267 6965 730a 2020  free energies.  
+00009760: 2020 2020 2020 2323 2062 6f6f 7473 7472        ## bootstr
+00009770: 6170 206e 6565 6473 2074 6f20 6265 2061  ap needs to be a
+00009780: 2062 6f6f 6c65 616e 0a20 2020 2020 2020   boolean.       
+00009790: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+000097a0: 6365 2862 6f6f 7473 7472 6170 2c20 626f  ce(bootstrap, bo
+000097b0: 6f6c 293a 0a20 2020 2020 2020 2020 2020  ol):.           
+000097c0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+000097d0: 2822 626f 6f74 7374 7261 7020 6861 7320  ("bootstrap has 
+000097e0: 746f 2062 6520 6120 626f 6f6c 6561 6e2e  to be a boolean.
+000097f0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00009800: 626f 6f74 7374 7261 7020 3d20 626f 6f74  bootstrap = boot
+00009810: 7374 7261 700a 0a20 2020 2020 2020 2023  strap..        #
+00009820: 2320 626c 6f63 6b20 7369 7a65 2075 7365  # block size use
+00009830: 6420 696e 2062 6c6f 636b 2062 6f6f 7473  d in block boots
+00009840: 7472 6170 7069 6e67 0a20 2020 2020 2020  trapping.       
+00009850: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+00009860: 6365 2862 6f6f 7473 7472 6170 5f62 6c6f  ce(bootstrap_blo
+00009870: 636b 5f73 697a 652c 2069 6e74 293a 0a20  ck_size, int):. 
+00009880: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00009890: 2054 7970 6545 7272 6f72 2822 626f 6f74   TypeError("boot
+000098a0: 7374 7261 705f 626c 6f63 6b5f 7369 7a65  strap_block_size
+000098b0: 2068 6173 2074 6f20 6265 2061 6e20 696e   has to be an in
+000098c0: 7465 6765 722e 2229 0a20 2020 2020 2020  teger.").       
+000098d0: 2073 656c 662e 626f 6f74 7374 7261 705f   self.bootstrap_
+000098e0: 626c 6f63 6b5f 7369 7a65 203d 2062 6f6f  block_size = boo
+000098f0: 7473 7472 6170 5f62 6c6f 636b 5f73 697a  tstrap_block_siz
+00009900: 650a 0a20 2020 2020 2020 2023 2320 6e75  e..        ## nu
+00009910: 6d62 6572 206f 6620 7265 7065 6174 7320  mber of repeats 
+00009920: 696e 2062 6c6f 636b 2062 6f6f 7473 7472  in block bootstr
+00009930: 6170 7069 6e67 0a20 2020 2020 2020 2069  apping.        i
+00009940: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+00009950: 2862 6f6f 7473 7472 6170 5f6e 756d 5f72  (bootstrap_num_r
+00009960: 6570 2c20 696e 7429 3a0a 2020 2020 2020  ep, int):.      
+00009970: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
+00009980: 4572 726f 7228 2262 6f6f 7473 7472 6170  Error("bootstrap
+00009990: 5f6e 756d 5f72 6570 2068 6173 2074 6f20  _num_rep has to 
+000099a0: 6265 2061 6e20 696e 7465 6765 722e 2229  be an integer.")
+000099b0: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
+000099c0: 6f74 7374 7261 705f 6e75 6d5f 7265 7020  otstrap_num_rep 
+000099d0: 3d20 626f 6f74 7374 7261 705f 6e75 6d5f  = bootstrap_num_
+000099e0: 7265 700a 0a20 2020 2020 2020 2023 2320  rep..        ## 
+000099f0: 7768 6574 6865 7220 746f 2070 7269 6e74  whether to print
+00009a00: 2074 6865 2064 6574 6169 6c65 6420 696e   the detailed in
+00009a10: 666f 726d 6174 696f 6e20 6f66 2073 6f6c  formation of sol
+00009a20: 7669 6e67 204d 4241 5220 6571 7561 7469  ving MBAR equati
+00009a30: 6f6e 730a 2020 2020 2020 2020 2323 2076  ons.        ## v
+00009a40: 6572 626f 7365 206e 6565 6473 2074 6f20  erbose needs to 
+00009a50: 6265 2061 2062 6f6f 6c65 616e 0a20 2020  be a boolean.   
+00009a60: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
+00009a70: 7374 616e 6365 2876 6572 626f 7365 2c20  stance(verbose, 
+00009a80: 626f 6f6c 293a 0a20 2020 2020 2020 2020  bool):.         
+00009a90: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
+00009aa0: 6f72 2822 7665 7262 6f73 6520 6861 7320  or("verbose has 
+00009ab0: 746f 2062 6520 6120 626f 6f6c 6561 6e2e  to be a boolean.
+00009ac0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00009ad0: 7665 7262 6f73 6520 3d20 7665 7262 6f73  verbose = verbos
+00009ae0: 650a 0a20 2020 2020 2020 2023 2320 6d65  e..        ## me
+00009af0: 7468 6f64 2075 7365 6420 746f 2073 6f6c  thod used to sol
+00009b00: 7665 2074 6865 204d 4241 5220 6571 7561  ve the MBAR equa
+00009b10: 7469 6f6e 0a20 2020 2020 2020 2069 6620  tion.        if 
+00009b20: 6e6f 7420 6973 696e 7374 616e 6365 286d  not isinstance(m
+00009b30: 6574 686f 642c 2073 7472 293a 0a20 2020  ethod, str):.   
+00009b40: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+00009b50: 7970 6545 7272 6f72 2822 6d65 7468 6f64  ypeError("method
+00009b60: 2068 6173 2074 6f20 6265 2061 2073 7472   has to be a str
+00009b70: 696e 672e 2229 0a20 2020 2020 2020 2069  ing.").        i
+00009b80: 6620 6d65 7468 6f64 206e 6f74 2069 6e20  f method not in 
+00009b90: 5b22 4e65 7774 6f6e 222c 2022 4c2d 4246  ["Newton", "L-BF
+00009ba0: 4753 2d42 225d 3a0a 2020 2020 2020 2020  GS-B"]:.        
+00009bb0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00009bc0: 7272 6f72 2822 6d65 7468 6f64 2068 6173  rror("method has
+00009bd0: 2074 6f20 6265 204e 6577 746f 6e20 6f72   to be Newton or
+00009be0: 204c 2d42 4647 532d 422e 2229 0a20 2020   L-BFGS-B.").   
+00009bf0: 2020 2020 2073 656c 662e 6d65 7468 6f64       self.method
+00009c00: 203d 206d 6574 686f 640a 0a20 2020 2020   = method..     
+00009c10: 2020 2023 2320 736f 6c76 6520 7468 6520     ## solve the 
+00009c20: 4d42 4152 2065 7175 6174 696f 6e0a 2020  MBAR equation.  
+00009c30: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+00009c40: 6f74 7374 7261 7020 6973 2046 616c 7365  otstrap is False
+00009c50: 3a0a 2020 2020 2020 2020 2020 2020 6446  :.            dF
+00009c60: 5f69 6e69 7420 3d20 7365 6c66 2e65 6e65  _init = self.ene
+00009c70: 7267 792e 6e65 775f 7a65 726f 7328 7365  rgy.new_zeros(se
+00009c80: 6c66 2e4d 202d 2031 290a 2020 2020 2020  lf.M - 1).      
+00009c90: 2020 2020 2020 6446 203d 205f 736f 6c76        dF = _solv
+00009ca0: 655f 6d62 6172 280a 2020 2020 2020 2020  e_mbar(.        
+00009cb0: 2020 2020 2020 2020 6446 5f69 6e69 742e          dF_init.
+00009cc0: 746f 2873 656c 662e 6465 7669 6365 292c  to(self.device),
+00009cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009ce0: 2073 656c 662e 656e 6572 6779 2e74 6f28   self.energy.to(
+00009cf0: 7365 6c66 2e64 6576 6963 6529 2c0a 2020  self.device),.  
+00009d00: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00009d10: 6c66 2e6e 756d 5f63 6f6e 662e 746f 2873  lf.num_conf.to(s
+00009d20: 656c 662e 6465 7669 6365 292c 0a20 2020  elf.device),.   
+00009d30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00009d40: 662e 6d65 7468 6f64 2c0a 2020 2020 2020  f.method,.      
+00009d50: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00009d60: 6261 7463 685f 7369 7a65 2c0a 2020 2020  batch_size,.    
+00009d70: 2020 2020 2020 2020 2020 2020 7665 7262              verb
+00009d80: 6f73 653d 7365 6c66 2e76 6572 626f 7365  ose=self.verbose
+00009d90: 2c0a 2020 2020 2020 2020 2020 2020 292e  ,.            ).
+00009da0: 6370 7528 290a 0a20 2020 2020 2020 2020  cpu()..         
+00009db0: 2020 2023 2320 7368 6966 7420 7365 6c66     ## shift self
+00009dc0: 2e5f 4620 7375 6368 2074 6861 7420 5c73  ._F such that \s
+00009dd0: 756d 5f69 2046 5b69 5d2a 6e75 6d5f 636f  um_i F[i]*num_co
+00009de0: 6e66 5b69 5d20 3d20 300a 2020 2020 2020  nf[i] = 0.      
+00009df0: 2020 2020 2020 4620 3d20 746f 7263 682e        F = torch.
+00009e00: 6361 7428 5b64 462e 6e65 775f 7a65 726f  cat([dF.new_zero
+00009e10: 7328 3129 2c20 6446 5d29 0a20 2020 2020  s(1), dF]).     
+00009e20: 2020 2020 2020 2070 6920 3d20 7365 6c66         pi = self
+00009e30: 2e6e 756d 5f63 6f6e 6620 2f20 7365 6c66  .num_conf / self
+00009e40: 2e4e 0a20 2020 2020 2020 2020 2020 2073  .N.            s
+00009e50: 656c 662e 5f46 203d 2046 202d 2074 6f72  elf._F = F - tor
+00009e60: 6368 2e73 756d 2870 6920 2a20 4629 0a0a  ch.sum(pi * F)..
+00009e70: 2020 2020 2020 2020 2020 2020 6220 3d20              b = 
+00009e80: 2d73 656c 662e 5f46 202d 2074 6f72 6368  -self._F - torch
+00009e90: 2e6c 6f67 2873 656c 662e 6e75 6d5f 636f  .log(self.num_co
+00009ea0: 6e66 290a 2020 2020 2020 2020 2020 2020  nf).            
+00009eb0: 7365 6c66 2e5f 6c6f 675f 7072 6f62 5f6d  self._log_prob_m
+00009ec0: 6978 203d 2074 6f72 6368 2e6c 6f67 7375  ix = torch.logsu
+00009ed0: 6d65 7870 282d 2873 656c 662e 656e 6572  mexp(-(self.ener
+00009ee0: 6779 202b 2062 5b3a 2c20 4e6f 6e65 5d29  gy + b[:, None])
+00009ef0: 2c20 6469 6d3d 3029 0a20 2020 2020 2020  , dim=0).       
+00009f00: 2020 2020 2073 656c 662e 5f6c 6f67 5f6d       self._log_m
+00009f10: 7520 3d20 2d73 656c 662e 6c6f 675f 7072  u = -self.log_pr
+00009f20: 6f62 5f6d 6978 0a0a 2020 2020 2020 2020  ob_mix..        
+00009f30: 2020 2020 2323 2043 6f6d 7075 7465 2073      ## Compute s
+00009f40: 656c 662e 5f46 5f63 6f76 2075 6e64 6572  elf._F_cov under
+00009f50: 2074 6865 2063 6f6e 7374 7261 696e 7420   the constraint 
+00009f60: 7468 6174 205c 7375 6d5f 6920 465b 695d  that \sum_i F[i]
+00009f70: 2a6e 756d 5f63 6f6e 665b 695d 203d 2030  *num_conf[i] = 0
+00009f80: 0a0a 2020 2020 2020 2020 2020 2020 2323  ..            ##
+00009f90: 2054 6865 7265 2061 7265 2074 776f 2077   There are two w
+00009fa0: 6179 7320 746f 2063 6f6d 7075 7465 2074  ays to compute t
+00009fb0: 6865 2063 6f76 6172 6961 6e63 6520 6d61  he covariance ma
+00009fc0: 7472 6978 206f 6620 7365 6c66 2e5f 460a  trix of self._F.
+00009fd0: 2020 2020 2020 2020 2020 2020 2323 2053              ## S
+00009fe0: 6565 2065 7175 6174 696f 6e20 342e 3220  ee equation 4.2 
+00009ff0: 616e 6420 362e 3420 696e 2074 6865 2066  and 6.4 in the f
+0000a000: 6f6c 6c6f 7769 6e67 2070 6170 6572 2066  ollowing paper f
+0000a010: 6f72 2064 6574 6169 6c73 0a20 2020 2020  or details.     
+0000a020: 2020 2020 2020 2023 2320 224b 6f6e 672c         ## "Kong,
+0000a030: 2041 2e2c 2065 7420 616c 2e20 2241 2074   A., et al. "A t
+0000a040: 6865 6f72 7920 6f66 2073 7461 7469 7374  heory of statist
+0000a050: 6963 616c 206d 6f64 656c 7320 666f 7220  ical models for 
+0000a060: 4d6f 6e74 6520 4361 726c 6f20 696e 7465  Monte Carlo inte
+0000a070: 6772 6174 696f 6e2e 220a 2020 2020 2020  gration.".      
+0000a080: 2020 2020 2020 2323 204a 6f75 726e 616c        ## Journal
+0000a090: 206f 6620 7468 6520 526f 7961 6c20 5374   of the Royal St
+0000a0a0: 6174 6973 7469 6361 6c20 536f 6369 6574  atistical Societ
+0000a0b0: 7920 5365 7269 6573 2042 3a20 5374 6174  y Series B: Stat
+0000a0c0: 6973 7469 6361 6c20 4d65 7468 6f64 6f6c  istical Methodol
+0000a0d0: 6f67 7920 3635 2e33 0a20 2020 2020 2020  ogy 65.3.       
+0000a0e0: 2020 2020 2023 2320 2832 3030 3329 3a20       ## (2003): 
+0000a0f0: 3538 352d 3630 342e 2220 6874 7470 733a  585-604." https:
+0000a100: 2f2f 646f 692e 6f72 672f 3130 2e31 3131  //doi.org/10.111
+0000a110: 312f 3134 3637 2d39 3836 382e 3030 3430  1/1467-9868.0040
+0000a120: 340a 0a20 2020 2020 2020 2020 2020 2023  4..            #
+0000a130: 2320 5468 6520 6669 7273 7420 7761 7920  # The first way 
+0000a140: 6173 2073 686f 776e 2069 6e20 7468 6520  as shown in the 
+0000a150: 666f 6c6c 6f77 696e 6720 7573 6573 2065  following uses e
+0000a160: 7175 6174 696f 6e20 342e 320a 2020 2020  quation 4.2.    
+0000a170: 2020 2020 2020 2020 2323 2074 6869 7320          ## this 
+0000a180: 6d65 7468 6f64 2069 7320 6d6f 7265 2067  method is more g
+0000a190: 656e 6572 616c 2074 6861 6e20 7468 6520  eneral than the 
+0000a1a0: 666f 6c6c 6f77 696e 6720 6d65 7468 6f64  following method
+0000a1b0: 2c20 6d65 616e 696e 6720 7468 6174 0a20  , meaning that. 
+0000a1c0: 2020 2020 2020 2020 2020 2023 2320 6974             ## it
+0000a1d0: 2063 616e 2061 6c73 6f20 6265 2075 7365   can also be use
+0000a1e0: 6420 746f 2063 6f6d 7075 7465 2063 6f76  d to compute cov
+0000a1f0: 6172 6961 6e63 6520 6d61 7472 6978 2066  ariance matrix f
+0000a200: 6f72 2070 6572 7475 7262 6564 2073 7461  or perturbed sta
+0000a210: 7465 732e 0a20 2020 2020 2020 2020 2020  tes..           
+0000a220: 2023 2320 5468 6572 6566 6f72 6520 6974   ## Therefore it
+0000a230: 2069 7320 7573 6564 2068 6572 652e 0a20   is used here.. 
+0000a240: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a250: 5020 3d20 746f 7263 682e 6578 7028 0a20  P = torch.exp(. 
+0000a260: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+0000a270: 2873 656c 662e 656e 6572 6779 202d 2073  (self.energy - s
+0000a280: 656c 662e 5f46 5b3a 2c20 4e6f 6e65 5d20  elf._F[:, None] 
+0000a290: 2b20 7365 6c66 2e5f 6c6f 675f 7072 6f62  + self._log_prob
+0000a2a0: 5f6d 6978 290a 2020 2020 2020 2020 2020  _mix).          
+0000a2b0: 2020 292e 7428 290a 2020 2020 2020 2020    ).t().        
+0000a2c0: 2020 2020 5720 3d20 746f 7263 682e 6469      W = torch.di
+0000a2d0: 6167 2873 656c 662e 6e75 6d5f 636f 6e66  ag(self.num_conf
+0000a2e0: 290a 2020 2020 2020 2020 2020 2020 512c  ).            Q,
+0000a2f0: 2052 203d 2074 6f72 6368 2e6c 696e 616c   R = torch.linal
+0000a300: 672e 7172 2873 656c 662e 5029 0a20 2020  g.qr(self.P).   
+0000a310: 2020 2020 2020 2020 2041 203d 2074 6f72           A = tor
+0000a320: 6368 2e65 7965 2873 656c 662e 4d2c 2064  ch.eye(self.M, d
+0000a330: 6576 6963 653d 572e 6465 7669 6365 2920  evice=W.device) 
+0000a340: 2d20 5220 4020 5720 4020 522e 540a 2020  - R @ W @ R.T.  
+0000a350: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000a360: 465f 636f 7620 3d20 522e 5420 4020 746f  F_cov = R.T @ to
+0000a370: 7263 682e 6c69 6e61 6c67 2e70 696e 7628  rch.linalg.pinv(
+0000a380: 412c 2068 6572 6d69 7469 616e 3d54 7275  A, hermitian=Tru
+0000a390: 652c 2072 746f 6c3d 3165 2d38 2920 4020  e, rtol=1e-8) @ 
+0000a3a0: 520a 0a20 2020 2020 2020 2020 2020 2023  R..            #
+0000a3b0: 2023 2054 6865 2073 6563 6f6e 6420 7761   # The second wa
+0000a3c0: 7920 7573 6573 2065 7175 6174 696f 6e20  y uses equation 
+0000a3d0: 362e 340a 2020 2020 2020 2020 2020 2020  6.4.            
+0000a3e0: 2320 6966 2073 656c 662e 5f62 6174 6368  # if self._batch
+0000a3f0: 5f73 697a 6520 6973 204e 6f6e 653a 0a20  _size is None:. 
+0000a400: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+0000a410: 2048 203d 205f 636f 6d70 7574 655f 6865   H = _compute_he
+0000a420: 7373 6961 6e5f 6c6f 675f 6c69 6b65 6c69  ssian_log_likeli
+0000a430: 686f 6f64 5f6f 665f 4628 0a20 2020 2020  hood_of_F(.     
+0000a440: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0000a450: 2073 656c 662e 5f46 2c20 7365 6c66 2e65   self._F, self.e
+0000a460: 6e65 7267 792c 2073 656c 662e 6e75 6d5f  nergy, self.num_
+0000a470: 636f 6e66 0a20 2020 2020 2020 2020 2020  conf.           
+0000a480: 2023 2020 2020 2029 0a20 2020 2020 2020   #     ).       
+0000a490: 2020 2020 2023 2065 6c73 653a 0a20 2020       # else:.   
+0000a4a0: 2020 2020 2020 2020 2023 2020 2020 2048           #     H
+0000a4b0: 203d 205f 636f 6d70 7574 655f 6865 7373   = _compute_hess
+0000a4c0: 6961 6e5f 6c6f 675f 6c69 6b65 6c69 686f  ian_log_likeliho
+0000a4d0: 6f64 5f6f 665f 465f 696e 5f62 6174 6368  od_of_F_in_batch
+0000a4e0: 280a 2020 2020 2020 2020 2020 2020 2320  (.            # 
+0000a4f0: 2020 2020 2020 2020 7365 6c66 2e5f 462c          self._F,
+0000a500: 2073 656c 662e 656e 6572 6779 2c20 7365   self.energy, se
+0000a510: 6c66 2e6e 756d 5f63 6f6e 662c 2073 656c  lf.num_conf, sel
+0000a520: 662e 5f62 6174 6368 5f73 697a 650a 2020  f._batch_size.  
+0000a530: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+0000a540: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+0000a550: 4870 203d 2048 2e6e 6577 5f7a 6572 6f73  Hp = H.new_zeros
+0000a560: 2828 7365 6c66 2e4d 202b 2031 2c20 7365  ((self.M + 1, se
+0000a570: 6c66 2e4d 202b 2031 2929 2e63 7075 2829  lf.M + 1)).cpu()
+0000a580: 0a20 2020 2020 2020 2020 2020 2023 2048  .            # H
+0000a590: 705b 3020 3a20 7365 6c66 2e4d 2c20 3020  p[0 : self.M, 0 
+0000a5a0: 3a20 7365 6c66 2e4d 5d20 3d20 480a 2020  : self.M] = H.  
+0000a5b0: 2020 2020 2020 2020 2020 2320 4870 5b73            # Hp[s
+0000a5c0: 656c 662e 4d2c 2030 203a 2073 656c 662e  elf.M, 0 : self.
+0000a5d0: 4d5d 203d 202d 7365 6c66 2e6e 756d 5f63  M] = -self.num_c
+0000a5e0: 6f6e 660a 2020 2020 2020 2020 2020 2020  onf.            
+0000a5f0: 2320 4870 5b30 203a 2073 656c 662e 4d2c  # Hp[0 : self.M,
+0000a600: 2073 656c 662e 4d5d 203d 202d 7365 6c66   self.M] = -self
+0000a610: 2e6e 756d 5f63 6f6e 660a 2020 2020 2020  .num_conf.      
+0000a620: 2020 2020 2020 2320 4870 5b73 656c 662e        # Hp[self.
+0000a630: 4d2c 2073 656c 662e 4d5d 203d 2030 0a20  M, self.M] = 0. 
+0000a640: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
+0000a650: 662e 5f46 5f63 6f76 203d 2074 6f72 6368  f._F_cov = torch
+0000a660: 2e6c 696e 616c 672e 696e 7628 2d48 7029  .linalg.inv(-Hp)
+0000a670: 5b30 203a 2073 656c 662e 4d2c 2030 203a  [0 : self.M, 0 :
+0000a680: 2073 656c 662e 4d5d 0a20 2020 2020 2020   self.M].       
+0000a690: 2020 2020 2023 2073 656c 662e 5f46 5f63       # self._F_c
+0000a6a0: 6f76 203d 2073 656c 662e 5f46 5f63 6f76  ov = self._F_cov
+0000a6b0: 202d 2074 6f72 6368 2e64 6961 6728 3120   - torch.diag(1 
+0000a6c0: 2f20 7365 6c66 2e6e 756d 5f63 6f6e 6629  / self.num_conf)
+0000a6d0: 202b 2031 202f 2073 656c 662e 4e0a 0a20   + 1 / self.N.. 
+0000a6e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a6f0: 5f46 5f73 7464 203d 2073 656c 662e 5f46  _F_std = self._F
+0000a700: 5f63 6f76 2e64 6961 676f 6e61 6c28 292e  _cov.diagonal().
+0000a710: 7371 7274 2829 0a0a 2020 2020 2020 2020  sqrt()..        
+0000a720: 2020 2020 7365 6c66 2e5f 4465 6c74 6146      self._DeltaF
+0000a730: 203d 2073 656c 662e 5f46 5b4e 6f6e 652c   = self._F[None,
+0000a740: 203a 5d20 2d20 7365 6c66 2e5f 465b 3a2c   :] - self._F[:,
+0000a750: 204e 6f6e 655d 0a20 2020 2020 2020 2020   None].         
+0000a760: 2020 2073 656c 662e 5f44 656c 7461 465f     self._DeltaF_
+0000a770: 636f 7620 3d20 280a 2020 2020 2020 2020  cov = (.        
+0000a780: 2020 2020 2020 2020 7365 6c66 2e5f 465f          self._F_
+0000a790: 636f 762e 6469 6167 2829 5b3a 2c20 4e6f  cov.diag()[:, No
+0000a7a0: 6e65 5d0a 2020 2020 2020 2020 2020 2020  ne].            
+0000a7b0: 2020 2020 2b20 7365 6c66 2e5f 465f 636f      + self._F_co
+0000a7c0: 762e 6469 6167 2829 5b4e 6f6e 652c 203a  v.diag()[None, :
+0000a7d0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000a7e0: 2020 2d20 3220 2a20 7365 6c66 2e5f 465f    - 2 * self._F_
+0000a7f0: 636f 760a 2020 2020 2020 2020 2020 2020  cov.            
+0000a800: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0000a810: 6c66 2e5f 4465 6c74 6146 5f73 7464 203d  lf._DeltaF_std =
+0000a820: 2073 656c 662e 5f44 656c 7461 465f 636f   self._DeltaF_co
+0000a830: 762e 7371 7274 2829 0a0a 2020 2020 2020  v.sqrt()..      
+0000a840: 2020 656c 6966 2073 656c 662e 626f 6f74    elif self.boot
+0000a850: 7374 7261 7020 6973 2054 7275 653a 0a20  strap is True:. 
+0000a860: 2020 2020 2020 2020 2020 2064 4673 203d             dFs =
+0000a870: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
+0000a880: 6c6f 675f 7072 6f62 5f6d 6978 203d 205b  log_prob_mix = [
+0000a890: 5d0a 2020 2020 2020 2020 2020 2020 6446  ].            dF
+0000a8a0: 5f69 6e69 7420 3d20 7365 6c66 2e65 6e65  _init = self.ene
+0000a8b0: 7267 792e 6e65 775f 7a65 726f 7328 7365  rgy.new_zeros(se
+0000a8c0: 6c66 2e4d 202d 2031 290a 2020 2020 2020  lf.M - 1).      
+0000a8d0: 2020 2020 2020 7365 6c66 2e5f 636f 6e66        self._conf
+0000a8e0: 5f69 6478 203d 205b 5d0a 2020 2020 2020  _idx = [].      
+0000a8f0: 2020 2020 2020 666f 7220 5f20 696e 2072        for _ in r
+0000a900: 616e 6765 2873 656c 662e 626f 6f74 7374  ange(self.bootst
+0000a910: 7261 705f 6e75 6d5f 7265 7029 3a0a 2020  rap_num_rep):.  
+0000a920: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000a930: 6e66 5f69 6478 203d 205f 626f 6f74 7374  nf_idx = _bootst
+0000a940: 7261 705f 636f 6e66 5f69 6478 280a 2020  rap_conf_idx(.  
+0000a950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a960: 2020 7365 6c66 2e6e 756d 5f63 6f6e 662e    self.num_conf.
+0000a970: 746f 2874 6f72 6368 2e69 6e74 3634 292c  to(torch.int64),
+0000a980: 2073 656c 662e 626f 6f74 7374 7261 705f   self.bootstrap_
+0000a990: 626c 6f63 6b5f 7369 7a65 0a20 2020 2020  block_size.     
+0000a9a0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000a9b0: 2020 2020 2020 2020 2020 2020 2064 4620               dF 
+0000a9c0: 3d20 5f73 6f6c 7665 5f6d 6261 7228 0a20  = _solve_mbar(. 
+0000a9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9e0: 2020 2064 465f 696e 6974 2e74 6f28 7365     dF_init.to(se
+0000a9f0: 6c66 2e64 6576 6963 6529 2c0a 2020 2020  lf.device),.    
+0000aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa10: 7365 6c66 2e65 6e65 7267 795b 3a2c 2063  self.energy[:, c
+0000aa20: 6f6e 665f 6964 785d 2e74 6f28 7365 6c66  onf_idx].to(self
+0000aa30: 2e64 6576 6963 6529 2c0a 2020 2020 2020  .device),.      
+0000aa40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000aa50: 6c66 2e6e 756d 5f63 6f6e 662e 746f 2873  lf.num_conf.to(s
+0000aa60: 656c 662e 6465 7669 6365 292c 0a20 2020  elf.device),.   
+0000aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa80: 2073 656c 662e 6d65 7468 6f64 2c0a 2020   self.method,.  
+0000aa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aaa0: 2020 7365 6c66 2e5f 6261 7463 685f 7369    self._batch_si
+0000aab0: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
+0000aac0: 2020 2020 2020 2020 7665 7262 6f73 653d          verbose=
+0000aad0: 7365 6c66 2e76 6572 626f 7365 2c0a 2020  self.verbose,.  
+0000aae0: 2020 2020 2020 2020 2020 2020 2020 292e                ).
+0000aaf0: 6370 7528 290a 2020 2020 2020 2020 2020  cpu().          
+0000ab00: 2020 2020 2020 6446 5f69 6e69 7420 3d20        dF_init = 
+0000ab10: 6446 0a20 2020 2020 2020 2020 2020 2020  dF.             
+0000ab20: 2020 2064 4673 2e61 7070 656e 6428 6446     dFs.append(dF
+0000ab30: 2e63 6c6f 6e65 2829 290a 0a20 2020 2020  .clone())..     
+0000ab40: 2020 2020 2020 2020 2020 2046 203d 2074             F = t
+0000ab50: 6f72 6368 2e63 6174 285b 6446 2e6e 6577  orch.cat([dF.new
+0000ab60: 5f7a 6572 6f73 2831 292c 2064 465d 290a  _zeros(1), dF]).
+0000ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab80: 2323 2073 6869 6674 2046 2073 7563 6820  ## shift F such 
+0000ab90: 7468 6174 205c 7375 6d5f 6920 465b 695d  that \sum_i F[i]
+0000aba0: 2a6e 756d 5f63 6f6e 665b 695d 203d 2030  *num_conf[i] = 0
+0000abb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000abc0: 2070 6920 3d20 7365 6c66 2e6e 756d 5f63   pi = self.num_c
+0000abd0: 6f6e 6620 2f20 7365 6c66 2e4e 0a20 2020  onf / self.N.   
+0000abe0: 2020 2020 2020 2020 2020 2020 2046 203d               F =
+0000abf0: 2046 202d 2074 6f72 6368 2e73 756d 2870   F - torch.sum(p
+0000ac00: 6920 2a20 4629 0a0a 2020 2020 2020 2020  i * F)..        
+0000ac10: 2020 2020 2020 2020 6220 3d20 2d46 202d          b = -F -
+0000ac20: 2074 6f72 6368 2e6c 6f67 2873 656c 662e   torch.log(self.
+0000ac30: 6e75 6d5f 636f 6e66 202f 2073 656c 662e  num_conf / self.
+0000ac40: 4e29 0a20 2020 2020 2020 2020 2020 2020  N).             
+0000ac50: 2020 206c 6f67 5f70 726f 625f 6d69 782e     log_prob_mix.
+0000ac60: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
+0000ac70: 2020 2020 2020 2020 2020 2020 746f 7263              torc
+0000ac80: 682e 6c6f 6773 756d 6578 7028 2d28 7365  h.logsumexp(-(se
+0000ac90: 6c66 2e65 6e65 7267 795b 3a2c 2063 6f6e  lf.energy[:, con
+0000aca0: 665f 6964 785d 202b 2062 5b3a 2c20 4e6f  f_idx] + b[:, No
+0000acb0: 6e65 5d29 2c20 6469 6d3d 3029 0a20 2020  ne]), dim=0).   
+0000acc0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000acd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ace0: 656c 662e 5f63 6f6e 665f 6964 782e 6170  elf._conf_idx.ap
+0000acf0: 7065 6e64 2863 6f6e 665f 6964 7829 0a0a  pend(conf_idx)..
+0000ad00: 2020 2020 2020 2020 2020 2020 6446 203d              dF =
+0000ad10: 2074 6f72 6368 2e73 7461 636b 2864 4673   torch.stack(dFs
+0000ad20: 2c20 6469 6d3d 3129 0a20 2020 2020 2020  , dim=1).       
+0000ad30: 2020 2020 2046 203d 2074 6f72 6368 2e63       F = torch.c
+0000ad40: 6174 285b 6446 2e6e 6577 5f7a 6572 6f73  at([dF.new_zeros
+0000ad50: 2831 2c20 6446 2e73 6861 7065 5b31 5d29  (1, dF.shape[1])
+0000ad60: 2c20 6446 5d2c 2064 696d 3d30 290a 0a20  , dF], dim=0).. 
+0000ad70: 2020 2020 2020 2020 2020 2023 2320 7368             ## sh
+0000ad80: 6966 7420 4620 7375 6368 2074 6861 7420  ift F such that 
+0000ad90: 5c73 756d 5f69 2046 5b69 5d2a 6e75 6d5f  \sum_i F[i]*num_
+0000ada0: 636f 6e66 5b69 5d20 3d20 300a 2020 2020  conf[i] = 0.    
+0000adb0: 2020 2020 2020 2020 7069 203d 2073 656c          pi = sel
+0000adc0: 662e 6e75 6d5f 636f 6e66 202f 2073 656c  f.num_conf / sel
+0000add0: 662e 4e0a 2020 2020 2020 2020 2020 2020  f.N.            
+0000ade0: 7365 6c66 2e5f 465f 626f 6f74 7374 7261  self._F_bootstra
+0000adf0: 7020 3d20 4620 2d20 746f 7263 682e 7375  p = F - torch.su
+0000ae00: 6d28 7069 5b3a 2c20 4e6f 6e65 5d20 2a20  m(pi[:, None] * 
+0000ae10: 462c 2064 696d 3d30 290a 0a20 2020 2020  F, dim=0)..     
+0000ae20: 2020 2020 2020 2073 656c 662e 5f46 203d         self._F =
+0000ae30: 2074 6f72 6368 2e6d 6561 6e28 7365 6c66   torch.mean(self
+0000ae40: 2e5f 465f 626f 6f74 7374 7261 702c 2064  ._F_bootstrap, d
+0000ae50: 696d 3d31 290a 2020 2020 2020 2020 2020  im=1).          
+0000ae60: 2020 7365 6c66 2e5f 465f 7374 6420 3d20    self._F_std = 
+0000ae70: 746f 7263 682e 7374 6428 7365 6c66 2e5f  torch.std(self._
+0000ae80: 465f 626f 6f74 7374 7261 702c 2064 696d  F_bootstrap, dim
+0000ae90: 3d31 290a 2020 2020 2020 2020 2020 2020  =1).            
+0000aea0: 7365 6c66 2e5f 465f 636f 7620 3d20 746f  self._F_cov = to
+0000aeb0: 7263 682e 636f 7628 7365 6c66 2e5f 465f  rch.cov(self._F_
+0000aec0: 626f 6f74 7374 7261 7029 0a0a 2020 2020  bootstrap)..    
+0000aed0: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
+0000aee0: 675f 7072 6f62 5f6d 6978 203d 2074 6f72  g_prob_mix = tor
+0000aef0: 6368 2e73 7461 636b 286c 6f67 5f70 726f  ch.stack(log_pro
+0000af00: 625f 6d69 782c 2064 696d 3d30 290a 2020  b_mix, dim=0).  
+0000af10: 2020 2020 2020 2020 2020 4465 6c74 6146            DeltaF
+0000af20: 203d 2064 465b 4e6f 6e65 2c20 3a2c 203a   = dF[None, :, :
+0000af30: 5d20 2d20 6446 5b3a 2c20 4e6f 6e65 2c20  ] - dF[:, None, 
+0000af40: 3a5d 0a20 2020 2020 2020 2020 2020 2073  :].            s
+0000af50: 656c 662e 5f44 656c 7461 4620 3d20 746f  elf._DeltaF = to
+0000af60: 7263 682e 6d65 616e 2844 656c 7461 462c  rch.mean(DeltaF,
+0000af70: 2064 696d 3d32 290a 2020 2020 2020 2020   dim=2).        
+0000af80: 2020 2020 7365 6c66 2e5f 4465 6c74 6146      self._DeltaF
+0000af90: 5f73 7464 203d 2074 6f72 6368 2e73 7464  _std = torch.std
+0000afa0: 2844 656c 7461 462c 2064 696d 3d32 290a  (DeltaF, dim=2).
+0000afb0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000afc0: 2020 2064 6566 2046 2873 656c 6629 202d     def F(self) -
+0000afd0: 3e20 6e70 2e6e 6461 7272 6179 3a0a 2020  > np.ndarray:.  
+0000afe0: 2020 2020 2020 2222 2246 7265 6520 656e        """Free en
+0000aff0: 6572 6769 6573 206f 6620 7468 6520 7374  ergies of the st
+0000b000: 6174 6573 2075 6e64 6572 2074 6865 2063  ates under the c
+0000b010: 6f6e 7374 7261 696e 7420 3a6d 6174 683a  onstraint :math:
+0000b020: 605c 7375 6d5f 7b6b 3d31 7d5e 7b4d 7d20  `\sum_{k=1}^{M} 
+0000b030: 4e5f 6b20 2a20 465f 6b20 3d20 3060 2c0a  N_k * F_k = 0`,.
+0000b040: 2020 2020 2020 2020 7768 6572 6520 3a6d          where :m
+0000b050: 6174 683a 604e 5f6b 6020 6973 2074 6865  ath:`N_k` is the
+0000b060: 206e 756d 6265 7220 6f66 2063 6f6e 666f   number of confo
+0000b070: 726d 6174 696f 6e73 2073 616d 706c 6564  rmations sampled
+0000b080: 2066 726f 6d20 7374 6174 6520 6b2e 0a20   from state k.. 
+0000b090: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000b0a0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000b0b0: 462e 6370 7528 292e 6e75 6d70 7928 290a  F.cpu().numpy().
+0000b0c0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000b0d0: 2020 2064 6566 2046 5f73 7464 2873 656c     def F_std(sel
+0000b0e0: 6629 202d 3e20 6e70 2e6e 6461 7272 6179  f) -> np.ndarray
+0000b0f0: 3a0a 2020 2020 2020 2020 2222 2253 7461  :.        """Sta
+0000b100: 6e64 6172 6420 6465 7669 6174 696f 6e20  ndard deviation 
+0000b110: 6f66 2074 6865 2066 7265 6520 656e 6572  of the free ener
+0000b120: 6769 6573 206f 6620 7468 6520 7374 6174  gies of the stat
+0000b130: 6573 2075 6e64 6572 2074 6865 2063 6f6e  es under the con
+0000b140: 7374 7261 696e 740a 2020 2020 2020 2020  straint.        
+0000b150: 3a6d 6174 683a 605c 7375 6d5f 7b6b 3d31  :math:`\sum_{k=1
+0000b160: 7d5e 7b4d 7d20 4e5f 6b20 2a20 465f 6b20  }^{M} N_k * F_k 
+0000b170: 3d20 3060 2c0a 2020 2020 2020 2020 7768  = 0`,.        wh
+0000b180: 6572 6520 3a6d 6174 683a 604e 5f6b 6020  ere :math:`N_k` 
+0000b190: 6973 2074 6865 206e 756d 6265 7220 6f66  is the number of
+0000b1a0: 2063 6f6e 666f 726d 6174 696f 6e73 2073   conformations s
+0000b1b0: 616d 706c 6564 2066 726f 6d20 7374 6174  ampled from stat
+0000b1c0: 6520 6b2e 0a20 2020 2020 2020 2022 2222  e k..        """
+0000b1d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000b1e0: 7365 6c66 2e5f 465f 7374 642e 6370 7528  self._F_std.cpu(
+0000b1f0: 292e 6e75 6d70 7928 290a 0a20 2020 2040  ).numpy()..    @
+0000b200: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+0000b210: 2046 5f63 6f76 2873 656c 6629 202d 3e20   F_cov(self) -> 
+0000b220: 6e70 2e6e 6461 7272 6179 3a0a 2020 2020  np.ndarray:.    
+0000b230: 2020 2020 2222 2243 6f76 6172 6961 6e63      """Covarianc
+0000b240: 6520 6d61 7472 6978 206f 6620 7468 6520  e matrix of the 
+0000b250: 6672 6565 2065 6e65 7267 6965 7320 6f66  free energies of
+0000b260: 2074 6865 2073 7461 7465 7320 756e 6465   the states unde
+0000b270: 7220 7468 6520 636f 6e73 7472 6169 6e74  r the constraint
+0000b280: 0a20 2020 2020 2020 203a 6d61 7468 3a60  .        :math:`
+0000b290: 5c73 756d 5f7b 6b3d 317d 5e7b 4d7d 204e  \sum_{k=1}^{M} N
+0000b2a0: 5f6b 202a 2046 5f6b 203d 2030 602c 0a20  _k * F_k = 0`,. 
+0000b2b0: 2020 2020 2020 2077 6865 7265 203a 6d61         where :ma
+0000b2c0: 7468 3a60 4e5f 6b60 2069 7320 7468 6520  th:`N_k` is the 
+0000b2d0: 6e75 6d62 6572 206f 6620 636f 6e66 6f72  number of confor
+0000b2e0: 6d61 7469 6f6e 7320 7361 6d70 6c65 6420  mations sampled 
+0000b2f0: 6672 6f6d 2073 7461 7465 206b 2e0a 2020  from state k..  
+0000b300: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000b310: 2020 7265 7475 726e 2073 656c 662e 5f46    return self._F
+0000b320: 5f63 6f76 2e63 7075 2829 2e6e 756d 7079  _cov.cpu().numpy
+0000b330: 2829 0a0a 2020 2020 4070 726f 7065 7274  ()..    @propert
+0000b340: 790a 2020 2020 6465 6620 4465 6c74 6146  y.    def DeltaF
+0000b350: 2873 656c 6629 202d 3e20 6e70 2e6e 6461  (self) -> np.nda
+0000b360: 7272 6179 3a0a 2020 2020 2020 2020 2222  rray:.        ""
+0000b370: 2246 7265 6520 656e 6572 6779 2064 6966  "Free energy dif
+0000b380: 6665 7265 6e63 6520 6265 7477 6565 6e20  ference between 
+0000b390: 7374 6174 6573 2e0a 2020 2020 2020 2020  states..        
+0000b3a0: 3a6d 6174 683a 605c 6d61 7468 726d 7b44  :math:`\mathrm{D
+0000b3b0: 656c 7461 467d 5b69 2c6a 5d60 2069 7320  eltaF}[i,j]` is 
+0000b3c0: 7468 6520 6672 6565 2065 6e65 7267 7920  the free energy 
+0000b3d0: 6469 6666 6572 656e 6365 2062 6574 7765  difference betwe
+0000b3e0: 656e 2073 7461 7465 206a 2061 6e64 2073  en state j and s
+0000b3f0: 7461 7465 2069 2c0a 2020 2020 2020 2020  tate i,.        
+0000b400: 692e 652e 2c20 3a6d 6174 683a 605c 6d61  i.e., :math:`\ma
+0000b410: 7468 726d 7b44 656c 7461 467d 5b69 2c6a  thrm{DeltaF}[i,j
+0000b420: 5d20 3d20 465b 6a5d 202d 2046 5b69 5d60  ] = F[j] - F[i]`
+0000b430: 202e 0a20 2020 2020 2020 2022 2222 0a20   ..        """. 
+0000b440: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000b450: 6c66 2e5f 4465 6c74 6146 2e63 7075 2829  lf._DeltaF.cpu()
+0000b460: 2e6e 756d 7079 2829 0a0a 2020 2020 4070  .numpy()..    @p
+0000b470: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000b480: 4465 6c74 6146 5f73 7464 2873 656c 6629  DeltaF_std(self)
+0000b490: 202d 3e20 6e70 2e6e 6461 7272 6179 3a0a   -> np.ndarray:.
+0000b4a0: 2020 2020 2020 2020 2222 2253 7461 6e64          """Stand
+0000b4b0: 6172 6420 6465 7669 6174 696f 6e20 6f66  ard deviation of
+0000b4c0: 2074 6865 2066 7265 6520 656e 6572 6779   the free energy
+0000b4d0: 2064 6966 6665 7265 6e63 6520 6265 7477   difference betw
+0000b4e0: 6565 6e20 7374 6174 6573 2e0a 2020 2020  een states..    
+0000b4f0: 2020 2020 3a6d 6174 683a 605c 6d61 7468      :math:`\math
+0000b500: 726d 7b44 656c 7461 465f 7374 647d 5b69  rm{DeltaF_std}[i
+0000b510: 2c6a 5d60 2069 7320 7468 6520 7374 616e  ,j]` is the stan
+0000b520: 6461 7264 2064 6576 6961 7469 6f6e 206f  dard deviation o
+0000b530: 6620 7468 6520 6672 6565 2065 6e65 7267  f the free energ
+0000b540: 790a 2020 2020 2020 2020 6469 6666 6572  y.        differ
+0000b550: 656e 6365 203a 6d61 7468 3a60 5c6d 6174  ence :math:`\mat
+0000b560: 6872 6d7b 4465 6c74 6146 7d5b 692c 6a5d  hrm{DeltaF}[i,j]
+0000b570: 602e 0a20 2020 2020 2020 2022 2222 0a20  `..        """. 
+0000b580: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000b590: 6c66 2e5f 4465 6c74 6146 5f73 7464 2e63  lf._DeltaF_std.c
+0000b5a0: 7075 2829 2e6e 756d 7079 2829 0a0a 2020  pu().numpy()..  
+0000b5b0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000b5c0: 6465 6620 6c6f 675f 7072 6f62 5f6d 6978  def log_prob_mix
+0000b5d0: 2873 656c 6629 202d 3e20 6e70 2e6e 6461  (self) -> np.nda
+0000b5e0: 7272 6179 3a0a 2020 2020 2020 2020 2222  rray:.        ""
+0000b5f0: 2274 6865 206c 6f67 2070 726f 6261 6269  "the log probabi
+0000b600: 6c69 7479 2064 656e 7369 7479 206f 6620  lity density of 
+0000b610: 636f 6e66 6f72 6d61 7469 6f6e 7320 696e  conformations in
+0000b620: 2074 6865 206d 6978 7475 7265 2064 6973   the mixture dis
+0000b630: 7472 6962 7574 696f 6e2e 2222 220a 2020  tribution.""".  
+0000b640: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000b650: 662e 5f6c 6f67 5f70 726f 625f 6d69 782e  f._log_prob_mix.
+0000b660: 6370 7528 292e 6e75 6d70 7928 290a 0a20  cpu().numpy().. 
+0000b670: 2020 2064 6566 2063 616c 6375 6c61 7465     def calculate
+0000b680: 5f66 7265 655f 656e 6572 6769 6573 5f6f  _free_energies_o
+0000b690: 665f 7065 7274 7572 6265 645f 7374 6174  f_perturbed_stat
+0000b6a0: 6573 2873 656c 662c 2065 6e65 7267 795f  es(self, energy_
+0000b6b0: 7065 7274 7572 6265 6429 3a0a 2020 2020  perturbed):.    
+0000b6c0: 2020 2020 2222 2263 616c 6375 6c61 7465      """calculate
+0000b6d0: 2066 7265 6520 656e 6572 6769 6573 2066   free energies f
+0000b6e0: 6f72 2070 6572 7475 7262 6564 2073 7461  or perturbed sta
+0000b6f0: 7465 732e 0a0a 2020 2020 2020 2020 5061  tes...        Pa
+0000b700: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+0000b710: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020   -----------.   
+0000b720: 2020 2020 2065 6e65 7267 795f 7065 7274       energy_pert
+0000b730: 7572 6265 643a 2032 2d44 2066 6c6f 6174  urbed: 2-D float
+0000b740: 206e 6461 7272 6179 2077 6974 6820 7369   ndarray with si
+0000b750: 7a65 206f 6620 284c 2c4e 290a 2020 2020  ze of (L,N).    
+0000b760: 2020 2020 2020 2020 6561 6368 2072 6f77          each row
+0000b770: 206f 6620 7468 6520 656e 6572 6779 5f70   of the energy_p
+0000b780: 6572 7475 7262 6564 206d 6174 7269 7820  erturbed matrix 
+0000b790: 7265 7072 6573 656e 7473 2061 2073 7461  represents a sta
+0000b7a0: 7465 2061 6e64 0a20 2020 2020 2020 2020  te and.         
+0000b7b0: 2020 2074 6865 2076 616c 7565 2065 6e65     the value ene
+0000b7c0: 7267 795f 7065 7274 7572 6265 645b 6c2c  rgy_perturbed[l,
+0000b7d0: 6e5d 2072 6570 7265 7365 6e74 7320 7468  n] represents th
+0000b7e0: 6520 7265 6475 6365 6420 656e 6572 6779  e reduced energy
+0000b7f0: 0a20 2020 2020 2020 2020 2020 206f 6620  .            of 
+0000b800: 7468 6520 6e27 7468 2063 6f6e 666f 726d  the n'th conform
+0000b810: 6174 696f 6e20 696e 2074 6865 206c 2774  ation in the l't
+0000b820: 6820 7065 7274 7572 6265 6420 7374 6174  h perturbed stat
+0000b830: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
+0000b840: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+0000b850: 2d2d 2d0a 2020 2020 2020 2020 7265 7375  ---.        resu
+0000b860: 6c74 733a 2064 6963 740a 2020 2020 2020  lts: dict.      
+0000b870: 2020 2020 2020 6120 6469 6374 696f 6e61        a dictiona
+0000b880: 7279 2063 6f6e 7461 696e 696e 6720 7468  ry containing th
+0000b890: 6520 666f 6c6c 6f77 696e 6720 6b65 7973  e following keys
+0000b8a0: 3a0a 0a20 2020 2020 2020 2020 2020 202a  :..            *
+0000b8b0: 2a46 2a2a 202d 2074 6865 2066 7265 6520  *F** - the free 
+0000b8c0: 656e 6572 6779 206f 6620 7468 6520 7065  energy of the pe
+0000b8d0: 7274 7572 6265 6420 7374 6174 6573 2e0a  rturbed states..
+0000b8e0: 0a20 2020 2020 2020 2020 2020 202a 2a46  .            **F
+0000b8f0: 5f73 7464 2a2a 202d 2074 6865 2073 7461  _std** - the sta
+0000b900: 6e64 6172 6420 6465 7669 6174 696f 6e20  ndard deviation 
+0000b910: 6f66 2074 6865 2066 7265 6520 656e 6572  of the free ener
+0000b920: 6779 206f 6620 7468 6520 7065 7274 7572  gy of the pertur
+0000b930: 6265 6420 7374 6174 6573 2e20 0a0a 2020  bed states. ..  
+0000b940: 2020 2020 2020 2020 2020 2a2a 465f 636f            **F_co
+0000b950: 762a 2a20 2d20 7468 6520 636f 7661 7269  v** - the covari
+0000b960: 616e 6365 2062 6574 7765 656e 2074 6865  ance between the
+0000b970: 2066 7265 6520 656e 6572 6769 6573 206f   free energies o
+0000b980: 6620 7468 6520 7065 7274 7572 6265 6420  f the perturbed 
+0000b990: 7374 6174 6573 2e0a 0a20 2020 2020 2020  states...       
+0000b9a0: 2020 2020 202a 2a44 656c 7461 462a 2a20       **DeltaF** 
+0000b9b0: 2d20 3a6d 6174 683a 605c 6d61 7468 726d  - :math:`\mathrm
+0000b9c0: 7b44 656c 7461 467d 5b6b 2c6c 5d60 2069  {DeltaF}[k,l]` i
+0000b9d0: 7320 7468 6520 6672 6565 2065 6e65 7267  s the free energ
+0000b9e0: 7920 6469 6666 6572 656e 6365 2062 6574  y difference bet
+0000b9f0: 7765 656e 2073 7461 7465 2020 2020 2020  ween state      
+0000ba00: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+0000ba10: 2020 203a 6d61 7468 3a60 6b60 2061 6e64     :math:`k` and
+0000ba20: 2073 7461 7465 203a 6d61 7468 3a60 6c60   state :math:`l`
+0000ba30: 2c20 692e 652e 2c20 3a6d 6174 683a 605c  , i.e., :math:`\
+0000ba40: 6d61 7468 726d 7b44 656c 7461 467d 5b6b  mathrm{DeltaF}[k
+0000ba50: 2c6c 5d20 3d20 465b 6c5d 202d 2046 5b6b  ,l] = F[l] - F[k
+0000ba60: 5d60 202e 0a0a 2020 2020 2020 2020 2020  ]` ...          
+0000ba70: 2020 2a2a 4465 6c74 6146 5f73 7464 2a2a    **DeltaF_std**
+0000ba80: 202d 2074 6865 2073 7461 6e64 6172 6420   - the standard 
+0000ba90: 6465 7669 6174 696f 6e20 6f66 2074 6865  deviation of the
+0000baa0: 2066 7265 6520 656e 6572 6779 2064 6966   free energy dif
+0000bab0: 6665 7265 6e63 652e 0a20 2020 2020 2020  ference..       
+0000bac0: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
+0000bad0: 2069 7369 6e73 7461 6e63 6528 656e 6572   isinstance(ener
+0000bae0: 6779 5f70 6572 7475 7262 6564 2c20 6e70  gy_perturbed, np
+0000baf0: 2e6e 6461 7272 6179 293a 0a20 2020 2020  .ndarray):.     
+0000bb00: 2020 2020 2020 2065 6e65 7267 795f 7065         energy_pe
+0000bb10: 7274 7572 6265 6420 3d20 656e 6572 6779  rturbed = energy
+0000bb20: 5f70 6572 7475 7262 6564 2e61 7374 7970  _perturbed.astyp
+0000bb30: 6528 6e70 2e66 6c6f 6174 3634 290a 2020  e(np.float64).  
+0000bb40: 2020 2020 2020 2020 2020 656e 6572 6779            energy
+0000bb50: 5f70 6572 7475 7262 6564 203d 2074 6f72  _perturbed = tor
+0000bb60: 6368 2e66 726f 6d5f 6e75 6d70 7928 656e  ch.from_numpy(en
+0000bb70: 6572 6779 5f70 6572 7475 7262 6564 290a  ergy_perturbed).
+0000bb80: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+0000bb90: 6e73 7461 6e63 6528 656e 6572 6779 5f70  nstance(energy_p
+0000bba0: 6572 7475 7262 6564 2c20 746f 7263 682e  erturbed, torch.
+0000bbb0: 5465 6e73 6f72 293a 0a20 2020 2020 2020  Tensor):.       
+0000bbc0: 2020 2020 2065 6e65 7267 795f 7065 7274       energy_pert
+0000bbd0: 7572 6265 6420 3d20 656e 6572 6779 5f70  urbed = energy_p
+0000bbe0: 6572 7475 7262 6564 2e64 6f75 626c 6528  erturbed.double(
+0000bbf0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0000bc00: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000bc10: 6520 5479 7065 4572 726f 7228 2265 6e65  e TypeError("ene
+0000bc20: 7267 795f 7065 7274 7572 6265 6420 6861  rgy_perturbed ha
+0000bc30: 7320 746f 2062 6520 6120 322d 4420 6e64  s to be a 2-D nd
+0000bc40: 6172 7261 7920 6f72 2061 2032 2d44 2074  array or a 2-D t
+0000bc50: 656e 736f 722e 2229 0a0a 2020 2020 2020  ensor.")..      
+0000bc60: 2020 6966 2065 6e65 7267 795f 7065 7274    if energy_pert
+0000bc70: 7572 6265 642e 6e64 696d 2021 3d20 323a  urbed.ndim != 2:
+0000bc80: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0000bc90: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+0000bca0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000bcb0: 656e 6572 6779 5f70 6572 7475 7262 6564  energy_perturbed
+0000bcc0: 2068 6173 2074 6f20 6265 2061 2032 2d44   has to be a 2-D
+0000bcd0: 206e 6461 7272 6179 206f 7220 6120 322d   ndarray or a 2-
+0000bce0: 4420 7465 6e73 6f72 2e22 0a20 2020 2020  D tensor.".     
+0000bcf0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000bd00: 2069 6620 656e 6572 6779 5f70 6572 7475   if energy_pertu
+0000bd10: 7262 6564 2e73 6861 7065 5b31 5d20 213d  rbed.shape[1] !=
+0000bd20: 2073 656c 662e 656e 6572 6779 2e73 6861   self.energy.sha
+0000bd30: 7065 5b31 5d3a 0a20 2020 2020 2020 2020  pe[1]:.         
+0000bd40: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+0000bd50: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+0000bd60: 2020 2020 2022 7468 6520 6e75 6d62 6572       "the number
+0000bd70: 206f 6620 636f 6c75 6d6e 7320 696e 2065   of columns in e
+0000bd80: 6e65 7267 795f 7065 7274 7572 6265 6420  nergy_perturbed 
+0000bd90: 6861 7320 746f 2062 6520 6571 7561 6c20  has to be equal 
+0000bda0: 746f 2074 6865 206e 756d 6265 7220 6f66  to the number of
+0000bdb0: 2063 6f6c 756d 6e73 2069 6e20 656e 6572   columns in ener
+0000bdc0: 6779 2e22 0a20 2020 2020 2020 2020 2020  gy.".           
+0000bdd0: 2029 0a0a 2020 2020 2020 2020 4c20 3d20   )..        L = 
+0000bde0: 656e 6572 6779 5f70 6572 7475 7262 6564  energy_perturbed
+0000bdf0: 2e73 6861 7065 5b30 5d0a 0a20 2020 2020  .shape[0]..     
+0000be00: 2020 2046 203d 204e 6f6e 650a 2020 2020     F = None.    
+0000be10: 2020 2020 465f 636f 7620 3d20 4e6f 6e65      F_cov = None
+0000be20: 0a20 2020 2020 2020 2046 5f73 7464 203d  .        F_std =
+0000be30: 204e 6f6e 650a 0a20 2020 2020 2020 2069   None..        i
+0000be40: 6620 6e6f 7420 7365 6c66 2e62 6f6f 7473  f not self.boots
+0000be50: 7472 6170 3a0a 2020 2020 2020 2020 2020  trap:.          
+0000be60: 2020 6475 203d 2065 6e65 7267 795f 7065    du = energy_pe
+0000be70: 7274 7572 6265 6420 2b20 7365 6c66 2e5f  rturbed + self._
+0000be80: 6c6f 675f 7072 6f62 5f6d 6978 0a20 2020  log_prob_mix.   
+0000be90: 2020 2020 2020 2020 2046 203d 202d 746f           F = -to
+0000bea0: 7263 682e 6c6f 6773 756d 6578 7028 2d64  rch.logsumexp(-d
+0000beb0: 752c 2064 696d 3d31 290a 0a20 2020 2020  u, dim=1)..     
+0000bec0: 2020 2020 2020 2046 5f65 7874 203d 2074         F_ext = t
+0000bed0: 6f72 6368 2e63 6174 285b 7365 6c66 2e5f  orch.cat([self._
+0000bee0: 462c 2046 5d29 0a20 2020 2020 2020 2020  F, F]).         
+0000bef0: 2020 2055 203d 2074 6f72 6368 2e63 6174     U = torch.cat
+0000bf00: 285b 7365 6c66 2e65 6e65 7267 792c 2065  ([self.energy, e
+0000bf10: 6e65 7267 795f 7065 7274 7572 6265 645d  nergy_perturbed]
+0000bf20: 2c20 6469 6d3d 3029 2e74 2829 0a20 2020  , dim=0).t().   
+0000bf30: 2020 2020 2020 2020 2050 203d 2074 6f72           P = tor
+0000bf40: 6368 2e65 7870 282d 2855 202d 2046 5f65  ch.exp(-(U - F_e
+0000bf50: 7874 202b 2073 656c 662e 5f6c 6f67 5f70  xt + self._log_p
+0000bf60: 726f 625f 6d69 785b 3a2c 204e 6f6e 655d  rob_mix[:, None]
+0000bf70: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+0000bf80: 5720 3d20 746f 7263 682e 6469 6167 2874  W = torch.diag(t
+0000bf90: 6f72 6368 2e63 6174 285b 7365 6c66 2e6e  orch.cat([self.n
+0000bfa0: 756d 5f63 6f6e 662c 2073 656c 662e 6e75  um_conf, self.nu
+0000bfb0: 6d5f 636f 6e66 2e6e 6577 5f7a 6572 6f73  m_conf.new_zeros
+0000bfc0: 284c 295d 2929 0a20 2020 2020 2020 2020  (L)])).         
+0000bfd0: 2020 2051 2c20 5220 3d20 746f 7263 682e     Q, R = torch.
+0000bfe0: 6c69 6e61 6c67 2e71 7228 5029 0a20 2020  linalg.qr(P).   
+0000bff0: 2020 2020 2020 2020 2041 203d 2074 6f72           A = tor
+0000c000: 6368 2e65 7965 2873 656c 662e 4d20 2b20  ch.eye(self.M + 
+0000c010: 4c2c 2064 6576 6963 653d 572e 6465 7669  L, device=W.devi
+0000c020: 6365 2920 2d20 5220 4020 5720 4020 522e  ce) - R @ W @ R.
+0000c030: 540a 2020 2020 2020 2020 2020 2020 465f  T.            F_
+0000c040: 636f 7620 3d20 522e 5420 4020 746f 7263  cov = R.T @ torc
+0000c050: 682e 6c69 6e61 6c67 2e70 696e 7628 412c  h.linalg.pinv(A,
+0000c060: 2068 6572 6d69 7469 616e 3d54 7275 652c   hermitian=True,
+0000c070: 2072 746f 6c3d 3165 2d38 2920 4020 520a   rtol=1e-8) @ R.
+0000c080: 0a20 2020 2020 2020 2020 2020 2046 5f63  .            F_c
+0000c090: 6f76 203d 2046 5f63 6f76 5b73 656c 662e  ov = F_cov[self.
+0000c0a0: 4d20 3a2c 2073 656c 662e 4d20 3a5d 0a20  M :, self.M :]. 
+0000c0b0: 2020 2020 2020 2020 2020 2046 5f73 7464             F_std
+0000c0c0: 203d 2046 5f63 6f76 2e64 6961 676f 6e61   = F_cov.diagona
+0000c0d0: 6c28 292e 7371 7274 2829 0a0a 2020 2020  l().sqrt()..    
+0000c0e0: 2020 2020 2020 2020 4465 6c74 6146 203d          DeltaF =
+0000c0f0: 2046 5b4e 6f6e 652c 203a 5d20 2d20 465b   F[None, :] - F[
+0000c100: 3a2c 204e 6f6e 655d 0a20 2020 2020 2020  :, None].       
+0000c110: 2020 2020 2044 656c 7461 465f 636f 7620       DeltaF_cov 
+0000c120: 3d20 465f 636f 762e 6469 6167 2829 5b3a  = F_cov.diag()[:
+0000c130: 2c20 4e6f 6e65 5d20 2b20 465f 636f 762e  , None] + F_cov.
+0000c140: 6469 6167 2829 5b4e 6f6e 652c 203a 5d20  diag()[None, :] 
+0000c150: 2d20 3220 2a20 465f 636f 760a 2020 2020  - 2 * F_cov.    
+0000c160: 2020 2020 2020 2020 4465 6c74 6146 5f73          DeltaF_s
+0000c170: 7464 203d 2044 656c 7461 465f 636f 762e  td = DeltaF_cov.
+0000c180: 7371 7274 2829 0a20 2020 2020 2020 2065  sqrt().        e
+0000c190: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000c1a0: 2046 5f6c 6973 7420 3d20 5b5d 0a20 2020   F_list = [].   
+0000c1b0: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
+0000c1c0: 6e20 7261 6e67 6528 7365 6c66 2e62 6f6f  n range(self.boo
+0000c1d0: 7473 7472 6170 5f6e 756d 5f72 6570 293a  tstrap_num_rep):
+0000c1e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c1f0: 2064 7520 3d20 656e 6572 6779 5f70 6572   du = energy_per
+0000c200: 7475 7262 6564 5b3a 2c20 7365 6c66 2e5f  turbed[:, self._
+0000c210: 636f 6e66 5f69 6478 5b6b 5d5d 202b 2073  conf_idx[k]] + s
+0000c220: 656c 662e 5f6c 6f67 5f70 726f 625f 6d69  elf._log_prob_mi
+0000c230: 785b 6b5d 0a20 2020 2020 2020 2020 2020  x[k].           
+0000c240: 2020 2020 2046 203d 202d 746f 7263 682e       F = -torch.
+0000c250: 6c6f 6773 756d 6578 7028 2d64 752c 2064  logsumexp(-du, d
+0000c260: 696d 3d31 290a 2020 2020 2020 2020 2020  im=1).          
+0000c270: 2020 2020 2020 465f 6c69 7374 2e61 7070        F_list.app
+0000c280: 656e 6428 4629 0a20 2020 2020 2020 2020  end(F).         
+0000c290: 2020 2046 5f6c 6973 7420 3d20 746f 7263     F_list = torc
+0000c2a0: 682e 7374 6163 6b28 465f 6c69 7374 2c20  h.stack(F_list, 
+0000c2b0: 6469 6d3d 3129 0a20 2020 2020 2020 2020  dim=1).         
+0000c2c0: 2020 2046 203d 2074 6f72 6368 2e6d 6561     F = torch.mea
+0000c2d0: 6e28 465f 6c69 7374 2c20 6469 6d3d 3129  n(F_list, dim=1)
+0000c2e0: 0a20 2020 2020 2020 2020 2020 2046 5f73  .            F_s
+0000c2f0: 7464 203d 2074 6f72 6368 2e73 7464 2846  td = torch.std(F
+0000c300: 5f6c 6973 742c 2064 696d 3d31 290a 2020  _list, dim=1).  
+0000c310: 2020 2020 2020 2020 2020 465f 636f 7620            F_cov 
+0000c320: 3d20 746f 7263 682e 636f 7628 465f 6c69  = torch.cov(F_li
+0000c330: 7374 290a 0a20 2020 2020 2020 2020 2020  st)..           
+0000c340: 2044 656c 7461 4620 3d20 465b 4e6f 6e65   DeltaF = F[None
+0000c350: 2c20 3a5d 202d 2046 5b3a 2c20 4e6f 6e65  , :] - F[:, None
+0000c360: 5d0a 2020 2020 2020 2020 2020 2020 4465  ].            De
+0000c370: 6c74 6146 5f73 7464 203d 2074 6f72 6368  ltaF_std = torch
+0000c380: 2e73 7464 2846 5f6c 6973 745b 3a2c 203a  .std(F_list[:, :
+0000c390: 2c20 4e6f 6e65 5d20 2d20 465f 6c69 7374  , None] - F_list
+0000c3a0: 5b3a 2c20 4e6f 6e65 2c20 3a5d 2c20 6469  [:, None, :], di
+0000c3b0: 6d3d 3129 0a0a 2020 2020 2020 2020 7265  m=1)..        re
+0000c3c0: 7375 6c74 7320 3d20 7b0a 2020 2020 2020  sults = {.      
+0000c3d0: 2020 2020 2020 2246 223a 2046 2e6e 756d        "F": F.num
+0000c3e0: 7079 2829 2c0a 2020 2020 2020 2020 2020  py(),.          
+0000c3f0: 2020 2246 5f73 7464 223a 2046 5f73 7464    "F_std": F_std
+0000c400: 2e6e 756d 7079 2829 2c0a 2020 2020 2020  .numpy(),.      
+0000c410: 2020 2020 2020 2246 5f63 6f76 223a 2046        "F_cov": F
+0000c420: 5f63 6f76 2e6e 756d 7079 2829 2c0a 2020  _cov.numpy(),.  
+0000c430: 2020 2020 2020 2020 2020 2244 656c 7461            "Delta
+0000c440: 4622 3a20 4465 6c74 6146 2e6e 756d 7079  F": DeltaF.numpy
+0000c450: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+0000c460: 2244 656c 7461 465f 7374 6422 3a20 4465  "DeltaF_std": De
+0000c470: 6c74 6146 5f73 7464 2e6e 756d 7079 2829  ltaF_std.numpy()
+0000c480: 2c0a 2020 2020 2020 2020 7d0a 0a20 2020  ,.        }..   
+0000c490: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+0000c4a0: 6c74 730a 0a64 6566 205f 636f 6d70 7574  lts..def _comput
+0000c4b0: 655f 6c6f 6770 5f6f 665f 4628 462c 2065  e_logp_of_F(F, e
+0000c4c0: 6e65 7267 792c 206e 756d 5f63 6f6e 6629  nergy, num_conf)
+0000c4d0: 3a0a 2020 2020 6c6f 6770 203d 2028 0a20  :.    logp = (. 
+0000c4e0: 2020 2020 2020 2074 6f72 6368 2e73 756d         torch.sum
+0000c4f0: 286e 756d 5f63 6f6e 6620 2a20 4629 0a20  (num_conf * F). 
+0000c500: 2020 2020 2020 202d 2074 6f72 6368 2e6c         - torch.l
+0000c510: 6f67 7375 6d65 7870 282d 2865 6e65 7267  ogsumexp(-(energ
+0000c520: 792e 5420 2d20 746f 7263 682e 6c6f 6728  y.T - torch.log(
+0000c530: 6e75 6d5f 636f 6e66 2920 2d20 4629 2c20  num_conf) - F), 
+0000c540: 6469 6d3d 3129 2e73 756d 2829 0a20 2020  dim=1).sum().   
+0000c550: 2029 0a20 2020 2072 6574 7572 6e20 6c6f   ).    return lo
+0000c560: 6770 0a0a 0a64 6566 205f 636f 6d70 7574  gp...def _comput
+0000c570: 655f 6c6f 7373 5f61 6e64 5f67 7261 645f  e_loss_and_grad_
+0000c580: 6f66 5f64 4628 6446 2c20 656e 6572 6779  of_dF(dF, energy
+0000c590: 2c20 6e75 6d5f 636f 6e66 293a 0a20 2020  , num_conf):.   
+0000c5a0: 2022 2222 436f 6d70 7574 6520 7468 6520   """Compute the 
+0000c5b0: 6c6f 7373 2066 756e 6374 696f 6e20 616e  loss function an
+0000c5c0: 6420 7468 6520 6772 6164 6965 6e74 206f  d the gradient o
+0000c5d0: 6620 6446 2067 6976 656e 2065 6e65 7267  f dF given energ
+0000c5e0: 7920 616e 6420 6e75 6d5f 636f 6e66 2e0a  y and num_conf..
+0000c5f0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000c600: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0000c610: 2020 6446 3a20 312d 4420 666c 6f61 7420    dF: 1-D float 
+0000c620: 7465 6e73 6f72 2077 6974 6820 7369 7a65  tensor with size
+0000c630: 2028 4d2d 3129 0a20 2020 2020 2020 2054   (M-1).        T
+0000c640: 6865 2066 7265 6520 656e 6572 6779 2064  he free energy d
+0000c650: 6966 6665 7265 6e63 6520 6265 7477 6565  ifference betwee
+0000c660: 6e20 7374 6174 6520 3020 616e 6420 6f74  n state 0 and ot
+0000c670: 6865 7220 7374 6174 6573 2e20 5468 6520  her states. The 
+0000c680: 656e 7472 790a 2020 2020 2020 2020 6446  entry.        dF
+0000c690: 5b69 5d20 6973 2074 6865 2066 7265 6520  [i] is the free 
+0000c6a0: 656e 6572 6779 2064 6966 6665 7265 6e63  energy differenc
+0000c6b0: 6520 6265 7477 6565 6e20 7374 6174 6520  e between state 
+0000c6c0: 3020 616e 6420 7374 6174 6520 692b 312e  0 and state i+1.
+0000c6d0: 0a20 2020 2065 6e65 7267 793a 2032 2d44  .    energy: 2-D
+0000c6e0: 2066 6c6f 6174 2074 656e 736f 7220 7769   float tensor wi
+0000c6f0: 7468 2073 697a 6520 284d 2078 204e 290a  th size (M x N).
+0000c700: 2020 2020 2020 2020 4120 322d 4420 7465          A 2-D te
+0000c710: 6e73 6f72 2077 6974 6820 7369 7a65 206f  nsor with size o
+0000c720: 6620 4d20 7820 4e2c 2077 6865 7265 204d  f M x N, where M
+0000c730: 2069 7320 7468 6520 6e75 6d62 6572 206f   is the number o
+0000c740: 6620 7374 6174 730a 2020 2020 2020 2020  f stats.        
+0000c750: 616e 6420 4e20 6973 2074 6865 2074 6f74  and N is the tot
+0000c760: 616c 206e 756d 6265 7220 6f66 2063 6f6e  al number of con
+0000c770: 666f 726d 6174 696f 6e73 2e20 5468 6520  formations. The 
+0000c780: 656e 7472 7920 656e 6572 6779 5b69 2c6a  entry energy[i,j
+0000c790: 5d0a 2020 2020 6e75 6d5f 636f 6e66 3a20  ].    num_conf: 
+0000c7a0: 312d 4420 696e 7420 7465 6e73 6f72 2077  1-D int tensor w
+0000c7b0: 6974 6820 7369 7a65 2028 4d29 0a20 2020  ith size (M).   
+0000c7c0: 2020 2020 2041 2031 2d44 2074 656e 736f       A 1-D tenso
+0000c7d0: 7220 7769 7468 2073 697a 6520 6f66 204d  r with size of M
+0000c7e0: 2c20 7768 6572 6520 6e75 6d5f 636f 6e66  , where num_conf
+0000c7f0: 5b69 5d20 6973 2074 6865 206e 756d 206f  [i] is the num o
+0000c800: 660a 2020 2020 2020 2020 636f 6e66 6f72  f.        confor
+0000c810: 6d61 7469 6f6e 7320 7361 6d70 6c65 6420  mations sampled 
+0000c820: 6672 6f6d 2073 7461 7465 2069 2e20 5468  from state i. Th
+0000c830: 6572 6566 6f72 652c 2074 6f72 6368 2e73  erefore, torch.s
+0000c840: 756d 286e 756d 5f63 6f6e 6629 0a20 2020  um(num_conf).   
+0000c850: 2020 2020 2068 6173 2074 6f20 6265 2065       has to be e
+0000c860: 7175 616c 2074 6f20 4e2e 2041 6c6c 2065  qual to N. All e
+0000c870: 6e74 7269 6573 2069 6e20 6e75 6d5f 636f  ntries in num_co
+0000c880: 6e66 2068 6176 6520 746f 2062 6520 7374  nf have to be st
+0000c890: 7269 6374 6c79 0a20 2020 2020 2020 2067  rictly.        g
+0000c8a0: 7265 6174 6572 2074 6861 6e20 302e 0a20  reater than 0.. 
+0000c8b0: 2020 2022 2222 0a0a 2020 2020 2320 636f     """..    # co
+0000c8c0: 6d70 7574 6520 7468 6520 6c6f 7373 2066  mpute the loss f
+0000c8d0: 756e 6374 696f 6e0a 2020 2020 4620 3d20  unction.    F = 
+0000c8e0: 746f 7263 682e 6361 7428 5b64 462e 6e65  torch.cat([dF.ne
+0000c8f0: 775f 7a65 726f 7328 3129 2c20 6446 5d29  w_zeros(1), dF])
+0000c900: 0a20 2020 206c 6f67 7020 3d20 5f63 6f6d  .    logp = _com
+0000c910: 7075 7465 5f6c 6f67 705f 6f66 5f46 2846  pute_logp_of_F(F
+0000c920: 2c20 656e 6572 6779 2c20 6e75 6d5f 636f  , energy, num_co
+0000c930: 6e66 290a 2020 2020 6c6f 7373 203d 202d  nf).    loss = -
+0000c940: 6c6f 6770 202f 206e 756d 5f63 6f6e 662e  logp / num_conf.
+0000c950: 7375 6d28 290a 2020 2020 7520 3d20 656e  sum().    u = en
+0000c960: 6572 6779 202d 2046 5b3a 2c20 4e6f 6e65  ergy - F[:, None
+0000c970: 5d20 2d20 746f 7263 682e 6c6f 6728 6e75  ] - torch.log(nu
+0000c980: 6d5f 636f 6e66 295b 3a2c 204e 6f6e 655d  m_conf)[:, None]
+0000c990: 0a0a 2020 2020 2320 636f 6d70 7574 6520  ..    # compute 
+0000c9a0: 7468 6520 6772 6164 6965 6e74 206f 6620  the gradient of 
+0000c9b0: 7468 6520 6c6f 7373 2066 756e 6374 696f  the loss functio
+0000c9c0: 6e0a 2020 2020 7020 3d20 746f 7263 682e  n.    p = torch.
+0000c9d0: 736f 6674 6d61 7828 2d75 2c20 6469 6d3d  softmax(-u, dim=
+0000c9e0: 3029 0a20 2020 2067 7261 6420 3d20 746f  0).    grad = to
+0000c9f0: 7263 682e 6d65 616e 2870 2c20 6469 6d3d  rch.mean(p, dim=
+0000ca00: 3129 202d 206e 756d 5f63 6f6e 6620 2f20  1) - num_conf / 
+0000ca10: 6e75 6d5f 636f 6e66 2e73 756d 2829 0a20  num_conf.sum(). 
+0000ca20: 2020 2067 7261 6420 3d20 6772 6164 5b31     grad = grad[1
+0000ca30: 3a5d 0a0a 2020 2020 7265 7475 726e 206c  :]..    return l
+0000ca40: 6f73 732c 2067 7261 640a 0a0a 6465 6620  oss, grad...def 
+0000ca50: 5f63 6f6d 7075 7465 5f6c 6f73 735f 616e  _compute_loss_an
+0000ca60: 645f 6772 6164 5f6f 665f 6446 5f69 6e5f  d_grad_of_dF_in_
+0000ca70: 6261 7463 6828 6446 2c20 656e 6572 6779  batch(dF, energy
+0000ca80: 2c20 6e75 6d5f 636f 6e66 2c20 6261 7463  , num_conf, batc
+0000ca90: 685f 7369 7a65 3a20 696e 7429 3a0a 2020  h_size: int):.  
+0000caa0: 2020 2222 2254 6869 7320 6973 2074 6865    """This is the
+0000cab0: 2062 6174 6368 2076 6572 7369 6f6e 206f   batch version o
+0000cac0: 6620 5f63 6f6d 7075 7465 5f6c 6f73 735f  f _compute_loss_
+0000cad0: 616e 645f 6772 6164 5f6f 665f 6446 2e0a  and_grad_of_dF..
+0000cae0: 2020 2020 5468 6520 6261 7463 6820 7665      The batch ve
+0000caf0: 7273 696f 6e20 6973 2075 7365 6420 7768  rsion is used wh
+0000cb00: 656e 2074 6865 2073 697a 6520 6f66 2065  en the size of e
+0000cb10: 6e65 7267 7920 6973 2074 6f6f 206c 6172  nergy is too lar
+0000cb20: 6765 2074 6f20 6669 7420 696e 746f 2074  ge to fit into t
+0000cb30: 6865 0a20 2020 206d 656d 6f72 7920 6f66  he.    memory of
+0000cb40: 2061 2047 5055 2e20 5468 6520 656e 6572   a GPU. The ener
+0000cb50: 6779 206d 6174 7269 7820 6973 2073 706c  gy matrix is spl
+0000cb60: 6974 2069 6e74 6f20 6d75 6c74 6970 6c65  it into multiple
+0000cb70: 2062 6174 6368 6573 2061 6e64 2074 6865   batches and the
+0000cb80: 0a20 2020 2063 616c 6375 6c61 7469 6f6e  .    calculation
+0000cb90: 2069 7320 646f 6e65 2073 6571 7565 6e74   is done sequent
+0000cba0: 6961 6c6c 792e 0a0a 2020 2020 5468 6520  ially...    The 
+0000cbb0: 7061 7261 6d65 7465 7273 2061 7265 2074  parameters are t
+0000cbc0: 6865 2073 616d 6520 6173 205f 636f 6d70  he same as _comp
+0000cbd0: 7574 655f 6c6f 7373 5f61 6e64 5f67 7261  ute_loss_and_gra
+0000cbe0: 645f 6f66 5f64 462e 0a20 2020 2022 2222  d_of_dF..    """
+0000cbf0: 0a0a 2020 2020 6e20 3d20 6e75 6d5f 636f  ..    n = num_co
+0000cc00: 6e66 0a20 2020 204e 203d 2074 6f72 6368  nf.    N = torch
+0000cc10: 2e73 756d 286e 290a 2020 2020 6e5f 6f76  .sum(n).    n_ov
+0000cc20: 6572 5f4e 203d 206e 202f 204e 0a0a 2020  er_N = n / N..  
+0000cc30: 2020 6966 2065 6e65 7267 792e 7368 6170    if energy.shap
+0000cc40: 655b 315d 2025 2062 6174 6368 5f73 697a  e[1] % batch_siz
+0000cc50: 6520 3d3d 2030 3a0a 2020 2020 2020 2020  e == 0:.        
+0000cc60: 6e75 6d5f 6261 7463 6820 3d20 656e 6572  num_batch = ener
+0000cc70: 6779 2e73 6861 7065 5b31 5d20 2f2f 2062  gy.shape[1] // b
+0000cc80: 6174 6368 5f73 697a 650a 2020 2020 656c  atch_size.    el
+0000cc90: 7365 3a0a 2020 2020 2020 2020 6e75 6d5f  se:.        num_
+0000cca0: 6261 7463 6820 3d20 656e 6572 6779 2e73  batch = energy.s
+0000ccb0: 6861 7065 5b31 5d20 2f2f 2062 6174 6368  hape[1] // batch
+0000ccc0: 5f73 697a 6520 2b20 310a 0a20 2020 2046  _size + 1..    F
+0000ccd0: 203d 2074 6f72 6368 2e63 6174 285b 6446   = torch.cat([dF
+0000cce0: 2e6e 6577 5f7a 6572 6f73 2831 292c 2064  .new_zeros(1), d
+0000ccf0: 465d 290a 2020 2020 6c6f 7373 203d 202d  F]).    loss = -
+0000cd00: 746f 7263 682e 7375 6d28 6e75 6d5f 636f  torch.sum(num_co
+0000cd10: 6e66 202a 2046 290a 2020 2020 6772 6164  nf * F).    grad
+0000cd20: 203d 202d 6e75 6d5f 636f 6e66 0a0a 2020   = -num_conf..  
+0000cd30: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+0000cd40: 286e 756d 5f62 6174 6368 293a 0a20 2020  (num_batch):.   
+0000cd50: 2020 2020 2065 6e65 7267 795f 6261 7463       energy_batc
+0000cd60: 6820 3d20 656e 6572 6779 5b3a 2c20 6920  h = energy[:, i 
+0000cd70: 2a20 6261 7463 685f 7369 7a65 203a 2028  * batch_size : (
+0000cd80: 6920 2b20 3129 202a 2062 6174 6368 5f73  i + 1) * batch_s
+0000cd90: 697a 655d 0a20 2020 2020 2020 2075 203d  ize].        u =
+0000cda0: 2065 6e65 7267 795f 6261 7463 682e 6375   energy_batch.cu
+0000cdb0: 6461 2829 202d 2074 6f72 6368 2e6c 6f67  da() - torch.log
+0000cdc0: 286e 756d 5f63 6f6e 6629 5b3a 2c20 4e6f  (num_conf)[:, No
+0000cdd0: 6e65 5d20 2d20 465b 3a2c 204e 6f6e 655d  ne] - F[:, None]
+0000cde0: 0a20 2020 2020 2020 206c 6f73 7320 2b3d  .        loss +=
+0000cdf0: 2074 6f72 6368 2e6c 6f67 7375 6d65 7870   torch.logsumexp
+0000ce00: 282d 752c 2064 696d 3d30 292e 7375 6d28  (-u, dim=0).sum(
+0000ce10: 290a 0a20 2020 2020 2020 2070 203d 2074  )..        p = t
+0000ce20: 6f72 6368 2e73 6f66 746d 6178 282d 752c  orch.softmax(-u,
+0000ce30: 2064 696d 3d30 290a 2020 2020 2020 2020   dim=0).        
+0000ce40: 6772 6164 202b 3d20 746f 7263 682e 7375  grad += torch.su
+0000ce50: 6d28 702c 2064 696d 3d31 290a 0a20 2020  m(p, dim=1)..   
+0000ce60: 206c 6f73 7320 3d20 6c6f 7373 202f 204e   loss = loss / N
+0000ce70: 0a20 2020 2067 7261 6420 3d20 6772 6164  .    grad = grad
+0000ce80: 202f 204e 0a20 2020 2067 7261 6420 3d20   / N.    grad = 
+0000ce90: 6772 6164 5b31 3a5d 0a20 2020 2072 6574  grad[1:].    ret
+0000cea0: 7572 6e20 6c6f 7373 2c20 6772 6164 0a0a  urn loss, grad..
+0000ceb0: 0a64 6566 205f 636f 6d70 7574 655f 6865  .def _compute_he
+0000cec0: 7373 6961 6e5f 6c6f 675f 6c69 6b65 6c69  ssian_log_likeli
+0000ced0: 686f 6f64 5f6f 665f 4628 462c 2065 6e65  hood_of_F(F, ene
+0000cee0: 7267 792c 206e 756d 5f63 6f6e 6629 3a0a  rgy, num_conf):.
+0000cef0: 2020 2020 7520 3d20 656e 6572 6779 202d      u = energy -
+0000cf00: 2046 5b3a 2c20 4e6f 6e65 5d20 2d20 746f   F[:, None] - to
+0000cf10: 7263 682e 6c6f 6728 6e75 6d5f 636f 6e66  rch.log(num_conf
+0000cf20: 295b 3a2c 204e 6f6e 655d 0a20 2020 2070  )[:, None].    p
+0000cf30: 203d 2074 6f72 6368 2e73 6f66 746d 6178   = torch.softmax
+0000cf40: 282d 752c 2064 696d 3d30 290a 2020 2020  (-u, dim=0).    
+0000cf50: 7070 203d 2074 6f72 6368 2e6d 6174 6d75  pp = torch.matmu
+0000cf60: 6c28 702c 2070 2e54 290a 2020 2020 4820  l(p, p.T).    H 
+0000cf70: 3d20 7070 202d 2074 6f72 6368 2e64 6961  = pp - torch.dia
+0000cf80: 6728 746f 7263 682e 7375 6d28 702c 2031  g(torch.sum(p, 1
+0000cf90: 2929 0a20 2020 2072 6574 7572 6e20 480a  )).    return H.
+0000cfa0: 0a0a 6465 6620 5f63 6f6d 7075 7465 5f68  ..def _compute_h
+0000cfb0: 6573 7369 616e 5f6c 6f67 5f6c 696b 656c  essian_log_likel
+0000cfc0: 6968 6f6f 645f 6f66 5f46 5f69 6e5f 6261  ihood_of_F_in_ba
+0000cfd0: 7463 6828 462c 2065 6e65 7267 792c 206e  tch(F, energy, n
+0000cfe0: 756d 5f63 6f6e 662c 2062 6174 6368 5f73  um_conf, batch_s
+0000cff0: 697a 653a 2069 6e74 293a 0a20 2020 2069  ize: int):.    i
+0000d000: 6620 656e 6572 6779 2e73 6861 7065 5b31  f energy.shape[1
+0000d010: 5d20 2520 6261 7463 685f 7369 7a65 203d  ] % batch_size =
+0000d020: 3d20 303a 0a20 2020 2020 2020 206e 756d  = 0:.        num
+0000d030: 5f62 6174 6368 203d 2065 6e65 7267 792e  _batch = energy.
+0000d040: 7368 6170 655b 315d 202f 2f20 6261 7463  shape[1] // batc
+0000d050: 685f 7369 7a65 0a20 2020 2065 6c73 653a  h_size.    else:
+0000d060: 0a20 2020 2020 2020 206e 756d 5f62 6174  .        num_bat
+0000d070: 6368 203d 2065 6e65 7267 792e 7368 6170  ch = energy.shap
+0000d080: 655b 315d 202f 2f20 6261 7463 685f 7369  e[1] // batch_si
+0000d090: 7a65 202b 2031 0a0a 2020 2020 4820 3d20  ze + 1..    H = 
+0000d0a0: 462e 6e65 775f 7a65 726f 7328 2846 2e73  F.new_zeros((F.s
+0000d0b0: 6861 7065 5b30 5d2c 2046 2e73 6861 7065  hape[0], F.shape
+0000d0c0: 5b30 5d29 292e 6375 6461 2829 0a20 2020  [0])).cuda().   
+0000d0d0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+0000d0e0: 6e75 6d5f 6261 7463 6829 3a0a 2020 2020  num_batch):.    
+0000d0f0: 2020 2020 656e 6572 6779 5f62 6174 6368      energy_batch
+0000d100: 203d 2065 6e65 7267 795b 3a2c 2069 202a   = energy[:, i *
+0000d110: 2062 6174 6368 5f73 697a 6520 3a20 2869   batch_size : (i
+0000d120: 202b 2031 2920 2a20 6261 7463 685f 7369   + 1) * batch_si
+0000d130: 7a65 5d0a 2020 2020 2020 2020 7520 3d20  ze].        u = 
+0000d140: 656e 6572 6779 5f62 6174 6368 2e63 7564  energy_batch.cud
+0000d150: 6128 2920 2d20 465b 3a2c 204e 6f6e 655d  a() - F[:, None]
+0000d160: 202d 2074 6f72 6368 2e6c 6f67 286e 756d   - torch.log(num
+0000d170: 5f63 6f6e 6629 5b3a 2c20 4e6f 6e65 5d0a  _conf)[:, None].
+0000d180: 0a20 2020 2020 2020 2070 203d 2074 6f72  .        p = tor
+0000d190: 6368 2e73 6f66 746d 6178 282d 752c 2064  ch.softmax(-u, d
+0000d1a0: 696d 3d30 290a 2020 2020 2020 2020 7070  im=0).        pp
+0000d1b0: 203d 2074 6f72 6368 2e6d 6174 6d75 6c28   = torch.matmul(
+0000d1c0: 702c 2070 2e54 290a 2020 2020 2020 2020  p, p.T).        
+0000d1d0: 4820 2b3d 2070 7020 2d20 746f 7263 682e  H += pp - torch.
+0000d1e0: 6469 6167 2874 6f72 6368 2e73 756d 2870  diag(torch.sum(p
+0000d1f0: 2c20 3129 290a 0a20 2020 2072 6574 7572  , 1))..    retur
+0000d200: 6e20 480a 0a0a 6465 6620 5f63 6f6d 7075  n H...def _compu
+0000d210: 7465 5f68 6573 7369 616e 5f6c 6f73 735f  te_hessian_loss_
+0000d220: 6f66 5f64 4628 6446 2c20 656e 6572 6779  of_dF(dF, energy
+0000d230: 2c20 6e75 6d5f 636f 6e66 293a 0a20 2020  , num_conf):.   
+0000d240: 204e 203d 2074 6f72 6368 2e73 756d 286e   N = torch.sum(n
+0000d250: 756d 5f63 6f6e 6629 0a20 2020 2046 203d  um_conf).    F =
+0000d260: 2074 6f72 6368 2e63 6174 285b 6446 2e6e   torch.cat([dF.n
+0000d270: 6577 5f7a 6572 6f73 2831 292c 2064 465d  ew_zeros(1), dF]
+0000d280: 290a 2020 2020 4820 3d20 5f63 6f6d 7075  ).    H = _compu
+0000d290: 7465 5f68 6573 7369 616e 5f6c 6f67 5f6c  te_hessian_log_l
+0000d2a0: 696b 656c 6968 6f6f 645f 6f66 5f46 2846  ikelihood_of_F(F
+0000d2b0: 2c20 656e 6572 6779 2c20 6e75 6d5f 636f  , energy, num_co
+0000d2c0: 6e66 290a 2020 2020 4820 3d20 2d48 5b31  nf).    H = -H[1
+0000d2d0: 3a2c 2031 3a5d 202f 204e 0a20 2020 2072  :, 1:] / N.    r
+0000d2e0: 6574 7572 6e20 480a 0a0a 6465 6620 5f63  eturn H...def _c
+0000d2f0: 6f6d 7075 7465 5f68 6573 7369 616e 5f6c  ompute_hessian_l
+0000d300: 6f73 735f 6f66 5f64 465f 696e 5f62 6174  oss_of_dF_in_bat
+0000d310: 6368 2864 462c 2065 6e65 7267 792c 206e  ch(dF, energy, n
+0000d320: 756d 5f63 6f6e 662c 2062 6174 6368 5f73  um_conf, batch_s
+0000d330: 697a 653a 2069 6e74 293a 0a20 2020 204e  ize: int):.    N
+0000d340: 203d 2074 6f72 6368 2e73 756d 286e 756d   = torch.sum(num
+0000d350: 5f63 6f6e 6629 0a20 2020 2046 203d 2074  _conf).    F = t
+0000d360: 6f72 6368 2e63 6174 285b 6446 2e6e 6577  orch.cat([dF.new
+0000d370: 5f7a 6572 6f73 2831 292c 2064 465d 290a  _zeros(1), dF]).
+0000d380: 2020 2020 4820 3d20 5f63 6f6d 7075 7465      H = _compute
+0000d390: 5f68 6573 7369 616e 5f6c 6f67 5f6c 696b  _hessian_log_lik
+0000d3a0: 656c 6968 6f6f 645f 6f66 5f46 5f69 6e5f  elihood_of_F_in_
+0000d3b0: 6261 7463 6828 462c 2065 6e65 7267 792c  batch(F, energy,
+0000d3c0: 206e 756d 5f63 6f6e 662c 2062 6174 6368   num_conf, batch
+0000d3d0: 5f73 697a 6529 0a20 2020 2048 203d 202d  _size).    H = -
+0000d3e0: 485b 313a 2c20 313a 5d20 2f20 4e0a 2020  H[1:, 1:] / N.  
+0000d3f0: 2020 7265 7475 726e 2048 0a0a 0a64 6566    return H...def
+0000d400: 205f 736f 6c76 655f 6d62 6172 2864 465f   _solve_mbar(dF_
+0000d410: 696e 6974 2c20 656e 6572 6779 2c20 6e75  init, energy, nu
+0000d420: 6d5f 636f 6e66 2c20 6d65 7468 6f64 2c20  m_conf, method, 
+0000d430: 6261 7463 685f 7369 7a65 3d4e 6f6e 652c  batch_size=None,
+0000d440: 2076 6572 626f 7365 3d46 616c 7365 293a   verbose=False):
+0000d450: 0a20 2020 2069 6620 6261 7463 685f 7369  .    if batch_si
+0000d460: 7a65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ze is not None:.
+0000d470: 2020 2020 2020 2020 6966 206d 6574 686f          if metho
+0000d480: 6420 3d3d 2022 4e65 7774 6f6e 223a 0a20  d == "Newton":. 
+0000d490: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0000d4a0: 7473 203d 2066 6d69 6e5f 6e65 7774 6f6e  ts = fmin_newton
+0000d4b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000d4c0: 2020 663d 5f63 6f6d 7075 7465 5f6c 6f73    f=_compute_los
+0000d4d0: 735f 616e 645f 6772 6164 5f6f 665f 6446  s_and_grad_of_dF
+0000d4e0: 5f69 6e5f 6261 7463 682c 0a20 2020 2020  _in_batch,.     
+0000d4f0: 2020 2020 2020 2020 2020 2068 6573 733d             hess=
+0000d500: 5f63 6f6d 7075 7465 5f68 6573 7369 616e  _compute_hessian
+0000d510: 5f6c 6f73 735f 6f66 5f64 465f 696e 5f62  _loss_of_dF_in_b
+0000d520: 6174 6368 2c0a 2020 2020 2020 2020 2020  atch,.          
+0000d530: 2020 2020 2020 785f 696e 6974 3d64 465f        x_init=dF_
+0000d540: 696e 6974 2c0a 2020 2020 2020 2020 2020  init,.          
+0000d550: 2020 2020 2020 6172 6773 3d28 656e 6572        args=(ener
+0000d560: 6779 2c20 6e75 6d5f 636f 6e66 2c20 6261  gy, num_conf, ba
+0000d570: 7463 685f 7369 7a65 292c 0a20 2020 2020  tch_size),.     
+0000d580: 2020 2020 2020 2020 2020 2076 6572 626f             verbo
+0000d590: 7365 3d76 6572 626f 7365 2c0a 2020 2020  se=verbose,.    
+0000d5a0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000d5b0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0000d5c0: 756c 7473 5b22 7822 5d0a 0a20 2020 2020  ults["x"]..     
+0000d5d0: 2020 2065 6c69 6620 6d65 7468 6f64 203d     elif method =
+0000d5e0: 3d20 224c 2d42 4647 532d 4222 3a0a 2020  = "L-BFGS-B":.  
+0000d5f0: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
+0000d600: 7320 3d20 7b22 6469 7370 223a 2076 6572  s = {"disp": ver
+0000d610: 626f 7365 2c20 2267 746f 6c22 3a20 3165  bose, "gtol": 1e
+0000d620: 2d38 7d0a 2020 2020 2020 2020 2020 2020  -8}.            
+0000d630: 7265 7375 6c74 7320 3d20 6f70 7469 6d69  results = optimi
+0000d640: 7a65 2e6d 696e 696d 697a 6528 0a20 2020  ze.minimize(.   
+0000d650: 2020 2020 2020 2020 2020 2020 206c 616d               lam
+0000d660: 6264 6120 783a 205b 0a20 2020 2020 2020  bda x: [.       
+0000d670: 2020 2020 2020 2020 2020 2020 2072 2e63               r.c
+0000d680: 7075 2829 2e6e 756d 7079 2829 0a20 2020  pu().numpy().   
+0000d690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6a0: 2066 6f72 2072 2069 6e20 5f63 6f6d 7075   for r in _compu
+0000d6b0: 7465 5f6c 6f73 735f 616e 645f 6772 6164  te_loss_and_grad
+0000d6c0: 5f6f 665f 6446 5f69 6e5f 6261 7463 6828  _of_dF_in_batch(
+0000d6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d6e0: 2020 2020 2020 2020 2065 6e65 7267 792e           energy.
+0000d6f0: 6e65 775f 7465 6e73 6f72 2878 292c 2065  new_tensor(x), e
+0000d700: 6e65 7267 792c 206e 756d 5f63 6f6e 662c  nergy, num_conf,
+0000d710: 2062 6174 6368 5f73 697a 650a 2020 2020   batch_size.    
+0000d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d730: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000d740: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
+0000d750: 2020 2020 2064 465f 696e 6974 2e63 7075       dF_init.cpu
+0000d760: 2829 2e6e 756d 7079 2829 2c0a 2020 2020  ().numpy(),.    
+0000d770: 2020 2020 2020 2020 2020 2020 6a61 633d              jac=
+0000d780: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+0000d790: 2020 2020 2020 6d65 7468 6f64 3d22 4c2d        method="L-
+0000d7a0: 4246 4753 2d42 222c 0a20 2020 2020 2020  BFGS-B",.       
+0000d7b0: 2020 2020 2020 2020 2074 6f6c 3d31 652d           tol=1e-
+0000d7c0: 3132 2c0a 2020 2020 2020 2020 2020 2020  12,.            
+0000d7d0: 2020 2020 6f70 7469 6f6e 733d 6f70 7469      options=opti
+0000d7e0: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
+0000d7f0: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
+0000d800: 6574 7572 6e20 746f 7263 682e 6672 6f6d  eturn torch.from
+0000d810: 5f6e 756d 7079 2872 6573 756c 7473 5b22  _numpy(results["
+0000d820: 7822 5d29 0a20 2020 2065 6c73 653a 0a20  x"]).    else:. 
+0000d830: 2020 2020 2020 2069 6620 6d65 7468 6f64         if method
+0000d840: 203d 3d20 224e 6577 746f 6e22 3a0a 2020   == "Newton":.  
+0000d850: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000d860: 7320 3d20 666d 696e 5f6e 6577 746f 6e28  s = fmin_newton(
+0000d870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d880: 2066 3d5f 636f 6d70 7574 655f 6c6f 7373   f=_compute_loss
+0000d890: 5f61 6e64 5f67 7261 645f 6f66 5f64 462c  _and_grad_of_dF,
+0000d8a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d8b0: 2068 6573 733d 5f63 6f6d 7075 7465 5f68   hess=_compute_h
+0000d8c0: 6573 7369 616e 5f6c 6f73 735f 6f66 5f64  essian_loss_of_d
+0000d8d0: 462c 0a20 2020 2020 2020 2020 2020 2020  F,.             
+0000d8e0: 2020 2078 5f69 6e69 743d 6446 5f69 6e69     x_init=dF_ini
+0000d8f0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+0000d900: 2020 2061 7267 733d 2865 6e65 7267 792c     args=(energy,
+0000d910: 206e 756d 5f63 6f6e 6629 2c0a 2020 2020   num_conf),.    
+0000d920: 2020 2020 2020 2020 2020 2020 7665 7262              verb
+0000d930: 6f73 653d 7665 7262 6f73 652c 0a20 2020  ose=verbose,.   
+0000d940: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000d950: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0000d960: 7375 6c74 735b 2278 225d 0a20 2020 2020  sults["x"].     
+0000d970: 2020 2065 6c69 6620 6d65 7468 6f64 203d     elif method =
+0000d980: 3d20 224c 2d42 4647 532d 4222 3a0a 2020  = "L-BFGS-B":.  
+0000d990: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
+0000d9a0: 7320 3d20 7b22 6469 7370 223a 2076 6572  s = {"disp": ver
+0000d9b0: 626f 7365 2c20 2267 746f 6c22 3a20 3165  bose, "gtol": 1e
+0000d9c0: 2d38 7d0a 2020 2020 2020 2020 2020 2020  -8}.            
+0000d9d0: 7265 7375 6c74 7320 3d20 6f70 7469 6d69  results = optimi
+0000d9e0: 7a65 2e6d 696e 696d 697a 6528 0a20 2020  ze.minimize(.   
+0000d9f0: 2020 2020 2020 2020 2020 2020 206c 616d               lam
+0000da00: 6264 6120 783a 205b 0a20 2020 2020 2020  bda x: [.       
+0000da10: 2020 2020 2020 2020 2020 2020 2072 2e63               r.c
+0000da20: 7075 2829 2e6e 756d 7079 2829 0a20 2020  pu().numpy().   
+0000da30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da40: 2066 6f72 2072 2069 6e20 5f63 6f6d 7075   for r in _compu
+0000da50: 7465 5f6c 6f73 735f 616e 645f 6772 6164  te_loss_and_grad
+0000da60: 5f6f 665f 6446 280a 2020 2020 2020 2020  _of_dF(.        
+0000da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da80: 656e 6572 6779 2e6e 6577 5f74 656e 736f  energy.new_tenso
+0000da90: 7228 7829 2c20 656e 6572 6779 2c20 6e75  r(x), energy, nu
+0000daa0: 6d5f 636f 6e66 0a20 2020 2020 2020 2020  m_conf.         
+0000dab0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000dac0: 2020 2020 2020 2020 2020 2020 205d 2c0a               ],.
+0000dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dae0: 6446 5f69 6e69 742e 6370 7528 292e 6e75  dF_init.cpu().nu
+0000daf0: 6d70 7928 292c 0a20 2020 2020 2020 2020  mpy(),.         
+0000db00: 2020 2020 2020 206a 6163 3d54 7275 652c         jac=True,
+0000db10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000db20: 206d 6574 686f 643d 224c 2d42 4647 532d   method="L-BFGS-
+0000db30: 4222 2c0a 2020 2020 2020 2020 2020 2020  B",.            
+0000db40: 2020 2020 746f 6c3d 3165 2d31 322c 0a20      tol=1e-12,. 
+0000db50: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000db60: 7074 696f 6e73 3d6f 7074 696f 6e73 2c0a  ptions=options,.
+0000db70: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000db80: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000db90: 2074 6f72 6368 2e66 726f 6d5f 6e75 6d70   torch.from_nump
+0000dba0: 7928 7265 7375 6c74 735b 2278 225d 290a  y(results["x"]).
+0000dbb0: 0a0a 6465 6620 5f62 6f6f 7473 7472 6170  ..def _bootstrap
+0000dbc0: 5f63 6f6e 665f 6964 7828 6e75 6d5f 636f  _conf_idx(num_co
+0000dbd0: 6e66 2c20 626f 6f74 7374 7261 705f 626c  nf, bootstrap_bl
+0000dbe0: 6f63 6b5f 7369 7a65 293a 0a20 2020 206e  ock_size):.    n
+0000dbf0: 756d 5f63 6f6e 665f 6375 6d73 756d 203d  um_conf_cumsum =
+0000dc00: 2074 6f72 6368 2e63 756d 7375 6d28 6e75   torch.cumsum(nu
+0000dc10: 6d5f 636f 6e66 2c20 6469 6d3d 3029 2e74  m_conf, dim=0).t
+0000dc20: 6f6c 6973 7428 290a 2020 2020 6e75 6d5f  olist().    num_
+0000dc30: 636f 6e66 5f63 756d 7375 6d2e 706f 7028  conf_cumsum.pop(
+0000dc40: 2d31 290a 2020 2020 6e75 6d5f 636f 6e66  -1).    num_conf
+0000dc50: 5f63 756d 7375 6d20 3d20 5b30 5d20 2b20  _cumsum = [0] + 
+0000dc60: 6e75 6d5f 636f 6e66 5f63 756d 7375 6d0a  num_conf_cumsum.
+0000dc70: 2020 2020 636f 6e66 5f69 6478 203d 205b      conf_idx = [
+0000dc80: 5d0a 2020 2020 666f 7220 6920 696e 2072  ].    for i in r
+0000dc90: 616e 6765 286c 656e 286e 756d 5f63 6f6e  ange(len(num_con
+0000dca0: 6629 293a 0a20 2020 2020 2020 206c 656e  f)):.        len
+0000dcb0: 5f73 6571 203d 2069 6e74 286e 756d 5f63  _seq = int(num_c
+0000dcc0: 6f6e 665b 695d 2920 2023 2320 7573 696e  onf[i])  ## usin
+0000dcd0: 6720 6369 7263 756c 6172 2062 6c6f 636b  g circular block
+0000dce0: 2062 6f6f 7473 7472 6170 0a20 2020 2020   bootstrap.     
+0000dcf0: 2020 206e 756d 5f73 616d 706c 655f 626c     num_sample_bl
+0000dd00: 6f63 6b20 3d20 696e 7428 6e70 2e63 6569  ock = int(np.cei
+0000dd10: 6c28 6c65 6e5f 7365 7120 2f20 626f 6f74  l(len_seq / boot
+0000dd20: 7374 7261 705f 626c 6f63 6b5f 7369 7a65  strap_block_size
+0000dd30: 2929 0a20 2020 2020 2020 2069 6478 7320  )).        idxs 
+0000dd40: 3d20 746f 7263 682e 7261 6e64 696e 7428  = torch.randint(
+0000dd50: 302c 206c 656e 5f73 6571 2c20 286e 756d  0, len_seq, (num
+0000dd60: 5f73 616d 706c 655f 626c 6f63 6b2c 2929  _sample_block,))
+0000dd70: 0a20 2020 2020 2020 2073 616d 706c 655f  .        sample_
+0000dd80: 6964 7820 3d20 746f 7263 682e 6361 7428  idx = torch.cat(
+0000dd90: 0a20 2020 2020 2020 2020 2020 205b 746f  .            [to
+0000dda0: 7263 682e 6172 616e 6765 2869 6478 2c20  rch.arange(idx, 
+0000ddb0: 6964 7820 2b20 626f 6f74 7374 7261 705f  idx + bootstrap_
+0000ddc0: 626c 6f63 6b5f 7369 7a65 2920 666f 7220  block_size) for 
+0000ddd0: 6964 7820 696e 2069 6478 735d 0a20 2020  idx in idxs].   
+0000dde0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+0000ddf0: 616d 706c 655f 6964 7820 3d20 746f 7263  ample_idx = torc
+0000de00: 682e 7265 6d61 696e 6465 7228 7361 6d70  h.remainder(samp
+0000de10: 6c65 5f69 6478 2c20 6c65 6e5f 7365 7129  le_idx, len_seq)
+0000de20: 0a20 2020 2020 2020 2073 616d 706c 655f  .        sample_
+0000de30: 6964 7820 3d20 7361 6d70 6c65 5f69 6478  idx = sample_idx
+0000de40: 5b30 3a6c 656e 5f73 6571 5d0a 2020 2020  [0:len_seq].    
+0000de50: 2020 2020 7361 6d70 6c65 5f69 6478 203d      sample_idx =
+0000de60: 2073 616d 706c 655f 6964 7820 2b20 6e75   sample_idx + nu
+0000de70: 6d5f 636f 6e66 5f63 756d 7375 6d5b 695d  m_conf_cumsum[i]
+0000de80: 0a20 2020 2020 2020 2063 6f6e 665f 6964  .        conf_id
+0000de90: 782e 6170 7065 6e64 2873 616d 706c 655f  x.append(sample_
+0000dea0: 6964 7829 0a20 2020 2063 6f6e 665f 6964  idx).    conf_id
+0000deb0: 7820 3d20 746f 7263 682e 6361 7428 636f  x = torch.cat(co
+0000dec0: 6e66 5f69 6478 290a 2020 2020 7265 7475  nf_idx).    retu
+0000ded0: 726e 2063 6f6e 665f 6964 780a 0a0a 6465  rn conf_idx...de
+0000dee0: 6620 666d 696e 5f6e 6577 746f 6e28 662c  f fmin_newton(f,
+0000def0: 2068 6573 732c 2078 5f69 6e69 742c 2061   hess, x_init, a
+0000df00: 7267 733d 2829 2c20 7665 7262 6f73 653d  rgs=(), verbose=
+0000df10: 5472 7565 2c20 6570 733d 3165 2d31 322c  True, eps=1e-12,
+0000df20: 206d 6178 5f69 7465 723d 3330 3029 3a0a   max_iter=300):.
+0000df30: 2020 2020 2222 224d 696e 696d 697a 6520      """Minimize 
+0000df40: 6120 6675 6e63 7469 6f6e 2077 6974 6820  a function with 
+0000df50: 7468 6520 4e65 7774 6f6e 2773 206d 6574  the Newton's met
+0000df60: 686f 642e 0a0a 2020 2020 466f 7220 6465  hod...    For de
+0000df70: 7461 696c 7320 6f66 2074 6865 204e 6577  tails of the New
+0000df80: 746f 6e27 7320 6d65 7468 6f64 2c20 7365  ton's method, se
+0000df90: 6520 4368 6170 7465 7220 392e 3520 6f66  e Chapter 9.5 of
+0000dfa0: 2050 726f 662e 2042 6f79 6427 7320 626f   Prof. Boyd's bo
+0000dfb0: 6f6b 0a20 2020 2060 436f 6e76 6578 204f  ok.    `Convex O
+0000dfc0: 7074 696d 697a 6174 696f 6e20 3c68 7474  ptimization <htt
+0000dfd0: 7073 3a2f 2f77 6562 2e73 7461 6e66 6f72  ps://web.stanfor
+0000dfe0: 642e 6564 752f 7e62 6f79 642f 6376 7862  d.edu/~boyd/cvxb
+0000dff0: 6f6f 6b2f 3e60 5f2e 0a0a 2020 2020 4172  ook/>`_...    Ar
+0000e000: 6773 3a0a 2020 2020 2020 2020 6620 2863  gs:.        f (c
+0000e010: 616c 6c61 626c 6529 3a20 7468 6520 6f62  allable): the ob
+0000e020: 6a65 6374 6976 6520 6675 6e63 7469 6f6e  jective function
+0000e030: 2074 6f20 6265 206d 696e 696d 697a 6564   to be minimized
+0000e040: 2e0a 2020 2020 2020 2020 2020 2020 6628  ..            f(
+0000e050: 783a 5465 6e73 6f72 2c20 2a61 7267 7329  x:Tensor, *args)
+0000e060: 202d 3e20 2028 793a 5465 6e73 6f72 2c20   ->  (y:Tensor, 
+0000e070: 6772 6164 3a54 656e 736f 7229 2c20 7768  grad:Tensor), wh
+0000e080: 6572 650a 2020 2020 2020 2020 2020 2020  ere.            
+0000e090: 7920 6973 2074 6865 2066 756e 6374 696f  y is the functio
+0000e0a0: 6e20 7661 6c75 6520 616e 6420 6772 6164  n value and grad
+0000e0b0: 2069 7320 7468 6520 6772 6164 6965 6e74   is the gradient
+0000e0c0: 2e0a 2020 2020 2020 2020 6865 7373 2028  ..        hess (
+0000e0d0: 6361 6c6c 6162 6c65 293a 2074 6865 2066  callable): the f
+0000e0e0: 756e 6374 696f 6e20 746f 2063 6f6d 7075  unction to compu
+0000e0f0: 7465 2074 6865 2048 6573 7369 616e 206d  te the Hessian m
+0000e100: 6174 7269 782e 0a20 2020 2020 2020 2020  atrix..         
+0000e110: 2020 2068 6573 7328 783a 5465 6e73 6f72     hess(x:Tensor
+0000e120: 2c20 2a61 7267 7329 202d 3e20 6120 7477  , *args) -> a tw
+0000e130: 6f20 6469 6d65 6e73 696f 6e61 6c20 7465  o dimensional te
+0000e140: 6e73 6f72 2e0a 2020 2020 2020 2020 785f  nsor..        x_
+0000e150: 696e 6974 2028 5465 6e73 6f72 293a 2074  init (Tensor): t
+0000e160: 6865 2069 6e69 7469 616c 2076 616c 7565  he initial value
+0000e170: 2e0a 2020 2020 2020 2020 6172 6773 2028  ..        args (
+0000e180: 7475 706c 6529 3a20 6578 7472 6120 7061  tuple): extra pa
+0000e190: 7261 6d65 7465 7273 2066 6f72 2066 2061  rameters for f a
+0000e1a0: 6e64 2068 6573 732e 0a20 2020 2020 2020  nd hess..       
+0000e1b0: 2076 6572 626f 7365 2028 626f 6f6c 293a   verbose (bool):
+0000e1c0: 2077 6865 7468 6572 2074 6f20 7072 696e   whether to prin
+0000e1d0: 7420 6d69 6e69 6d69 7a69 6e67 206c 6f67  t minimizing log
+0000e1e0: 2069 6e66 6f72 6d61 7469 6f6e 2e0a 2020   information..  
+0000e1f0: 2020 2020 2020 6570 7320 2866 6c6f 6174        eps (float
+0000e200: 293a 2074 6f6c 6572 616e 6365 2066 6f72  ): tolerance for
+0000e210: 2073 746f 7070 696e 670a 2020 2020 2020   stopping.      
+0000e220: 2020 6d61 785f 6974 6572 2028 696e 7429    max_iter (int)
+0000e230: 3a20 6d61 7869 6d75 6d20 6e75 6d62 6572  : maximum number
+0000e240: 206f 6620 6974 6572 6174 696f 6e73 2e0a   of iterations..
+0000e250: 2020 2020 2222 220a 0a20 2020 2023 2320      """..    ## 
+0000e260: 636f 6e73 7461 6e74 7320 7573 6564 2069  constants used i
+0000e270: 6e20 6261 636b 7472 6163 6b69 6e67 206c  n backtracking l
+0000e280: 696e 6520 7365 6172 6368 0a20 2020 2061  ine search.    a
+0000e290: 6c70 6861 2c20 6265 7461 203d 2030 2e30  lpha, beta = 0.0
+0000e2a0: 312c 2030 2e32 0a0a 2020 2020 2323 204e  1, 0.2..    ## N
+0000e2b0: 6577 746f 6e27 7320 6d65 7468 6f64 2066  ewton's method f
+0000e2c0: 6f72 206d 696e 696d 697a 696e 6720 7468  or minimizing th
+0000e2d0: 6520 6675 6e63 7469 6f6e 0a20 2020 2069  e function.    i
+0000e2e0: 6e64 785f 6974 6572 203d 2030 0a0a 2020  ndx_iter = 0..  
+0000e2f0: 2020 4e5f 6675 6e63 203d 2030 0a0a 2020    N_func = 0..  
+0000e300: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
+0000e310: 2020 2020 2020 7072 696e 7428 223d 3d3d        print("===
+0000e320: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000e330: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0000e340: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000e350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000e360: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000e370: 3d3d 3d3d 3d22 290a 0a20 2020 2020 2020  =====")..       
-0000e380: 2070 7269 6e74 2822 2020 2020 2020 2020   print("        
-0000e390: 2020 2020 2020 2020 5255 4e4e 494e 4720          RUNNING 
-0000e3a0: 5448 4520 4e45 5754 4f4e 2753 204d 4554  THE NEWTON'S MET
-0000e3b0: 484f 4420 2020 2020 2020 2020 2020 2020  HOD             
-0000e3c0: 2020 2020 2020 2020 5c6e 2229 0a20 2020          \n").   
-0000e3d0: 2020 2020 2070 7269 6e74 2822 2020 2020       print("    
-0000e3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3f0: 2020 2020 2020 202a 202a 202a 2020 2020         * * *    
-0000e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e410: 2020 2020 2020 2020 2020 2020 5c6e 2229              \n")
-0000e420: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
-0000e430: 2220 2020 2020 2020 2020 2020 2020 2020  "               
-0000e440: 2020 2020 2054 6f6c 6572 616e 6365 2045       Tolerance E
-0000e450: 5053 203d 207b 6570 733a 2e35 457d 2020  PS = {eps:.5E}  
-0000e460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e470: 5c6e 2229 0a0a 2020 2020 2323 2063 6865  \n")..    ## che
-0000e480: 636b 2069 6620 785f 696e 6974 2069 7320  ck if x_init is 
-0000e490: 6120 7079 746f 7263 6820 7465 6e73 6f72  a pytorch tensor
-0000e4a0: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
-0000e4b0: 6365 2878 5f69 6e69 742c 2074 6f72 6368  ce(x_init, torch
-0000e4c0: 2e54 656e 736f 7229 3a0a 2020 2020 2020  .Tensor):.      
-0000e4d0: 2020 7820 3d20 785f 696e 6974 2e63 6c6f    x = x_init.clo
-0000e4e0: 6e65 2829 2e64 6574 6163 6828 292e 7265  ne().detach().re
-0000e4f0: 7175 6972 6573 5f67 7261 645f 2846 616c  quires_grad_(Fal
-0000e500: 7365 290a 2020 2020 656c 7365 3a0a 2020  se).    else:.  
-0000e510: 2020 2020 2020 7820 3d20 785f 696e 6974        x = x_init
-0000e520: 0a0a 2020 2020 7768 696c 6520 696e 6478  ..    while indx
-0000e530: 5f69 7465 7220 3c20 6d61 785f 6974 6572  _iter < max_iter
-0000e540: 3a0a 2020 2020 2020 2020 6c6f 7373 2c20  :.        loss, 
-0000e550: 6772 6164 203d 2066 2878 2c20 2a61 7267  grad = f(x, *arg
-0000e560: 7329 0a20 2020 2020 2020 204e 5f66 756e  s).        N_fun
-0000e570: 6320 2b3d 2031 0a0a 2020 2020 2020 2020  c += 1..        
-0000e580: 6966 2069 7369 6e73 7461 6e63 6528 785f  if isinstance(x_
-0000e590: 696e 6974 2c20 746f 7263 682e 5465 6e73  init, torch.Tens
-0000e5a0: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
-0000e5b0: 2077 6974 6820 746f 7263 682e 6e6f 5f67   with torch.no_g
-0000e5c0: 7261 6428 293a 0a20 2020 2020 2020 2020  rad():.         
-0000e5d0: 2020 2020 2020 2048 203d 2068 6573 7328         H = hess(
-0000e5e0: 782c 202a 6172 6773 290a 2020 2020 2020  x, *args).      
-0000e5f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000e600: 2020 2020 4820 3d20 6865 7373 2878 2c20      H = hess(x, 
-0000e610: 2a61 7267 7329 0a0a 2020 2020 2020 2020  *args)..        
-0000e620: 6966 2069 7369 6e73 7461 6e63 6528 6772  if isinstance(gr
-0000e630: 6164 2c20 746f 7263 682e 5465 6e73 6f72  ad, torch.Tensor
-0000e640: 293a 0a20 2020 2020 2020 2020 2020 206e  ):.            n
-0000e650: 6577 746f 6e5f 6469 7265 6374 696f 6e20  ewton_direction 
-0000e660: 3d20 746f 7263 682e 6c69 6e61 6c67 2e73  = torch.linalg.s
-0000e670: 6f6c 7665 2848 2c20 2d67 7261 6429 0a20  olve(H, -grad). 
-0000e680: 2020 2020 2020 2020 2020 206e 6577 746f             newto
-0000e690: 6e5f 6465 6372 656d 656e 745f 7371 7561  n_decrement_squa
-0000e6a0: 7265 203d 2074 6f72 6368 2e73 756d 282d  re = torch.sum(-
-0000e6b0: 6772 6164 202a 206e 6577 746f 6e5f 6469  grad * newton_di
-0000e6c0: 7265 6374 696f 6e29 0a20 2020 2020 2020  rection).       
-0000e6d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000e6e0: 2020 206e 6577 746f 6e5f 6469 7265 6374     newton_direct
-0000e6f0: 696f 6e20 3d20 6e70 2e6c 696e 616c 672e  ion = np.linalg.
-0000e700: 736f 6c76 6528 482c 202d 6772 6164 290a  solve(H, -grad).
-0000e710: 2020 2020 2020 2020 2020 2020 6e65 7774              newt
-0000e720: 6f6e 5f64 6563 7265 6d65 6e74 5f73 7175  on_decrement_squ
-0000e730: 6172 6520 3d20 6e70 2e73 756d 282d 6772  are = np.sum(-gr
-0000e740: 6164 202a 206e 6577 746f 6e5f 6469 7265  ad * newton_dire
-0000e750: 6374 696f 6e29 0a0a 2020 2020 2020 2020  ction)..        
-0000e760: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
-0000e770: 2020 2020 2020 2020 7072 696e 7428 0a20          print(. 
-0000e780: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000e790: 2241 7420 6974 6572 6174 6520 7b69 6e64  "At iterate {ind
-0000e7a0: 785f 6974 6572 3a34 647d 3b20 663d 207b  x_iter:4d}; f= {
-0000e7b0: 6c6f 7373 2e69 7465 6d28 293a 2e35 457d  loss.item():.5E}
-0000e7c0: 3b22 2c0a 2020 2020 2020 2020 2020 2020  ;",.            
-0000e7d0: 2020 2020 6622 7c31 2f32 2a4e 6577 746f      f"|1/2*Newto
-0000e7e0: 6e5f 6465 6372 656d 656e 745e 327c 3a20  n_decrement^2|: 
-0000e7f0: 7b6e 6577 746f 6e5f 6465 6372 656d 656e  {newton_decremen
-0000e800: 745f 7371 7561 7265 2e69 7465 6d28 292f  t_square.item()/
-0000e810: 323a 2e35 457d 5c6e 222c 0a20 2020 2020  2:.5E}\n",.     
-0000e820: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000e830: 2020 6966 206e 6577 746f 6e5f 6465 6372    if newton_decr
-0000e840: 656d 656e 745f 7371 7561 7265 202f 2032  ement_square / 2
-0000e850: 2e30 203c 3d20 6570 733a 0a20 2020 2020  .0 <= eps:.     
-0000e860: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
-0000e870: 2020 2020 2020 2323 2062 6163 6b74 7261        ## backtra
-0000e880: 636b 696e 6720 6c69 6e65 2073 6561 7263  cking line searc
-0000e890: 680a 2020 2020 2020 2020 6d61 785f 6c73  h.        max_ls
-0000e8a0: 5f69 7465 7220 3d20 3130 300a 2020 2020  _iter = 100.    
-0000e8b0: 2020 2020 7374 6570 5f73 697a 6520 3d20      step_size = 
-0000e8c0: 312e 300a 0a20 2020 2020 2020 2069 6e64  1.0..        ind
-0000e8d0: 785f 6c73 5f69 7465 7220 3d20 300a 2020  x_ls_iter = 0.  
-0000e8e0: 2020 2020 2020 7768 696c 6520 696e 6478        while indx
-0000e8f0: 5f6c 735f 6974 6572 203c 206d 6178 5f6c  _ls_iter < max_l
-0000e900: 735f 6974 6572 3a0a 2020 2020 2020 2020  s_iter:.        
-0000e910: 2020 2020 7461 7267 6574 5f6c 6f73 732c      target_loss,
-0000e920: 205f 203d 2066 2878 202b 2073 7465 705f   _ = f(x + step_
-0000e930: 7369 7a65 202a 206e 6577 746f 6e5f 6469  size * newton_di
-0000e940: 7265 6374 696f 6e2c 202a 6172 6773 290a  rection, *args).
-0000e950: 0a20 2020 2020 2020 2020 2020 204e 5f66  .            N_f
-0000e960: 756e 6320 2b3d 2031 0a20 2020 2020 2020  unc += 1.       
-0000e970: 2020 2020 2061 7070 726f 7869 6d61 7465       approximate
-0000e980: 5f6c 6f73 7320 3d20 6c6f 7373 202b 2073  _loss = loss + s
-0000e990: 7465 705f 7369 7a65 202a 2061 6c70 6861  tep_size * alpha
-0000e9a0: 202a 2028 2d6e 6577 746f 6e5f 6465 6372   * (-newton_decr
-0000e9b0: 656d 656e 745f 7371 7561 7265 290a 2020  ement_square).  
-0000e9c0: 2020 2020 2020 2020 2020 6966 2074 6172            if tar
-0000e9d0: 6765 745f 6c6f 7373 203c 2061 7070 726f  get_loss < appro
-0000e9e0: 7869 6d61 7465 5f6c 6f73 733a 0a20 2020  ximate_loss:.   
-0000e9f0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-0000ea00: 616b 0a20 2020 2020 2020 2020 2020 2065  ak.            e
-0000ea10: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000ea20: 2020 2020 2073 7465 705f 7369 7a65 203d       step_size =
-0000ea30: 2073 7465 705f 7369 7a65 202a 2062 6574   step_size * bet
-0000ea40: 610a 2020 2020 2020 2020 2020 2020 696e  a.            in
-0000ea50: 6478 5f6c 735f 6974 6572 202b 3d20 310a  dx_ls_iter += 1.
-0000ea60: 0a20 2020 2020 2020 2078 203d 2078 202b  .        x = x +
-0000ea70: 2073 7465 705f 7369 7a65 202a 206e 6577   step_size * new
-0000ea80: 746f 6e5f 6469 7265 6374 696f 6e0a 2020  ton_direction.  
-0000ea90: 2020 2020 2020 696e 6478 5f69 7465 7220        indx_iter 
-0000eaa0: 2b3d 2031 0a0a 2020 2020 6966 2076 6572  += 1..    if ver
-0000eab0: 626f 7365 3a0a 2020 2020 2020 2020 7072  bose:.        pr
-0000eac0: 696e 7428 224e 5f69 7465 7220 2020 3d20  int("N_iter   = 
-0000ead0: 746f 7461 6c20 6e75 6d62 6572 206f 6620  total number of 
-0000eae0: 6974 6572 6174 696f 6e73 2229 0a20 2020  iterations").   
-0000eaf0: 2020 2020 2070 7269 6e74 2822 4e5f 6675       print("N_fu
-0000eb00: 6e63 2020 203d 2074 6f74 616c 206e 756d  nc   = total num
-0000eb10: 6265 7220 6f66 2066 756e 6374 696f 6e20  ber of function 
-0000eb20: 616e 6420 6772 6164 6965 6e74 2065 7661  and gradient eva
-0000eb30: 6c75 6174 696f 6e73 2229 0a20 2020 2020  luations").     
-0000eb40: 2020 2070 7269 6e74 2822 4620 2020 2020     print("F     
-0000eb50: 2020 203d 2066 696e 616c 2066 756e 6374     = final funct
-0000eb60: 696f 6e20 7661 6c75 6520 5c6e 2229 0a20  ion value \n"). 
-0000eb70: 2020 2020 2020 2070 7269 6e74 2822 2020         print("  
-0000eb80: 2020 2020 2020 2020 2020 202a 202a 202a             * * *
-0000eb90: 2020 2020 205c 6e22 290a 2020 2020 2020       \n").      
-0000eba0: 2020 7072 696e 7428 224e 5f69 7465 7220    print("N_iter 
-0000ebb0: 2020 204e 5f66 756e 6320 2020 2020 2020     N_func       
-0000ebc0: 2046 2229 0a20 2020 2020 2020 2070 7269   F").        pri
-0000ebd0: 6e74 2866 227b 696e 6478 5f69 7465 722b  nt(f"{indx_iter+
-0000ebe0: 313a 3664 7d20 2020 207b 4e5f 6675 6e63  1:6d}    {N_func
-0000ebf0: 3a36 647d 2020 2020 7b6c 6f73 732e 6974  :6d}    {loss.it
-0000ec00: 656d 2829 3a2e 3645 7d22 290a 2020 2020  em():.6E}").    
-0000ec10: 2020 2020 7072 696e 7428 6622 2020 4620      print(f"  F 
-0000ec20: 3d20 7b6c 6f73 732e 6974 656d 2829 3a2e  = {loss.item():.
-0000ec30: 3132 667d 205c 6e22 290a 0a20 2020 2020  12f} \n")..     
-0000ec40: 2020 2069 6620 6e65 7774 6f6e 5f64 6563     if newton_dec
-0000ec50: 7265 6d65 6e74 5f73 7175 6172 6520 2f20  rement_square / 
-0000ec60: 322e 3020 3c3d 2065 7073 2061 6e64 2069  2.0 <= eps and i
-0000ec70: 6e64 785f 6974 6572 203c 206d 6178 5f69  ndx_iter < max_i
-0000ec80: 7465 723a 0a20 2020 2020 2020 2020 2020  ter:.           
-0000ec90: 2070 7269 6e74 2822 434f 4e56 4552 4745   print("CONVERGE
-0000eca0: 4e43 453a 2031 2f32 2a4e 6577 746f 6e5f  NCE: 1/2*Newton_
-0000ecb0: 6465 6372 656d 656e 745e 3220 3c20 4550  decrement^2 < EP
-0000ecc0: 5322 290a 2020 2020 2020 2020 656c 7365  S").        else
-0000ecd0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-0000ece0: 696e 7428 2243 4f4e 5645 5247 454e 4345  int("CONVERGENCE
-0000ecf0: 3a20 4e55 4d5f 4f46 5f49 5445 5241 5449  : NUM_OF_ITERATI
-0000ed00: 4f4e 2052 4541 4348 204d 4158 5f49 5445  ON REACH MAX_ITE
-0000ed10: 5241 5449 4f4e 2229 0a0a 2020 2020 7265  RATION")..    re
-0000ed20: 7475 726e 207b 0a20 2020 2020 2020 2022  turn {.        "
-0000ed30: 7822 3a20 782c 0a20 2020 2020 2020 2022  x": x,.        "
-0000ed40: 4e5f 6974 6572 223a 2069 6e64 785f 6974  N_iter": indx_it
-0000ed50: 6572 202b 2031 2c0a 2020 2020 2020 2020  er + 1,.        
-0000ed60: 224e 5f66 756e 6322 3a20 4e5f 6675 6e63  "N_func": N_func
-0000ed70: 2c0a 2020 2020 2020 2020 2246 223a 206c  ,.        "F": l
-0000ed80: 6f73 732e 6974 656d 2829 2c0a 2020 2020  oss.item(),.    
-0000ed90: 2020 2020 2268 616c 665f 6e65 7774 6f6e      "half_newton
-0000eda0: 5f64 6563 7265 6d65 6e74 5f73 7175 6172  _decrement_squar
-0000edb0: 6522 3a20 6e65 7774 6f6e 5f64 6563 7265  e": newton_decre
-0000edc0: 6d65 6e74 5f73 7175 6172 6520 2f20 322e  ment_square / 2.
-0000edd0: 302c 0a20 2020 207d 0a94 7d94 288c 1146  0,.    }..}.(..F
-0000ede0: 6173 744d 4241 522e 5f5f 696e 6974 5f5f  astMBAR.__init__
-0000edf0: 948c 0364 6566 944b 124d 2a01 8794 8c0a  ...def.K.M*.....
-0000ee00: 4661 7374 4d42 4152 2e46 946a 3709 0000  FastMBAR.F.j7...
-0000ee10: 4d2c 014d 3101 8794 8c0e 4661 7374 4d42  M,.M1.....FastMB
-0000ee20: 4152 2e46 5f73 7464 946a 3709 0000 4d33  AR.F_std.j7...M3
-0000ee30: 014d 3901 8794 8c0e 4661 7374 4d42 4152  .M9.....FastMBAR
-0000ee40: 2e46 5f63 6f76 946a 3709 0000 4d3b 014d  .F_cov.j7...M;.M
-0000ee50: 4101 8794 8c0f 4661 7374 4d42 4152 2e44  A.....FastMBAR.D
-0000ee60: 656c 7461 4694 6a37 0900 004d 4301 4d49  eltaF.j7...MC.MI
-0000ee70: 0187 948c 1346 6173 744d 4241 522e 4465  .....FastMBAR.De
-0000ee80: 6c74 6146 5f73 7464 946a 3709 0000 4d4b  ltaF_std.j7...MK
-0000ee90: 014d 5101 8794 8c15 4661 7374 4d42 4152  .MQ.....FastMBAR
-0000eea0: 2e6c 6f67 5f70 726f 625f 6d69 7894 6a37  .log_prob_mix.j7
-0000eeb0: 0900 004d 5301 4d56 0187 948c 3446 6173  ...MS.MV....4Fas
-0000eec0: 744d 4241 522e 6361 6c63 756c 6174 655f  tMBAR.calculate_
-0000eed0: 6672 6565 5f65 6e65 7267 6965 735f 6f66  free_energies_of
-0000eee0: 5f70 6572 7475 7262 6564 5f73 7461 7465  _perturbed_state
-0000eef0: 7394 6a37 0900 004d 5801 4db3 0187 948c  s.j7...MX.M.....
-0000ef00: 0846 6173 744d 4241 5294 8c05 636c 6173  .FastMBAR...clas
-0000ef10: 7394 4b08 4db3 0187 948c 125f 636f 6d70  s.K.M......_comp
-0000ef20: 7574 655f 6c6f 6770 5f6f 665f 4694 6a37  ute_logp_of_F.j7
-0000ef30: 0900 004d b501 4dba 0187 948c 1c5f 636f  ...M..M......_co
-0000ef40: 6d70 7574 655f 6c6f 7373 5f61 6e64 5f67  mpute_loss_and_g
-0000ef50: 7261 645f 6f66 5f64 4694 6a37 0900 004d  rad_of_dF.j7...M
-0000ef60: bd01 4dd9 0187 948c 255f 636f 6d70 7574  ..M.....%_comput
-0000ef70: 655f 6c6f 7373 5f61 6e64 5f67 7261 645f  e_loss_and_grad_
-0000ef80: 6f66 5f64 465f 696e 5f62 6174 6368 946a  of_dF_in_batch.j
-0000ef90: 3709 0000 4ddc 014d fd01 8794 8c24 5f63  7...M..M.....$_c
-0000efa0: 6f6d 7075 7465 5f68 6573 7369 616e 5f6c  ompute_hessian_l
-0000efb0: 6f67 5f6c 696b 656c 6968 6f6f 645f 6f66  og_likelihood_of
-0000efc0: 5f46 946a 3709 0000 4d00 024d 0502 8794  _F.j7...M..M....
-0000efd0: 8c2d 5f63 6f6d 7075 7465 5f68 6573 7369  .-_compute_hessi
-0000efe0: 616e 5f6c 6f67 5f6c 696b 656c 6968 6f6f  an_log_likelihoo
-0000eff0: 645f 6f66 5f46 5f69 6e5f 6261 7463 6894  d_of_F_in_batch.
-0000f000: 6a37 0900 004d 0802 4d17 0287 948c 1b5f  j7...M..M......_
-0000f010: 636f 6d70 7574 655f 6865 7373 6961 6e5f  compute_hessian_
-0000f020: 6c6f 7373 5f6f 665f 6446 946a 3709 0000  loss_of_dF.j7...
-0000f030: 4d1a 024d 1f02 8794 8c24 5f63 6f6d 7075  M..M.....$_compu
-0000f040: 7465 5f68 6573 7369 616e 5f6c 6f73 735f  te_hessian_loss_
-0000f050: 6f66 5f64 465f 696e 5f62 6174 6368 946a  of_dF_in_batch.j
-0000f060: 3709 0000 4d22 024d 2702 8794 8c0b 5f73  7...M".M'....._s
-0000f070: 6f6c 7665 5f6d 6261 7294 6a37 0900 004d  olve_mbar.j7...M
-0000f080: 2a02 4d5f 0287 948c 135f 626f 6f74 7374  *.M_....._bootst
-0000f090: 7261 705f 636f 6e66 5f69 6478 946a 3709  rap_conf_idx.j7.
-0000f0a0: 0000 4d62 024d 7302 8794 8c0b 666d 696e  ..Mb.Ms.....fmin
-0000f0b0: 5f6e 6577 746f 6e94 6a37 0900 004d 7602  _newton.j7...Mv.
-0000f0c0: 4ddf 0287 9475 7d94 288c 0846 6173 744d  M....u}.(..FastM
-0000f0d0: 4241 5294 6a1c 0300 008c 1146 6173 744d  BAR.j......FastM
-0000f0e0: 4241 522e 5f5f 696e 6974 5f5f 946a 1c03  BAR.__init__.j..
-0000f0f0: 0000 8c34 4661 7374 4d42 4152 2e63 616c  ...4FastMBAR.cal
-0000f100: 6375 6c61 7465 5f66 7265 655f 656e 6572  culate_free_ener
-0000f110: 6769 6573 5f6f 665f 7065 7274 7572 6265  gies_of_perturbe
-0000f120: 645f 7374 6174 6573 946a 1c03 0000 758c  d_states.j....u.
-0000f130: 0846 6173 744d 4241 5294 7494 7375 622e  .FastMBAR.t.sub.
+0000e350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d22  ==============="
+0000e360: 290a 0a20 2020 2020 2020 2070 7269 6e74  )..        print
+0000e370: 2822 2020 2020 2020 2020 2020 2020 2020  ("              
+0000e380: 2020 5255 4e4e 494e 4720 5448 4520 4e45    RUNNING THE NE
+0000e390: 5754 4f4e 2753 204d 4554 484f 4420 2020  WTON'S METHOD   
+0000e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3b0: 2020 5c6e 2229 0a20 2020 2020 2020 2070    \n").        p
+0000e3c0: 7269 6e74 2822 2020 2020 2020 2020 2020  rint("          
+0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3e0: 202a 202a 202a 2020 2020 2020 2020 2020   * * *          
+0000e3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e400: 2020 2020 2020 5c6e 2229 0a20 2020 2020        \n").     
+0000e410: 2020 2070 7269 6e74 2866 2220 2020 2020     print(f"     
+0000e420: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+0000e430: 6f6c 6572 616e 6365 2045 5053 203d 207b  olerance EPS = {
+0000e440: 6570 733a 2e35 457d 2020 2020 2020 2020  eps:.5E}        
+0000e450: 2020 2020 2020 2020 2020 5c6e 2229 0a0a            \n")..
+0000e460: 2020 2020 2323 2063 6865 636b 2069 6620      ## check if 
+0000e470: 785f 696e 6974 2069 7320 6120 7079 746f  x_init is a pyto
+0000e480: 7263 6820 7465 6e73 6f72 0a20 2020 2069  rch tensor.    i
+0000e490: 6620 6973 696e 7374 616e 6365 2878 5f69  f isinstance(x_i
+0000e4a0: 6e69 742c 2074 6f72 6368 2e54 656e 736f  nit, torch.Tenso
+0000e4b0: 7229 3a0a 2020 2020 2020 2020 7820 3d20  r):.        x = 
+0000e4c0: 785f 696e 6974 2e63 6c6f 6e65 2829 2e64  x_init.clone().d
+0000e4d0: 6574 6163 6828 292e 7265 7175 6972 6573  etach().requires
+0000e4e0: 5f67 7261 645f 2846 616c 7365 290a 2020  _grad_(False).  
+0000e4f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000e500: 7820 3d20 785f 696e 6974 0a0a 2020 2020  x = x_init..    
+0000e510: 7768 696c 6520 696e 6478 5f69 7465 7220  while indx_iter 
+0000e520: 3c20 6d61 785f 6974 6572 3a0a 2020 2020  < max_iter:.    
+0000e530: 2020 2020 6c6f 7373 2c20 6772 6164 203d      loss, grad =
+0000e540: 2066 2878 2c20 2a61 7267 7329 0a20 2020   f(x, *args).   
+0000e550: 2020 2020 204e 5f66 756e 6320 2b3d 2031       N_func += 1
+0000e560: 0a0a 2020 2020 2020 2020 6966 2069 7369  ..        if isi
+0000e570: 6e73 7461 6e63 6528 785f 696e 6974 2c20  nstance(x_init, 
+0000e580: 746f 7263 682e 5465 6e73 6f72 293a 0a20  torch.Tensor):. 
+0000e590: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+0000e5a0: 746f 7263 682e 6e6f 5f67 7261 6428 293a  torch.no_grad():
+0000e5b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e5c0: 2048 203d 2068 6573 7328 782c 202a 6172   H = hess(x, *ar
+0000e5d0: 6773 290a 2020 2020 2020 2020 656c 7365  gs).        else
+0000e5e0: 3a0a 2020 2020 2020 2020 2020 2020 4820  :.            H 
+0000e5f0: 3d20 6865 7373 2878 2c20 2a61 7267 7329  = hess(x, *args)
+0000e600: 0a0a 2020 2020 2020 2020 6966 2069 7369  ..        if isi
+0000e610: 6e73 7461 6e63 6528 6772 6164 2c20 746f  nstance(grad, to
+0000e620: 7263 682e 5465 6e73 6f72 293a 0a20 2020  rch.Tensor):.   
+0000e630: 2020 2020 2020 2020 206e 6577 746f 6e5f           newton_
+0000e640: 6469 7265 6374 696f 6e20 3d20 746f 7263  direction = torc
+0000e650: 682e 6c69 6e61 6c67 2e73 6f6c 7665 2848  h.linalg.solve(H
+0000e660: 2c20 2d67 7261 6429 0a20 2020 2020 2020  , -grad).       
+0000e670: 2020 2020 206e 6577 746f 6e5f 6465 6372       newton_decr
+0000e680: 656d 656e 745f 7371 7561 7265 203d 2074  ement_square = t
+0000e690: 6f72 6368 2e73 756d 282d 6772 6164 202a  orch.sum(-grad *
+0000e6a0: 206e 6577 746f 6e5f 6469 7265 6374 696f   newton_directio
+0000e6b0: 6e29 0a20 2020 2020 2020 2065 6c73 653a  n).        else:
+0000e6c0: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
+0000e6d0: 746f 6e5f 6469 7265 6374 696f 6e20 3d20  ton_direction = 
+0000e6e0: 6e70 2e6c 696e 616c 672e 736f 6c76 6528  np.linalg.solve(
+0000e6f0: 482c 202d 6772 6164 290a 2020 2020 2020  H, -grad).      
+0000e700: 2020 2020 2020 6e65 7774 6f6e 5f64 6563        newton_dec
+0000e710: 7265 6d65 6e74 5f73 7175 6172 6520 3d20  rement_square = 
+0000e720: 6e70 2e73 756d 282d 6772 6164 202a 206e  np.sum(-grad * n
+0000e730: 6577 746f 6e5f 6469 7265 6374 696f 6e29  ewton_direction)
+0000e740: 0a0a 2020 2020 2020 2020 6966 2076 6572  ..        if ver
+0000e750: 626f 7365 3a0a 2020 2020 2020 2020 2020  bose:.          
+0000e760: 2020 7072 696e 7428 0a20 2020 2020 2020    print(.       
+0000e770: 2020 2020 2020 2020 2066 2241 7420 6974           f"At it
+0000e780: 6572 6174 6520 7b69 6e64 785f 6974 6572  erate {indx_iter
+0000e790: 3a34 647d 3b20 663d 207b 6c6f 7373 2e69  :4d}; f= {loss.i
+0000e7a0: 7465 6d28 293a 2e35 457d 3b22 2c0a 2020  tem():.5E};",.  
+0000e7b0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0000e7c0: 7c31 2f32 2a4e 6577 746f 6e5f 6465 6372  |1/2*Newton_decr
+0000e7d0: 656d 656e 745e 327c 3a20 7b6e 6577 746f  ement^2|: {newto
+0000e7e0: 6e5f 6465 6372 656d 656e 745f 7371 7561  n_decrement_squa
+0000e7f0: 7265 2e69 7465 6d28 292f 323a 2e35 457d  re.item()/2:.5E}
+0000e800: 5c6e 222c 0a20 2020 2020 2020 2020 2020  \n",.           
+0000e810: 2029 0a0a 2020 2020 2020 2020 6966 206e   )..        if n
+0000e820: 6577 746f 6e5f 6465 6372 656d 656e 745f  ewton_decrement_
+0000e830: 7371 7561 7265 202f 2032 2e30 203c 3d20  square / 2.0 <= 
+0000e840: 6570 733a 0a20 2020 2020 2020 2020 2020  eps:.           
+0000e850: 2062 7265 616b 0a0a 2020 2020 2020 2020   break..        
+0000e860: 2323 2062 6163 6b74 7261 636b 696e 6720  ## backtracking 
+0000e870: 6c69 6e65 2073 6561 7263 680a 2020 2020  line search.    
+0000e880: 2020 2020 6d61 785f 6c73 5f69 7465 7220      max_ls_iter 
+0000e890: 3d20 3130 300a 2020 2020 2020 2020 7374  = 100.        st
+0000e8a0: 6570 5f73 697a 6520 3d20 312e 300a 0a20  ep_size = 1.0.. 
+0000e8b0: 2020 2020 2020 2069 6e64 785f 6c73 5f69         indx_ls_i
+0000e8c0: 7465 7220 3d20 300a 2020 2020 2020 2020  ter = 0.        
+0000e8d0: 7768 696c 6520 696e 6478 5f6c 735f 6974  while indx_ls_it
+0000e8e0: 6572 203c 206d 6178 5f6c 735f 6974 6572  er < max_ls_iter
+0000e8f0: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
+0000e900: 7267 6574 5f6c 6f73 732c 205f 203d 2066  rget_loss, _ = f
+0000e910: 2878 202b 2073 7465 705f 7369 7a65 202a  (x + step_size *
+0000e920: 206e 6577 746f 6e5f 6469 7265 6374 696f   newton_directio
+0000e930: 6e2c 202a 6172 6773 290a 0a20 2020 2020  n, *args)..     
+0000e940: 2020 2020 2020 204e 5f66 756e 6320 2b3d         N_func +=
+0000e950: 2031 0a20 2020 2020 2020 2020 2020 2061   1.            a
+0000e960: 7070 726f 7869 6d61 7465 5f6c 6f73 7320  pproximate_loss 
+0000e970: 3d20 6c6f 7373 202b 2073 7465 705f 7369  = loss + step_si
+0000e980: 7a65 202a 2061 6c70 6861 202a 2028 2d6e  ze * alpha * (-n
+0000e990: 6577 746f 6e5f 6465 6372 656d 656e 745f  ewton_decrement_
+0000e9a0: 7371 7561 7265 290a 2020 2020 2020 2020  square).        
+0000e9b0: 2020 2020 6966 2074 6172 6765 745f 6c6f      if target_lo
+0000e9c0: 7373 203c 2061 7070 726f 7869 6d61 7465  ss < approximate
+0000e9d0: 5f6c 6f73 733a 0a20 2020 2020 2020 2020  _loss:.         
+0000e9e0: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+0000e9f0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000ea00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ea10: 7465 705f 7369 7a65 203d 2073 7465 705f  tep_size = step_
+0000ea20: 7369 7a65 202a 2062 6574 610a 2020 2020  size * beta.    
+0000ea30: 2020 2020 2020 2020 696e 6478 5f6c 735f          indx_ls_
+0000ea40: 6974 6572 202b 3d20 310a 0a20 2020 2020  iter += 1..     
+0000ea50: 2020 2078 203d 2078 202b 2073 7465 705f     x = x + step_
+0000ea60: 7369 7a65 202a 206e 6577 746f 6e5f 6469  size * newton_di
+0000ea70: 7265 6374 696f 6e0a 2020 2020 2020 2020  rection.        
+0000ea80: 696e 6478 5f69 7465 7220 2b3d 2031 0a0a  indx_iter += 1..
+0000ea90: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+0000eaa0: 2020 2020 2020 2020 7072 696e 7428 224e          print("N
+0000eab0: 5f69 7465 7220 2020 3d20 746f 7461 6c20  _iter   = total 
+0000eac0: 6e75 6d62 6572 206f 6620 6974 6572 6174  number of iterat
+0000ead0: 696f 6e73 2229 0a20 2020 2020 2020 2070  ions").        p
+0000eae0: 7269 6e74 2822 4e5f 6675 6e63 2020 203d  rint("N_func   =
+0000eaf0: 2074 6f74 616c 206e 756d 6265 7220 6f66   total number of
+0000eb00: 2066 756e 6374 696f 6e20 616e 6420 6772   function and gr
+0000eb10: 6164 6965 6e74 2065 7661 6c75 6174 696f  adient evaluatio
+0000eb20: 6e73 2229 0a20 2020 2020 2020 2070 7269  ns").        pri
+0000eb30: 6e74 2822 4620 2020 2020 2020 203d 2066  nt("F        = f
+0000eb40: 696e 616c 2066 756e 6374 696f 6e20 7661  inal function va
+0000eb50: 6c75 6520 5c6e 2229 0a20 2020 2020 2020  lue \n").       
+0000eb60: 2070 7269 6e74 2822 2020 2020 2020 2020   print("        
+0000eb70: 2020 2020 202a 202a 202a 2020 2020 205c       * * *     \
+0000eb80: 6e22 290a 2020 2020 2020 2020 7072 696e  n").        prin
+0000eb90: 7428 224e 5f69 7465 7220 2020 204e 5f66  t("N_iter    N_f
+0000eba0: 756e 6320 2020 2020 2020 2046 2229 0a20  unc        F"). 
+0000ebb0: 2020 2020 2020 2070 7269 6e74 2866 227b         print(f"{
+0000ebc0: 696e 6478 5f69 7465 722b 313a 3664 7d20  indx_iter+1:6d} 
+0000ebd0: 2020 207b 4e5f 6675 6e63 3a36 647d 2020     {N_func:6d}  
+0000ebe0: 2020 7b6c 6f73 732e 6974 656d 2829 3a2e    {loss.item():.
+0000ebf0: 3645 7d22 290a 2020 2020 2020 2020 7072  6E}").        pr
+0000ec00: 696e 7428 6622 2020 4620 3d20 7b6c 6f73  int(f"  F = {los
+0000ec10: 732e 6974 656d 2829 3a2e 3132 667d 205c  s.item():.12f} \
+0000ec20: 6e22 290a 0a20 2020 2020 2020 2069 6620  n")..        if 
+0000ec30: 6e65 7774 6f6e 5f64 6563 7265 6d65 6e74  newton_decrement
+0000ec40: 5f73 7175 6172 6520 2f20 322e 3020 3c3d  _square / 2.0 <=
+0000ec50: 2065 7073 2061 6e64 2069 6e64 785f 6974   eps and indx_it
+0000ec60: 6572 203c 206d 6178 5f69 7465 723a 0a20  er < max_iter:. 
+0000ec70: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000ec80: 2822 434f 4e56 4552 4745 4e43 453a 2031  ("CONVERGENCE: 1
+0000ec90: 2f32 2a4e 6577 746f 6e5f 6465 6372 656d  /2*Newton_decrem
+0000eca0: 656e 745e 3220 3c20 4550 5322 290a 2020  ent^2 < EPS").  
+0000ecb0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000ecc0: 2020 2020 2020 2020 7072 696e 7428 2243          print("C
+0000ecd0: 4f4e 5645 5247 454e 4345 3a20 4e55 4d5f  ONVERGENCE: NUM_
+0000ece0: 4f46 5f49 5445 5241 5449 4f4e 2052 4541  OF_ITERATION REA
+0000ecf0: 4348 204d 4158 5f49 5445 5241 5449 4f4e  CH MAX_ITERATION
+0000ed00: 2229 0a0a 2020 2020 7265 7475 726e 207b  ")..    return {
+0000ed10: 0a20 2020 2020 2020 2022 7822 3a20 782c  .        "x": x,
+0000ed20: 0a20 2020 2020 2020 2022 4e5f 6974 6572  .        "N_iter
+0000ed30: 223a 2069 6e64 785f 6974 6572 202b 2031  ": indx_iter + 1
+0000ed40: 2c0a 2020 2020 2020 2020 224e 5f66 756e  ,.        "N_fun
+0000ed50: 6322 3a20 4e5f 6675 6e63 2c0a 2020 2020  c": N_func,.    
+0000ed60: 2020 2020 2246 223a 206c 6f73 732e 6974      "F": loss.it
+0000ed70: 656d 2829 2c0a 2020 2020 2020 2020 2268  em(),.        "h
+0000ed80: 616c 665f 6e65 7774 6f6e 5f64 6563 7265  alf_newton_decre
+0000ed90: 6d65 6e74 5f73 7175 6172 6522 3a20 6e65  ment_square": ne
+0000eda0: 7774 6f6e 5f64 6563 7265 6d65 6e74 5f73  wton_decrement_s
+0000edb0: 7175 6172 6520 2f20 322e 302c 0a20 2020  quare / 2.0,.   
+0000edc0: 207d 0a94 7d94 288c 1146 6173 744d 4241   }..}.(..FastMBA
+0000edd0: 522e 5f5f 696e 6974 5f5f 948c 0364 6566  R.__init__...def
+0000ede0: 944b 124d 2a01 8794 8c0a 4661 7374 4d42  .K.M*.....FastMB
+0000edf0: 4152 2e46 946a 3209 0000 4d2c 014d 3101  AR.F.j2...M,.M1.
+0000ee00: 8794 8c0e 4661 7374 4d42 4152 2e46 5f73  ....FastMBAR.F_s
+0000ee10: 7464 946a 3209 0000 4d33 014d 3901 8794  td.j2...M3.M9...
+0000ee20: 8c0e 4661 7374 4d42 4152 2e46 5f63 6f76  ..FastMBAR.F_cov
+0000ee30: 946a 3209 0000 4d3b 014d 4101 8794 8c0f  .j2...M;.MA.....
+0000ee40: 4661 7374 4d42 4152 2e44 656c 7461 4694  FastMBAR.DeltaF.
+0000ee50: 6a32 0900 004d 4301 4d49 0187 948c 1346  j2...MC.MI.....F
+0000ee60: 6173 744d 4241 522e 4465 6c74 6146 5f73  astMBAR.DeltaF_s
+0000ee70: 7464 946a 3209 0000 4d4b 014d 5101 8794  td.j2...MK.MQ...
+0000ee80: 8c15 4661 7374 4d42 4152 2e6c 6f67 5f70  ..FastMBAR.log_p
+0000ee90: 726f 625f 6d69 7894 6a32 0900 004d 5301  rob_mix.j2...MS.
+0000eea0: 4d56 0187 948c 3446 6173 744d 4241 522e  MV....4FastMBAR.
+0000eeb0: 6361 6c63 756c 6174 655f 6672 6565 5f65  calculate_free_e
+0000eec0: 6e65 7267 6965 735f 6f66 5f70 6572 7475  nergies_of_pertu
+0000eed0: 7262 6564 5f73 7461 7465 7394 6a32 0900  rbed_states.j2..
+0000eee0: 004d 5801 4db3 0187 948c 0846 6173 744d  .MX.M......FastM
+0000eef0: 4241 5294 6a8f 0200 004b 084d b301 8794  BAR.j....K.M....
+0000ef00: 8c12 5f63 6f6d 7075 7465 5f6c 6f67 705f  .._compute_logp_
+0000ef10: 6f66 5f46 946a 3209 0000 4db5 014d ba01  of_F.j2...M..M..
+0000ef20: 8794 8c1c 5f63 6f6d 7075 7465 5f6c 6f73  ...._compute_los
+0000ef30: 735f 616e 645f 6772 6164 5f6f 665f 6446  s_and_grad_of_dF
+0000ef40: 946a 3209 0000 4dbd 014d d901 8794 8c25  .j2...M..M.....%
+0000ef50: 5f63 6f6d 7075 7465 5f6c 6f73 735f 616e  _compute_loss_an
+0000ef60: 645f 6772 6164 5f6f 665f 6446 5f69 6e5f  d_grad_of_dF_in_
+0000ef70: 6261 7463 6894 6a32 0900 004d dc01 4dfd  batch.j2...M..M.
+0000ef80: 0187 948c 245f 636f 6d70 7574 655f 6865  ....$_compute_he
+0000ef90: 7373 6961 6e5f 6c6f 675f 6c69 6b65 6c69  ssian_log_likeli
+0000efa0: 686f 6f64 5f6f 665f 4694 6a32 0900 004d  hood_of_F.j2...M
+0000efb0: 0002 4d05 0287 948c 2d5f 636f 6d70 7574  ..M.....-_comput
+0000efc0: 655f 6865 7373 6961 6e5f 6c6f 675f 6c69  e_hessian_log_li
+0000efd0: 6b65 6c69 686f 6f64 5f6f 665f 465f 696e  kelihood_of_F_in
+0000efe0: 5f62 6174 6368 946a 3209 0000 4d08 024d  _batch.j2...M..M
+0000eff0: 1702 8794 8c1b 5f63 6f6d 7075 7465 5f68  ......_compute_h
+0000f000: 6573 7369 616e 5f6c 6f73 735f 6f66 5f64  essian_loss_of_d
+0000f010: 4694 6a32 0900 004d 1a02 4d1f 0287 948c  F.j2...M..M.....
+0000f020: 245f 636f 6d70 7574 655f 6865 7373 6961  $_compute_hessia
+0000f030: 6e5f 6c6f 7373 5f6f 665f 6446 5f69 6e5f  n_loss_of_dF_in_
+0000f040: 6261 7463 6894 6a32 0900 004d 2202 4d27  batch.j2...M".M'
+0000f050: 0287 948c 0b5f 736f 6c76 655f 6d62 6172  ....._solve_mbar
+0000f060: 946a 3209 0000 4d2a 024d 5f02 8794 8c13  .j2...M*.M_.....
+0000f070: 5f62 6f6f 7473 7472 6170 5f63 6f6e 665f  _bootstrap_conf_
+0000f080: 6964 7894 6a32 0900 004d 6202 4d73 0287  idx.j2...Mb.Ms..
+0000f090: 948c 0b66 6d69 6e5f 6e65 7774 6f6e 946a  ...fmin_newton.j
+0000f0a0: 3209 0000 4d76 024d df02 8794 757d 9428  2...Mv.M....u}.(
+0000f0b0: 8c08 4661 7374 4d42 4152 946a e902 0000  ..FastMBAR.j....
+0000f0c0: 8c11 4661 7374 4d42 4152 2e5f 5f69 6e69  ..FastMBAR.__ini
+0000f0d0: 745f 5f94 6ae9 0200 008c 3446 6173 744d  t__.j.....4FastM
+0000f0e0: 4241 522e 6361 6c63 756c 6174 655f 6672  BAR.calculate_fr
+0000f0f0: 6565 5f65 6e65 7267 6965 735f 6f66 5f70  ee_energies_of_p
+0000f100: 6572 7475 7262 6564 5f73 7461 7465 7394  erturbed_states.
+0000f110: 6ae9 0200 0075 8c08 4661 7374 4d42 4152  j....u..FastMBAR
+0000f120: 9474 9473 7562 2e                        .t.sub.
```

### Comparing `fastmbar-1.0/docs/build/.doctrees/examples.doctree` & `fastmbar-1.0rc1/docs/build/.doctrees/examples.doctree`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/.doctrees/index.doctree` & `fastmbar-1.0rc1/docs/build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/.doctrees/references.doctree` & `fastmbar-1.0rc1/docs/build/.doctrees/references.doctree`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/.doctrees/usage.doctree` & `fastmbar-1.0rc1/docs/build/.doctrees/usage.doctree`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_images/Fig_1.png` & `fastmbar-1.0rc1/docs/build/_images/Fig_1.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_images/Fig_11.png` & `fastmbar-1.0rc1/docs/build/_images/Fig_11.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_images/Fig_2.png` & `fastmbar-1.0rc1/docs/build/_images/Fig_2.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_images/Fig_21.png` & `fastmbar-1.0rc1/docs/build/_images/Fig_21.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_images/PMF.png` & `fastmbar-1.0rc1/docs/build/_images/PMF.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_images/PMF1.png` & `fastmbar-1.0rc1/docs/build/_images/PMF1.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_images/energy_matrix.png` & `fastmbar-1.0rc1/docs/build/_images/energy_matrix.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_modules/index.html` & `fastmbar-1.0rc1/docs/build/_modules/index.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_modules/FastMBAR/fastmbar.html` & `fastmbar-1.0rc1/docs/build/_modules/FastMBAR/fastmbar.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_sources/butane_PMF.rst` & `fastmbar-1.0rc1/docs/build/_sources/butane_PMF.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_sources/dialanine_PMF.rst` & `fastmbar-1.0rc1/docs/build/_sources/dialanine_PMF.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_sources/examples.rst` & `fastmbar-1.0rc1/docs/build/_sources/examples.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_sources/index.rst` & `fastmbar-1.0rc1/docs/build/_sources/index.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_sources/references.rst` & `fastmbar-1.0rc1/docs/build/_sources/references.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_sources/usage.rst` & `fastmbar-1.0rc1/docs/build/_sources/usage.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/_sphinx_javascript_frameworks_compat.js` & `fastmbar-1.0rc1/docs/build/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/basic.css` & `fastmbar-1.0rc1/docs/build/_static/basic.css`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/clipboard.min.js` & `fastmbar-1.0rc1/docs/build/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/copybutton.css` & `fastmbar-1.0rc1/docs/build/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/copybutton.js` & `fastmbar-1.0rc1/docs/build/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/copybutton_funcs.js` & `fastmbar-1.0rc1/docs/build/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/doctools.js` & `fastmbar-1.0rc1/docs/build/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/jquery-3.6.0.js` & `fastmbar-1.0rc1/docs/build/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/jquery.js` & `fastmbar-1.0rc1/docs/build/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/language_data.js` & `fastmbar-1.0rc1/docs/build/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/logo.ai` & `fastmbar-1.0rc1/docs/build/_static/logo.ai`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/logo.eps` & `fastmbar-1.0rc1/docs/build/_static/logo.eps`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/logo.png` & `fastmbar-1.0rc1/docs/build/_static/logo.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/pygments.css` & `fastmbar-1.0rc1/docs/build/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/searchtools.js` & `fastmbar-1.0rc1/docs/build/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/underscore-1.13.1.js` & `fastmbar-1.0rc1/docs/build/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/underscore.js` & `fastmbar-1.0rc1/docs/build/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/webpack-macros.html` & `fastmbar-1.0rc1/docs/build/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/images/logo_binder.svg` & `fastmbar-1.0rc1/docs/build/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/images/logo_colab.png` & `fastmbar-1.0rc1/docs/build/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/images/logo_deepnote.svg` & `fastmbar-1.0rc1/docs/build/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/images/logo_jupyterhub.svg` & `fastmbar-1.0rc1/docs/build/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/da/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/da/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/da/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/de/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/de/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/de/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/el/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/el/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/el/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/es/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/es/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/es/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/et/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/et/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/et/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/id/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/id/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/id/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/it/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/it/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/it/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/no/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/no/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/no/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/te/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/te/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/te/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/th/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/th/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/th/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo` & `fastmbar-1.0rc1/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `fastmbar-1.0rc1/docs/build/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/scripts/bootstrap.js` & `fastmbar-1.0rc1/docs/build/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/scripts/bootstrap.js.map` & `fastmbar-1.0rc1/docs/build/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/scripts/pydata-sphinx-theme.js` & `fastmbar-1.0rc1/docs/build/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/scripts/pydata-sphinx-theme.js.map` & `fastmbar-1.0rc1/docs/build/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/scripts/sphinx-book-theme.js` & `fastmbar-1.0rc1/docs/build/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/scripts/sphinx-book-theme.js.map` & `fastmbar-1.0rc1/docs/build/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/styles/bootstrap.css` & `fastmbar-1.0rc1/docs/build/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/styles/pydata-sphinx-theme.css` & `fastmbar-1.0rc1/docs/build/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/styles/sphinx-book-theme.css` & `fastmbar-1.0rc1/docs/build/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `fastmbar-1.0rc1/docs/build/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/source/butane_PMF.rst` & `fastmbar-1.0rc1/docs/source/butane_PMF.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/source/conf.py` & `fastmbar-1.0rc1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/source/dialanine_PMF.rst` & `fastmbar-1.0rc1/docs/source/dialanine_PMF.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/source/examples.rst` & `fastmbar-1.0rc1/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/source/index.rst` & `fastmbar-1.0rc1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/source/references.rst` & `fastmbar-1.0rc1/docs/source/references.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/source/usage.rst` & `fastmbar-1.0rc1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/source/_static/logo.ai` & `fastmbar-1.0rc1/docs/source/_static/logo.ai`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/source/_static/logo.eps` & `fastmbar-1.0rc1/docs/source/_static/logo.eps`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/docs/source/_static/logo.png` & `fastmbar-1.0rc1/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/LICENSE` & `fastmbar-1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/README.rst` & `fastmbar-1.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.0/pyproject.toml` & `fastmbar-1.0rc1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "FastMBAR"
-version = "1.0"
+name = "fastmbar"
+version = "1.0-rc1"
 authors = [
   { name="Xinqiang Ding", email="Xinqiang.Ding@tufts.edu" }
 ]
 description = "A fast solver for large scale MBAR/UWHAM equations"
 readme = "README.rst"
 license = { file="LICENSE" }
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    'numpy>=1.20.0',
+    'numpy>=1.24.0',
     'scipy>=1.11.0',
-    'torch>=2.0.0',
-    'pytest>=7.4.0'
+    'torch>=2.0.0'
 ]
 
 [project.urls]
 "Homepage" = "https://fastmbar.readthedocs.io"
 "Bug Tracker" = "https://github.com/BrooksResearchGroup-UM/FastMBAR/issues"
 
 [tool.hatch.build]
```

### Comparing `fastmbar-1.0/PKG-INFO` & `fastmbar-1.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: FastMBAR
-Version: 1.0
+Name: fastmbar
+Version: 1.0rc1
 Summary: A fast solver for large scale MBAR/UWHAM equations
 Project-URL: Homepage, https://fastmbar.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/BrooksResearchGroup-UM/FastMBAR/issues
 Author-email: Xinqiang Ding <Xinqiang.Ding@tufts.edu>
 License: MIT License
         
         Copyright (c) 2018 Xinqiang Ding, Charles L. Brooks III
@@ -26,17 +26,16 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
-Requires-Dist: numpy>=1.20.0
-Requires-Dist: pytest>=7.4.0
+Requires-Python: >=3.10
+Requires-Dist: numpy>=1.24.0
 Requires-Dist: scipy>=1.11.0
 Requires-Dist: torch>=2.0.0
 Description-Content-Type: text/x-rst
 
 .. image:: https://travis-ci.org/xqding/FastMBAR.svg?branch=master
     :target: https://travis-ci.org/xqding/FastMBAR
```

