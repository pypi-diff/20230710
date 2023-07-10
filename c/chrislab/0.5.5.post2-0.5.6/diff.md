# Comparing `tmp/chrislab-0.5.5.post2.tar.gz` & `tmp/chrislab-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrislab-0.5.5.post2.tar", last modified: Sun Jul  9 16:03:41 2023, max compression
+gzip compressed data, was "chrislab-0.5.6.tar", last modified: Mon Jul 10 03:20:34 2023, max compression
```

## Comparing `chrislab-0.5.5.post2.tar` & `chrislab-0.5.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:03:41.478681 chrislab-0.5.5.post2/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1066 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/LICENSE
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      836 2023-07-09 16:03:41.478681 chrislab-0.5.5.post2/PKG-INFO
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      291 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/README.md
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       81 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/pyproject.toml
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1011 2023-07-09 16:03:41.478681 chrislab-0.5.5.post2/setup.cfg
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:03:41.470681 chrislab-0.5.5.post2/src/
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:03:41.470681 chrislab-0.5.5.post2/src/chrislab/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/chrislab/__init__.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:03:41.474681 chrislab-0.5.5.post2/src/chrislab/common/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/chrislab/common/__init__.py
--rwxr-xr-x   0 chrisjihee (1000016) users    (1000001)     7852 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/chrislab/common/downloader.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12638 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/chrislab/common/tokenizer_korbert.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    11372 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/chrislab/common/util.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:03:41.474681 chrislab-0.5.5.post2/src/chrislab/language/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/chrislab/language/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1319 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/chrislab/language/cli.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14142 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/chrislab/language/converter.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     9408 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/chrislab/language/evaluater.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    39568 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/chrislab/language/finetuner.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     6833 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/chrislab/language/modeling.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14491 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/chrislab/language/predictor.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:03:41.474681 chrislab-0.5.5.post2/src/chrislab.egg-info/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      836 2023-07-09 16:03:41.000000 chrislab-0.5.5.post2/src/chrislab.egg-info/PKG-INFO
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1541 2023-07-09 16:03:41.000000 chrislab-0.5.5.post2/src/chrislab.egg-info/SOURCES.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        1 2023-07-09 16:03:41.000000 chrislab-0.5.5.post2/src/chrislab.egg-info/dependency_links.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      132 2023-07-09 16:03:41.000000 chrislab-0.5.5.post2/src/chrislab.egg-info/entry_points.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       97 2023-07-09 16:03:41.000000 chrislab-0.5.5.post2/src/chrislab.egg-info/requires.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       17 2023-07-09 16:03:41.000000 chrislab-0.5.5.post2/src/chrislab.egg-info/top_level.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        1 2023-07-09 16:03:41.000000 chrislab-0.5.5.post2/src/chrislab.egg-info/zip-safe
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:03:41.474681 chrislab-0.5.5.post2/src/nlpbook/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       95 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12843 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/arguments.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:03:41.474681 chrislab-0.5.5.post2/src/nlpbook/cls/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       59 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/cls/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     8835 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/cls/cli.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     5177 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/cls/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2646 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/cls/task.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2246 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/data_utils.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:03:41.474681 chrislab-0.5.5.post2/src/nlpbook/dp/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      142 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/dp/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12298 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/dp/cli.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    18570 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/dp/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    11240 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/dp/model.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     6968 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/dp/task.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2057 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/factory.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:03:41.478681 chrislab-0.5.5.post2/src/nlpbook/generation/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      170 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/generation/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     4280 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/generation/arguments.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     5354 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/generation/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      882 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/generation/deploy.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1293 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/generation/task.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     8968 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/metrics.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:03:41.478681 chrislab-0.5.5.post2/src/nlpbook/ner/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       87 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/ner/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    18164 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/ner/cli.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14181 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/ner/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    10013 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/ner/task.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:03:41.478681 chrislab-0.5.5.post2/src/nlpbook/paircls/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       62 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/paircls/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2654 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/paircls/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      641 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/paircls/deploy.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:03:41.478681 chrislab-0.5.5.post2/src/nlpbook/qa/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      146 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/qa/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     4984 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/qa/arguments.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    17080 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/qa/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      639 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/qa/deploy.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2072 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/qa/task.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     9761 2023-07-08 17:51:04.000000 chrislab-0.5.5.post2/src/nlpbook/utils.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1066 2023-07-09 16:17:16.000000 chrislab-0.5.6/LICENSE
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      830 2023-07-10 03:20:34.718400 chrislab-0.5.6/PKG-INFO
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      291 2023-07-09 16:17:16.000000 chrislab-0.5.6/README.md
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       81 2023-07-09 16:17:16.000000 chrislab-0.5.6/pyproject.toml
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1005 2023-07-10 03:20:34.718400 chrislab-0.5.6/setup.cfg
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.714400 chrislab-0.5.6/src/
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.714400 chrislab-0.5.6/src/chrislab/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/__init__.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.714400 chrislab-0.5.6/src/chrislab/common/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/common/__init__.py
+-rwxr-xr-x   0 chrisjihee (1000016) users    (1000001)     7852 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/common/downloader.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12638 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/common/tokenizer_korbert.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    11372 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/common/util.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/chrislab/language/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/language/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1319 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/language/cli.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14142 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/language/converter.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     9408 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/language/evaluater.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    39568 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/language/finetuner.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     6833 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/language/modeling.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14491 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/language/predictor.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.714400 chrislab-0.5.6/src/chrislab.egg-info/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      830 2023-07-10 03:20:34.000000 chrislab-0.5.6/src/chrislab.egg-info/PKG-INFO
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1541 2023-07-10 03:20:34.000000 chrislab-0.5.6/src/chrislab.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        1 2023-07-10 03:20:34.000000 chrislab-0.5.6/src/chrislab.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      132 2023-07-10 03:20:34.000000 chrislab-0.5.6/src/chrislab.egg-info/entry_points.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       97 2023-07-10 03:20:34.000000 chrislab-0.5.6/src/chrislab.egg-info/requires.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       17 2023-07-10 03:20:34.000000 chrislab-0.5.6/src/chrislab.egg-info/top_level.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        1 2023-07-10 03:20:34.000000 chrislab-0.5.6/src/chrislab.egg-info/zip-safe
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/nlpbook/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       70 2023-07-10 02:57:42.000000 chrislab-0.5.6/src/nlpbook/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    15545 2023-07-10 03:01:27.000000 chrislab-0.5.6/src/nlpbook/arguments.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/nlpbook/cls/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       59 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/cls/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     8835 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/cls/cli.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     5177 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/cls/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2646 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/cls/task.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2246 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/data_utils.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/nlpbook/dp/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      142 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/dp/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12298 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/dp/cli.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    18570 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/dp/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    11240 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/dp/model.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     6968 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/dp/task.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2057 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/factory.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/nlpbook/generation/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      170 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/generation/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     4280 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/generation/arguments.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     5354 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/generation/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      882 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/generation/deploy.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1293 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/generation/task.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     8968 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/metrics.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/nlpbook/ner/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       87 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/ner/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    18164 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/ner/cli.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14181 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/ner/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    10013 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/ner/task.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/nlpbook/paircls/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       62 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/paircls/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2654 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/paircls/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      641 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/paircls/deploy.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/nlpbook/qa/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      146 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/qa/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     4984 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/qa/arguments.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    17080 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/qa/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      639 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/qa/deploy.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2072 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/qa/task.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     9761 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/utils.py
```

### Comparing `chrislab-0.5.5.post2/LICENSE` & `chrislab-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/PKG-INFO` & `chrislab-0.5.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.5.post2
+Version: 0.5.6
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.5.post2/setup.cfg` & `chrislab-0.5.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chrislab
-version = 0.5.5.post2
+version = 0.5.6
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrislab
 description = An advanced tool for doing experimental study.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `chrislab-0.5.5.post2/src/chrislab/common/downloader.py` & `chrislab-0.5.6/src/chrislab/common/downloader.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/chrislab/common/tokenizer_korbert.py` & `chrislab-0.5.6/src/chrislab/common/tokenizer_korbert.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/chrislab/common/util.py` & `chrislab-0.5.6/src/chrislab/common/util.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/chrislab/language/cli.py` & `chrislab-0.5.6/src/chrislab/language/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/chrislab/language/converter.py` & `chrislab-0.5.6/src/chrislab/language/converter.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/chrislab/language/evaluater.py` & `chrislab-0.5.6/src/chrislab/language/evaluater.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/chrislab/language/finetuner.py` & `chrislab-0.5.6/src/chrislab/language/finetuner.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/chrislab/language/modeling.py` & `chrislab-0.5.6/src/chrislab/language/modeling.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/chrislab/language/predictor.py` & `chrislab-0.5.6/src/chrislab/language/predictor.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/chrislab.egg-info/PKG-INFO` & `chrislab-0.5.6/src/chrislab.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.5.post2
+Version: 0.5.6
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.5.post2/src/chrislab.egg-info/SOURCES.txt` & `chrislab-0.5.6/src/chrislab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/arguments.py` & `chrislab-0.5.6/src/nlpbook/arguments.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 from datetime import datetime
 from pathlib import Path
 from typing import List
 
 import pandas as pd
 import pytorch_lightning
 import transformers
+import typer
 from dataclasses_json import DataClassJsonMixin
 from pytorch_lightning.accelerators import Accelerator
 from pytorch_lightning.loggers import CSVLogger
 from pytorch_lightning.strategies import Strategy
 
-from chrisbase.io import files, make_parent_dir, hr, str_table, out_hr, out_table, get_hostname, get_hostaddr, running_file, first_or, cwd, configure_dual_logger, configure_unit_logger
+from chrisbase.io import files, make_parent_dir, hr, str_table, out_hr, out_table, get_hostname, get_hostaddr, running_file, first_or, cwd, configure_dual_logger, configure_unit_logger, LoggingFormat
 from chrisbase.time import now, str_delta
 from chrisbase.util import to_dataframe
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
@@ -307,14 +308,98 @@
     def set_seed(self) -> None:
         if self.learning.seed is not None:
             transformers.set_seed(self.learning.seed)
             pytorch_lightning.seed_everything(self.learning.seed)
         else:
             logger.warning("not fixed seed")
 
+    @staticmethod
+    def from_args(
+            # env
+            project: str = None,
+            job_name: str = None,
+            debugging: bool = False,
+            # data
+            data_home: str = "data",
+            data_name: str = None,
+            train_file: str = None,
+            valid_file: str = None,
+            test_file: str = None,
+            num_check: int = 2,
+            # model
+            pretrained: str = "pretrained-com/KLUE-RoBERTa",
+            model_home: str = "finetuning",
+            model_name: str = None,
+            seq_len: int = 128,
+            # hardware
+            accelerator: str = "gpu",
+            precision: str = "32-true",
+            strategy: str = "auto",
+            device: List[int] = (0,),
+            batch_size: int = 100,
+            # learning
+            validate_fmt: str = None,
+            validate_on: float = 0.1,
+            num_save: int = 1,
+            save_by: str = None,
+            epochs: int = 1,
+            lr: float = 5e-5,
+            seed: int = 7,
+    ) -> "TrainerArguments":
+        pretrained = Path(pretrained)
+        return TrainerArguments(
+            env=ProjectEnv(
+                project=project,
+                job_name=job_name if job_name else pretrained.name,
+                debugging=debugging,
+                msg_level=logging.DEBUG if debugging else logging.INFO,
+                msg_format=LoggingFormat.DEBUG if debugging else LoggingFormat.CHECK,
+            ),
+            data=DataOption(
+                home=data_home,
+                name=data_name,
+                files=DataFiles(
+                    train=train_file,
+                    valid=valid_file,
+                    test=test_file,
+                ),
+                num_check=num_check,
+            ),
+            model=ModelOption(
+                pretrained=pretrained,
+                home=model_home,
+                name=model_name,
+                seq_len=seq_len,
+            ),
+            hardware=HardwareOption(
+                accelerator=accelerator,
+                precision=precision,
+                strategy=strategy,
+                devices=device,
+                batch_size=batch_size,
+            ),
+            learning=LearningOption(
+                validate_fmt=validate_fmt,
+                validate_on=validate_on,
+                num_save=num_save,
+                save_by=save_by,
+                epochs=epochs,
+                lr=lr,
+                seed=seed,
+            ),
+        )
+
+
+class AppTyper(typer.Typer):
+    def __init__(self):
+        super().__init__(
+            add_completion=False,
+            pretty_exceptions_enable=False,
+        )
+
 
 class ArgumentsUsing:
     def __init__(self, args: CommonArguments, delete_on_exit: bool = True):
         self.args: CommonArguments = args
         self.delete_on_exit: bool = delete_on_exit
 
     def __enter__(self) -> Path:
```

