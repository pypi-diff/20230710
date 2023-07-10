# Comparing `tmp/pyglottolog-3.8.0.tar.gz` & `tmp/pyglottolog-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglottolog-3.8.0.tar", last modified: Fri May 20 10:39:21 2022, max compression
+gzip compressed data, was "pyglottolog-3.9.0.tar", last modified: Tue May 24 18:17:38 2022, max compression
```

## Comparing `pyglottolog-3.8.0.tar` & `pyglottolog-3.9.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-20 10:39:21.956956 pyglottolog-3.8.0/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    11357 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/LICENSE
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       93 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/MANIFEST.in
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     8829 2022-05-20 10:39:21.956956 pyglottolog-3.8.0/PKG-INFO
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6745 2021-12-08 11:25:59.000000 pyglottolog-3.8.0/README.md
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       75 2021-05-15 05:29:42.000000 pyglottolog-3.8.0/requirements.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      404 2022-05-20 10:39:21.956956 pyglottolog-3.8.0/setup.cfg
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1874 2022-05-20 10:37:49.000000 pyglottolog-3.8.0/setup.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-20 10:39:21.948956 pyglottolog-3.8.0/src/
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-20 10:39:21.948956 pyglottolog-3.8.0/src/pyglottolog/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       90 2022-05-20 10:38:02.000000 pyglottolog-3.8.0/src/pyglottolog/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2615 2021-04-08 05:34:52.000000 pyglottolog-3.8.0/src/pyglottolog/__main__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      602 2022-05-17 06:21:46.000000 pyglottolog-3.8.0/src/pyglottolog/_compat.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-20 10:39:21.952956 pyglottolog-3.8.0/src/pyglottolog/admin_commands/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      333 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/bib.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     8248 2021-05-15 06:47:22.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/check.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      156 2021-05-12 09:43:27.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/elpubbib.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      355 2022-05-17 13:54:52.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/evobib.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2079 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/fixgeojson.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      192 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/isobib.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      169 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/isoretirements.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1369 2021-02-27 16:48:50.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/langindex.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1822 2022-05-17 07:53:11.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/langscibib.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      144 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/ldhbib.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      882 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/lff2tree.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      705 2021-05-12 09:03:12.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/release.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      151 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/tree2lff.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      349 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/update.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      835 2022-05-18 08:14:32.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/updatebib.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      922 2021-12-08 12:43:47.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/updatelinks.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      829 2021-02-27 16:48:50.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/updatemacroareas.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      633 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/updatemetadata.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1354 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/updatesources.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      772 2021-02-27 16:49:13.000000 pyglottolog-3.8.0/src/pyglottolog/admin_commands/writelanguoidstats.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    18121 2021-05-16 08:07:24.000000 pyglottolog-3.8.0/src/pyglottolog/api.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      696 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/cli_util.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-20 10:39:21.952956 pyglottolog-3.8.0/src/pyglottolog/commands/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/commands/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1325 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/commands/create.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      661 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/commands/edit.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4290 2021-04-08 05:39:07.000000 pyglottolog-3.8.0/src/pyglottolog/commands/htmlmap.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1023 2021-02-27 16:47:41.000000 pyglottolog-3.8.0/src/pyglottolog/commands/iso2codes.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      722 2021-02-27 16:47:10.000000 pyglottolog-3.8.0/src/pyglottolog/commands/langdatastats.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1135 2021-02-27 16:46:30.000000 pyglottolog-3.8.0/src/pyglottolog/commands/langsearch.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      323 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/commands/languoids.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      685 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/commands/refsearch.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      429 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/commands/searchindex.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1585 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/commands/show.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1952 2021-02-27 16:45:49.000000 pyglottolog-3.8.0/src/pyglottolog/commands/tree.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-20 10:39:21.952956 pyglottolog-3.8.0/src/pyglottolog/config/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5547 2021-05-15 13:13:28.000000 pyglottolog-3.8.0/src/pyglottolog/config/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      647 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/config/aes_sources.ini
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      861 2021-03-09 07:01:44.000000 pyglottolog-3.8.0/src/pyglottolog/config/aes_status.ini
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5181 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/config/document_types.ini
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      562 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/config/editors.ini
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1188 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/config/language_types.ini
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      897 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/config/languoid_levels.ini
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1091 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/config/macroareas.ini
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      595 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/config/med_types.ini
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      481 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/config/publication.ini
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5336 2021-05-16 05:49:03.000000 pyglottolog-3.8.0/src/pyglottolog/fts.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    12075 2021-05-17 07:21:01.000000 pyglottolog-3.8.0/src/pyglottolog/iso.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-20 10:39:21.952956 pyglottolog-3.8.0/src/pyglottolog/languoids/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      409 2021-05-15 14:46:22.000000 pyglottolog-3.8.0/src/pyglottolog/languoids/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    22477 2022-05-17 05:28:43.000000 pyglottolog-3.8.0/src/pyglottolog/languoids/languoid.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    11731 2021-12-08 14:58:52.000000 pyglottolog-3.8.0/src/pyglottolog/languoids/models.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     9442 2021-05-16 05:46:34.000000 pyglottolog-3.8.0/src/pyglottolog/lff.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-20 10:39:21.952956 pyglottolog-3.8.0/src/pyglottolog/links/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      559 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/links/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4731 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/links/aiatsis.json
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2484 2021-05-12 13:14:22.000000 pyglottolog-3.8.0/src/pyglottolog/links/aiatsis.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1055 2021-02-27 16:29:42.000000 pyglottolog-3.8.0/src/pyglottolog/links/crubadan.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    11598 2021-12-08 12:27:26.000000 pyglottolog-3.8.0/src/pyglottolog/links/endangeredlanguages.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2706 2022-05-20 10:23:31.000000 pyglottolog-3.8.0/src/pyglottolog/links/util.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1990 2021-12-08 15:01:06.000000 pyglottolog-3.8.0/src/pyglottolog/links/wikidata.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2937 2021-05-12 13:38:00.000000 pyglottolog-3.8.0/src/pyglottolog/metadata.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5552 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/monster.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-20 10:39:21.952956 pyglottolog-3.8.0/src/pyglottolog/monsterlib/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/monsterlib/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      103 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/monsterlib/roman.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      137 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/objects.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-20 10:39:21.956956 pyglottolog-3.8.0/src/pyglottolog/references/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      327 2021-05-06 12:49:44.000000 pyglottolog-3.8.0/src/pyglottolog/references/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    15410 2021-12-08 15:03:15.000000 pyglottolog-3.8.0/src/pyglottolog/references/bibfiles.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    40802 2022-05-17 06:21:46.000000 pyglottolog-3.8.0/src/pyglottolog/references/bibfiles_db.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5746 2022-05-17 06:22:43.000000 pyglottolog-3.8.0/src/pyglottolog/references/bibtex.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      541 2021-05-06 12:49:44.000000 pyglottolog-3.8.0/src/pyglottolog/references/bibtex_undiacritic.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4108 2021-05-12 09:40:20.000000 pyglottolog-3.8.0/src/pyglottolog/references/elpubbib.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1556 2021-05-06 12:49:44.000000 pyglottolog-3.8.0/src/pyglottolog/references/evobib.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1836 2021-05-06 12:49:44.000000 pyglottolog-3.8.0/src/pyglottolog/references/hhtypes.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3524 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/references/isbns.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      591 2021-05-06 12:49:44.000000 pyglottolog-3.8.0/src/pyglottolog/references/ldh.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    13107 2021-05-06 12:49:44.000000 pyglottolog-3.8.0/src/pyglottolog/references/libmonster.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      758 2021-05-06 12:49:44.000000 pyglottolog-3.8.0/src/pyglottolog/references/roman.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2678 2021-05-06 12:49:44.000000 pyglottolog-3.8.0/src/pyglottolog/references/util.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-20 10:39:21.948956 pyglottolog-3.8.0/src/pyglottolog/templates/
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-20 10:39:21.956956 pyglottolog-3.8.0/src/pyglottolog/templates/htmlmap/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1307 2021-04-08 05:11:39.000000 pyglottolog-3.8.0/src/pyglottolog/templates/htmlmap/htmlmap.html
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1778 2022-05-20 08:31:22.000000 pyglottolog-3.8.0/src/pyglottolog/templates/htmlmap/htmlmap.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3364 2021-02-17 15:41:12.000000 pyglottolog-3.8.0/src/pyglottolog/util.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-20 10:39:21.948956 pyglottolog-3.8.0/src/pyglottolog.egg-info/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     8829 2022-05-20 10:39:21.000000 pyglottolog-3.8.0/src/pyglottolog.egg-info/PKG-INFO
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3434 2022-05-20 10:39:21.000000 pyglottolog-3.8.0/src/pyglottolog.egg-info/SOURCES.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2022-05-20 10:39:21.000000 pyglottolog-3.8.0/src/pyglottolog.egg-info/dependency_links.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      107 2022-05-20 10:39:21.000000 pyglottolog-3.8.0/src/pyglottolog.egg-info/entry_points.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2021-02-17 15:42:44.000000 pyglottolog-3.8.0/src/pyglottolog.egg-info/not-zip-safe
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      384 2022-05-20 10:39:21.000000 pyglottolog-3.8.0/src/pyglottolog.egg-info/requires.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       12 2022-05-20 10:39:21.000000 pyglottolog-3.8.0/src/pyglottolog.egg-info/top_level.txt
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-24 18:17:38.559695 pyglottolog-3.9.0/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    11357 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/LICENSE
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       93 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/MANIFEST.in
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     8829 2022-05-24 18:17:38.559695 pyglottolog-3.9.0/PKG-INFO
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6745 2021-12-08 11:25:59.000000 pyglottolog-3.9.0/README.md
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       75 2021-05-15 05:29:42.000000 pyglottolog-3.9.0/requirements.txt
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      404 2022-05-24 18:17:38.559695 pyglottolog-3.9.0/setup.cfg
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1874 2022-05-24 18:16:16.000000 pyglottolog-3.9.0/setup.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-24 18:17:38.551695 pyglottolog-3.9.0/src/
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-24 18:17:38.555695 pyglottolog-3.9.0/src/pyglottolog/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       90 2022-05-24 18:16:31.000000 pyglottolog-3.9.0/src/pyglottolog/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2615 2021-04-08 05:34:52.000000 pyglottolog-3.9.0/src/pyglottolog/__main__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      602 2022-05-17 06:21:46.000000 pyglottolog-3.9.0/src/pyglottolog/_compat.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-24 18:17:38.555695 pyglottolog-3.9.0/src/pyglottolog/admin_commands/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      333 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/bib.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     8248 2021-05-15 06:47:22.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/check.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      156 2021-05-12 09:43:27.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/elpubbib.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      355 2022-05-17 13:54:52.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/evobib.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2079 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/fixgeojson.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      192 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/isobib.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      169 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/isoretirements.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1369 2021-02-27 16:48:50.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/langindex.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1822 2022-05-17 07:53:11.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/langscibib.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      144 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/ldhbib.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      882 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/lff2tree.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      705 2021-05-12 09:03:12.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/release.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      151 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/tree2lff.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      349 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/update.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      835 2022-05-18 08:14:32.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/updatebib.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      922 2021-12-08 12:43:47.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/updatelinks.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      829 2021-02-27 16:48:50.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/updatemacroareas.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      633 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/updatemetadata.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1354 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/updatesources.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      772 2021-02-27 16:49:13.000000 pyglottolog-3.9.0/src/pyglottolog/admin_commands/writelanguoidstats.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    18121 2021-05-16 08:07:24.000000 pyglottolog-3.9.0/src/pyglottolog/api.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      696 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/cli_util.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-24 18:17:38.559695 pyglottolog-3.9.0/src/pyglottolog/commands/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/commands/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1325 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/commands/create.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      661 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/commands/edit.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4290 2021-04-08 05:39:07.000000 pyglottolog-3.9.0/src/pyglottolog/commands/htmlmap.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1023 2021-02-27 16:47:41.000000 pyglottolog-3.9.0/src/pyglottolog/commands/iso2codes.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      722 2021-02-27 16:47:10.000000 pyglottolog-3.9.0/src/pyglottolog/commands/langdatastats.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1135 2021-02-27 16:46:30.000000 pyglottolog-3.9.0/src/pyglottolog/commands/langsearch.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      323 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/commands/languoids.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      685 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/commands/refsearch.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      429 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/commands/searchindex.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1585 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/commands/show.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1952 2021-02-27 16:45:49.000000 pyglottolog-3.9.0/src/pyglottolog/commands/tree.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-24 18:17:38.559695 pyglottolog-3.9.0/src/pyglottolog/config/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5547 2021-05-15 13:13:28.000000 pyglottolog-3.9.0/src/pyglottolog/config/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      647 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/config/aes_sources.ini
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      861 2021-03-09 07:01:44.000000 pyglottolog-3.9.0/src/pyglottolog/config/aes_status.ini
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5181 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/config/document_types.ini
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      562 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/config/editors.ini
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1188 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/config/language_types.ini
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      897 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/config/languoid_levels.ini
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1091 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/config/macroareas.ini
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      595 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/config/med_types.ini
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      481 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/config/publication.ini
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5336 2021-05-16 05:49:03.000000 pyglottolog-3.9.0/src/pyglottolog/fts.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    12075 2021-05-17 07:21:01.000000 pyglottolog-3.9.0/src/pyglottolog/iso.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-24 18:17:38.559695 pyglottolog-3.9.0/src/pyglottolog/languoids/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      409 2021-05-15 14:46:22.000000 pyglottolog-3.9.0/src/pyglottolog/languoids/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    22477 2022-05-17 05:28:43.000000 pyglottolog-3.9.0/src/pyglottolog/languoids/languoid.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    11731 2021-12-08 14:58:52.000000 pyglottolog-3.9.0/src/pyglottolog/languoids/models.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     9442 2021-05-16 05:46:34.000000 pyglottolog-3.9.0/src/pyglottolog/lff.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-24 18:17:38.559695 pyglottolog-3.9.0/src/pyglottolog/links/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      559 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/links/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4731 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/links/aiatsis.json
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2508 2022-05-23 11:22:38.000000 pyglottolog-3.9.0/src/pyglottolog/links/aiatsis.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1113 2022-05-23 11:16:08.000000 pyglottolog-3.9.0/src/pyglottolog/links/crubadan.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    11598 2021-12-08 12:27:26.000000 pyglottolog-3.9.0/src/pyglottolog/links/endangeredlanguages.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2706 2022-05-20 10:23:31.000000 pyglottolog-3.9.0/src/pyglottolog/links/util.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1990 2021-12-08 15:01:06.000000 pyglottolog-3.9.0/src/pyglottolog/links/wikidata.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2937 2021-05-12 13:38:00.000000 pyglottolog-3.9.0/src/pyglottolog/metadata.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5552 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/monster.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-24 18:17:38.559695 pyglottolog-3.9.0/src/pyglottolog/monsterlib/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/monsterlib/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      103 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/monsterlib/roman.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      137 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/objects.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-24 18:17:38.559695 pyglottolog-3.9.0/src/pyglottolog/references/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      327 2021-05-06 12:49:44.000000 pyglottolog-3.9.0/src/pyglottolog/references/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    15410 2021-12-08 15:03:15.000000 pyglottolog-3.9.0/src/pyglottolog/references/bibfiles.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    40802 2022-05-17 06:21:46.000000 pyglottolog-3.9.0/src/pyglottolog/references/bibfiles_db.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5746 2022-05-17 06:22:43.000000 pyglottolog-3.9.0/src/pyglottolog/references/bibtex.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      541 2021-05-06 12:49:44.000000 pyglottolog-3.9.0/src/pyglottolog/references/bibtex_undiacritic.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4108 2021-05-12 09:40:20.000000 pyglottolog-3.9.0/src/pyglottolog/references/elpubbib.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1556 2021-05-06 12:49:44.000000 pyglottolog-3.9.0/src/pyglottolog/references/evobib.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1836 2021-05-06 12:49:44.000000 pyglottolog-3.9.0/src/pyglottolog/references/hhtypes.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3524 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/references/isbns.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      591 2021-05-06 12:49:44.000000 pyglottolog-3.9.0/src/pyglottolog/references/ldh.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    13107 2021-05-06 12:49:44.000000 pyglottolog-3.9.0/src/pyglottolog/references/libmonster.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      758 2021-05-06 12:49:44.000000 pyglottolog-3.9.0/src/pyglottolog/references/roman.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2678 2021-05-06 12:49:44.000000 pyglottolog-3.9.0/src/pyglottolog/references/util.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-24 18:17:38.551695 pyglottolog-3.9.0/src/pyglottolog/templates/
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-24 18:17:38.559695 pyglottolog-3.9.0/src/pyglottolog/templates/htmlmap/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1307 2021-04-08 05:11:39.000000 pyglottolog-3.9.0/src/pyglottolog/templates/htmlmap/htmlmap.html
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1778 2022-05-20 08:31:22.000000 pyglottolog-3.9.0/src/pyglottolog/templates/htmlmap/htmlmap.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3364 2021-02-17 15:41:12.000000 pyglottolog-3.9.0/src/pyglottolog/util.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-24 18:17:38.555695 pyglottolog-3.9.0/src/pyglottolog.egg-info/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     8829 2022-05-24 18:17:38.000000 pyglottolog-3.9.0/src/pyglottolog.egg-info/PKG-INFO
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3434 2022-05-24 18:17:38.000000 pyglottolog-3.9.0/src/pyglottolog.egg-info/SOURCES.txt
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2022-05-24 18:17:38.000000 pyglottolog-3.9.0/src/pyglottolog.egg-info/dependency_links.txt
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      107 2022-05-24 18:17:38.000000 pyglottolog-3.9.0/src/pyglottolog.egg-info/entry_points.txt
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2021-02-17 15:42:44.000000 pyglottolog-3.9.0/src/pyglottolog.egg-info/not-zip-safe
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      384 2022-05-24 18:17:38.000000 pyglottolog-3.9.0/src/pyglottolog.egg-info/requires.txt
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       12 2022-05-24 18:17:38.000000 pyglottolog-3.9.0/src/pyglottolog.egg-info/top_level.txt
```

### Comparing `pyglottolog-3.8.0/LICENSE` & `pyglottolog-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/PKG-INFO` & `pyglottolog-3.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglottolog
-Version: 3.8.0
+Version: 3.9.0
 Summary: python package for glottolog data curation
 Home-page: https://github.com/clld/pyglottolog
 Author: Robert Forkel
 Author-email: forkel@shh.mpg.de
 License: Apache 2.0
 Description: # pyglottolog
