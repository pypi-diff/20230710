# Comparing `tmp/Nitrous-0.9.0.tar.gz` & `tmp/nitrous-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Nitrous-0.9.0.tar", last modified: Thu Sep 30 10:38:26 2021, max compression
+gzip compressed data, was "Nitrous-0.9.3.tar", last modified: Mon Jul 10 20:46:40 2023, max compression
```

## Comparing `Nitrous-0.9.0.tar` & `nitrous-0.9.3.tar`

### file list

```diff
@@ -1,522 +1,524 @@
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.119788 Nitrous-0.9.0/
--rw-r-----   0 drocco    (1000) drocco    (1000)   104045 2019-07-06 00:29:02.000000 Nitrous-0.9.0/CHANGELOG.txt
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1348 2019-07-02 13:55:25.000000 Nitrous-0.9.0/CONTRIBUTORS.txt
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1201 2019-07-02 13:55:25.000000 Nitrous-0.9.0/LICENSE.txt
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1293 2019-07-02 13:55:25.000000 Nitrous-0.9.0/MANIFEST.in
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.027787 Nitrous-0.9.0/Nitrous.egg-info/
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1362 2021-09-30 10:38:25.000000 Nitrous-0.9.0/Nitrous.egg-info/PKG-INFO
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2021-09-30 10:38:25.000000 Nitrous-0.9.0/Nitrous.egg-info/SOURCES.txt
--rw-r--r--   0 drocco    (1000) drocco    (1000)       73 2021-09-30 10:38:25.000000 Nitrous-0.9.0/Nitrous.egg-info/dependency_links.txt
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1263 2021-09-30 10:38:25.000000 Nitrous-0.9.0/Nitrous.egg-info/entry_points.txt
--rw-r--r--   0 drocco    (1000) drocco    (1000)        1 2020-01-29 18:18:06.000000 Nitrous-0.9.0/Nitrous.egg-info/not-zip-safe
--rw-r--r--   0 drocco    (1000) drocco    (1000)      132 2021-09-30 10:38:25.000000 Nitrous-0.9.0/Nitrous.egg-info/requires.txt
--rw-r--r--   0 drocco    (1000) drocco    (1000)       17 2021-09-30 10:38:25.000000 Nitrous-0.9.0/Nitrous.egg-info/top_level.txt
--rw-r-----   0 drocco    (1000) drocco    (1000)     1362 2021-09-30 10:38:26.119788 Nitrous-0.9.0/PKG-INFO
--rw-r-----   0 drocco    (1000) drocco    (1000)      206 2020-06-18 23:52:54.000000 Nitrous-0.9.0/README.md
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.027787 Nitrous-0.9.0/doc/
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2051 2019-07-02 13:55:25.000000 Nitrous-0.9.0/doc/README.txt
--rwxr-xr-x   0 drocco    (1000) drocco    (1000)      473 2019-07-02 13:55:25.000000 Nitrous-0.9.0/doc/build_api_docs.sh
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1548 2019-07-02 13:55:25.000000 Nitrous-0.9.0/doc/doc.ini
--rw-r-----   0 drocco    (1000) drocco    (1000)       79 2021-09-30 10:38:26.119788 Nitrous-0.9.0/setup.cfg
--rw-r-----   0 drocco    (1000) drocco    (1000)     3421 2021-09-30 10:37:32.000000 Nitrous-0.9.0/setup.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      651 2019-07-02 13:55:25.000000 Nitrous-0.9.0/test.cfg
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.031787 Nitrous-0.9.0/tests/
--rw-r-----   0 drocco    (1000) drocco    (1000)        0 2020-06-18 23:52:54.000000 Nitrous-0.9.0/tests/__init__.py
--rw-r-----   0 drocco    (1000) drocco    (1000)      557 2020-12-02 23:05:11.000000 Nitrous-0.9.0/tests/conftest.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    14057 2021-06-21 20:14:44.000000 Nitrous-0.9.0/tests/test_expose.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     8471 2020-12-02 23:05:11.000000 Nitrous-0.9.0/tests/test_expose_with_identity.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     2292 2020-12-02 23:05:11.000000 Nitrous-0.9.0/tests/test_expose_with_transaction.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     5288 2021-06-21 20:14:44.000000 Nitrous-0.9.0/tests/test_expose_with_validate.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     2527 2021-01-12 20:53:26.000000 Nitrous-0.9.0/tests/test_rest.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     4710 2020-12-02 23:05:11.000000 Nitrous-0.9.0/tests/test_validate.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.031787 Nitrous-0.9.0/tools/
--rwxr-x---   0 drocco    (1000) drocco    (1000)      570 2020-06-18 23:52:54.000000 Nitrous-0.9.0/tools/codename.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     1601 2020-06-18 23:52:54.000000 Nitrous-0.9.0/tools/test_all_quickstarts.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    16987 2020-06-18 23:52:54.000000 Nitrous-0.9.0/tools/tgsetup.py
--rw-r-----   0 drocco    (1000) drocco    (1000)      378 2020-06-18 23:52:54.000000 Nitrous-0.9.0/tools/toolbox-start.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.035787 Nitrous-0.9.0/turbogears/
--rw-r-----   0 drocco    (1000) drocco    (1000)     1362 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/__init__.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.035787 Nitrous-0.9.0/turbogears/command/
--rw-r--r--   0 drocco    (1000) drocco    (1000)       78 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/command/__init__.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    11511 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/command/base.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    20674 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/command/i18n.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     2538 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/command/info.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     6216 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/command/kid2genshi.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     4233 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/command/sacommand.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    11147 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/config.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    21492 2021-06-21 21:49:20.000000 Nitrous-0.9.0/turbogears/controllers.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.035787 Nitrous-0.9.0/turbogears/database/
--rw-r-----   0 drocco    (1000) drocco    (1000)     2304 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/database/__init__.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     5852 2020-06-19 00:58:07.000000 Nitrous-0.9.0/turbogears/database/sqlalchemy_support.py
--rw-r-----   0 drocco    (1000) drocco    (1000)      479 2021-01-12 02:06:44.000000 Nitrous-0.9.0/turbogears/decorator.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     1662 2020-11-30 21:29:57.000000 Nitrous-0.9.0/turbogears/dispatchers.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    11652 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/docgen.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     8186 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/errorhandling.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      130 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/filters.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     3729 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/finddata.py
--rw-r-----   0 drocco    (1000) drocco    (1000)      677 2019-07-02 15:15:53.000000 Nitrous-0.9.0/turbogears/hooks.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.035787 Nitrous-0.9.0/turbogears/i18n/
--rw-r--r--   0 drocco    (1000) drocco    (1000)      575 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/__init__.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.083788 Nitrous-0.9.0/turbogears/i18n/data/
--rw-r--r--   0 drocco    (1000) drocco    (1000)      831 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/TurboGears.pot
--rw-r--r--   0 drocco    (1000) drocco    (1000)       19 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/__init__.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      877 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/af.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      876 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/af_ZA.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    12416 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/am.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    12437 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/am_ET.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15683 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_AE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_BH.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15680 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_DZ.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_EG.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15683 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_IN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_IQ.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    16078 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_JO.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_KW.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    16078 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_LB.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_LY.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15680 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_MA.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_OM.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15914 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_QA.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15914 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_SA.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_SD.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    16078 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_SY.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15908 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_TN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15914 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ar_YE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1894 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/be.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1897 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/be_BY.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    20441 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/bg.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    20444 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/bg_BG.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2167 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/bn.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2150 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/bn_IN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     7319 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ca.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     7322 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ca_ES.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9976 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/cs.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9979 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/cs_CZ.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6863 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/da.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6866 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/da_DK.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.023787 Nitrous-0.9.0/turbogears/i18n/data/de/
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.083788 Nitrous-0.9.0/turbogears/i18n/data/de/LC_MESSAGES/
--rw-r--r--   0 drocco    (1000) drocco    (1000)      806 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/de/LC_MESSAGES/TurboGears.mo
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1010 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/de/LC_MESSAGES/TurboGears.po
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8596 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/de.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8611 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/de_AT.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8623 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/de_BE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     3855 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/de_CH.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8599 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/de_DE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8599 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/de_LU.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    22153 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/el.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    22156 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/el_GR.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14894 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14878 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_AU.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14915 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_BE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14893 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_BW.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14896 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_CA.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14894 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_GB.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14894 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_HK.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14893 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_IE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14893 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_IN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14880 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_MT.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14878 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_NZ.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14881 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_PH.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14884 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_SG.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14897 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_US.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14896 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_US_POSIX.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14897 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_VI.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14893 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_ZA.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14893 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/en_ZW.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     7744 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/eo.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8235 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_AR.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_BO.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_CL.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_CO.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_CR.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_DO.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_EC.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_ES.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_GT.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_HN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_MX.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_NI.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_PA.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_PE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_PR.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_PY.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_SV.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8239 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_US.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_UY.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/es_VE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6290 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/et.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6293 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/et_EE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      882 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/eu.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      919 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/eu_ES.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    28717 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/fa.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8295 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/fa_AF.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    28761 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/fa_IR.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     7097 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/fi.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     7100 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/fi_FI.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      914 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/fo.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      917 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/fo_FO.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9519 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/fr.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9518 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/fr_BE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9506 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/fr_CA.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9519 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/fr_CH.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9522 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/fr_FR.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9518 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/fr_LU.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9701 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ga.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9700 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ga_IE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      889 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/gl.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      888 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/gl_ES.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1993 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/gu.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1976 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/gu_IN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    10058 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/gv.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    10057 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/gv_GB.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    17877 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/he.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    17880 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/he_IL.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    19593 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/hi.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    19576 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/hi_IN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6680 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/hr.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6683 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/hr_HR.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9192 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/hu.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9195 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/hu_HU.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2072 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/hy.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2075 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/hy_AM.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2071 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/hy_AM_REVISED.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9750 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/id.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9749 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/id_ID.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      984 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/is.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      987 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/is_IS.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6845 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/it.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6849 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/it_CH.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6848 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/it_IT.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    17814 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ja.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    17817 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ja_JP.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1835 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/kk.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1838 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/kk_KZ.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      934 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/kl.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      933 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/kl_GL.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2024 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/kn.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2007 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/kn_IN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15459 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ko.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15449 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ko_KR.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9775 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/kok.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    15432 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/kok_IN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      917 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/kw.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      916 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/kw_GB.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     7222 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/lt.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     7225 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/lt_LT.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     7467 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/lv.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     7470 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/lv_LV.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1915 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/mk.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1918 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/mk_MK.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9674 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/mr.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9657 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/mr_IN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     5628 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ms.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     5598 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ms_BN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     5627 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ms_MY.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    16356 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/mt.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    16359 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/mt_MT.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6984 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/nb.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6987 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/nb_NO.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6873 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/nl.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6876 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/nl_BE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6876 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/nl_NL.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      911 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/nn.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      914 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/nn_NO.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6984 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/no.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6987 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/no_NO.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      913 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/om.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      914 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/om_ET.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      914 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/om_KE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1856 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/pa.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1839 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/pa_IN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6840 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/pl.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6843 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/pl_PL.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6091 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ps.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6141 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ps_AF.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     7802 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/pt.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     7789 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/pt_BR.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2733 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/pt_PT.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6672 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ro.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6675 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ro_RO.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    28474 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ru.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    28481 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ru_RU.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    28502 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ru_UA.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6983 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sh.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6986 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sh_YU.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     7265 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sk.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     7268 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sk_SK.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.023787 Nitrous-0.9.0/turbogears/i18n/data/sl/
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.083788 Nitrous-0.9.0/turbogears/i18n/data/sl/LC_MESSAGES/
--rw-r--r--   0 drocco    (1000) drocco    (1000)      800 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sl/LC_MESSAGES/TurboGears.mo
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1003 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sl/LC_MESSAGES/TurboGears.po
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6915 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sl.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6918 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sl_SI.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2846 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/so.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2849 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/so_DJ.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2849 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/so_ET.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2849 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/so_KE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2849 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/so_SO.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      887 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sq.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      890 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sq_AL.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    16831 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sr.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    16834 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sr_YU.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    12296 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sv.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    12299 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sv_FI.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    12299 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sv_SE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2481 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sw.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2484 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sw_KE.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2484 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/sw_TZ.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    20542 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ta.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    20525 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ta_IN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2162 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/te.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2145 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/te_IN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    21761 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/th.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    21764 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/th_TH.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    12428 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ti.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    12413 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ti_ER.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    12461 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/ti_ET.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9075 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/tr.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9078 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/tr_TR.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    27036 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/uk.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    27039 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/uk_UA.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6467 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/vi.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6470 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/vi_VN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14539 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/zh.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    14531 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/zh_CN.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    11757 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/zh_HK.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    11757 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/zh_MO.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1468 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/zh_SG.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)    11791 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/data/zh_TW.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     6479 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/i18n/format.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     3373 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/kidutils.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.083788 Nitrous-0.9.0/turbogears/i18n/pygettext/
--rw-r--r--   0 drocco    (1000) drocco    (1000)       11 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/pygettext/__init__.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     6282 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/i18n/pygettext/catalog.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     5775 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/i18n/pygettext/msgfmt.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    28753 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/i18n/pygettext/pygettext.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.083788 Nitrous-0.9.0/turbogears/i18n/sagettext/
--rw-r-----   0 drocco    (1000) drocco    (1000)     4010 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/i18n/sagettext/__init__.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     1051 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/i18n/sagettext/model.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.087788 Nitrous-0.9.0/turbogears/i18n/tests/
--rw-r-----   0 drocco    (1000) drocco    (1000)      840 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/i18n/tests/__init__.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     3425 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/i18n/tests/test_format.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     1164 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/i18n/tests/test_kidutils.py
--rw-r-----   0 drocco    (1000) drocco    (1000)      654 2019-07-02 15:15:53.000000 Nitrous-0.9.0/turbogears/i18n/tests/test_so_gettext.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     1521 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/i18n/tests/test_tg_gettext.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      230 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/tests/test_toolboxadmi18n.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      292 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/i18n/tests/test_utils.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     5378 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/i18n/tg_gettext.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     3874 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/i18n/utils.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.087788 Nitrous-0.9.0/turbogears/identity/
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1650 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/identity/__init__.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     7105 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/identity/base.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    10757 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/identity/conditions.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     4325 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/identity/exceptions.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    15683 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/identity/saprovider.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.087788 Nitrous-0.9.0/turbogears/identity/tests/
--rw-r-----   0 drocco    (1000) drocco    (1000)      487 2019-07-02 15:15:53.000000 Nitrous-0.9.0/turbogears/identity/tests/__init__.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     9038 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/identity/tests/test_identity.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    25091 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/identity/tests/test_identity_sa.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     1014 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/identity/tests/test_visit.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     7855 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/identity/tests/test_visit_sa.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     9375 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/identity/visitor.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     1600 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/release.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.087788 Nitrous-0.9.0/turbogears/rest/
--rw-r-----   0 drocco    (1000) drocco    (1000)     5556 2021-01-12 20:53:26.000000 Nitrous-0.9.0/turbogears/rest/__init__.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      559 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/scheduler.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    11943 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/startup.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.087788 Nitrous-0.9.0/turbogears/static/
--rw-r--r--   0 drocco    (1000) drocco    (1000)        0 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/__init__.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.087788 Nitrous-0.9.0/turbogears/static/css/
--rw-r--r--   0 drocco    (1000) drocco    (1000)        0 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/css/__init__.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1157 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/css/interpreter.css
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1319 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/css/toolbox.css
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1243 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/css/widget.css
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.095788 Nitrous-0.9.0/turbogears/static/images/
--rw-r--r--   0 drocco    (1000) drocco    (1000)        0 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/images/__init__.py
--rw-r-----   0 drocco    (1000) drocco    (1000)      363 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/add.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     2734 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/admi18n.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      300 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/arrow_down.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      206 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/arrow_down_small.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     1024 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/arrow_left.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      280 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/arrow_right.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      261 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/arrow_up.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      205 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/arrow_up_small.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     1989 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/catwalk.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     2996 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/catwalk_logo.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      181 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/catwalk_logo_bg.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      222 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/column_chooser.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     3689 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/designer.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      610 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/discard.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      412 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/edit.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      665 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/file.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     1070 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/folder.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     2323 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/identity.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     3510 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/info.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     1410 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/play.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      341 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/remove.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      301 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/save.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     2679 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/shell.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      993 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/small_gear.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     1503 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/stop.png
--rw-r--r--   0 drocco    (1000) drocco    (1000)      121 2019-07-02 13:45:17.000000 Nitrous-0.9.0/turbogears/static/images/table.gif
--rw-r-----   0 drocco    (1000) drocco    (1000)     2781 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/tg_power.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     4010 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/tg_under_the_hood.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     2529 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/tg_under_the_hood_sans_gear.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     2633 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/toolbox_logo.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      147 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/toolbox_top_baggrund.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      151 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/toolbox_top_vertical_line.png
--rw-r-----   0 drocco    (1000) drocco    (1000)    33365 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/top.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      525 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/top_bg.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      153 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/transp.png
--rw-r-----   0 drocco    (1000) drocco    (1000)      672 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/trash.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     4179 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/static/images/widgets.png
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.095788 Nitrous-0.9.0/turbogears/static/js/
--rw-r--r--   0 drocco    (1000) drocco    (1000)        0 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/js/__init__.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      151 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/js/i18n_base.js
--rw-r--r--   0 drocco    (1000) drocco    (1000)     4348 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/js/interpreter.js
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.095788 Nitrous-0.9.0/turbogears/static/js/tool-man/
--rw-r--r--   0 drocco    (1000) drocco    (1000)      879 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/js/tool-man/cookies.js
--rw-r--r--   0 drocco    (1000) drocco    (1000)     4138 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/js/tool-man/coordinates.js
--rw-r--r--   0 drocco    (1000) drocco    (1000)     4717 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/js/tool-man/core.js
--rw-r--r--   0 drocco    (1000) drocco    (1000)      528 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/js/tool-man/css.js
--rw-r--r--   0 drocco    (1000) drocco    (1000)     7124 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/js/tool-man/drag.js
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2476 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/js/tool-man/dragsort.js
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1192 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/static/js/tool-man/events.js
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.103788 Nitrous-0.9.0/turbogears/tests/
--rw-r-----   0 drocco    (1000) drocco    (1000)      446 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/__init__.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.103788 Nitrous-0.9.0/turbogears/tests/catwalk_models/
--rw-r--r--   0 drocco    (1000) drocco    (1000)        0 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/catwalk_models/__init__.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1230 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/catwalk_models/browse.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.103788 Nitrous-0.9.0/turbogears/tests/catwalk_models/catwalk-session/
--rw-r-----   0 drocco    (1000) drocco    (1000)      237 2019-07-02 14:03:58.000000 Nitrous-0.9.0/turbogears/tests/catwalk_models/catwalk-session/session.pkl
--rw-r--r--   0 drocco    (1000) drocco    (1000)      479 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/catwalk_models/model_list.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      426 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/catwalk_models/model_structure.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      409 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/catwalk_models/single_join.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      488 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/config.cfg
--rw-r--r--   0 drocco    (1000) drocco    (1000)       84 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/tests/configfile.cfg
--rw-r--r--   0 drocco    (1000) drocco    (1000)      667 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/form.html
--rw-r--r--   0 drocco    (1000) drocco    (1000)      441 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/form.kid
--rw-r-----   0 drocco    (1000) drocco    (1000)       75 2020-01-13 15:36:07.000000 Nitrous-0.9.0/turbogears/tests/genshi_new_text_format.txt
--rw-r-----   0 drocco    (1000) drocco    (1000)       60 2020-01-13 15:29:36.000000 Nitrous-0.9.0/turbogears/tests/genshi_old_text_format.txt
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.023787 Nitrous-0.9.0/turbogears/tests/locale/
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.023787 Nitrous-0.9.0/turbogears/tests/locale/en/
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.103788 Nitrous-0.9.0/turbogears/tests/locale/en/LC_MESSAGES/
--rw-r--r--   0 drocco    (1000) drocco    (1000)      377 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/locale/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 drocco    (1000) drocco    (1000)      589 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/locale/en/LC_MESSAGES/messages.po
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.023787 Nitrous-0.9.0/turbogears/tests/locale/fi/
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.103788 Nitrous-0.9.0/turbogears/tests/locale/fi/LC_MESSAGES/
--rw-r-----   0 drocco    (1000) drocco    (1000)     1616 2019-07-02 14:03:58.000000 Nitrous-0.9.0/turbogears/tests/locale/fi/LC_MESSAGES/messages.mo
--rw-r--r--   0 drocco    (1000) drocco    (1000)      638 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/locale/fi/LC_MESSAGES/messages.po
--rw-r--r--   0 drocco    (1000) drocco    (1000)       96 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/othertemplate.kid
--rw-r--r--   0 drocco    (1000) drocco    (1000)      148 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/paginate.html
--rw-r--r--   0 drocco    (1000) drocco    (1000)      209 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/simple.html
--rw-r--r--   0 drocco    (1000) drocco    (1000)      157 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/simple.kid
--rw-r-----   0 drocco    (1000) drocco    (1000)     6197 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/test_catwalk.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6627 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/test_command_i18n.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     2808 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/test_config.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    36387 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/test_controllers.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     3057 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/test_decorator.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    12899 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/test_errorhandling.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     4547 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/test_expose.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    44646 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/test_paginate.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     4138 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/test_restmethod.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     3249 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/test_safemultipart.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     4411 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/test_session_mapper.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    11897 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/test_sqlalchemy.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     1829 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/test_testutil.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    15197 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/test_util.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     5141 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/test_validators.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    20752 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/tests/test_view.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)       34 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/tests/textfmt.tmpl
--rw-r-----   0 drocco    (1000) drocco    (1000)    10051 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/testutil.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.103788 Nitrous-0.9.0/turbogears/toolbox/
--rw-r-----   0 drocco    (1000) drocco    (1000)       65 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/toolbox/__init__.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.107788 Nitrous-0.9.0/turbogears/toolbox/admi18n/
--rw-r-----   0 drocco    (1000) drocco    (1000)    11148 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/toolbox/admi18n/__init__.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     4358 2019-07-02 15:15:53.000000 Nitrous-0.9.0/turbogears/toolbox/admi18n/internationalization.html
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8824 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/admi18n/language.html
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8589 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/admi18n/languageManagement.html
--rw-r--r--   0 drocco    (1000) drocco    (1000)     5961 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/admi18n/po_view.html
--rw-r--r--   0 drocco    (1000) drocco    (1000)     5720 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/admi18n/stringCollection.html
--rw-r-----   0 drocco    (1000) drocco    (1000)     5441 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/toolbox/base.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.107788 Nitrous-0.9.0/turbogears/toolbox/catwalk/
--rw-r-----   0 drocco    (1000) drocco    (1000)    42486 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/__init__.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    11740 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/browse.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     4683 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/browse_grid.html
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6123 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/catwalk.html
--rw-r--r--   0 drocco    (1000) drocco    (1000)     8055 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/columns.html
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.023787 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.107788 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/css/
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2583 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/css/catwalk.css
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.107788 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/
--rw-r-----   0 drocco    (1000) drocco    (1000)     2779 2019-07-02 15:15:53.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/browse.js
--rw-r--r--   0 drocco    (1000) drocco    (1000)    45693 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/catwalk.js
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.111788 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9409 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/AmiJS.js
--rw-r--r--   0 drocco    (1000) drocco    (1000)       49 2019-07-02 13:45:16.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/blank.gif
--rw-r--r--   0 drocco    (1000) drocco    (1000)      200 2019-07-02 13:45:16.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/close.gif
--rw-r--r--   0 drocco    (1000) drocco    (1000)      999 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/greybox.css
--rw-r--r--   0 drocco    (1000) drocco    (1000)     4741 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/greybox.js
--rw-r--r--   0 drocco    (1000) drocco    (1000)     4296 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/greybox__.js
--rw-r--r--   0 drocco    (1000) drocco    (1000)     4843 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/greybox_inline.js
--rw-r-----   0 drocco    (1000) drocco    (1000)     6336 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/logo.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     2960 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/overlay.png
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1742 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/console.html
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.111788 Nitrous-0.9.0/turbogears/toolbox/designer/
--rw-r-----   0 drocco    (1000) drocco    (1000)    13003 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/toolbox/designer/__init__.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     4946 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/designer/modelDesigner.html
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.027787 Nitrous-0.9.0/turbogears/toolbox/designer/static/
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.111788 Nitrous-0.9.0/turbogears/toolbox/designer/static/css/
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2464 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/css/style.css
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.111788 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.111788 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/images/
--rw-r--r--   0 drocco    (1000) drocco    (1000)       64 2019-07-02 13:45:16.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/images/back.gif
--rw-r-----   0 drocco    (1000) drocco    (1000)     2839 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/images/shadow.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     2961 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/images/shadow_bottom.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     2893 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/images/shadow_corner.png
--rw-r-----   0 drocco    (1000) drocco    (1000)     2989 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/images/shadow_right.png
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2426 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/index.html
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.111788 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/
--rw-r-----   0 drocco    (1000) drocco    (1000)     3981 2019-07-02 14:03:58.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/ajax.js
--rw-r-----   0 drocco    (1000) drocco    (1000)     2397 2019-07-02 15:15:53.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/animator.js
--rw-r-----   0 drocco    (1000) drocco    (1000)     1868 2019-07-02 15:15:53.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/generic.js
--rw-r-----   0 drocco    (1000) drocco    (1000)     6146 2019-07-02 15:15:53.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/io.js
--rw-r-----   0 drocco    (1000) drocco    (1000)    16064 2019-07-02 15:15:53.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/main.js
--rw-r-----   0 drocco    (1000) drocco    (1000)    23822 2019-07-02 15:15:53.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/objects.js
--rw-r-----   0 drocco    (1000) drocco    (1000)     1098 2019-07-02 15:15:53.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/settings.js
--rw-r-----   0 drocco    (1000) drocco    (1000)     3473 2019-07-02 15:15:53.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/sql_types.js
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.115788 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/styles/
--rw-r--r--   0 drocco    (1000) drocco    (1000)     3526 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/styles/bar.css
--rw-r--r--   0 drocco    (1000) drocco    (1000)     3077 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/styles/style.css
--rw-r-----   0 drocco    (1000) drocco    (1000)      220 2019-07-02 15:15:53.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/styles/style.js
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.115788 Nitrous-0.9.0/turbogears/toolbox/designer/static/images/
--rw-r-----   0 drocco    (1000) drocco    (1000)      750 2019-07-02 13:46:08.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/images/info.png
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.115788 Nitrous-0.9.0/turbogears/toolbox/designer/static/javascript/
--rw-r--r--   0 drocco    (1000) drocco    (1000)    55991 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/javascript/modelDesigner.js
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.115788 Nitrous-0.9.0/turbogears/toolbox/designer/static/sessions/
--rw-r--r--   0 drocco    (1000) drocco    (1000)     6037 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/sessions/Survey.js
--rw-r--r--   0 drocco    (1000) drocco    (1000)     3271 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/sessions/TurboTunes.js
--rw-r--r--   0 drocco    (1000) drocco    (1000)     9963 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/designer/static/sessions/WebShop.js
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1099 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/info.html
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1871 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/main.html
--rw-r--r--   0 drocco    (1000) drocco    (1000)     1393 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/master.html
--rw-r-----   0 drocco    (1000) drocco    (1000)     2733 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/toolbox/shell.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     4305 2019-07-02 13:55:25.000000 Nitrous-0.9.0/turbogears/toolbox/widgets.html
--rw-r-----   0 drocco    (1000) drocco    (1000)    25291 2021-06-21 20:14:44.000000 Nitrous-0.9.0/turbogears/util.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     8769 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/validators.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.115788 Nitrous-0.9.0/turbogears/view/
--rw-r--r--   0 drocco    (1000) drocco    (1000)       68 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/view/__init__.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    19317 2021-06-21 21:49:20.000000 Nitrous-0.9.0/turbogears/view/base.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)     2348 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/view/genshisupport.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     1550 2021-01-12 20:52:24.000000 Nitrous-0.9.0/turbogears/view/json.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.115788 Nitrous-0.9.0/turbogears/view/templates/
--rw-r--r--   0 drocco    (1000) drocco    (1000)        0 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/view/templates/__init__.py
--rw-r--r--   0 drocco    (1000) drocco    (1000)      749 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/view/templates/sitetemplate.kid
--rw-r-----   0 drocco    (1000) drocco    (1000)      896 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/view/text.py
-drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2021-09-30 10:38:26.119788 Nitrous-0.9.0/turbogears/visit/
--rw-r--r--   0 drocco    (1000) drocco    (1000)      528 2019-07-02 13:55:26.000000 Nitrous-0.9.0/turbogears/visit/__init__.py
--rw-r-----   0 drocco    (1000) drocco    (1000)    12619 2021-09-30 10:37:32.000000 Nitrous-0.9.0/turbogears/visit/api.py
--rw-r-----   0 drocco    (1000) drocco    (1000)     3720 2020-06-18 23:52:54.000000 Nitrous-0.9.0/turbogears/visit/savisit.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.669853 Nitrous-0.9.3/
+-rw-r-----   0 drocco    (1000) drocco    (1000)   104045 2019-07-06 00:29:02.000000 Nitrous-0.9.3/CHANGELOG.txt
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1348 2019-07-02 13:55:25.000000 Nitrous-0.9.3/CONTRIBUTORS.txt
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1201 2019-07-02 13:55:25.000000 Nitrous-0.9.3/LICENSE.txt
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1293 2019-07-02 13:55:25.000000 Nitrous-0.9.3/MANIFEST.in
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.565852 Nitrous-0.9.3/Nitrous.egg-info/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1273 2023-07-10 20:46:39.000000 Nitrous-0.9.3/Nitrous.egg-info/PKG-INFO
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15775 2023-07-10 20:46:39.000000 Nitrous-0.9.3/Nitrous.egg-info/SOURCES.txt
+-rw-r--r--   0 drocco    (1000) drocco    (1000)       73 2023-07-10 20:46:39.000000 Nitrous-0.9.3/Nitrous.egg-info/dependency_links.txt
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1263 2023-07-10 20:46:39.000000 Nitrous-0.9.3/Nitrous.egg-info/entry_points.txt
+-rw-r--r--   0 drocco    (1000) drocco    (1000)        1 2020-01-29 18:18:06.000000 Nitrous-0.9.3/Nitrous.egg-info/not-zip-safe
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      132 2023-07-10 20:46:39.000000 Nitrous-0.9.3/Nitrous.egg-info/requires.txt
+-rw-r--r--   0 drocco    (1000) drocco    (1000)       17 2023-07-10 20:46:39.000000 Nitrous-0.9.3/Nitrous.egg-info/top_level.txt
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1273 2023-07-10 20:46:40.669853 Nitrous-0.9.3/PKG-INFO
+-rw-r-----   0 drocco    (1000) drocco    (1000)      206 2020-06-18 23:52:54.000000 Nitrous-0.9.3/README.md
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.565852 Nitrous-0.9.3/doc/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2051 2019-07-02 13:55:25.000000 Nitrous-0.9.3/doc/README.txt
+-rwxr-xr-x   0 drocco    (1000) drocco    (1000)      473 2019-07-02 13:55:25.000000 Nitrous-0.9.3/doc/build_api_docs.sh
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1548 2019-07-02 13:55:25.000000 Nitrous-0.9.3/doc/doc.ini
+-rw-r-----   0 drocco    (1000) drocco    (1000)       79 2023-07-10 20:46:40.669853 Nitrous-0.9.3/setup.cfg
+-rw-r-----   0 drocco    (1000) drocco    (1000)     3421 2023-07-10 20:43:30.000000 Nitrous-0.9.3/setup.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      651 2019-07-02 13:55:25.000000 Nitrous-0.9.3/test.cfg
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.569852 Nitrous-0.9.3/tests/
+-rw-r-----   0 drocco    (1000) drocco    (1000)        0 2020-06-18 23:52:54.000000 Nitrous-0.9.3/tests/__init__.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)      557 2020-12-02 23:05:11.000000 Nitrous-0.9.3/tests/conftest.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    14797 2023-07-10 20:43:30.000000 Nitrous-0.9.3/tests/test_expose.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     8471 2020-12-02 23:05:11.000000 Nitrous-0.9.3/tests/test_expose_with_identity.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2292 2020-12-02 23:05:11.000000 Nitrous-0.9.3/tests/test_expose_with_transaction.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     5288 2021-06-21 20:14:44.000000 Nitrous-0.9.3/tests/test_expose_with_validate.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     3215 2023-07-10 20:41:23.000000 Nitrous-0.9.3/tests/test_resource_exception_handling.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1433 2023-07-10 20:41:23.000000 Nitrous-0.9.3/tests/test_resource_init_exception_handling.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2527 2021-01-12 20:53:26.000000 Nitrous-0.9.3/tests/test_rest.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     4710 2020-12-02 23:05:11.000000 Nitrous-0.9.3/tests/test_validate.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.569852 Nitrous-0.9.3/tools/
+-rwxr-x---   0 drocco    (1000) drocco    (1000)      570 2020-06-18 23:52:54.000000 Nitrous-0.9.3/tools/codename.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1601 2020-06-18 23:52:54.000000 Nitrous-0.9.3/tools/test_all_quickstarts.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    16987 2020-06-18 23:52:54.000000 Nitrous-0.9.3/tools/tgsetup.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)      378 2020-06-18 23:52:54.000000 Nitrous-0.9.3/tools/toolbox-start.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.573852 Nitrous-0.9.3/turbogears/
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1362 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/__init__.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.573852 Nitrous-0.9.3/turbogears/command/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)       78 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/command/__init__.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    11511 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/command/base.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    20674 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/command/i18n.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2538 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/command/info.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     6216 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/command/kid2genshi.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     4233 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/command/sacommand.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    11147 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/config.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    21466 2023-07-10 20:43:30.000000 Nitrous-0.9.3/turbogears/controllers.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.573852 Nitrous-0.9.3/turbogears/database/
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2304 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/database/__init__.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     5852 2020-06-19 00:58:07.000000 Nitrous-0.9.3/turbogears/database/sqlalchemy_support.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)      479 2021-01-12 02:06:44.000000 Nitrous-0.9.3/turbogears/decorator.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1662 2020-11-30 21:29:57.000000 Nitrous-0.9.3/turbogears/dispatchers.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    11652 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/docgen.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     8186 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/errorhandling.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      130 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/filters.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     3729 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/finddata.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)      677 2019-07-02 15:15:53.000000 Nitrous-0.9.3/turbogears/hooks.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.573852 Nitrous-0.9.3/turbogears/i18n/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      575 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/__init__.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.629853 Nitrous-0.9.3/turbogears/i18n/data/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      831 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/TurboGears.pot
+-rw-r--r--   0 drocco    (1000) drocco    (1000)       19 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/__init__.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      877 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/af.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      876 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/af_ZA.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    12416 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/am.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    12437 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/am_ET.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15683 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_AE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_BH.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15680 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_DZ.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_EG.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15683 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_IN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_IQ.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    16078 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_JO.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_KW.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    16078 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_LB.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_LY.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15680 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_MA.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_OM.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15914 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_QA.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15914 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_SA.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15686 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_SD.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    16078 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_SY.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15908 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_TN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15914 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ar_YE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1894 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/be.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1897 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/be_BY.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    20441 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/bg.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    20444 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/bg_BG.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2167 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/bn.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2150 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/bn_IN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     7319 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ca.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     7322 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ca_ES.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9976 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/cs.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9979 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/cs_CZ.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6863 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/da.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6866 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/da_DK.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.557852 Nitrous-0.9.3/turbogears/i18n/data/de/
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.629853 Nitrous-0.9.3/turbogears/i18n/data/de/LC_MESSAGES/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      806 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/de/LC_MESSAGES/TurboGears.mo
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1010 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/de/LC_MESSAGES/TurboGears.po
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8596 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/de.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8611 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/de_AT.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8623 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/de_BE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     3855 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/de_CH.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8599 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/de_DE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8599 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/de_LU.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    22153 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/el.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    22156 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/el_GR.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14894 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14878 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_AU.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14915 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_BE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14893 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_BW.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14896 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_CA.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14894 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_GB.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14894 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_HK.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14893 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_IE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14893 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_IN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14880 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_MT.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14878 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_NZ.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14881 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_PH.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14884 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_SG.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14897 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_US.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14896 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_US_POSIX.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14897 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_VI.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14893 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_ZA.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14893 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/en_ZW.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     7744 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/eo.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8235 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_AR.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_BO.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_CL.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_CO.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_CR.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_DO.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_EC.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_ES.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_GT.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_HN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_MX.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_NI.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_PA.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_PE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_PR.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_PY.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_SV.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8239 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_US.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_UY.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/es_VE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6290 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/et.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6293 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/et_EE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      882 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/eu.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      919 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/eu_ES.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    28717 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/fa.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8295 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/fa_AF.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    28761 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/fa_IR.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     7097 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/fi.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     7100 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/fi_FI.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      914 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/fo.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      917 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/fo_FO.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9519 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/fr.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9518 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/fr_BE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9506 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/fr_CA.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9519 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/fr_CH.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9522 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/fr_FR.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9518 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/fr_LU.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9701 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ga.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9700 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ga_IE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      889 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/gl.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      888 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/gl_ES.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1993 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/gu.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1976 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/gu_IN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    10058 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/gv.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    10057 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/gv_GB.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    17877 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/he.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    17880 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/he_IL.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    19593 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/hi.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    19576 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/hi_IN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6680 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/hr.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6683 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/hr_HR.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9192 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/hu.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9195 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/hu_HU.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2072 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/hy.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2075 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/hy_AM.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2071 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/hy_AM_REVISED.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9750 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/id.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9749 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/id_ID.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      984 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/is.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      987 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/is_IS.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6845 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/it.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6849 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/it_CH.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6848 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/it_IT.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    17814 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ja.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    17817 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ja_JP.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1835 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/kk.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1838 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/kk_KZ.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      934 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/kl.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      933 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/kl_GL.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2024 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/kn.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2007 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/kn_IN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15459 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ko.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15449 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ko_KR.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9775 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/kok.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    15432 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/kok_IN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      917 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/kw.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      916 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/kw_GB.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     7222 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/lt.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     7225 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/lt_LT.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     7467 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/lv.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     7470 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/lv_LV.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1915 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/mk.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1918 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/mk_MK.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9674 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/mr.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9657 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/mr_IN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     5628 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ms.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     5598 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ms_BN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     5627 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ms_MY.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    16356 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/mt.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    16359 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/mt_MT.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6984 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/nb.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6987 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/nb_NO.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6873 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/nl.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6876 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/nl_BE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6876 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/nl_NL.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      911 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/nn.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      914 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/nn_NO.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6984 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/no.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6987 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/no_NO.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      913 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/om.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      914 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/om_ET.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      914 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/om_KE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1856 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/pa.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1839 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/pa_IN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6840 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/pl.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6843 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/pl_PL.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6091 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ps.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6141 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ps_AF.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     7802 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/pt.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     7789 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/pt_BR.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2733 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/pt_PT.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6672 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ro.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6675 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ro_RO.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    28474 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ru.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    28481 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ru_RU.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    28502 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ru_UA.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6983 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sh.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6986 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sh_YU.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     7265 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sk.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     7268 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sk_SK.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.557852 Nitrous-0.9.3/turbogears/i18n/data/sl/
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.629853 Nitrous-0.9.3/turbogears/i18n/data/sl/LC_MESSAGES/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      800 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sl/LC_MESSAGES/TurboGears.mo
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1003 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sl/LC_MESSAGES/TurboGears.po
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6915 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sl.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6918 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sl_SI.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2846 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/so.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2849 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/so_DJ.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2849 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/so_ET.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2849 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/so_KE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2849 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/so_SO.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      887 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sq.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      890 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sq_AL.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    16831 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sr.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    16834 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sr_YU.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    12296 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sv.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    12299 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sv_FI.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    12299 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sv_SE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2481 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sw.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2484 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sw_KE.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2484 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/sw_TZ.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    20542 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ta.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    20525 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ta_IN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2162 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/te.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2145 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/te_IN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    21761 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/th.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    21764 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/th_TH.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    12428 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ti.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    12413 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ti_ER.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    12461 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/ti_ET.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9075 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/tr.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9078 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/tr_TR.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    27036 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/uk.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    27039 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/uk_UA.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6467 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/vi.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6470 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/vi_VN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14539 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/zh.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    14531 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/zh_CN.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    11757 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/zh_HK.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    11757 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/zh_MO.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1468 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/zh_SG.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    11791 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/data/zh_TW.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     6479 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/i18n/format.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     3373 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/kidutils.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.629853 Nitrous-0.9.3/turbogears/i18n/pygettext/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)       11 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/pygettext/__init__.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     6282 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/i18n/pygettext/catalog.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     5775 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/i18n/pygettext/msgfmt.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    28753 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/i18n/pygettext/pygettext.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.629853 Nitrous-0.9.3/turbogears/i18n/sagettext/
+-rw-r-----   0 drocco    (1000) drocco    (1000)     4010 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/i18n/sagettext/__init__.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1051 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/i18n/sagettext/model.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.629853 Nitrous-0.9.3/turbogears/i18n/tests/
+-rw-r-----   0 drocco    (1000) drocco    (1000)      840 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/i18n/tests/__init__.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     3425 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/i18n/tests/test_format.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1164 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/i18n/tests/test_kidutils.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)      654 2019-07-02 15:15:53.000000 Nitrous-0.9.3/turbogears/i18n/tests/test_so_gettext.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1521 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/i18n/tests/test_tg_gettext.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      230 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/tests/test_toolboxadmi18n.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      292 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/i18n/tests/test_utils.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     5378 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/i18n/tg_gettext.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     3874 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/i18n/utils.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.633853 Nitrous-0.9.3/turbogears/identity/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1650 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/identity/__init__.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     7105 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/identity/base.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    10757 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/identity/conditions.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     4325 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/identity/exceptions.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    15683 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/identity/saprovider.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.633853 Nitrous-0.9.3/turbogears/identity/tests/
+-rw-r-----   0 drocco    (1000) drocco    (1000)      487 2019-07-02 15:15:53.000000 Nitrous-0.9.3/turbogears/identity/tests/__init__.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     9038 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/identity/tests/test_identity.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    25091 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/identity/tests/test_identity_sa.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1014 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/identity/tests/test_visit.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     7855 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/identity/tests/test_visit_sa.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     9375 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/identity/visitor.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1600 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/release.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.633853 Nitrous-0.9.3/turbogears/rest/
+-rw-r-----   0 drocco    (1000) drocco    (1000)     5762 2023-07-10 20:41:23.000000 Nitrous-0.9.3/turbogears/rest/__init__.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      559 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/scheduler.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    11943 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/startup.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.633853 Nitrous-0.9.3/turbogears/static/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)        0 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/__init__.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.633853 Nitrous-0.9.3/turbogears/static/css/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)        0 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/css/__init__.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1157 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/css/interpreter.css
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1319 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/css/toolbox.css
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1243 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/css/widget.css
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.641853 Nitrous-0.9.3/turbogears/static/images/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)        0 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/images/__init__.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)      363 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/add.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2734 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/admi18n.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      300 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/arrow_down.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      206 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/arrow_down_small.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1024 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/arrow_left.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      280 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/arrow_right.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      261 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/arrow_up.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      205 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/arrow_up_small.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1989 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/catwalk.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2996 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/catwalk_logo.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      181 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/catwalk_logo_bg.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      222 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/column_chooser.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     3689 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/designer.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      610 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/discard.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      412 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/edit.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      665 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/file.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1070 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/folder.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2323 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/identity.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     3510 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/info.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1410 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/play.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      341 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/remove.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      301 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/save.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2679 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/shell.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      993 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/small_gear.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1503 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/stop.png
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      121 2019-07-02 13:45:17.000000 Nitrous-0.9.3/turbogears/static/images/table.gif
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2781 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/tg_power.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     4010 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/tg_under_the_hood.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2529 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/tg_under_the_hood_sans_gear.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2633 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/toolbox_logo.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      147 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/toolbox_top_baggrund.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      151 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/toolbox_top_vertical_line.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)    33365 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/top.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      525 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/top_bg.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      153 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/transp.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)      672 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/trash.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     4179 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/static/images/widgets.png
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.641853 Nitrous-0.9.3/turbogears/static/js/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)        0 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/js/__init__.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      151 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/js/i18n_base.js
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     4348 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/js/interpreter.js
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.645853 Nitrous-0.9.3/turbogears/static/js/tool-man/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      879 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/js/tool-man/cookies.js
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     4138 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/js/tool-man/coordinates.js
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     4717 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/js/tool-man/core.js
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      528 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/js/tool-man/css.js
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     7124 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/js/tool-man/drag.js
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2476 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/js/tool-man/dragsort.js
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1192 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/static/js/tool-man/events.js
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.649853 Nitrous-0.9.3/turbogears/tests/
+-rw-r-----   0 drocco    (1000) drocco    (1000)      446 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/__init__.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.649853 Nitrous-0.9.3/turbogears/tests/catwalk_models/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)        0 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/catwalk_models/__init__.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1230 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/catwalk_models/browse.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.653853 Nitrous-0.9.3/turbogears/tests/catwalk_models/catwalk-session/
+-rw-r-----   0 drocco    (1000) drocco    (1000)      237 2019-07-02 14:03:58.000000 Nitrous-0.9.3/turbogears/tests/catwalk_models/catwalk-session/session.pkl
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      479 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/catwalk_models/model_list.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      426 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/catwalk_models/model_structure.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      409 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/catwalk_models/single_join.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      488 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/config.cfg
+-rw-r--r--   0 drocco    (1000) drocco    (1000)       84 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/tests/configfile.cfg
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      667 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/form.html
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      441 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/form.kid
+-rw-r-----   0 drocco    (1000) drocco    (1000)       75 2020-01-13 15:36:07.000000 Nitrous-0.9.3/turbogears/tests/genshi_new_text_format.txt
+-rw-r-----   0 drocco    (1000) drocco    (1000)       60 2020-01-13 15:29:36.000000 Nitrous-0.9.3/turbogears/tests/genshi_old_text_format.txt
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.561852 Nitrous-0.9.3/turbogears/tests/locale/
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.561852 Nitrous-0.9.3/turbogears/tests/locale/en/
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.653853 Nitrous-0.9.3/turbogears/tests/locale/en/LC_MESSAGES/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      377 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/locale/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      589 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/locale/en/LC_MESSAGES/messages.po
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.561852 Nitrous-0.9.3/turbogears/tests/locale/fi/
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.653853 Nitrous-0.9.3/turbogears/tests/locale/fi/LC_MESSAGES/
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1616 2019-07-02 14:03:58.000000 Nitrous-0.9.3/turbogears/tests/locale/fi/LC_MESSAGES/messages.mo
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      638 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/locale/fi/LC_MESSAGES/messages.po
+-rw-r--r--   0 drocco    (1000) drocco    (1000)       96 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/othertemplate.kid
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      148 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/paginate.html
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      209 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/simple.html
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      157 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/simple.kid
+-rw-r-----   0 drocco    (1000) drocco    (1000)     6197 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/test_catwalk.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6627 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/test_command_i18n.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2808 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/test_config.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    36387 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/test_controllers.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     3057 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/test_decorator.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    12899 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/test_errorhandling.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     4547 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/test_expose.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    44646 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/test_paginate.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     4138 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/test_restmethod.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     3249 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/test_safemultipart.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     4411 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/test_session_mapper.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    11897 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/test_sqlalchemy.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1829 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/test_testutil.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    15197 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/test_util.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     5141 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/test_validators.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    20752 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/tests/test_view.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)       34 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/tests/textfmt.tmpl
+-rw-r-----   0 drocco    (1000) drocco    (1000)    10051 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/testutil.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.653853 Nitrous-0.9.3/turbogears/toolbox/
+-rw-r-----   0 drocco    (1000) drocco    (1000)       65 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/toolbox/__init__.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.653853 Nitrous-0.9.3/turbogears/toolbox/admi18n/
+-rw-r-----   0 drocco    (1000) drocco    (1000)    11148 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/toolbox/admi18n/__init__.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     4358 2019-07-02 15:15:53.000000 Nitrous-0.9.3/turbogears/toolbox/admi18n/internationalization.html
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8824 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/admi18n/language.html
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8589 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/admi18n/languageManagement.html
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     5961 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/admi18n/po_view.html
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     5720 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/admi18n/stringCollection.html
+-rw-r-----   0 drocco    (1000) drocco    (1000)     5441 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/toolbox/base.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.657853 Nitrous-0.9.3/turbogears/toolbox/catwalk/
+-rw-r-----   0 drocco    (1000) drocco    (1000)    42486 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/__init__.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    11740 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/browse.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     4683 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/browse_grid.html
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6123 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/catwalk.html
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     8055 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/columns.html
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.561852 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.657853 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/css/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2583 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/css/catwalk.css
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.657853 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2779 2019-07-02 15:15:53.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/browse.js
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    45693 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/catwalk.js
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.657853 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9409 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/AmiJS.js
+-rw-r--r--   0 drocco    (1000) drocco    (1000)       49 2019-07-02 13:45:16.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/blank.gif
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      200 2019-07-02 13:45:16.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/close.gif
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      999 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/greybox.css
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     4741 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/greybox.js
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     4296 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/greybox__.js
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     4843 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/greybox_inline.js
+-rw-r-----   0 drocco    (1000) drocco    (1000)     6336 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/logo.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2960 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/overlay.png
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1742 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/console.html
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.661853 Nitrous-0.9.3/turbogears/toolbox/designer/
+-rw-r-----   0 drocco    (1000) drocco    (1000)    13003 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/toolbox/designer/__init__.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     4946 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/designer/modelDesigner.html
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.561852 Nitrous-0.9.3/turbogears/toolbox/designer/static/
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.661853 Nitrous-0.9.3/turbogears/toolbox/designer/static/css/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2464 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/css/style.css
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.661853 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.661853 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/images/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)       64 2019-07-02 13:45:16.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/images/back.gif
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2839 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/images/shadow.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2961 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/images/shadow_bottom.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2893 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/images/shadow_corner.png
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2989 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/images/shadow_right.png
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2426 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/index.html
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.665853 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/
+-rw-r-----   0 drocco    (1000) drocco    (1000)     3981 2019-07-02 14:03:58.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/ajax.js
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2397 2019-07-02 15:15:53.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/animator.js
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1868 2019-07-02 15:15:53.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/generic.js
+-rw-r-----   0 drocco    (1000) drocco    (1000)     6146 2019-07-02 15:15:53.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/io.js
+-rw-r-----   0 drocco    (1000) drocco    (1000)    16064 2019-07-02 15:15:53.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/main.js
+-rw-r-----   0 drocco    (1000) drocco    (1000)    23822 2019-07-02 15:15:53.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/objects.js
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1098 2019-07-02 15:15:53.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/settings.js
+-rw-r-----   0 drocco    (1000) drocco    (1000)     3473 2019-07-02 15:15:53.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/sql_types.js
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.665853 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/styles/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     3526 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/styles/bar.css
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     3077 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/styles/style.css
+-rw-r-----   0 drocco    (1000) drocco    (1000)      220 2019-07-02 15:15:53.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/styles/style.js
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.665853 Nitrous-0.9.3/turbogears/toolbox/designer/static/images/
+-rw-r-----   0 drocco    (1000) drocco    (1000)      750 2019-07-02 13:46:08.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/images/info.png
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.665853 Nitrous-0.9.3/turbogears/toolbox/designer/static/javascript/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)    55991 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/javascript/modelDesigner.js
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.665853 Nitrous-0.9.3/turbogears/toolbox/designer/static/sessions/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     6037 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/sessions/Survey.js
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     3271 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/sessions/TurboTunes.js
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     9963 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/designer/static/sessions/WebShop.js
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1099 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/info.html
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1871 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/main.html
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     1393 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/master.html
+-rw-r-----   0 drocco    (1000) drocco    (1000)     2733 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/toolbox/shell.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     4305 2019-07-02 13:55:25.000000 Nitrous-0.9.3/turbogears/toolbox/widgets.html
+-rw-r-----   0 drocco    (1000) drocco    (1000)    25291 2021-06-21 20:14:44.000000 Nitrous-0.9.3/turbogears/util.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     8769 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/validators.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.669853 Nitrous-0.9.3/turbogears/view/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)       68 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/view/__init__.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    19426 2023-07-10 20:43:30.000000 Nitrous-0.9.3/turbogears/view/base.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)     2348 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/view/genshisupport.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     1550 2021-01-12 20:52:24.000000 Nitrous-0.9.3/turbogears/view/json.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.669853 Nitrous-0.9.3/turbogears/view/templates/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)        0 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/view/templates/__init__.py
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      749 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/view/templates/sitetemplate.kid
+-rw-r-----   0 drocco    (1000) drocco    (1000)      896 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/view/text.py
+drwxr-x---   0 drocco    (1000) drocco    (1000)        0 2023-07-10 20:46:40.669853 Nitrous-0.9.3/turbogears/visit/
+-rw-r--r--   0 drocco    (1000) drocco    (1000)      528 2019-07-02 13:55:26.000000 Nitrous-0.9.3/turbogears/visit/__init__.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)    12619 2021-09-30 10:37:32.000000 Nitrous-0.9.3/turbogears/visit/api.py
+-rw-r-----   0 drocco    (1000) drocco    (1000)     3720 2020-06-18 23:52:54.000000 Nitrous-0.9.3/turbogears/visit/savisit.py
```

### Comparing `Nitrous-0.9.0/CHANGELOG.txt` & `Nitrous-0.9.3/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/CONTRIBUTORS.txt` & `Nitrous-0.9.3/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/LICENSE.txt` & `Nitrous-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/MANIFEST.in` & `Nitrous-0.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/Nitrous.egg-info/PKG-INFO` & `Nitrous-0.9.3/Nitrous.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: Nitrous
-Version: 0.9.0
+Version: 0.9.3
 Summary: Nitrous gives TurboGears 1 a boost
 Home-page: https://bitbucket.org/brightlinkinfrastructure/nitrous
 Author: BrightLink
 Author-email: drocco@thebrightlink.com
 Maintainer: BrightLink
 Maintainer-email: drocco@thebrightlink.com
 License: MIT
