# Comparing `tmp/concrete-4.9.4.tar.gz` & `tmp/concrete-4.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/concrete-4.9.4.tar", last modified: Mon Jul 11 14:57:12 2016, max compression
+gzip compressed data, was "dist/concrete-4.9.6.tar", last modified: Tue Jul 19 00:48:43 2016, max compression
```

## Comparing `concrete-4.9.4.tar` & `concrete-4.9.6.tar`

### file list

```diff
@@ -1,193 +1,194 @@
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/examples/
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     6633 2016-07-06 11:24:06.000000 concrete-4.9.4/examples/annotate_example.py
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     1554 2016-07-06 11:24:06.000000 concrete-4.9.4/examples/annotator_server.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/scripts/
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     1475 2016-07-06 11:24:06.000000 concrete-4.9.4/scripts/create-comm.py
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     3904 2016-07-06 11:24:06.000000 concrete-4.9.4/scripts/create-comm-tarball.py
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     2003 2016-07-06 11:24:06.000000 concrete-4.9.4/scripts/concrete_diff.py
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     6415 2016-07-06 11:24:06.000000 concrete-4.9.4/scripts/convert_protocols.py
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     3425 2016-07-06 11:24:06.000000 concrete-4.9.4/scripts/compress-uuids.py
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     5644 2016-07-06 11:24:06.000000 concrete-4.9.4/scripts/tweets2concrete.py
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     5826 2016-07-06 11:24:06.000000 concrete-4.9.4/scripts/tweets2concrete
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     1436 2016-07-06 11:24:06.000000 concrete-4.9.4/scripts/validate_communication.py
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     3685 2016-07-06 11:24:06.000000 concrete-4.9.4/scripts/inspect_dependency_parses.py
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     3614 2016-07-06 11:24:06.000000 concrete-4.9.4/scripts/compress-uuids
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     6123 2016-07-06 11:24:06.000000 concrete-4.9.4/scripts/concrete_inspect.py
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     2305 2016-07-06 11:24:06.000000 concrete-4.9.4/scripts/concrete2json.py
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     1638 2016-07-06 11:24:06.000000 concrete-4.9.4/scripts/annotator_client.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     1587 2016-07-06 11:24:06.000000 concrete-4.9.4/LICENSE.md
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete.egg-info/
--rw-r--r--   0 cjmay      (501) cjmay      (501)       66 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete.egg-info/requires.txt
--rw-r--r--   0 cjmay      (501) cjmay      (501)     4704 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete.egg-info/SOURCES.txt
--rw-r--r--   0 cjmay      (501) cjmay      (501)        1 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete.egg-info/dependency_links.txt
--rw-r--r--   0 cjmay      (501) cjmay      (501)        9 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete.egg-info/top_level.txt
--rw-r--r--   0 cjmay      (501) cjmay      (501)      257 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete.egg-info/PKG-INFO
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/tests/
--rw-r--r--   0 cjmay      (501) cjmay      (501)    11941 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/test_uuid.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     7891 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/test_validate_communication.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    25708 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/test_file_io.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)      700 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/tweets.json.incomplete.gz
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/tests/util/
--rw-r--r--   0 cjmay      (501) cjmay      (501)     3232 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/util/test_annotator_wrapper.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     8270 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/util/test_tokenization.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    10421 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/test_simple_comm.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/tests/testdata/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      427 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/les-deux-chandeliers.tar.gz
--rw-r--r--   0 cjmay      (501) cjmay      (501)      980 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/tweets.json.incomplete.gz
--rw-r--r--   0 cjmay      (501) cjmay      (501)     9472 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/serif_dog-bites-man.concrete
--rw-r--r--   0 cjmay      (501) cjmay      (501)      521 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/les-deux-chandeliers.concrete
--rw-r--r--   0 cjmay      (501) cjmay      (501)      430 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/les-deux-chandeliers-perline.tar.gz
--rw-r--r--   0 cjmay      (501) cjmay      (501)      651 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/simple.tar.bz2
--rw-r--r--   0 cjmay      (501) cjmay      (501)      508 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/simple_concatenated.bz2
--rw-r--r--   0 cjmay      (501) cjmay      (501)     4603 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/tweets.deleted.json
--rw-r--r--   0 cjmay      (501) cjmay      (501)     4472 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/tweets.json
--rw-r--r--   0 cjmay      (501) cjmay      (501)      273 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/simple_1.concrete.bz2
--rw-r--r--   0 cjmay      (501) cjmay      (501)      400 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/les-deux-chandeliers.txt
--rw-r--r--   0 cjmay      (501) cjmay      (501)     4482 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/tweets.bad-line-unicode.json
--rw-r--r--   0 cjmay      (501) cjmay      (501)    10240 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/simple_nested.tar
--rw-r--r--   0 cjmay      (501) cjmay      (501)      851 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/simple_concatenated
--rw-r--r--   0 cjmay      (501) cjmay      (501)      449 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/simple_concatenated.gz
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/tests/testdata/a/
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/tests/testdata/a/b/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      283 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/a/b/simple_1.concrete
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/tests/testdata/a/c/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      285 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/a/c/simple_3.concrete
--rw-r--r--   0 cjmay      (501) cjmay      (501)      283 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/a/c/simple_2.concrete
--rw-r--r--   0 cjmay      (501) cjmay      (501)      967 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/tweets.json.gz
--rw-r--r--   0 cjmay      (501) cjmay      (501)     6676 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/tweets.invalid.json
--rw-r--r--   0 cjmay      (501) cjmay      (501)     1183 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/simple.zip
--rw-r--r--   0 cjmay      (501) cjmay      (501)    10240 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/simple.tar
--rw-r--r--   0 cjmay      (501) cjmay      (501)      578 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/les-deux-chandeliers.concrete.tar.gz
--rw-r--r--   0 cjmay      (501) cjmay      (501)      285 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/simple_3.concrete
--rw-r--r--   0 cjmay      (501) cjmay      (501)      283 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/simple_1.concrete
--rw-r--r--   0 cjmay      (501) cjmay      (501)     4476 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/tweets.unicode.json
--rw-r--r--   0 cjmay      (501) cjmay      (501)      589 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/simple.tar.gz
--rw-r--r--   0 cjmay      (501) cjmay      (501)      242 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/simple_1.concrete.gz
--rw-r--r--   0 cjmay      (501) cjmay      (501)      283 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/simple_2.concrete
--rw-r--r--   0 cjmay      (501) cjmay      (501)     4479 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/testdata/tweets.bad-line.json
--rw-r--r--   0 cjmay      (501) cjmay      (501)      218 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/test_helper.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     4539 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/test_mem_io.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     2684 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/test_annotator.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     1243 2016-07-06 11:24:06.000000 concrete-4.9.4/tests/test_repr.py
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     1806 2016-07-06 13:23:28.000000 concrete-4.9.4/tests/test_twitter.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/language/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/language/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     5539 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/language/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       34 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/language/__init__.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/search/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/search/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    18100 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/search/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    20952 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/search/Feedback.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    13182 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/search/Search.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       56 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/search/__init__.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/util/
--rw-r--r--   0 cjmay      (501) cjmay      (501)    16503 2016-07-06 11:24:06.000000 concrete-4.9.4/concrete/util/redis_io.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     6416 2016-07-06 11:24:06.000000 concrete-4.9.4/concrete/util/references.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    12690 2016-07-06 11:24:06.000000 concrete-4.9.4/concrete/util/concrete_uuid.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)      159 2016-07-06 11:24:06.000000 concrete-4.9.4/concrete/util/unnone.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     4121 2016-07-06 11:24:06.000000 concrete-4.9.4/concrete/util/json_fu.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    13297 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/util/file_io.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     1228 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/util/thrift_factory.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     2657 2016-07-06 11:24:06.000000 concrete-4.9.4/concrete/util/annotator_wrapper.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     7897 2016-07-06 13:23:28.000000 concrete-4.9.4/concrete/util/twitter.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     2657 2016-07-06 11:24:06.000000 concrete-4.9.4/concrete/util/tokenization.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     9501 2016-07-06 11:24:06.000000 concrete-4.9.4/concrete/util/simple_comm.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     1109 2016-07-06 11:24:06.000000 concrete-4.9.4/concrete/util/mem_io.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)      300 2016-07-06 11:24:06.000000 concrete-4.9.4/concrete/util/__init__.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)      283 2016-07-06 11:24:06.000000 concrete-4.9.4/concrete/util/net.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    30090 2016-07-06 11:24:06.000000 concrete-4.9.4/concrete/validate.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/uuid/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/uuid/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     2620 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/uuid/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       34 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/uuid/__init__.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/entities/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/entities/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    24622 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/entities/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       34 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/entities/__init__.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/nitf/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/nitf/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    39943 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/nitf/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       34 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/nitf/__init__.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/email/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/email/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    15593 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/email/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       34 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/email/__init__.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/access/
--rw-r--r--   0 cjmay      (501) cjmay      (501)     7774 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/access/Retriever.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/access/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    11414 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/access/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     8309 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/access/Sender.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       57 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/access/__init__.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/services/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/services/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)      777 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/services/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    21822 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/services/Annotator.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     5601 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/services/Sender.py
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     2764 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/services/Annotator-remote
--rw-r--r--   0 cjmay      (501) cjmay      (501)       57 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/services/__init__.py
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)     2198 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/services/Sender-remote
--rw-r--r--   0 cjmay      (501) cjmay      (501)    22090 2016-07-06 11:24:06.000000 concrete-4.9.4/concrete/inspect.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/exceptions/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/exceptions/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     3048 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/exceptions/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       34 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/exceptions/__init__.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)      514 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/version.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/spans/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/spans/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     6457 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/spans/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       34 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/spans/__init__.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/audio/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/audio/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     4030 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/audio/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       34 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/audio/__init__.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/clustering/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/clustering/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    15030 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/clustering/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       34 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/clustering/__init__.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/situations/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/situations/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    58827 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/situations/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       34 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/situations/__init__.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/communication/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/communication/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    33440 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/communication/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       34 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/communication/__init__.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)      855 2016-07-06 11:24:06.000000 concrete-4.9.4/concrete/__init__.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/twitter/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/twitter/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    49890 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/twitter/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       34 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/twitter/__init__.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/structure/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/structure/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    92891 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/structure/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       34 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/structure/__init__.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/metadata/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/metadata/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    33491 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/metadata/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       34 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/metadata/__init__.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/concrete/linking/
--rw-r--r--   0 cjmay      (501) cjmay      (501)      303 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/linking/constants.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    11290 2016-07-11 14:56:55.000000 concrete-4.9.4/concrete/linking/ttypes.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)       34 2016-07-11 14:53:38.000000 concrete-4.9.4/concrete/linking/__init__.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     1309 2016-07-11 14:56:55.000000 concrete-4.9.4/setup.py
-drwxr-xr-x   0 cjmay      (501) cjmay      (501)        0 2016-07-11 14:57:12.000000 concrete-4.9.4/integration-tests/
--rw-r--r--   0 cjmay      (501) cjmay      (501)     7805 2016-07-06 11:24:06.000000 concrete-4.9.4/integration-tests/test_create_comm_tarball.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)    10136 2016-07-06 13:23:28.000000 concrete-4.9.4/integration-tests/test_tweets2concrete.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     3851 2016-07-06 11:24:06.000000 concrete-4.9.4/integration-tests/test_compress_uuids.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     9443 2016-07-06 11:24:06.000000 concrete-4.9.4/integration-tests/test_concrete_inspect.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     3527 2016-07-06 11:24:06.000000 concrete-4.9.4/integration-tests/test_streams.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     3560 2016-07-06 11:24:06.000000 concrete-4.9.4/integration-tests/test_create_comm.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)     2138 2016-07-06 11:24:06.000000 concrete-4.9.4/integration-tests/redis_server.py
--rwxr-xr-x   0 cjmay      (501) cjmay      (501)    28187 2016-07-06 11:24:06.000000 concrete-4.9.4/integration-tests/test_redis_io.py
--rw-r--r--   0 cjmay      (501) cjmay      (501)      205 2016-07-06 11:24:06.000000 concrete-4.9.4/tox.ini
--rw-r--r--   0 cjmay      (501) cjmay      (501)     1079 2016-07-11 14:56:55.000000 concrete-4.9.4/ubuntu.Dockerfile
--rw-r--r--   0 cjmay      (501) cjmay      (501)     4971 2016-07-11 14:56:55.000000 concrete-4.9.4/README.md
--rw-r--r--   0 cjmay      (501) cjmay      (501)     1113 2016-07-11 14:56:55.000000 concrete-4.9.4/Dockerfile
--rw-r--r--   0 cjmay      (501) cjmay      (501)       25 2016-07-06 11:24:06.000000 concrete-4.9.4/pytest.ini
--rw-r--r--   0 cjmay      (501) cjmay      (501)      320 2016-07-06 11:24:06.000000 concrete-4.9.4/MANIFEST.in
--rw-r--r--   0 cjmay      (501) cjmay      (501)       19 2016-07-06 11:24:06.000000 concrete-4.9.4/test-requirements.txt
--rw-r--r--   0 cjmay      (501) cjmay      (501)       14 2016-07-06 11:24:06.000000 concrete-4.9.4/requirements.txt
--rw-r--r--   0 cjmay      (501) cjmay      (501)      116 2016-07-11 14:57:12.000000 concrete-4.9.4/setup.cfg
--rw-r--r--   0 cjmay      (501) cjmay      (501)      257 2016-07-11 14:57:12.000000 concrete-4.9.4/PKG-INFO
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/access/
+-rw-r--r--   0 cmay      (1385) staff    (20063)     7774 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/access/Retriever.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     8309 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/access/Sender.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)       57 2016-07-05 18:36:29.000000 concrete-4.9.6/concrete/access/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/access/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    11414 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/access/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/audio/
+-rw-r--r--   0 cmay      (1385) staff    (20063)       34 2016-03-04 03:38:41.000000 concrete-4.9.6/concrete/audio/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/audio/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     4030 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/audio/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/clustering/
+-rw-r--r--   0 cmay      (1385) staff    (20063)       34 2016-03-04 03:38:41.000000 concrete-4.9.6/concrete/clustering/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/clustering/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    15030 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/clustering/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/communication/
+-rw-r--r--   0 cmay      (1385) staff    (20063)       34 2016-03-04 03:38:41.000000 concrete-4.9.6/concrete/communication/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/communication/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    33440 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/communication/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/email/
+-rw-r--r--   0 cmay      (1385) staff    (20063)       34 2016-03-04 03:38:41.000000 concrete-4.9.6/concrete/email/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/email/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    15593 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/email/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/entities/
+-rw-r--r--   0 cmay      (1385) staff    (20063)       34 2016-03-04 03:38:41.000000 concrete-4.9.6/concrete/entities/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/entities/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    24622 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/entities/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/exceptions/
+-rw-r--r--   0 cmay      (1385) staff    (20063)       34 2016-03-04 03:38:41.000000 concrete-4.9.6/concrete/exceptions/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/exceptions/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     3048 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/exceptions/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/language/
+-rw-r--r--   0 cmay      (1385) staff    (20063)       34 2016-03-04 03:38:41.000000 concrete-4.9.6/concrete/language/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/language/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     5539 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/language/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/linking/
+-rw-r--r--   0 cmay      (1385) staff    (20063)       34 2016-03-04 03:38:41.000000 concrete-4.9.6/concrete/linking/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/linking/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    11290 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/linking/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/metadata/
+-rw-r--r--   0 cmay      (1385) staff    (20063)       34 2016-03-04 03:38:41.000000 concrete-4.9.6/concrete/metadata/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/metadata/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    33491 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/metadata/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/nitf/
+-rw-r--r--   0 cmay      (1385) staff    (20063)       34 2016-03-04 03:38:41.000000 concrete-4.9.6/concrete/nitf/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/nitf/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    39943 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/nitf/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/search/
+-rw-r--r--   0 cmay      (1385) staff    (20063)    20952 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/search/Feedback.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    13182 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/search/Search.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)       56 2016-07-16 10:03:49.000000 concrete-4.9.6/concrete/search/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/search/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    18100 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/search/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/services/
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     2764 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/services/Annotator-remote
+-rw-r--r--   0 cmay      (1385) staff    (20063)    21822 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/services/Annotator.py
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     2198 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/services/Sender-remote
+-rw-r--r--   0 cmay      (1385) staff    (20063)     5601 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/services/Sender.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)       57 2016-06-27 16:49:26.000000 concrete-4.9.6/concrete/services/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/services/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      777 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/services/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/situations/
+-rw-r--r--   0 cmay      (1385) staff    (20063)       34 2016-03-04 03:38:40.000000 concrete-4.9.6/concrete/situations/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/situations/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    58827 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/situations/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/spans/
+-rw-r--r--   0 cmay      (1385) staff    (20063)       34 2016-03-04 03:38:40.000000 concrete-4.9.6/concrete/spans/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/spans/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     6457 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/spans/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/structure/
+-rw-r--r--   0 cmay      (1385) staff    (20063)       34 2016-03-04 03:38:40.000000 concrete-4.9.6/concrete/structure/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/structure/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    92891 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/structure/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/twitter/
+-rw-r--r--   0 cmay      (1385) staff    (20063)       34 2016-03-04 03:38:40.000000 concrete-4.9.6/concrete/twitter/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/twitter/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    49890 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/twitter/ttypes.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/util/
+-rw-r--r--   0 cmay      (1385) staff    (20063)      300 2016-01-29 18:50:02.000000 concrete-4.9.6/concrete/util/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     2657 2016-02-19 03:52:23.000000 concrete-4.9.6/concrete/util/annotator_wrapper.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    12690 2016-03-10 20:18:09.000000 concrete-4.9.6/concrete/util/concrete_uuid.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    13297 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/util/file_io.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     4121 2016-01-29 18:50:02.000000 concrete-4.9.6/concrete/util/json_fu.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     1109 2016-02-19 03:52:23.000000 concrete-4.9.6/concrete/util/mem_io.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      283 2016-01-16 11:13:51.000000 concrete-4.9.6/concrete/util/net.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    16503 2016-02-04 01:09:53.000000 concrete-4.9.6/concrete/util/redis_io.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     6416 2016-01-29 18:50:02.000000 concrete-4.9.6/concrete/util/references.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     2622 2016-07-19 00:47:59.000000 concrete-4.9.6/concrete/util/search_wrapper.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     9501 2016-05-17 00:20:53.000000 concrete-4.9.6/concrete/util/simple_comm.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     1228 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/util/thrift_factory.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     2657 2016-02-04 01:09:53.000000 concrete-4.9.6/concrete/util/tokenization.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     7897 2016-07-16 10:03:49.000000 concrete-4.9.6/concrete/util/twitter.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      159 2016-02-04 01:09:53.000000 concrete-4.9.6/concrete/util/unnone.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete/uuid/
+-rw-r--r--   0 cmay      (1385) staff    (20063)       34 2016-03-04 03:38:41.000000 concrete-4.9.6/concrete/uuid/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      303 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/uuid/constants.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     2620 2016-07-19 00:47:24.000000 concrete-4.9.6/concrete/uuid/ttypes.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      855 2016-02-19 03:52:23.000000 concrete-4.9.6/concrete/__init__.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    22090 2016-03-31 14:25:46.000000 concrete-4.9.6/concrete/inspect.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    30090 2016-02-19 03:52:23.000000 concrete-4.9.6/concrete/validate.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      514 2016-07-19 00:47:59.000000 concrete-4.9.6/concrete/version.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete.egg-info/
+-rw-r--r--   0 cmay      (1385) staff    (20063)      257 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete.egg-info/PKG-INFO
+-rw-r--r--   0 cmay      (1385) staff    (20063)     4739 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete.egg-info/SOURCES.txt
+-rw-r--r--   0 cmay      (1385) staff    (20063)        1 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete.egg-info/dependency_links.txt
+-rw-r--r--   0 cmay      (1385) staff    (20063)       66 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete.egg-info/requires.txt
+-rw-r--r--   0 cmay      (1385) staff    (20063)        9 2016-07-19 00:48:41.000000 concrete-4.9.6/concrete.egg-info/top_level.txt
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/examples/
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     6633 2016-02-19 03:52:23.000000 concrete-4.9.6/examples/annotate_example.py
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     1554 2016-02-19 03:52:23.000000 concrete-4.9.6/examples/annotator_server.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/integration-tests/
+-rw-r--r--   0 cmay      (1385) staff    (20063)     2138 2016-02-19 03:52:23.000000 concrete-4.9.6/integration-tests/redis_server.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     3851 2016-06-06 10:33:38.000000 concrete-4.9.6/integration-tests/test_compress_uuids.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     9443 2016-03-31 14:25:46.000000 concrete-4.9.6/integration-tests/test_concrete_inspect.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     3560 2016-05-17 00:20:53.000000 concrete-4.9.6/integration-tests/test_create_comm.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     7805 2016-05-17 00:20:53.000000 concrete-4.9.6/integration-tests/test_create_comm_tarball.py
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)    28187 2016-02-19 03:52:23.000000 concrete-4.9.6/integration-tests/test_redis_io.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     3527 2016-02-19 03:52:23.000000 concrete-4.9.6/integration-tests/test_streams.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    10136 2016-07-16 10:03:49.000000 concrete-4.9.6/integration-tests/test_tweets2concrete.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/scripts/
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     1638 2016-02-19 03:52:23.000000 concrete-4.9.6/scripts/annotator_client.py
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     3614 2016-06-06 10:33:38.000000 concrete-4.9.6/scripts/compress-uuids
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     3425 2016-06-06 10:33:38.000000 concrete-4.9.6/scripts/compress-uuids.py
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     2305 2016-02-19 03:52:23.000000 concrete-4.9.6/scripts/concrete2json.py
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     2003 2016-02-19 03:52:23.000000 concrete-4.9.6/scripts/concrete_diff.py
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     6123 2016-03-31 14:25:46.000000 concrete-4.9.6/scripts/concrete_inspect.py
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     6415 2016-02-19 03:52:23.000000 concrete-4.9.6/scripts/convert_protocols.py
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     3904 2016-05-25 13:26:07.000000 concrete-4.9.6/scripts/create-comm-tarball.py
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     1475 2016-05-17 00:20:54.000000 concrete-4.9.6/scripts/create-comm.py
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     3685 2016-02-19 03:52:23.000000 concrete-4.9.6/scripts/inspect_dependency_parses.py
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     5826 2016-06-06 10:33:38.000000 concrete-4.9.6/scripts/tweets2concrete
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     5644 2016-06-27 16:49:26.000000 concrete-4.9.6/scripts/tweets2concrete.py
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     1436 2016-02-19 03:52:23.000000 concrete-4.9.6/scripts/validate_communication.py
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/tests/
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/tests/testdata/
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/tests/testdata/a/
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/tests/testdata/a/b/
+-rw-r--r--   0 cmay      (1385) staff    (20063)      283 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/a/b/simple_1.concrete
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/tests/testdata/a/c/
+-rw-r--r--   0 cmay      (1385) staff    (20063)      283 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/a/c/simple_2.concrete
+-rw-r--r--   0 cmay      (1385) staff    (20063)      285 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/a/c/simple_3.concrete
+-rw-r--r--   0 cmay      (1385) staff    (20063)      430 2016-05-17 00:20:54.000000 concrete-4.9.6/tests/testdata/les-deux-chandeliers-perline.tar.gz
+-rw-r--r--   0 cmay      (1385) staff    (20063)      521 2016-05-17 00:20:54.000000 concrete-4.9.6/tests/testdata/les-deux-chandeliers.concrete
+-rw-r--r--   0 cmay      (1385) staff    (20063)      578 2016-05-17 00:20:54.000000 concrete-4.9.6/tests/testdata/les-deux-chandeliers.concrete.tar.gz
+-rw-r--r--   0 cmay      (1385) staff    (20063)      427 2016-05-17 00:20:54.000000 concrete-4.9.6/tests/testdata/les-deux-chandeliers.tar.gz
+-rw-r--r--   0 cmay      (1385) staff    (20063)      400 2016-05-17 00:20:54.000000 concrete-4.9.6/tests/testdata/les-deux-chandeliers.txt
+-rw-r--r--   0 cmay      (1385) staff    (20063)     9472 2016-01-16 11:13:52.000000 concrete-4.9.6/tests/testdata/serif_dog-bites-man.concrete
+-rw-r--r--   0 cmay      (1385) staff    (20063)    10240 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/simple.tar
+-rw-r--r--   0 cmay      (1385) staff    (20063)      651 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/simple.tar.bz2
+-rw-r--r--   0 cmay      (1385) staff    (20063)      589 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/simple.tar.gz
+-rw-r--r--   0 cmay      (1385) staff    (20063)     1183 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/simple.zip
+-rw-r--r--   0 cmay      (1385) staff    (20063)      283 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/simple_1.concrete
+-rw-r--r--   0 cmay      (1385) staff    (20063)      273 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/simple_1.concrete.bz2
+-rw-r--r--   0 cmay      (1385) staff    (20063)      242 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/simple_1.concrete.gz
+-rw-r--r--   0 cmay      (1385) staff    (20063)      283 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/simple_2.concrete
+-rw-r--r--   0 cmay      (1385) staff    (20063)      285 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/simple_3.concrete
+-rw-r--r--   0 cmay      (1385) staff    (20063)      851 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/simple_concatenated
+-rw-r--r--   0 cmay      (1385) staff    (20063)      508 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/simple_concatenated.bz2
+-rw-r--r--   0 cmay      (1385) staff    (20063)      449 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/simple_concatenated.gz
+-rw-r--r--   0 cmay      (1385) staff    (20063)    10240 2016-03-31 12:57:53.000000 concrete-4.9.6/tests/testdata/simple_nested.tar
+-rw-r--r--   0 cmay      (1385) staff    (20063)     4482 2016-06-27 16:49:26.000000 concrete-4.9.6/tests/testdata/tweets.bad-line-unicode.json
+-rw-r--r--   0 cmay      (1385) staff    (20063)     4479 2016-02-19 03:52:23.000000 concrete-4.9.6/tests/testdata/tweets.bad-line.json
+-rw-r--r--   0 cmay      (1385) staff    (20063)     4603 2016-02-19 03:52:23.000000 concrete-4.9.6/tests/testdata/tweets.deleted.json
+-rw-r--r--   0 cmay      (1385) staff    (20063)     6676 2016-02-19 03:52:23.000000 concrete-4.9.6/tests/testdata/tweets.invalid.json
+-rw-r--r--   0 cmay      (1385) staff    (20063)     4472 2016-02-19 03:52:23.000000 concrete-4.9.6/tests/testdata/tweets.json
+-rw-r--r--   0 cmay      (1385) staff    (20063)      967 2016-02-19 03:52:23.000000 concrete-4.9.6/tests/testdata/tweets.json.gz
+-rw-r--r--   0 cmay      (1385) staff    (20063)      980 2016-02-19 03:52:23.000000 concrete-4.9.6/tests/testdata/tweets.json.incomplete.gz
+-rw-r--r--   0 cmay      (1385) staff    (20063)     4476 2016-06-27 16:49:26.000000 concrete-4.9.6/tests/testdata/tweets.unicode.json
+drwxr-xr-x   0 cmay      (1385) staff    (20063)        0 2016-07-19 00:48:41.000000 concrete-4.9.6/tests/util/
+-rw-r--r--   0 cmay      (1385) staff    (20063)     3232 2016-02-04 01:09:53.000000 concrete-4.9.6/tests/util/test_annotator_wrapper.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     8270 2016-02-19 03:52:23.000000 concrete-4.9.6/tests/util/test_tokenization.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     2684 2016-02-19 03:52:23.000000 concrete-4.9.6/tests/test_annotator.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    25708 2016-05-17 00:20:54.000000 concrete-4.9.6/tests/test_file_io.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      218 2016-03-31 13:51:27.000000 concrete-4.9.6/tests/test_helper.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     4539 2016-02-19 03:52:23.000000 concrete-4.9.6/tests/test_mem_io.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     1243 2016-03-31 13:51:27.000000 concrete-4.9.6/tests/test_repr.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     2069 2016-07-19 00:47:59.000000 concrete-4.9.6/tests/test_search.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    10421 2016-04-18 01:16:19.000000 concrete-4.9.6/tests/test_simple_comm.py
+-rwxr-xr-x   0 cmay      (1385) staff    (20063)     1806 2016-07-16 10:03:49.000000 concrete-4.9.6/tests/test_twitter.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)    11941 2016-02-19 03:52:23.000000 concrete-4.9.6/tests/test_uuid.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)     7891 2016-03-31 13:51:27.000000 concrete-4.9.6/tests/test_validate_communication.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)      700 2016-02-19 03:52:23.000000 concrete-4.9.6/tests/tweets.json.incomplete.gz
+-rw-r--r--   0 cmay      (1385) staff    (20063)     1145 2016-07-19 00:47:24.000000 concrete-4.9.6/Dockerfile
+-rw-r--r--   0 cmay      (1385) staff    (20063)     1587 2016-02-19 03:52:23.000000 concrete-4.9.6/LICENSE.md
+-rw-r--r--   0 cmay      (1385) staff    (20063)      294 2016-07-16 10:03:54.000000 concrete-4.9.6/MANIFEST.in
+-rw-r--r--   0 cmay      (1385) staff    (20063)     4971 2016-07-19 00:47:24.000000 concrete-4.9.6/README.md
+-rw-r--r--   0 cmay      (1385) staff    (20063)       25 2016-06-06 10:32:56.000000 concrete-4.9.6/pytest.ini
+-rw-r--r--   0 cmay      (1385) staff    (20063)       14 2016-01-29 18:50:02.000000 concrete-4.9.6/requirements.txt
+-rw-r--r--   0 cmay      (1385) staff    (20063)     1309 2016-07-19 00:47:24.000000 concrete-4.9.6/setup.py
+-rw-r--r--   0 cmay      (1385) staff    (20063)       19 2016-01-29 18:50:02.000000 concrete-4.9.6/test-requirements.txt
+-rw-r--r--   0 cmay      (1385) staff    (20063)      205 2016-01-29 18:50:02.000000 concrete-4.9.6/tox.ini
+-rw-r--r--   0 cmay      (1385) staff    (20063)      257 2016-07-19 00:48:41.000000 concrete-4.9.6/PKG-INFO
+-rw-r--r--   0 cmay      (1385) staff    (20063)      116 2016-07-19 00:48:41.000000 concrete-4.9.6/setup.cfg
```

### Comparing `concrete-4.9.4/examples/annotate_example.py` & `concrete-4.9.6/examples/annotate_example.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/examples/annotator_server.py` & `concrete-4.9.6/examples/annotator_server.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/scripts/create-comm.py` & `concrete-4.9.6/scripts/create-comm.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/scripts/create-comm-tarball.py` & `concrete-4.9.6/scripts/create-comm-tarball.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/scripts/concrete_diff.py` & `concrete-4.9.6/scripts/concrete_diff.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/scripts/convert_protocols.py` & `concrete-4.9.6/scripts/convert_protocols.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/scripts/compress-uuids.py` & `concrete-4.9.6/scripts/compress-uuids.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/scripts/tweets2concrete.py` & `concrete-4.9.6/scripts/tweets2concrete.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/scripts/tweets2concrete` & `concrete-4.9.6/scripts/tweets2concrete`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/scripts/validate_communication.py` & `concrete-4.9.6/scripts/validate_communication.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/scripts/inspect_dependency_parses.py` & `concrete-4.9.6/scripts/inspect_dependency_parses.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/scripts/compress-uuids` & `concrete-4.9.6/scripts/compress-uuids`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/scripts/concrete_inspect.py` & `concrete-4.9.6/scripts/concrete_inspect.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/scripts/concrete2json.py` & `concrete-4.9.6/scripts/concrete2json.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/scripts/annotator_client.py` & `concrete-4.9.6/scripts/annotator_client.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/LICENSE.md` & `concrete-4.9.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete.egg-info/SOURCES.txt` & `concrete-4.9.6/concrete.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 README.md
 pytest.ini
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
 tox.ini