### Comparing `chrislab-0.5.5.post2/src/nlpbook/cls/cli.py` & `chrislab-0.5.6/src/nlpbook/cls/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/cls/corpus.py` & `chrislab-0.5.6/src/nlpbook/cls/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/cls/task.py` & `chrislab-0.5.6/src/nlpbook/cls/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/data_utils.py` & `chrislab-0.5.6/src/nlpbook/data_utils.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/dp/cli.py` & `chrislab-0.5.6/src/nlpbook/dp/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/dp/corpus.py` & `chrislab-0.5.6/src/nlpbook/dp/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/dp/model.py` & `chrislab-0.5.6/src/nlpbook/dp/model.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/dp/task.py` & `chrislab-0.5.6/src/nlpbook/dp/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/factory.py` & `chrislab-0.5.6/src/nlpbook/factory.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/generation/arguments.py` & `chrislab-0.5.6/src/nlpbook/generation/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/generation/corpus.py` & `chrislab-0.5.6/src/nlpbook/generation/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/generation/deploy.py` & `chrislab-0.5.6/src/nlpbook/generation/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/generation/task.py` & `chrislab-0.5.6/src/nlpbook/generation/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/metrics.py` & `chrislab-0.5.6/src/nlpbook/metrics.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/ner/cli.py` & `chrislab-0.5.6/src/nlpbook/ner/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/ner/corpus.py` & `chrislab-0.5.6/src/nlpbook/ner/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/ner/task.py` & `chrislab-0.5.6/src/nlpbook/ner/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/paircls/corpus.py` & `chrislab-0.5.6/src/nlpbook/paircls/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/paircls/deploy.py` & `chrislab-0.5.6/src/nlpbook/paircls/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/qa/arguments.py` & `chrislab-0.5.6/src/nlpbook/qa/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/qa/corpus.py` & `chrislab-0.5.6/src/nlpbook/qa/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/qa/deploy.py` & `chrislab-0.5.6/src/nlpbook/qa/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/qa/task.py` & `chrislab-0.5.6/src/nlpbook/qa/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5.post2/src/nlpbook/utils.py` & `chrislab-0.5.6/src/nlpbook/utils.py`

 * *Files identical despite different names*