```

### Comparing `pyglottolog-3.8.0/README.md` & `pyglottolog-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/setup.py` & `pyglottolog-3.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 from setuptools import setup, find_packages
 
 
 setup(
     name='pyglottolog',
-    version='3.8.0',
+    version='3.9.0',
     author='Robert Forkel',
     author_email='forkel@shh.mpg.de',
     description='python package for glottolog data curation',
     long_description=pathlib.Path('README.md').read_text(encoding='utf-8'),
     long_description_content_type='text/markdown',
     keywords='data linguistics',
     license='Apache 2.0',
```

### Comparing `pyglottolog-3.8.0/src/pyglottolog/__main__.py` & `pyglottolog-3.9.0/src/pyglottolog/__main__.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/_compat.py` & `pyglottolog-3.9.0/src/pyglottolog/_compat.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/admin_commands/check.py` & `pyglottolog-3.9.0/src/pyglottolog/admin_commands/check.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/admin_commands/fixgeojson.py` & `pyglottolog-3.9.0/src/pyglottolog/admin_commands/fixgeojson.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/admin_commands/langindex.py` & `pyglottolog-3.9.0/src/pyglottolog/admin_commands/langindex.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/admin_commands/langscibib.py` & `pyglottolog-3.9.0/src/pyglottolog/admin_commands/langscibib.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/admin_commands/lff2tree.py` & `pyglottolog-3.9.0/src/pyglottolog/admin_commands/lff2tree.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/admin_commands/release.py` & `pyglottolog-3.9.0/src/pyglottolog/admin_commands/release.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/admin_commands/updatebib.py` & `pyglottolog-3.9.0/src/pyglottolog/admin_commands/updatebib.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/admin_commands/updatelinks.py` & `pyglottolog-3.9.0/src/pyglottolog/admin_commands/updatelinks.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/admin_commands/updatemacroareas.py` & `pyglottolog-3.9.0/src/pyglottolog/admin_commands/updatemacroareas.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/admin_commands/updatemetadata.py` & `pyglottolog-3.9.0/src/pyglottolog/admin_commands/updatemetadata.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/admin_commands/updatesources.py` & `pyglottolog-3.9.0/src/pyglottolog/admin_commands/updatesources.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/admin_commands/writelanguoidstats.py` & `pyglottolog-3.9.0/src/pyglottolog/admin_commands/writelanguoidstats.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/api.py` & `pyglottolog-3.9.0/src/pyglottolog/api.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/cli_util.py` & `pyglottolog-3.9.0/src/pyglottolog/cli_util.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/commands/create.py` & `pyglottolog-3.9.0/src/pyglottolog/commands/create.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/commands/edit.py` & `pyglottolog-3.9.0/src/pyglottolog/commands/edit.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/commands/htmlmap.py` & `pyglottolog-3.9.0/src/pyglottolog/commands/htmlmap.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/commands/iso2codes.py` & `pyglottolog-3.9.0/src/pyglottolog/commands/iso2codes.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/commands/langdatastats.py` & `pyglottolog-3.9.0/src/pyglottolog/commands/langdatastats.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/commands/langsearch.py` & `pyglottolog-3.9.0/src/pyglottolog/commands/langsearch.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/commands/refsearch.py` & `pyglottolog-3.9.0/src/pyglottolog/commands/refsearch.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/commands/show.py` & `pyglottolog-3.9.0/src/pyglottolog/commands/show.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/commands/tree.py` & `pyglottolog-3.9.0/src/pyglottolog/commands/tree.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/config/__init__.py` & `pyglottolog-3.9.0/src/pyglottolog/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/config/aes_sources.ini` & `pyglottolog-3.9.0/src/pyglottolog/config/aes_sources.ini`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/config/aes_status.ini` & `pyglottolog-3.9.0/src/pyglottolog/config/aes_status.ini`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/config/document_types.ini` & `pyglottolog-3.9.0/src/pyglottolog/config/document_types.ini`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/config/editors.ini` & `pyglottolog-3.9.0/src/pyglottolog/config/editors.ini`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/config/language_types.ini` & `pyglottolog-3.9.0/src/pyglottolog/config/language_types.ini`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/config/languoid_levels.ini` & `pyglottolog-3.9.0/src/pyglottolog/config/languoid_levels.ini`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/config/macroareas.ini` & `pyglottolog-3.9.0/src/pyglottolog/config/macroareas.ini`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/config/med_types.ini` & `pyglottolog-3.9.0/src/pyglottolog/config/med_types.ini`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/fts.py` & `pyglottolog-3.9.0/src/pyglottolog/fts.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/iso.py` & `pyglottolog-3.9.0/src/pyglottolog/iso.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/languoids/languoid.py` & `pyglottolog-3.9.0/src/pyglottolog/languoids/languoid.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/languoids/models.py` & `pyglottolog-3.9.0/src/pyglottolog/languoids/models.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/lff.py` & `pyglottolog-3.9.0/src/pyglottolog/lff.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/links/__init__.py` & `pyglottolog-3.9.0/src/pyglottolog/links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/links/aiatsis.json` & `pyglottolog-3.9.0/src/pyglottolog/links/aiatsis.json`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/links/aiatsis.py` & `pyglottolog-3.9.0/src/pyglottolog/links/aiatsis.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
          "e9a9ea06-d821-4b53-a05f-877409a1a19c/download/aiatsis_austlang_endpoint_001.csv"
 # We get the mapping from AIATSIS to Glottolog from Chirila:
 URL = 'http://chirila.yale.edu/languages'
 
 
 class AIATSIS(LinkProvider):
     def iterupdated(self, languoids):  # pragma: no cover
+        return
         res = reader(
             io.StringIO(requests.get(MD_URL).content.decode('utf-8-sig')),
             dialect=Dialect(skipBlankRows=True, commentPrefix='<'),
             dicts=True)
-        md = {d['language_code']: d for d in res}
+        md = {d['language_code']: d for d in res if 'language_code' in d}
         lmap = collections.defaultdict(set)
-        return
         for line in requests.get(URL).text.splitlines():
             if line.startswith('var curItem'):
                 line = line.split('=', maxsplit=1)[1]
                 d = json.loads(line)
                 if d['AIATSIS_Code'] and d['Glottolog_ID']:
                     codes = [c.strip().replace('*', '') for c in d['AIATSIS_Code'].split(',')]
                     for code in codes:
```

### Comparing `pyglottolog-3.8.0/src/pyglottolog/links/crubadan.py` & `pyglottolog-3.9.0/src/pyglottolog/links/crubadan.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,16 +18,17 @@
             },
             headers={"accept": "application/json", "x-requested-with": "XMLHttpRequest"},
         ).json()
         for row in data['aaData']:
             yield (row[1].strip(), row[2].strip())
 
 