-ubuntu.Dockerfile
 concrete/__init__.py
 concrete/inspect.py
 concrete/validate.py
 concrete/version.py
 concrete.egg-info/PKG-INFO
 concrete.egg-info/SOURCES.txt
 concrete.egg-info/dependency_links.txt
@@ -82,14 +81,15 @@
 concrete/util/concrete_uuid.py
 concrete/util/file_io.py
 concrete/util/json_fu.py
 concrete/util/mem_io.py
 concrete/util/net.py
 concrete/util/redis_io.py
 concrete/util/references.py
+concrete/util/search_wrapper.py
 concrete/util/simple_comm.py
 concrete/util/thrift_factory.py
 concrete/util/tokenization.py
 concrete/util/twitter.py
 concrete/util/unnone.py
 concrete/uuid/__init__.py
 concrete/uuid/constants.py
@@ -118,14 +118,15 @@
 scripts/tweets2concrete.py
 scripts/validate_communication.py
 tests/test_annotator.py
 tests/test_file_io.py
 tests/test_helper.py
 tests/test_mem_io.py
 tests/test_repr.py
+tests/test_search.py
 tests/test_simple_comm.py
 tests/test_twitter.py
 tests/test_uuid.py
 tests/test_validate_communication.py
 tests/tweets.json.incomplete.gz
 tests/testdata/les-deux-chandeliers-perline.tar.gz
 tests/testdata/les-deux-chandeliers.concrete