-Download-URL: https://bitbucket.org/brightlinkinfrastructure/nitrous/get/v0.9.0.tar.gz
-Description: 
-        Project Nitrous
-        ===============
-        
-        Project Nitrous is a port of TurboGears 1 to Python 3 and a modern
-        development stack.
-        
-        It is intended to ease support for legacy projects in a post-Python 2
-        world. If you're starting a new project, Nitrous isn't for you: check
-        out one of these excellent Python Web Frameworks: Pyramid, Django, or
-        Flask.
-        
-        Nitrous is maintained by BrightLink.
-        
+Download-URL: https://bitbucket.org/brightlinkinfrastructure/nitrous/get/v0.9.3.tar.gz
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Framework :: TurboGears
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE.txt
+
+
+Project Nitrous
+===============
+
+Project Nitrous is a port of TurboGears 1 to Python 3 and a modern
+development stack.
+
+It is intended to ease support for legacy projects in a post-Python 2
+world. If you're starting a new project, Nitrous isn't for you: check
+out one of these excellent Python Web Frameworks: Pyramid, Django, or
+Flask.
+
+Nitrous is maintained by BrightLink.
+
+
```

### Comparing `Nitrous-0.9.0/Nitrous.egg-info/SOURCES.txt` & `Nitrous-0.9.3/Nitrous.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 doc/doc.ini
 tests/__init__.py
 tests/conftest.py
 tests/test_expose.py
 tests/test_expose_with_identity.py
 tests/test_expose_with_transaction.py
 tests/test_expose_with_validate.py