-class CRUBADAN(LinkProvider):
-    def iterupdated(self, languoids):  # pragma: no cover
-        lmap = collections.defaultdict(list)
-        for lid, iso in iter_id_iso():
-            lmap[iso].append(lid)
-        for lang in languoids:
-            links = ["http://crubadan.org/languages/" + c for c in lmap.get(lang.iso, [])]
-            if lang.update_links('crubadan.org', links):
-                yield lang
+# crubadan.org seems to no longer be operational
+#class CRUBADAN(LinkProvider):
+#    def iterupdated(self, languoids):  # pragma: no cover
+#        lmap = collections.defaultdict(list)
+#        for lid, iso in iter_id_iso():
+#            lmap[iso].append(lid)
+#        for lang in languoids:
+#            links = ["http://crubadan.org/languages/" + c for c in lmap.get(lang.iso, [])]
+#            if lang.update_links('crubadan.org', links):
+#                yield lang
```

### Comparing `pyglottolog-3.8.0/src/pyglottolog/links/endangeredlanguages.py` & `pyglottolog-3.9.0/src/pyglottolog/links/endangeredlanguages.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/links/util.py` & `pyglottolog-3.9.0/src/pyglottolog/links/util.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/links/wikidata.py` & `pyglottolog-3.9.0/src/pyglottolog/links/wikidata.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/metadata.py` & `pyglottolog-3.9.0/src/pyglottolog/metadata.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/monster.py` & `pyglottolog-3.9.0/src/pyglottolog/monster.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/references/bibfiles.py` & `pyglottolog-3.9.0/src/pyglottolog/references/bibfiles.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/references/bibfiles_db.py` & `pyglottolog-3.9.0/src/pyglottolog/references/bibfiles_db.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/references/bibtex.py` & `pyglottolog-3.9.0/src/pyglottolog/references/bibtex.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/references/bibtex_undiacritic.py` & `pyglottolog-3.9.0/src/pyglottolog/references/bibtex_undiacritic.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/references/elpubbib.py` & `pyglottolog-3.9.0/src/pyglottolog/references/elpubbib.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/references/evobib.py` & `pyglottolog-3.9.0/src/pyglottolog/references/evobib.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/references/hhtypes.py` & `pyglottolog-3.9.0/src/pyglottolog/references/hhtypes.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/references/isbns.py` & `pyglottolog-3.9.0/src/pyglottolog/references/isbns.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/references/ldh.py` & `pyglottolog-3.9.0/src/pyglottolog/references/ldh.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/references/libmonster.py` & `pyglottolog-3.9.0/src/pyglottolog/references/libmonster.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/references/roman.py` & `pyglottolog-3.9.0/src/pyglottolog/references/roman.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/references/util.py` & `pyglottolog-3.9.0/src/pyglottolog/references/util.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/templates/htmlmap/htmlmap.html` & `pyglottolog-3.9.0/src/pyglottolog/templates/htmlmap/htmlmap.html`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/templates/htmlmap/htmlmap.js` & `pyglottolog-3.9.0/src/pyglottolog/templates/htmlmap/htmlmap.js`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog/util.py` & `pyglottolog-3.9.0/src/pyglottolog/util.py`

 * *Files identical despite different names*

### Comparing `pyglottolog-3.8.0/src/pyglottolog.egg-info/PKG-INFO` & `pyglottolog-3.9.0/src/pyglottolog.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglottolog
-Version: 3.8.0
+Version: 3.9.0
 Summary: python package for glottolog data curation
 Home-page: https://github.com/clld/pyglottolog
 Author: Robert Forkel
 Author-email: forkel@shh.mpg.de
 License: Apache 2.0
 Description: # pyglottolog
```

### Comparing `pyglottolog-3.8.0/src/pyglottolog.egg-info/SOURCES.txt` & `pyglottolog-3.9.0/src/pyglottolog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