```

### Comparing `concrete-4.9.4/tests/test_uuid.py` & `concrete-4.9.6/tests/test_uuid.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/test_validate_communication.py` & `concrete-4.9.6/tests/test_validate_communication.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/test_file_io.py` & `concrete-4.9.6/tests/test_file_io.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/tweets.json.incomplete.gz` & `concrete-4.9.6/tests/tweets.json.incomplete.gz`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/util/test_annotator_wrapper.py` & `concrete-4.9.6/tests/util/test_annotator_wrapper.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/util/test_tokenization.py` & `concrete-4.9.6/tests/util/test_tokenization.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/test_simple_comm.py` & `concrete-4.9.6/tests/test_simple_comm.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/tweets.json.incomplete.gz` & `concrete-4.9.6/tests/testdata/tweets.json.incomplete.gz`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/serif_dog-bites-man.concrete` & `concrete-4.9.6/tests/testdata/serif_dog-bites-man.concrete`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/les-deux-chandeliers.concrete` & `concrete-4.9.6/tests/testdata/les-deux-chandeliers.concrete`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/simple.tar.bz2` & `concrete-4.9.6/tests/testdata/simple.tar.bz2`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/tweets.deleted.json` & `concrete-4.9.6/tests/testdata/tweets.deleted.json`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/tweets.json` & `concrete-4.9.6/tests/testdata/tweets.json`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/tweets.bad-line-unicode.json` & `concrete-4.9.6/tests/testdata/tweets.bad-line-unicode.json`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/simple_nested.tar` & `concrete-4.9.6/tests/testdata/simple_nested.tar`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/simple_concatenated` & `concrete-4.9.6/tests/testdata/simple_concatenated`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/tweets.json.gz` & `concrete-4.9.6/tests/testdata/tweets.json.gz`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/tweets.invalid.json` & `concrete-4.9.6/tests/testdata/tweets.invalid.json`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/simple.zip` & `concrete-4.9.6/tests/testdata/simple.zip`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/simple.tar` & `concrete-4.9.6/tests/testdata/simple.tar`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/les-deux-chandeliers.concrete.tar.gz` & `concrete-4.9.6/tests/testdata/les-deux-chandeliers.concrete.tar.gz`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/tweets.unicode.json` & `concrete-4.9.6/tests/testdata/tweets.unicode.json`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/simple.tar.gz` & `concrete-4.9.6/tests/testdata/simple.tar.gz`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/testdata/tweets.bad-line.json` & `concrete-4.9.6/tests/testdata/tweets.bad-line.json`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/test_mem_io.py` & `concrete-4.9.6/tests/test_mem_io.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/test_annotator.py` & `concrete-4.9.6/tests/test_annotator.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/test_repr.py` & `concrete-4.9.6/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/tests/test_twitter.py` & `concrete-4.9.6/tests/test_twitter.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/language/ttypes.py` & `concrete-4.9.6/concrete/language/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/search/ttypes.py` & `concrete-4.9.6/concrete/search/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/search/Feedback.py` & `concrete-4.9.6/concrete/search/Feedback.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/search/Search.py` & `concrete-4.9.6/concrete/search/Search.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/util/redis_io.py` & `concrete-4.9.6/concrete/util/redis_io.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/util/references.py` & `concrete-4.9.6/concrete/util/references.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/util/concrete_uuid.py` & `concrete-4.9.6/concrete/util/concrete_uuid.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/util/json_fu.py` & `concrete-4.9.6/concrete/util/json_fu.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/util/file_io.py` & `concrete-4.9.6/concrete/util/file_io.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/util/thrift_factory.py` & `concrete-4.9.6/concrete/util/thrift_factory.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/util/annotator_wrapper.py` & `concrete-4.9.6/concrete/util/annotator_wrapper.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/util/twitter.py` & `concrete-4.9.6/concrete/util/twitter.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/util/tokenization.py` & `concrete-4.9.6/concrete/util/tokenization.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/util/simple_comm.py` & `concrete-4.9.6/concrete/util/simple_comm.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/util/mem_io.py` & `concrete-4.9.6/concrete/util/mem_io.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/validate.py` & `concrete-4.9.6/concrete/validate.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/uuid/ttypes.py` & `concrete-4.9.6/concrete/uuid/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/entities/ttypes.py` & `concrete-4.9.6/concrete/entities/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/nitf/ttypes.py` & `concrete-4.9.6/concrete/nitf/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/email/ttypes.py` & `concrete-4.9.6/concrete/email/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/access/Retriever.py` & `concrete-4.9.6/concrete/access/Retriever.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/access/ttypes.py` & `concrete-4.9.6/concrete/access/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/access/Sender.py` & `concrete-4.9.6/concrete/access/Sender.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/services/ttypes.py` & `concrete-4.9.6/concrete/services/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/services/Annotator.py` & `concrete-4.9.6/concrete/services/Annotator.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/services/Sender.py` & `concrete-4.9.6/concrete/services/Sender.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/services/Annotator-remote` & `concrete-4.9.6/concrete/services/Annotator-remote`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/services/Sender-remote` & `concrete-4.9.6/concrete/services/Sender-remote`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/inspect.py` & `concrete-4.9.6/concrete/inspect.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/exceptions/ttypes.py` & `concrete-4.9.6/concrete/exceptions/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/version.py` & `concrete-4.9.6/concrete/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '4.9.4'
+__version__ = '4.9.6'
 
 
 def concrete_library_version():
     return __version__
 
 
 def concrete_schema_version():