+tests/test_resource_exception_handling.py
+tests/test_resource_init_exception_handling.py
 tests/test_rest.py
 tests/test_validate.py
 tools/codename.py
 tools/test_all_quickstarts.py
 tools/tgsetup.py
 tools/toolbox-start.py
 turbogears/__init__.py
```

### Comparing `Nitrous-0.9.0/Nitrous.egg-info/entry_points.txt` & `Nitrous-0.9.3/Nitrous.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/PKG-INFO` & `Nitrous-0.9.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: Nitrous
-Version: 0.9.0
+Version: 0.9.3
 Summary: Nitrous gives TurboGears 1 a boost
 Home-page: https://bitbucket.org/brightlinkinfrastructure/nitrous
 Author: BrightLink
 Author-email: drocco@thebrightlink.com
 Maintainer: BrightLink
 Maintainer-email: drocco@thebrightlink.com
 License: MIT
-Download-URL: https://bitbucket.org/brightlinkinfrastructure/nitrous/get/v0.9.0.tar.gz
-Description: 
-        Project Nitrous
-        ===============
-        
-        Project Nitrous is a port of TurboGears 1 to Python 3 and a modern
-        development stack.
-        
-        It is intended to ease support for legacy projects in a post-Python 2
-        world. If you're starting a new project, Nitrous isn't for you: check
-        out one of these excellent Python Web Frameworks: Pyramid, Django, or
-        Flask.
-        
-        Nitrous is maintained by BrightLink.
-        
+Download-URL: https://bitbucket.org/brightlinkinfrastructure/nitrous/get/v0.9.3.tar.gz
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Framework :: TurboGears
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE.txt
+
+
+Project Nitrous
+===============
+
+Project Nitrous is a port of TurboGears 1 to Python 3 and a modern
+development stack.
+
+It is intended to ease support for legacy projects in a post-Python 2
+world. If you're starting a new project, Nitrous isn't for you: check
+out one of these excellent Python Web Frameworks: Pyramid, Django, or
+Flask.
+
+Nitrous is maintained by BrightLink.
+
+
```

### Comparing `Nitrous-0.9.0/doc/README.txt` & `Nitrous-0.9.3/doc/README.txt`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/doc/doc.ini` & `Nitrous-0.9.3/doc/doc.ini`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/setup.py` & `Nitrous-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 import sys
 
 from setuptools import setup, find_packages
 
 
-version = "0.9.0"
+version = "0.9.3"
 description = "Nitrous gives TurboGears 1 a boost"
 long_description = """
 Project Nitrous
 ===============
 
 Project Nitrous is a port of TurboGears 1 to Python 3 and a modern
 development stack.
```

### Comparing `Nitrous-0.9.0/test.cfg` & `Nitrous-0.9.3/test.cfg`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/tests/conftest.py` & `Nitrous-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/tests/test_expose.py` & `Nitrous-0.9.3/tests/test_expose.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,22 @@
             'front_9': a_file.fullvalue()[:9]
         }
 
     @expose()
     def positional_argument(self, arrrrrrg):
         return {}
 
+    @expose('csv')
+    def csv(self):
+        return b'a,b,c\n1,2,3'
+
+    @expose('csv')
+    def csv_generator(self):
+        yield b'a,b,c\n1,2,3'
+
 
 @pytest.fixture
 def app():
     return make_app(Root)
 
 
 def test_plain_expose_should_return_json(app):
@@ -216,14 +224,30 @@
     }
 
     response = app.get('/plain_expose_with_params', params=params)
 
     assert response.headers['content-type'].startswith('text/html')
 
 
+def test_exposed_csv_generator_should_return_csv(app):
+    response = app.get('/csv_generator', headers={'Accept': 'text/csv'})
+
+    assert response.headers['content-type'].startswith('text/csv')
+    assert b'a,b,c\n1,2,3' == response.body
+
+
+def test_exposed_csv_string_should_return_csv(app):
+    # COREBT-15367 demonstration case: Nitrous incorrectly handled CSV
+    # method outputs not produced by a generator
+    response = app.get('/csv', headers={'Accept': 'text/csv'})
+
+    assert response.headers['content-type'].startswith('text/csv')
+    assert b'a,b,c\n1,2,3' == response.body
+
+
 def test_html_endpoint_should_return_html(app):
     response = app.get('/html')
 
     assert response.headers['content-type'].startswith('text/html')
 
 
 def test_html_endpoint_should_not_return_json(app):
```

### Comparing `Nitrous-0.9.0/tests/test_expose_with_identity.py` & `Nitrous-0.9.3/tests/test_expose_with_identity.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/tests/test_expose_with_transaction.py` & `Nitrous-0.9.3/tests/test_expose_with_transaction.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/tests/test_expose_with_validate.py` & `Nitrous-0.9.3/tests/test_expose_with_validate.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/tests/test_rest.py` & `Nitrous-0.9.3/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/tests/test_validate.py` & `Nitrous-0.9.3/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/tools/codename.py` & `Nitrous-0.9.3/tools/codename.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/tools/test_all_quickstarts.py` & `Nitrous-0.9.3/tools/test_all_quickstarts.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/tools/tgsetup.py` & `Nitrous-0.9.3/tools/tgsetup.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/__init__.py` & `Nitrous-0.9.3/turbogears/__init__.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/command/base.py` & `Nitrous-0.9.3/turbogears/command/base.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/command/i18n.py` & `Nitrous-0.9.3/turbogears/command/i18n.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/command/info.py` & `Nitrous-0.9.3/turbogears/command/info.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/command/kid2genshi.py` & `Nitrous-0.9.3/turbogears/command/kid2genshi.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/command/sacommand.py` & `Nitrous-0.9.3/turbogears/command/sacommand.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/config.py` & `Nitrous-0.9.3/turbogears/config.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/controllers.py` & `Nitrous-0.9.3/turbogears/controllers.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,16 +243,14 @@
             response.headers['Content-Type'] = content_type
         return output
     elif response.body:
         # If response.body is set, the view handler has already set a response
         # (e.g. a file), so don't process further
         return output
 
-    # FIXME: support CSV
-
     headers = {'Content-Type': content_type}
     output = view.render(output, template=template, format=format,
                          headers=headers, fragment=fragment, **options)
     content_type = headers['Content-Type']
 
     if content_type:
         response.headers['Content-Type'] = content_type
```

### Comparing `Nitrous-0.9.0/turbogears/database/__init__.py` & `Nitrous-0.9.3/turbogears/database/__init__.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/database/sqlalchemy_support.py` & `Nitrous-0.9.3/turbogears/database/sqlalchemy_support.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/dispatchers.py` & `Nitrous-0.9.3/turbogears/dispatchers.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/docgen.py` & `Nitrous-0.9.3/turbogears/docgen.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/errorhandling.py` & `Nitrous-0.9.3/turbogears/errorhandling.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/finddata.py` & `Nitrous-0.9.3/turbogears/finddata.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/hooks.py` & `Nitrous-0.9.3/turbogears/hooks.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/__init__.py` & `Nitrous-0.9.3/turbogears/i18n/__init__.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/TurboGears.pot` & `Nitrous-0.9.3/turbogears/i18n/data/TurboGears.pot`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/af.py` & `Nitrous-0.9.3/turbogears/i18n/data/af.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/af_ZA.py` & `Nitrous-0.9.3/turbogears/i18n/data/af_ZA.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/am.py` & `Nitrous-0.9.3/turbogears/i18n/data/am.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/am_ET.py` & `Nitrous-0.9.3/turbogears/i18n/data/am_ET.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_AE.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_AE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_BH.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_BH.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_DZ.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_DZ.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_EG.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_EG.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_IN.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_IN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_IQ.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_IQ.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_JO.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_JO.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_KW.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_KW.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_LB.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_LB.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_LY.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_LY.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_MA.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_MA.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_OM.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_OM.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_QA.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_QA.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_SA.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_SA.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_SD.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_SD.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_SY.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_SY.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_TN.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_TN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ar_YE.py` & `Nitrous-0.9.3/turbogears/i18n/data/ar_YE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/be.py` & `Nitrous-0.9.3/turbogears/i18n/data/be.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/be_BY.py` & `Nitrous-0.9.3/turbogears/i18n/data/be_BY.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/bg.py` & `Nitrous-0.9.3/turbogears/i18n/data/bg.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/bg_BG.py` & `Nitrous-0.9.3/turbogears/i18n/data/bg_BG.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/bn.py` & `Nitrous-0.9.3/turbogears/i18n/data/bn.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/bn_IN.py` & `Nitrous-0.9.3/turbogears/i18n/data/bn_IN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ca.py` & `Nitrous-0.9.3/turbogears/i18n/data/ca.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ca_ES.py` & `Nitrous-0.9.3/turbogears/i18n/data/ca_ES.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/cs.py` & `Nitrous-0.9.3/turbogears/i18n/data/cs.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/cs_CZ.py` & `Nitrous-0.9.3/turbogears/i18n/data/cs_CZ.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/da.py` & `Nitrous-0.9.3/turbogears/i18n/data/da.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/da_DK.py` & `Nitrous-0.9.3/turbogears/i18n/data/da_DK.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/de/LC_MESSAGES/TurboGears.mo` & `Nitrous-0.9.3/turbogears/i18n/data/de/LC_MESSAGES/TurboGears.mo`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/de/LC_MESSAGES/TurboGears.po` & `Nitrous-0.9.3/turbogears/i18n/data/de/LC_MESSAGES/TurboGears.po`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/de.py` & `Nitrous-0.9.3/turbogears/i18n/data/de.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/de_AT.py` & `Nitrous-0.9.3/turbogears/i18n/data/de_AT.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/de_BE.py` & `Nitrous-0.9.3/turbogears/i18n/data/de_BE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/de_CH.py` & `Nitrous-0.9.3/turbogears/i18n/data/de_CH.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/de_DE.py` & `Nitrous-0.9.3/turbogears/i18n/data/de_DE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/de_LU.py` & `Nitrous-0.9.3/turbogears/i18n/data/de_LU.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/el.py` & `Nitrous-0.9.3/turbogears/i18n/data/el.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/el_GR.py` & `Nitrous-0.9.3/turbogears/i18n/data/el_GR.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en.py` & `Nitrous-0.9.3/turbogears/i18n/data/en.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_AU.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_AU.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_BE.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_BE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_BW.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_BW.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_CA.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_CA.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_GB.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_GB.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_HK.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_HK.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_IE.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_IE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_IN.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_IN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_MT.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_MT.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_NZ.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_NZ.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_PH.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_PH.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_SG.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_SG.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_US.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_US.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_US_POSIX.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_US_POSIX.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_VI.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_VI.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_ZA.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_ZA.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/en_ZW.py` & `Nitrous-0.9.3/turbogears/i18n/data/en_ZW.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/eo.py` & `Nitrous-0.9.3/turbogears/i18n/data/eo.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es.py` & `Nitrous-0.9.3/turbogears/i18n/data/es.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_AR.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_AR.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_BO.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_BO.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_CL.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_CL.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_CO.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_CO.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_CR.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_CR.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_DO.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_DO.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_EC.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_EC.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_ES.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_ES.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_GT.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_GT.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_HN.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_HN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_MX.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_MX.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_NI.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_NI.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_PA.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_PA.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_PE.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_PE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_PR.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_PR.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_PY.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_PY.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_SV.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_SV.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_US.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_US.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_UY.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_UY.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/es_VE.py` & `Nitrous-0.9.3/turbogears/i18n/data/es_VE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/et.py` & `Nitrous-0.9.3/turbogears/i18n/data/et.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/et_EE.py` & `Nitrous-0.9.3/turbogears/i18n/data/et_EE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/eu.py` & `Nitrous-0.9.3/turbogears/i18n/data/eu.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/eu_ES.py` & `Nitrous-0.9.3/turbogears/i18n/data/eu_ES.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/fa.py` & `Nitrous-0.9.3/turbogears/i18n/data/fa.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/fa_AF.py` & `Nitrous-0.9.3/turbogears/i18n/data/fa_AF.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/fa_IR.py` & `Nitrous-0.9.3/turbogears/i18n/data/fa_IR.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/fi.py` & `Nitrous-0.9.3/turbogears/i18n/data/fi.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/fi_FI.py` & `Nitrous-0.9.3/turbogears/i18n/data/fi_FI.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/fo.py` & `Nitrous-0.9.3/turbogears/i18n/data/fo.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/fo_FO.py` & `Nitrous-0.9.3/turbogears/i18n/data/fo_FO.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/fr.py` & `Nitrous-0.9.3/turbogears/i18n/data/fr.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/fr_BE.py` & `Nitrous-0.9.3/turbogears/i18n/data/fr_BE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/fr_CA.py` & `Nitrous-0.9.3/turbogears/i18n/data/fr_CA.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/fr_CH.py` & `Nitrous-0.9.3/turbogears/i18n/data/fr_CH.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/fr_FR.py` & `Nitrous-0.9.3/turbogears/i18n/data/fr_FR.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/fr_LU.py` & `Nitrous-0.9.3/turbogears/i18n/data/fr_LU.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ga.py` & `Nitrous-0.9.3/turbogears/i18n/data/ga.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ga_IE.py` & `Nitrous-0.9.3/turbogears/i18n/data/ga_IE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/gl.py` & `Nitrous-0.9.3/turbogears/i18n/data/gl.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/gl_ES.py` & `Nitrous-0.9.3/turbogears/i18n/data/gl_ES.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/gu.py` & `Nitrous-0.9.3/turbogears/i18n/data/gu.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/gu_IN.py` & `Nitrous-0.9.3/turbogears/i18n/data/gu_IN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/gv.py` & `Nitrous-0.9.3/turbogears/i18n/data/gv.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/gv_GB.py` & `Nitrous-0.9.3/turbogears/i18n/data/gv_GB.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/he.py` & `Nitrous-0.9.3/turbogears/i18n/data/he.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/he_IL.py` & `Nitrous-0.9.3/turbogears/i18n/data/he_IL.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/hi.py` & `Nitrous-0.9.3/turbogears/i18n/data/hi.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/hi_IN.py` & `Nitrous-0.9.3/turbogears/i18n/data/hi_IN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/hr.py` & `Nitrous-0.9.3/turbogears/i18n/data/hr.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/hr_HR.py` & `Nitrous-0.9.3/turbogears/i18n/data/hr_HR.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/hu.py` & `Nitrous-0.9.3/turbogears/i18n/data/hu.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/hu_HU.py` & `Nitrous-0.9.3/turbogears/i18n/data/hu_HU.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/hy.py` & `Nitrous-0.9.3/turbogears/i18n/data/hy.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/hy_AM.py` & `Nitrous-0.9.3/turbogears/i18n/data/hy_AM.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/hy_AM_REVISED.py` & `Nitrous-0.9.3/turbogears/i18n/data/hy_AM_REVISED.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/id.py` & `Nitrous-0.9.3/turbogears/i18n/data/id.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/id_ID.py` & `Nitrous-0.9.3/turbogears/i18n/data/id_ID.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/is.py` & `Nitrous-0.9.3/turbogears/i18n/data/is.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/is_IS.py` & `Nitrous-0.9.3/turbogears/i18n/data/is_IS.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/it.py` & `Nitrous-0.9.3/turbogears/i18n/data/it.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/it_CH.py` & `Nitrous-0.9.3/turbogears/i18n/data/it_CH.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/it_IT.py` & `Nitrous-0.9.3/turbogears/i18n/data/it_IT.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ja.py` & `Nitrous-0.9.3/turbogears/i18n/data/ja.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ja_JP.py` & `Nitrous-0.9.3/turbogears/i18n/data/ja_JP.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/kk.py` & `Nitrous-0.9.3/turbogears/i18n/data/kk.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/kk_KZ.py` & `Nitrous-0.9.3/turbogears/i18n/data/kk_KZ.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/kl.py` & `Nitrous-0.9.3/turbogears/i18n/data/kl.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/kl_GL.py` & `Nitrous-0.9.3/turbogears/i18n/data/kl_GL.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/kn.py` & `Nitrous-0.9.3/turbogears/i18n/data/kn.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/kn_IN.py` & `Nitrous-0.9.3/turbogears/i18n/data/kn_IN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ko.py` & `Nitrous-0.9.3/turbogears/i18n/data/ko.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ko_KR.py` & `Nitrous-0.9.3/turbogears/i18n/data/ko_KR.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/kok.py` & `Nitrous-0.9.3/turbogears/i18n/data/kok.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/kok_IN.py` & `Nitrous-0.9.3/turbogears/i18n/data/kok_IN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/kw.py` & `Nitrous-0.9.3/turbogears/i18n/data/kw.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/kw_GB.py` & `Nitrous-0.9.3/turbogears/i18n/data/kw_GB.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/lt.py` & `Nitrous-0.9.3/turbogears/i18n/data/lt.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/lt_LT.py` & `Nitrous-0.9.3/turbogears/i18n/data/lt_LT.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/lv.py` & `Nitrous-0.9.3/turbogears/i18n/data/lv.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/lv_LV.py` & `Nitrous-0.9.3/turbogears/i18n/data/lv_LV.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/mk.py` & `Nitrous-0.9.3/turbogears/i18n/data/mk.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/mk_MK.py` & `Nitrous-0.9.3/turbogears/i18n/data/mk_MK.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/mr.py` & `Nitrous-0.9.3/turbogears/i18n/data/mr.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/mr_IN.py` & `Nitrous-0.9.3/turbogears/i18n/data/mr_IN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ms.py` & `Nitrous-0.9.3/turbogears/i18n/data/ms.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ms_BN.py` & `Nitrous-0.9.3/turbogears/i18n/data/ms_BN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ms_MY.py` & `Nitrous-0.9.3/turbogears/i18n/data/ms_MY.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/mt.py` & `Nitrous-0.9.3/turbogears/i18n/data/mt.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/mt_MT.py` & `Nitrous-0.9.3/turbogears/i18n/data/mt_MT.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/nb.py` & `Nitrous-0.9.3/turbogears/i18n/data/nb.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/nb_NO.py` & `Nitrous-0.9.3/turbogears/i18n/data/nb_NO.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/nl.py` & `Nitrous-0.9.3/turbogears/i18n/data/nl.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/nl_BE.py` & `Nitrous-0.9.3/turbogears/i18n/data/nl_BE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/nl_NL.py` & `Nitrous-0.9.3/turbogears/i18n/data/nl_NL.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/nn.py` & `Nitrous-0.9.3/turbogears/i18n/data/nn.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/nn_NO.py` & `Nitrous-0.9.3/turbogears/i18n/data/nn_NO.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/no.py` & `Nitrous-0.9.3/turbogears/i18n/data/no.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/no_NO.py` & `Nitrous-0.9.3/turbogears/i18n/data/no_NO.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/om.py` & `Nitrous-0.9.3/turbogears/i18n/data/om.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/om_ET.py` & `Nitrous-0.9.3/turbogears/i18n/data/om_ET.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/om_KE.py` & `Nitrous-0.9.3/turbogears/i18n/data/om_KE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/pa.py` & `Nitrous-0.9.3/turbogears/i18n/data/pa.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/pa_IN.py` & `Nitrous-0.9.3/turbogears/i18n/data/pa_IN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/pl.py` & `Nitrous-0.9.3/turbogears/i18n/data/pl.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/pl_PL.py` & `Nitrous-0.9.3/turbogears/i18n/data/pl_PL.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ps.py` & `Nitrous-0.9.3/turbogears/i18n/data/ps.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ps_AF.py` & `Nitrous-0.9.3/turbogears/i18n/data/ps_AF.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/pt.py` & `Nitrous-0.9.3/turbogears/i18n/data/pt.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/pt_BR.py` & `Nitrous-0.9.3/turbogears/i18n/data/pt_BR.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/pt_PT.py` & `Nitrous-0.9.3/turbogears/i18n/data/pt_PT.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ro.py` & `Nitrous-0.9.3/turbogears/i18n/data/ro.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ro_RO.py` & `Nitrous-0.9.3/turbogears/i18n/data/ro_RO.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ru.py` & `Nitrous-0.9.3/turbogears/i18n/data/ru.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ru_RU.py` & `Nitrous-0.9.3/turbogears/i18n/data/ru_RU.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ru_UA.py` & `Nitrous-0.9.3/turbogears/i18n/data/ru_UA.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sh.py` & `Nitrous-0.9.3/turbogears/i18n/data/sh.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sh_YU.py` & `Nitrous-0.9.3/turbogears/i18n/data/sh_YU.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sk.py` & `Nitrous-0.9.3/turbogears/i18n/data/sk.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sk_SK.py` & `Nitrous-0.9.3/turbogears/i18n/data/sk_SK.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sl/LC_MESSAGES/TurboGears.mo` & `Nitrous-0.9.3/turbogears/i18n/data/sl/LC_MESSAGES/TurboGears.mo`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sl/LC_MESSAGES/TurboGears.po` & `Nitrous-0.9.3/turbogears/i18n/data/sl/LC_MESSAGES/TurboGears.po`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sl.py` & `Nitrous-0.9.3/turbogears/i18n/data/sl.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sl_SI.py` & `Nitrous-0.9.3/turbogears/i18n/data/sl_SI.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/so.py` & `Nitrous-0.9.3/turbogears/i18n/data/so.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/so_DJ.py` & `Nitrous-0.9.3/turbogears/i18n/data/so_DJ.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/so_ET.py` & `Nitrous-0.9.3/turbogears/i18n/data/so_ET.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/so_KE.py` & `Nitrous-0.9.3/turbogears/i18n/data/so_KE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/so_SO.py` & `Nitrous-0.9.3/turbogears/i18n/data/so_SO.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sq.py` & `Nitrous-0.9.3/turbogears/i18n/data/sq.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sq_AL.py` & `Nitrous-0.9.3/turbogears/i18n/data/sq_AL.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sr.py` & `Nitrous-0.9.3/turbogears/i18n/data/sr.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sr_YU.py` & `Nitrous-0.9.3/turbogears/i18n/data/sr_YU.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sv.py` & `Nitrous-0.9.3/turbogears/i18n/data/sv.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sv_FI.py` & `Nitrous-0.9.3/turbogears/i18n/data/sv_FI.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sv_SE.py` & `Nitrous-0.9.3/turbogears/i18n/data/sv_SE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sw.py` & `Nitrous-0.9.3/turbogears/i18n/data/sw.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sw_KE.py` & `Nitrous-0.9.3/turbogears/i18n/data/sw_KE.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/sw_TZ.py` & `Nitrous-0.9.3/turbogears/i18n/data/sw_TZ.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ta.py` & `Nitrous-0.9.3/turbogears/i18n/data/ta.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ta_IN.py` & `Nitrous-0.9.3/turbogears/i18n/data/ta_IN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/te.py` & `Nitrous-0.9.3/turbogears/i18n/data/te.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/te_IN.py` & `Nitrous-0.9.3/turbogears/i18n/data/te_IN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/th.py` & `Nitrous-0.9.3/turbogears/i18n/data/th.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/th_TH.py` & `Nitrous-0.9.3/turbogears/i18n/data/th_TH.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ti.py` & `Nitrous-0.9.3/turbogears/i18n/data/ti.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ti_ER.py` & `Nitrous-0.9.3/turbogears/i18n/data/ti_ER.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/ti_ET.py` & `Nitrous-0.9.3/turbogears/i18n/data/ti_ET.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/tr.py` & `Nitrous-0.9.3/turbogears/i18n/data/tr.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/tr_TR.py` & `Nitrous-0.9.3/turbogears/i18n/data/tr_TR.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/uk.py` & `Nitrous-0.9.3/turbogears/i18n/data/uk.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/uk_UA.py` & `Nitrous-0.9.3/turbogears/i18n/data/uk_UA.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/vi.py` & `Nitrous-0.9.3/turbogears/i18n/data/vi.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/vi_VN.py` & `Nitrous-0.9.3/turbogears/i18n/data/vi_VN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/zh.py` & `Nitrous-0.9.3/turbogears/i18n/data/zh.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/zh_CN.py` & `Nitrous-0.9.3/turbogears/i18n/data/zh_CN.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/zh_HK.py` & `Nitrous-0.9.3/turbogears/i18n/data/zh_HK.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/zh_MO.py` & `Nitrous-0.9.3/turbogears/i18n/data/zh_MO.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/zh_SG.py` & `Nitrous-0.9.3/turbogears/i18n/data/zh_SG.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/data/zh_TW.py` & `Nitrous-0.9.3/turbogears/i18n/data/zh_TW.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/format.py` & `Nitrous-0.9.3/turbogears/i18n/format.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/kidutils.py` & `Nitrous-0.9.3/turbogears/i18n/kidutils.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/pygettext/catalog.py` & `Nitrous-0.9.3/turbogears/i18n/pygettext/catalog.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/pygettext/msgfmt.py` & `Nitrous-0.9.3/turbogears/i18n/pygettext/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/pygettext/pygettext.py` & `Nitrous-0.9.3/turbogears/i18n/pygettext/pygettext.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/sagettext/__init__.py` & `Nitrous-0.9.3/turbogears/i18n/sagettext/__init__.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/sagettext/model.py` & `Nitrous-0.9.3/turbogears/i18n/sagettext/model.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/tests/__init__.py` & `Nitrous-0.9.3/turbogears/i18n/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/tests/test_format.py` & `Nitrous-0.9.3/turbogears/i18n/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/tests/test_kidutils.py` & `Nitrous-0.9.3/turbogears/i18n/tests/test_kidutils.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/tests/test_so_gettext.py` & `Nitrous-0.9.3/turbogears/i18n/tests/test_so_gettext.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/tests/test_tg_gettext.py` & `Nitrous-0.9.3/turbogears/i18n/tests/test_tg_gettext.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/tg_gettext.py` & `Nitrous-0.9.3/turbogears/i18n/tg_gettext.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/i18n/utils.py` & `Nitrous-0.9.3/turbogears/i18n/utils.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/identity/__init__.py` & `Nitrous-0.9.3/turbogears/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/identity/base.py` & `Nitrous-0.9.3/turbogears/identity/base.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/identity/conditions.py` & `Nitrous-0.9.3/turbogears/identity/conditions.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/identity/exceptions.py` & `Nitrous-0.9.3/turbogears/identity/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/identity/saprovider.py` & `Nitrous-0.9.3/turbogears/identity/saprovider.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/identity/tests/test_identity.py` & `Nitrous-0.9.3/turbogears/identity/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/identity/tests/test_identity_sa.py` & `Nitrous-0.9.3/turbogears/identity/tests/test_identity_sa.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/identity/tests/test_visit.py` & `Nitrous-0.9.3/turbogears/identity/tests/test_visit.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/identity/tests/test_visit_sa.py` & `Nitrous-0.9.3/turbogears/identity/tests/test_visit_sa.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/identity/visitor.py` & `Nitrous-0.9.3/turbogears/identity/visitor.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/release.py` & `Nitrous-0.9.3/turbogears/release.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/rest/__init__.py` & `Nitrous-0.9.3/turbogears/rest/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,14 +137,18 @@
                 return resource_cls(id_validator(resource_id), self)
             except ValueError as e:
                 log.debug('Invalid resource id: %s (%s: %s)',
                           resource_id,
                           type(e).__name__,
                           e)
                 return vpath
+            except Exception as e:
+                log.debug('Unexpected error getting resource with id: '
+                          f'{resource_id} ({type(e).__name__}: {e})')
+                return vpath
 
         controller_cls._cp_dispatch = _cp_dispatch
 
         if not hasattr(controller_cls, 'default'):
             controller_cls.default = property(_default)
 
         return controller_cls
```

### Comparing `Nitrous-0.9.0/turbogears/scheduler.py` & `Nitrous-0.9.3/turbogears/scheduler.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/startup.py` & `Nitrous-0.9.3/turbogears/startup.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/css/interpreter.css` & `Nitrous-0.9.3/turbogears/static/css/interpreter.css`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/css/toolbox.css` & `Nitrous-0.9.3/turbogears/static/css/toolbox.css`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/css/widget.css` & `Nitrous-0.9.3/turbogears/static/css/widget.css`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/admi18n.png` & `Nitrous-0.9.3/turbogears/static/images/admi18n.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/arrow_left.png` & `Nitrous-0.9.3/turbogears/static/images/arrow_left.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/catwalk.png` & `Nitrous-0.9.3/turbogears/static/images/catwalk.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/catwalk_logo.png` & `Nitrous-0.9.3/turbogears/static/images/catwalk_logo.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/designer.png` & `Nitrous-0.9.3/turbogears/static/images/designer.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/discard.png` & `Nitrous-0.9.3/turbogears/static/images/discard.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/file.png` & `Nitrous-0.9.3/turbogears/static/images/file.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/folder.png` & `Nitrous-0.9.3/turbogears/static/images/folder.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/identity.png` & `Nitrous-0.9.3/turbogears/static/images/identity.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/info.png` & `Nitrous-0.9.3/turbogears/static/images/info.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/play.png` & `Nitrous-0.9.3/turbogears/static/images/play.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/shell.png` & `Nitrous-0.9.3/turbogears/static/images/shell.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/small_gear.png` & `Nitrous-0.9.3/turbogears/static/images/small_gear.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/stop.png` & `Nitrous-0.9.3/turbogears/static/images/stop.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/tg_power.png` & `Nitrous-0.9.3/turbogears/static/images/tg_power.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/tg_under_the_hood.png` & `Nitrous-0.9.3/turbogears/static/images/tg_under_the_hood.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/tg_under_the_hood_sans_gear.png` & `Nitrous-0.9.3/turbogears/static/images/tg_under_the_hood_sans_gear.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/toolbox_logo.png` & `Nitrous-0.9.3/turbogears/static/images/toolbox_logo.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/top.png` & `Nitrous-0.9.3/turbogears/static/images/top.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/top_bg.png` & `Nitrous-0.9.3/turbogears/static/images/top_bg.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/trash.png` & `Nitrous-0.9.3/turbogears/static/images/trash.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/images/widgets.png` & `Nitrous-0.9.3/turbogears/static/images/widgets.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/js/interpreter.js` & `Nitrous-0.9.3/turbogears/static/js/interpreter.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/js/tool-man/cookies.js` & `Nitrous-0.9.3/turbogears/static/js/tool-man/cookies.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/js/tool-man/coordinates.js` & `Nitrous-0.9.3/turbogears/static/js/tool-man/coordinates.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/js/tool-man/core.js` & `Nitrous-0.9.3/turbogears/static/js/tool-man/core.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/js/tool-man/css.js` & `Nitrous-0.9.3/turbogears/static/js/tool-man/css.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/js/tool-man/drag.js` & `Nitrous-0.9.3/turbogears/static/js/tool-man/drag.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/js/tool-man/dragsort.js` & `Nitrous-0.9.3/turbogears/static/js/tool-man/dragsort.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/static/js/tool-man/events.js` & `Nitrous-0.9.3/turbogears/static/js/tool-man/events.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/catwalk_models/browse.py` & `Nitrous-0.9.3/turbogears/tests/catwalk_models/browse.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/form.html` & `Nitrous-0.9.3/turbogears/tests/form.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/locale/en/LC_MESSAGES/messages.po` & `Nitrous-0.9.3/turbogears/tests/locale/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/locale/fi/LC_MESSAGES/messages.mo` & `Nitrous-0.9.3/turbogears/tests/locale/fi/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/locale/fi/LC_MESSAGES/messages.po` & `Nitrous-0.9.3/turbogears/tests/locale/fi/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_catwalk.py` & `Nitrous-0.9.3/turbogears/tests/test_catwalk.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_command_i18n.py` & `Nitrous-0.9.3/turbogears/tests/test_command_i18n.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_config.py` & `Nitrous-0.9.3/turbogears/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_controllers.py` & `Nitrous-0.9.3/turbogears/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_decorator.py` & `Nitrous-0.9.3/turbogears/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_errorhandling.py` & `Nitrous-0.9.3/turbogears/tests/test_errorhandling.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_expose.py` & `Nitrous-0.9.3/turbogears/tests/test_expose.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_paginate.py` & `Nitrous-0.9.3/turbogears/tests/test_paginate.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_restmethod.py` & `Nitrous-0.9.3/turbogears/tests/test_restmethod.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_safemultipart.py` & `Nitrous-0.9.3/turbogears/tests/test_safemultipart.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_session_mapper.py` & `Nitrous-0.9.3/turbogears/tests/test_session_mapper.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_sqlalchemy.py` & `Nitrous-0.9.3/turbogears/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_testutil.py` & `Nitrous-0.9.3/turbogears/tests/test_testutil.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_util.py` & `Nitrous-0.9.3/turbogears/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_validators.py` & `Nitrous-0.9.3/turbogears/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/tests/test_view.py` & `Nitrous-0.9.3/turbogears/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/testutil.py` & `Nitrous-0.9.3/turbogears/testutil.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/admi18n/__init__.py` & `Nitrous-0.9.3/turbogears/toolbox/admi18n/__init__.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/admi18n/internationalization.html` & `Nitrous-0.9.3/turbogears/toolbox/admi18n/internationalization.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/admi18n/language.html` & `Nitrous-0.9.3/turbogears/toolbox/admi18n/language.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/admi18n/languageManagement.html` & `Nitrous-0.9.3/turbogears/toolbox/admi18n/languageManagement.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/admi18n/po_view.html` & `Nitrous-0.9.3/turbogears/toolbox/admi18n/po_view.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/admi18n/stringCollection.html` & `Nitrous-0.9.3/turbogears/toolbox/admi18n/stringCollection.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/base.py` & `Nitrous-0.9.3/turbogears/toolbox/base.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/catwalk/__init__.py` & `Nitrous-0.9.3/turbogears/toolbox/catwalk/__init__.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/catwalk/browse.py` & `Nitrous-0.9.3/turbogears/toolbox/catwalk/browse.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/catwalk/browse_grid.html` & `Nitrous-0.9.3/turbogears/toolbox/catwalk/browse_grid.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/catwalk/catwalk.html` & `Nitrous-0.9.3/turbogears/toolbox/catwalk/catwalk.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/catwalk/columns.html` & `Nitrous-0.9.3/turbogears/toolbox/catwalk/columns.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/catwalk/static/css/catwalk.css` & `Nitrous-0.9.3/turbogears/toolbox/catwalk/static/css/catwalk.css`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/browse.js` & `Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/browse.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/catwalk.js` & `Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/catwalk.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/AmiJS.js` & `Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/AmiJS.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/greybox.css` & `Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/greybox.css`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/greybox.js` & `Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/greybox.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/greybox__.js` & `Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/greybox__.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/greybox_inline.js` & `Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/greybox_inline.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/logo.png` & `Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/logo.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/catwalk/static/javascript/greybox/overlay.png` & `Nitrous-0.9.3/turbogears/toolbox/catwalk/static/javascript/greybox/overlay.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/console.html` & `Nitrous-0.9.3/turbogears/toolbox/console.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/__init__.py` & `Nitrous-0.9.3/turbogears/toolbox/designer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/modelDesigner.html` & `Nitrous-0.9.3/turbogears/toolbox/designer/modelDesigner.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/css/style.css` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/css/style.css`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/images/shadow.png` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/images/shadow.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/images/shadow_bottom.png` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/images/shadow_bottom.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/images/shadow_corner.png` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/images/shadow_corner.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/images/shadow_right.png` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/images/shadow_right.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/index.html` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/index.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/ajax.js` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/ajax.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/animator.js` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/animator.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/generic.js` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/generic.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/io.js` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/io.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/main.js` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/main.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/objects.js` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/objects.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/settings.js` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/settings.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/js/sql_types.js` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/js/sql_types.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/styles/bar.css` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/styles/bar.css`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/diagram/styles/style.css` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/diagram/styles/style.css`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/images/info.png` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/images/info.png`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/javascript/modelDesigner.js` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/javascript/modelDesigner.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/sessions/Survey.js` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/sessions/Survey.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/sessions/TurboTunes.js` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/sessions/TurboTunes.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/designer/static/sessions/WebShop.js` & `Nitrous-0.9.3/turbogears/toolbox/designer/static/sessions/WebShop.js`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/info.html` & `Nitrous-0.9.3/turbogears/toolbox/info.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/main.html` & `Nitrous-0.9.3/turbogears/toolbox/main.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/master.html` & `Nitrous-0.9.3/turbogears/toolbox/master.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/shell.py` & `Nitrous-0.9.3/turbogears/toolbox/shell.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/toolbox/widgets.html` & `Nitrous-0.9.3/turbogears/toolbox/widgets.html`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/util.py` & `Nitrous-0.9.3/turbogears/util.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/validators.py` & `Nitrous-0.9.3/turbogears/validators.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/view/base.py` & `Nitrous-0.9.3/turbogears/view/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -590,7 +590,10 @@
             engines[plugin_name] = engine(stdvars, engine_options)
 
     if 'json' not in engines and 'default-json' in engines:
         engines['json'] = engines['default-json']
 
     if 'text' not in engines and 'default-text' in engines:
         engines['text'] = engines['default-text']
+
+    if 'csv' not in engines and 'default-text' in engines:
+        engines['csv'] = engines['default-text']
```

### Comparing `Nitrous-0.9.0/turbogears/view/genshisupport.py` & `Nitrous-0.9.3/turbogears/view/genshisupport.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/view/json.py` & `Nitrous-0.9.3/turbogears/view/json.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/view/templates/sitetemplate.kid` & `Nitrous-0.9.3/turbogears/view/templates/sitetemplate.kid`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/view/text.py` & `Nitrous-0.9.3/turbogears/view/text.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/visit/__init__.py` & `Nitrous-0.9.3/turbogears/visit/__init__.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/visit/api.py` & `Nitrous-0.9.3/turbogears/visit/api.py`

 * *Files identical despite different names*

### Comparing `Nitrous-0.9.0/turbogears/visit/savisit.py` & `Nitrous-0.9.3/turbogears/visit/savisit.py`

 * *Files identical despite different names*