```

### Comparing `concrete-4.9.4/concrete/spans/ttypes.py` & `concrete-4.9.6/concrete/spans/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/audio/ttypes.py` & `concrete-4.9.6/concrete/audio/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/clustering/ttypes.py` & `concrete-4.9.6/concrete/clustering/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/situations/ttypes.py` & `concrete-4.9.6/concrete/situations/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/communication/ttypes.py` & `concrete-4.9.6/concrete/communication/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/__init__.py` & `concrete-4.9.6/concrete/__init__.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/twitter/ttypes.py` & `concrete-4.9.6/concrete/twitter/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/structure/ttypes.py` & `concrete-4.9.6/concrete/structure/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/metadata/ttypes.py` & `concrete-4.9.6/concrete/metadata/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/concrete/linking/ttypes.py` & `concrete-4.9.6/concrete/linking/ttypes.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/setup.py` & `concrete-4.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/integration-tests/test_create_comm_tarball.py` & `concrete-4.9.6/integration-tests/test_create_comm_tarball.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/integration-tests/test_tweets2concrete.py` & `concrete-4.9.6/integration-tests/test_tweets2concrete.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/integration-tests/test_compress_uuids.py` & `concrete-4.9.6/integration-tests/test_compress_uuids.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/integration-tests/test_concrete_inspect.py` & `concrete-4.9.6/integration-tests/test_concrete_inspect.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/integration-tests/test_streams.py` & `concrete-4.9.6/integration-tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/integration-tests/test_create_comm.py` & `concrete-4.9.6/integration-tests/test_create_comm.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/integration-tests/redis_server.py` & `concrete-4.9.6/integration-tests/redis_server.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/integration-tests/test_redis_io.py` & `concrete-4.9.6/integration-tests/test_redis_io.py`

 * *Files identical despite different names*

### Comparing `concrete-4.9.4/ubuntu.Dockerfile` & `concrete-4.9.6/Dockerfile`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-FROM ubuntu:trusty
+FROM centos:7
 
-RUN apt-get update
+RUN yum update -y && yum clean all
 
-RUN apt-get install -y \
+RUN yum install -y \
         autoconf \
         automake \
-        curl \
         gcc \
         git \
         libtool \
         m4 \
         make \
-        pkg-config \
+        pkgconfig \
         python \
-        python-dev \
-        python-pip
+        python-devel \
+        tar
 
-RUN pip install --upgrade --ignore-installed setuptools six && \
+RUN curl https://bootstrap.pypa.io/get-pip.py | python && \
+    pip install --upgrade setuptools && \
+    pip install --upgrade setuptools && \
     pip install --upgrade \
         pytest \
         pytest-cov \
         pytest-mock \
         flake8 \
         redis
 
 WORKDIR /tmp
 RUN mkdir -p /usr/local/{include,lib}
 
 RUN curl http://download.redis.io/releases/redis-3.2.0.tar.gz | tar -xz && \
-    cd redis-3.2.0 && \
+    pushd redis-3.2.0 && \
     make && \
     make install && \
-    cd deps/hiredis && \
+    pushd deps/hiredis && \
     make install && \
-    cd ../.. && \
-    cd .. && \
+    popd && \
+    popd && \
     rm -rf redis-3.2.0*
 
 RUN ldconfig -v
 
 RUN useradd -m -U -s /bin/bash concrete && \
     passwd -l concrete
 ADD . /home/concrete/concrete-python
```

### Comparing `concrete-4.9.4/README.md` & `concrete-4.9.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2012-2015 Johns Hopkins University HLTCOE. All rights
+Copyright 2012-2016 Johns Hopkins University HLTCOE. All rights
 reserved.  This software is released under the 2-clause BSD license.
 See LICENSE.md in the project root directory.
 
 Concrete - Python
 =================
 
 Python modules and scripts for working with
```

